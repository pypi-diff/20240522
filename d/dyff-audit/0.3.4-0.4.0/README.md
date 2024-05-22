# Comparing `tmp/dyff_audit-0.3.4.tar.gz` & `tmp/dyff_audit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_audit-0.3.4.tar", last modified: Fri May 17 05:22:06 2024, max compression
+gzip compressed data, was "dyff_audit-0.4.0.tar", last modified: Wed May 22 20:53:01 2024, max compression
```

## Comparing `dyff_audit-0.3.4.tar` & `dyff_audit-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.918918 dyff_audit-0.3.4/
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1840 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1800 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3690 2024-05-17 05:22:06.917919 dyff_audit-0.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.901919 dyff_audit-0.3.4/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.908918 dyff_audit-0.3.4/dyff/audit/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/_internal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.909919 dyff_audit-0.3.4/dyff/audit/analysis/
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6108 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/analysis/context.py
--rw-rw-rw-   0 root         (0) root         (0)     1689 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/analysis/jupyter.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/analysis/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2814 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/analysis/python.py
--rw-rw-rw-   0 root         (0) root         (0)     2920 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/analysis/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.910919 dyff_audit-0.3.4/dyff/audit/data/
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/data/text.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/dynamic_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.911918 dyff_audit-0.3.4/dyff/audit/local/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5580 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/local/mocks.py
--rw-rw-rw-   0 root         (0) root         (0)    33208 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/local/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.911918 dyff_audit-0.3.4/dyff/audit/metrics/
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/metrics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/metrics/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4359 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/metrics/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.912918 dyff_audit-0.3.4/dyff/audit/scoring/
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/scoring/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/scoring/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/scoring/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/scoring/example.py
--rw-rw-rw-   0 root         (0) root         (0)    11999 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/scoring/text.py
--rw-rw-rw-   0 root         (0) root         (0)     5994 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/dyff/audit/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.917919 dyff_audit-0.3.4/dyff_audit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3690 2024-05-17 05:22:06.000000 dyff_audit-0.3.4/dyff_audit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1457 2024-05-17 05:22:06.000000 dyff_audit-0.3.4/dyff_audit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 05:22:06.000000 dyff_audit-0.3.4/dyff_audit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2024-05-17 05:22:06.000000 dyff_audit-0.3.4/dyff_audit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-17 05:22:06.000000 dyff_audit-0.3.4/dyff_audit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1911 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 05:22:06.918918 dyff_audit-0.3.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.914919 dyff_audit-0.3.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.904919 dyff_audit-0.3.4/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.915918 dyff_audit-0.3.4/tests/data/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     1196 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/data/dataset/part-0.parquet
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.915918 dyff_audit-0.3.4/tests/data/evaluation/
--rw-rw-rw-   0 root         (0) root         (0)     2990 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/data/evaluation/part-0.parquet
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.915918 dyff_audit-0.3.4/tests/data/module_jupyter_notebook/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/data/module_jupyter_notebook/notebook_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     5740 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/data/module_jupyter_notebook/test-notebook.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.904919 dyff_audit-0.3.4/tests/data/module_python_function/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.904919 dyff_audit-0.3.4/tests/data/module_python_function/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.916918 dyff_audit-0.3.4/tests/data/module_python_function/dyff/fake/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/data/module_python_function/dyff/fake/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/data/module_python_function/dyff/fake/method.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.904919 dyff_audit-0.3.4/tests/data/module_python_rubric/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.904919 dyff_audit-0.3.4/tests/data/module_python_rubric/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 05:22:06.916918 dyff_audit-0.3.4/tests/data/module_python_rubric/dyff/fake/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/data/module_python_rubric/dyff/fake/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/data/module_python_rubric/dyff/fake/rubric.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/test_import.py
--rw-rw-rw-   0 root         (0) root         (0)    20502 2024-05-17 05:22:00.000000 dyff_audit-0.3.4/tests/test_workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.386469 dyff_audit-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-22 20:53:01.386469 dyff_audit-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.371468 dyff_audit-0.4.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.377468 dyff_audit-0.4.0/dyff/audit/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/_internal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.378469 dyff_audit-0.4.0/dyff/audit/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6108 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/analysis/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/analysis/jupyter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/analysis/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2814 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/analysis/python.py
+-rw-rw-rw-   0 root         (0) root         (0)     2920 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/analysis/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.379469 dyff_audit-0.4.0/dyff/audit/data/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/data/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/dynamic_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.379469 dyff_audit-0.4.0/dyff/audit/local/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5580 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/local/mocks.py
+-rw-rw-rw-   0 root         (0) root         (0)    33326 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/local/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.380468 dyff_audit-0.4.0/dyff/audit/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/metrics/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4359 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/metrics/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.381469 dyff_audit-0.4.0/dyff/audit/scoring/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/scoring/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/scoring/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/scoring/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/scoring/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    11999 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/scoring/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/dyff/audit/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.385469 dyff_audit-0.4.0/dyff_audit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-22 20:53:01.000000 dyff_audit-0.4.0/dyff_audit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-05-22 20:53:01.000000 dyff_audit-0.4.0/dyff_audit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 20:53:01.000000 dyff_audit-0.4.0/dyff_audit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-22 20:53:01.000000 dyff_audit-0.4.0/dyff_audit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-22 20:53:01.000000 dyff_audit-0.4.0/dyff_audit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 20:53:01.386469 dyff_audit-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.383468 dyff_audit-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.373468 dyff_audit-0.4.0/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.383468 dyff_audit-0.4.0/tests/data/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/data/dataset/part-0.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.383468 dyff_audit-0.4.0/tests/data/evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/data/evaluation/part-0.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.384468 dyff_audit-0.4.0/tests/data/module_jupyter_notebook/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/data/module_jupyter_notebook/notebook_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     5740 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/data/module_jupyter_notebook/test-notebook.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.373468 dyff_audit-0.4.0/tests/data/module_python_function/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.373468 dyff_audit-0.4.0/tests/data/module_python_function/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.384468 dyff_audit-0.4.0/tests/data/module_python_function/dyff/fake/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/data/module_python_function/dyff/fake/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/data/module_python_function/dyff/fake/method.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.373468 dyff_audit-0.4.0/tests/data/module_python_rubric/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.373468 dyff_audit-0.4.0/tests/data/module_python_rubric/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:53:01.385469 dyff_audit-0.4.0/tests/data/module_python_rubric/dyff/fake/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/data/module_python_rubric/dyff/fake/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/data/module_python_rubric/dyff/fake/rubric.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/test_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    21584 2024-05-22 20:52:55.000000 dyff_audit-0.4.0/tests/test_workflows.py
```

### Comparing `dyff_audit-0.3.4/.gitignore` & `dyff_audit-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/.gitlab-ci.yml` & `dyff_audit-0.4.0/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
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
       - python-import-linter.yml
       - python-isort.yml
```

### Comparing `dyff_audit-0.3.4/.pre-commit-config.yaml` & `dyff_audit-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/.secrets.baseline` & `dyff_audit-0.4.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/CODE_OF_CONDUCT.md` & `dyff_audit-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/LICENSE` & `dyff_audit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/PKG-INFO` & `dyff_audit-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-audit
-Version: 0.3.4
+Version: 0.4.0
 Summary: Audit tools for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-audit
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-audit/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_audit-0.3.4/README.md` & `dyff_audit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/_internal.py` & `dyff_audit-0.4.0/dyff/audit/_internal.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/analysis/context.py` & `dyff_audit-0.4.0/dyff/audit/analysis/context.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/analysis/jupyter.py` & `dyff_audit-0.4.0/dyff/audit/analysis/jupyter.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/analysis/legacy.py` & `dyff_audit-0.4.0/dyff/audit/analysis/legacy.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/analysis/python.py` & `dyff_audit-0.4.0/dyff/audit/analysis/python.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/analysis/runners.py` & `dyff_audit-0.4.0/dyff/audit/analysis/runners.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/data/text.py` & `dyff_audit-0.4.0/dyff/audit/data/text.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/local/mocks.py` & `dyff_audit-0.4.0/dyff/audit/local/mocks.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/local/platform.py` & `dyff_audit-0.4.0/dyff/audit/local/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 # mypy: disable-error-code="import-untyped"
 from __future__ import annotations
 
 import json
-from datetime import datetime
+from datetime import datetime, timezone
 from pathlib import Path
 from typing import Any, Optional, Type
 
 import ruamel.yaml
 
 from dyff.client import Client, HttpResponseError
 from dyff.schema import ids
@@ -59,15 +59,15 @@
 
     def create(self, dataset_request: DatasetCreateRequest) -> Dataset:
         id = ids.generate_entity_id()
         dataset_dict = dataset_request.dict()
         dataset_dict["id"] = id
         dataset_dict["account"] = self._platform.account
         dataset_dict["status"] = EntityStatus.ready
-        dataset_dict["creationTime"] = datetime.now()
+        dataset_dict["creationTime"] = datetime.now(timezone.utc)
         dataset = Dataset.parse_obj(dataset_dict)
 
         cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".dataset.json", "w") as fout:
             fout.write(dataset.json())
         return dataset
@@ -418,15 +418,15 @@
             session = self.get(id)
             if session is None:
                 raise HttpResponseError(status_code=404)
             return session.status == EntityStatus.admitted
         except:
             return False
 
-    def token(self, id: str) -> str:
+    def token(self, id: str, expires: Optional[datetime] = None) -> str:
         return "dummy-token"
 
     def infer(
         self, id: str, endpoint: str, request: dict[str, Any]
     ) -> list[dict[str, Any]]:
         session = self.get(id)
         if session is None:
@@ -485,15 +485,15 @@
         measurement_spec = method.output.measurement
         if measurement_spec is None:
             raise ValueError("Method spec violates constraints")
 
         measurement = Measurement(
             account=analysis_request.account,
             id=id,
-            creationTime=datetime.now(),
+            creationTime=datetime.now(timezone.utc),
             status=EntityStatus.complete,
             scope=analysis_request.scope,
             method=ForeignMethod.parse_obj(method.dict()),
             arguments=analysis_request.arguments,
             inputs=analysis_request.inputs,
             **measurement_spec.dict(),
         )
@@ -538,15 +538,15 @@
 
     def create(self, method_request: MethodCreateRequest) -> Method:
         id = ids.generate_entity_id()
         method_dict = method_request.dict()
         method_dict["id"] = id
         method_dict["account"] = self._platform.account
         method_dict["status"] = EntityStatus.ready
-        method_dict["creationTime"] = datetime.now()
+        method_dict["creationTime"] = datetime.now(timezone.utc)
         method = Method.parse_obj(method_dict)
 
         cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".method.json", "w") as fout:
             fout.write(method.json())
         return method
@@ -565,15 +565,15 @@
 
     def create(self, module_request: ModuleCreateRequest) -> Module:
         id = ids.generate_entity_id()
         module_dict = module_request.dict()
         module_dict["id"] = id
         module_dict["account"] = self._platform.account
         module_dict["status"] = EntityStatus.ready
-        module_dict["creationTime"] = datetime.now()
+        module_dict["creationTime"] = datetime.now(timezone.utc)
         module = Module.parse_obj(module_dict)
 
         cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".module.json", "w") as fout:
             fout.write(module.json())
         return module
@@ -667,15 +667,15 @@
 
     def create(self, report_request: ReportCreateRequest) -> Report:
         id = ids.generate_entity_id()
         report_dict = report_request.dict()
         report_dict["id"] = id
         report_dict["account"] = self._platform.account
         report_dict["status"] = EntityStatus.ready
-        report_dict["creationTime"] = datetime.now()
+        report_dict["creationTime"] = datetime.now(timezone.utc)
 
         evaluation = self._platform.evaluations.get(report_request.evaluation)
         if evaluation is None:
             raise HttpResponseError(status_code=404)
         report_dict["dataset"] = evaluation.dataset
         report_dict["inferenceService"] = (
             evaluation.inferenceSession.inferenceService.id
@@ -716,15 +716,15 @@
         safetycase_spec = method.output.safetyCase
         if safetycase_spec is None:
             raise ValueError("Method spec violates constraints")
 
         safetycase = SafetyCase(
             account=analysis_request.account,
             id=id,
-            creationTime=datetime.now(),
+            creationTime=datetime.now(timezone.utc),
             status=EntityStatus.complete,
             scope=analysis_request.scope,
             method=ForeignMethod.parse_obj(method.dict()),
             arguments=analysis_request.arguments,
             inputs=analysis_request.inputs,
             # This covers: .name, .description
             **safetycase_spec.dict(),
```

### Comparing `dyff_audit-0.3.4/dyff/audit/metrics/base.py` & `dyff_audit-0.4.0/dyff/audit/metrics/base.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/metrics/text.py` & `dyff_audit-0.4.0/dyff/audit/metrics/text.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/scoring/base.py` & `dyff_audit-0.4.0/dyff/audit/scoring/base.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/scoring/classification.py` & `dyff_audit-0.4.0/dyff/audit/scoring/classification.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/scoring/example.py` & `dyff_audit-0.4.0/dyff/audit/scoring/example.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/scoring/text.py` & `dyff_audit-0.4.0/dyff/audit/scoring/text.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff/audit/workflows.py` & `dyff_audit-0.4.0/dyff/audit/workflows.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/dyff_audit.egg-info/PKG-INFO` & `dyff_audit-0.4.0/dyff_audit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-audit
-Version: 0.3.4
+Version: 0.4.0
 Summary: Audit tools for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-audit
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-audit/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_audit-0.3.4/dyff_audit.egg-info/SOURCES.txt` & `dyff_audit-0.4.0/dyff_audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/makefile` & `dyff_audit-0.4.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/pyproject.toml` & `dyff_audit-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/tests/conftest.py` & `dyff_audit-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/tests/data/dataset/part-0.parquet` & `dyff_audit-0.4.0/tests/data/dataset/part-0.parquet`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/tests/data/evaluation/part-0.parquet` & `dyff_audit-0.4.0/tests/data/evaluation/part-0.parquet`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/tests/data/module_jupyter_notebook/test-notebook.ipynb` & `dyff_audit-0.4.0/tests/data/module_jupyter_notebook/test-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/tests/data/module_python_function/dyff/fake/method.py` & `dyff_audit-0.4.0/tests/data/module_python_function/dyff/fake/method.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/tests/data/module_python_rubric/dyff/fake/rubric.py` & `dyff_audit-0.4.0/tests/data/module_python_rubric/dyff/fake/rubric.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/tests/test_import.py` & `dyff_audit-0.4.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.4/tests/test_workflows.py` & `dyff_audit-0.4.0/tests/test_workflows.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import os
 import time
 
 # mypy: disable-error-code="import-untyped"
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from pathlib import Path
 from typing import Any
 
 import pydantic
 import pytest
 
 from dyff.audit.local import mocks
@@ -98,25 +98,25 @@
 
     request.addfinalizer(terminate_session)
 
 
 def wait_for_ready(
     dyffapi: Client | DyffLocalPlatform, session_id: str, *, timeout: timedelta
 ):
-    then = datetime.now()
-    while (datetime.now() - then) < timeout:
+    then = datetime.now(timezone.utc)
+    while (datetime.now(timezone.utc) - then) < timeout:
         if dyffapi.inferencesessions.ready(session_id):
             return
         time.sleep(10)
     raise AssertionError("timeout")
 
 
 def wait_for_success(get_entity_fn, *, timeout: timedelta):
-    then = datetime.now()
-    while (datetime.now() - then) < timeout:
+    then = datetime.now(timezone.utc)
+    while (datetime.now(timezone.utc) - then) < timeout:
         try:
             status = get_entity_fn().status
             if is_status_success(status):
                 return
             elif is_status_failure(status):
                 raise AssertionError(f"failure status: {status}")
         except HttpResponseError as ex:
@@ -262,14 +262,44 @@
         )
     print(f"infer response: {response}")
 
 
 @pytest.mark.datafiles(DATA_DIR)
 @pytest.mark.depends(
     on=[
+        "test_inferencesessions_create",
+    ]
+)
+def test_inferencesessions_infer_with_created_token(
+    pytestconfig, dyffapi: Client | DyffLocalPlatform, ctx, datafiles
+):
+    session: InferenceSession = ctx["inferencesession"]
+    token = dyffapi.inferencesessions.token(
+        session.id, expires=datetime.now(timezone.utc) + timedelta(minutes=5)
+    )
+
+    if pytestconfig.getoption("test_remote"):
+        assert isinstance(dyffapi, Client)
+        session_client = dyffapi.inferencesessions.client(
+            session.id,
+            token,
+            interface=session.inferenceService.interface,
+        )
+        response = session_client.infer({"text": "Open the pod bay doors, Hal!"})
+    else:
+        assert isinstance(dyffapi, DyffLocalPlatform)
+        response = dyffapi.inferencesessions.infer(
+            session.id, "generate", {"text": "Open the pod bay doors, Hal!"}
+        )
+    print(f"infer response: {response}")
+
+
+@pytest.mark.datafiles(DATA_DIR)
+@pytest.mark.depends(
+    on=[
         "test_inferenceservices_create",
     ]
 )
 def test_evaluations_create(
     pytestconfig, dyffapi: Client | DyffLocalPlatform, ctx, datafiles
 ):
     account = ctx["account"]
@@ -277,15 +307,15 @@
 
     inferenceservice = ctx["inferenceservice"]
     evaluation_request = EvaluationCreateRequest(
         account=account,
         dataset=dataset.id,
         inferenceSession=EvaluationInferenceSessionRequest(
             inferenceService=inferenceservice.id,
-            expires=datetime.now() + timedelta(days=1),
+            expires=datetime.now(timezone.utc) + timedelta(days=1),
             replicas=1,
             useSpotPods=False,
         ),
         replications=2,
         workersPerReplica=2,
     )
     evaluation = dyffapi.evaluations.create(evaluation_request)
```

