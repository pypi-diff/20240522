# Comparing `tmp/safe_mol-0.1.7.tar.gz` & `tmp/safe_mol-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_mol-0.1.7.tar", last modified: Fri May 10 15:51:34 2024, max compression
+gzip compressed data, was "safe_mol-0.1.8.tar", last modified: Wed May 22 04:23:46 2024, max compression
```

## Comparing `safe_mol-0.1.7.tar` & `safe_mol-0.1.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.397455 safe_mol-0.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.397455 safe_mol-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 15:47:42.000000 safe_mol-0.1.7/DATA_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-05-10 15:47:42.000000 safe_mol-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-10 15:51:34.409455 safe_mol-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-10 15:47:42.000000 safe_mol-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.401455 safe_mol-0.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.401455 safe_mol-0.1.7/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/api/safe.md
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/api/safe.models.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/api/safe.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.401455 safe_mol-0.1.7/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.401455 safe_mol-0.1.7/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (127)    36030 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/assets/safe-construction.svg
--rw-r--r--   0 runner    (1001) docker     (127)    86699 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/assets/safe-tasks.svg
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/data_license.md
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)  1793089 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/tutorials/design-with-safe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36563 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/tutorials/extracting-representation-molfeat.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   138661 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/tutorials/getting-started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    91753 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/tutorials/how-it-works.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 15:47:42.000000 safe_mol-0.1.7/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.397455 safe_mol-0.1.7/expts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/expts/config/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/config/accelerate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/expts/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-data-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-notebook.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train-custom.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train-small.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1168 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/train-small.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      688 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/train.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/expts/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/tokenizer/_tokenizer-custom-mini-test.json
--rw-r--r--   0 runner    (1001) docker     (127)    46319 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/tokenizer/tokenizer-custom.json
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-10 15:47:42.000000 safe_mol-0.1.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-10 15:47:42.000000 safe_mol-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/safe/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39204 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/safe/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/collator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/safe/trainer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/configs/default_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22577 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/safe_mol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:51:30.000000 safe_mol-0.1.7/safe_mol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:51:34.409455 safe_mol-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-10 15:47:42.000000 safe_mol-0.1.7/tests/test_hgf_load.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 15:47:42.000000 safe_mol-0.1.7/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-10 15:47:42.000000 safe_mol-0.1.7/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-10 15:47:42.000000 safe_mol-0.1.7/tests/test_safe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.526844 safe_mol-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.514844 safe_mol-0.1.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.514844 safe_mol-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-22 04:19:54.000000 safe_mol-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 04:19:54.000000 safe_mol-0.1.8/DATA_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-05-22 04:19:54.000000 safe_mol-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-22 04:23:46.526844 safe_mol-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-22 04:19:54.000000 safe_mol-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.518844 safe_mol-0.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.518844 safe_mol-0.1.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/api/safe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/api/safe.models.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/api/safe.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.518844 safe_mol-0.1.8/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.518844 safe_mol-0.1.8/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36030 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/assets/safe-construction.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    86699 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/assets/safe-tasks.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/data_license.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.518844 safe_mol-0.1.8/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)  1793089 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/tutorials/design-with-safe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36563 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/tutorials/extracting-representation-molfeat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   138661 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/tutorials/getting-started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    91753 2024-05-22 04:19:54.000000 safe_mol-0.1.8/docs/tutorials/how-it-works.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-22 04:19:54.000000 safe_mol-0.1.8/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.514844 safe_mol-0.1.8/expts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.522844 safe_mol-0.1.8/expts/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/config/accelerate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.522844 safe_mol-0.1.8/expts/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/scripts/slurm-data-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/scripts/slurm-notebook.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/scripts/slurm-tokenizer-train-custom.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/scripts/slurm-tokenizer-train-small.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1168 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/scripts/slurm-tokenizer-train.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/scripts/train-small.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      688 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/scripts/train.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.522844 safe_mol-0.1.8/expts/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/tokenizer/_tokenizer-custom-mini-test.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46319 2024-05-22 04:19:54.000000 safe_mol-0.1.8/expts/tokenizer/tokenizer-custom.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-22 04:19:54.000000 safe_mol-0.1.8/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-22 04:19:54.000000 safe_mol-0.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.522844 safe_mol-0.1.8/safe/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39204 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.522844 safe_mol-0.1.8/safe/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/trainer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/trainer/collator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.526844 safe_mol-0.1.8/safe/trainer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/trainer/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/trainer/configs/default_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/trainer/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/trainer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/trainer/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22577 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-22 04:19:54.000000 safe_mol-0.1.8/safe/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.526844 safe_mol-0.1.8/safe_mol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-22 04:23:46.000000 safe_mol-0.1.8/safe_mol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-22 04:23:46.000000 safe_mol-0.1.8/safe_mol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:23:46.000000 safe_mol-0.1.8/safe_mol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 04:23:46.000000 safe_mol-0.1.8/safe_mol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:23:42.000000 safe_mol-0.1.8/safe_mol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 04:23:46.000000 safe_mol-0.1.8/safe_mol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 04:23:46.000000 safe_mol-0.1.8/safe_mol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:23:46.526844 safe_mol-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:23:46.526844 safe_mol-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-22 04:19:54.000000 safe_mol-0.1.8/tests/test_hgf_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 04:19:54.000000 safe_mol-0.1.8/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-22 04:19:54.000000 safe_mol-0.1.8/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-22 04:19:54.000000 safe_mol-0.1.8/tests/test_safe.py
```

### Comparing `safe_mol-0.1.7/.github/PULL_REQUEST_TEMPLATE.md` & `safe_mol-0.1.8/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/.github/workflows/code-check.yml` & `safe_mol-0.1.8/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/.github/workflows/doc.yml` & `safe_mol-0.1.8/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/.github/workflows/release.yml` & `safe_mol-0.1.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/.github/workflows/test.yml` & `safe_mol-0.1.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/.gitignore` & `safe_mol-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/LICENSE` & `safe_mol-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/PKG-INFO` & `safe_mol-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-mol
-Version: 0.1.7
+Version: 0.1.8
 Summary: Implementation of the 'Gotta be SAFE: a new framework for molecular design' paper
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/datamol-io/safe
 Project-URL: Bug Tracker, https://github.com/datamol-io/safe/issues
 Project-URL: Documentation, https://safe-docs.datamol.io/
 Keywords: safe,smiles,de novo,design,molecules
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: safe-mol Version: 0.1.7 Summary: Implementation of
+Metadata-Version: 2.1 Name: safe-mol Version: 0.1.8 Summary: Implementation of
 the 'Gotta be SAFE: a new framework for molecular design' paper Author-email:
 Emmanuel Noutahi
 gmail.com> License: Apache-2.0 Project-URL: Source Code, https://github.com/
 datamol-io/safe Project-URL: Bug Tracker, https://github.com/datamol-io/safe/
 issues Project-URL: Documentation, https://safe-docs.datamol.io/ Keywords:
 safe,smiles,de novo,design,molecules Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
```

### Comparing `safe_mol-0.1.7/README.md` & `safe_mol-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/api/safe.models.md` & `safe_mol-0.1.8/docs/api/safe.models.md`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/assets/safe-construction.svg` & `safe_mol-0.1.8/docs/assets/safe-construction.svg`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/assets/safe-tasks.svg` & `safe_mol-0.1.8/docs/assets/safe-tasks.svg`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/cli.md` & `safe_mol-0.1.8/docs/cli.md`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/index.md` & `safe_mol-0.1.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/tutorials/design-with-safe.ipynb` & `safe_mol-0.1.8/docs/tutorials/design-with-safe.ipynb`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/tutorials/extracting-representation-molfeat.ipynb` & `safe_mol-0.1.8/docs/tutorials/extracting-representation-molfeat.ipynb`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/tutorials/getting-started.ipynb` & `safe_mol-0.1.8/docs/tutorials/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/docs/tutorials/how-it-works.ipynb` & `safe_mol-0.1.8/docs/tutorials/how-it-works.ipynb`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/env.yml` & `safe_mol-0.1.8/env.yml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   - datamol
   - pandas <=2.1.1
   - numpy
   - pytorch >=2.0
   - transformers
   - datasets
   - tokenizers
-  - accelerate
+  - accelerate >=0.28.0 # for accelerator_config update
   - evaluate
   - wandb
   - huggingface_hub
 
   # Optional
   - deepspeed
```

### Comparing `safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train-custom.sh` & `safe_mol-0.1.8/expts/scripts/slurm-tokenizer-train-custom.sh`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train-small.sh` & `safe_mol-0.1.8/expts/scripts/slurm-tokenizer-train-small.sh`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train.sh` & `safe_mol-0.1.8/expts/scripts/slurm-tokenizer-train.sh`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/expts/scripts/train-small.sh` & `safe_mol-0.1.8/expts/scripts/train-small.sh`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/expts/scripts/train.sh` & `safe_mol-0.1.8/expts/scripts/train.sh`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/expts/tokenizer/_tokenizer-custom-mini-test.json` & `safe_mol-0.1.8/expts/tokenizer/_tokenizer-custom-mini-test.json`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/expts/tokenizer/tokenizer-custom.json` & `safe_mol-0.1.8/expts/tokenizer/tokenizer-custom.json`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/mkdocs.yml` & `safe_mol-0.1.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/pyproject.toml` & `safe_mol-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/converter.py` & `safe_mol-0.1.8/safe/converter.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/sample.py` & `safe_mol-0.1.8/safe/sample.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/tokenizer.py` & `safe_mol-0.1.8/safe/tokenizer.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/trainer/cli.py` & `safe_mol-0.1.8/safe/trainer/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,18 +328,20 @@
             )
             results.update(results_mse)
         return results
 
     if model_args.include_descriptors:
         training_args.label_names = ["labels", "mc_labels"]
 
+    # update dispatch_batches in accelerator
+    training_args.accelerator_config.dispatch_batches = data_args.streaming is not True
+
     trainer = SAFETrainer(
         model=model,
         tokenizer=None,  # we don't deal with the tokenizer at all, https://github.com/huggingface/tokenizers/issues/581 -_-
-        dispatch_batches=(data_args.streaming is not True),
         train_dataset=train_dataset.shuffle(seed=(training_args.seed or 42)),
         eval_dataset=dataset.get(eval_dataset_key_name, None),
         args=training_args,
         prop_loss_coeff=model_args.prop_loss_coeff,
         compute_metrics=compute_metrics if training_args.do_eval else None,
         data_collator=data_collator,
         preprocess_logits_for_metrics=(
```

### Comparing `safe_mol-0.1.7/safe/trainer/collator.py` & `safe_mol-0.1.8/safe/trainer/collator.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/trainer/configs/default_config.json` & `safe_mol-0.1.8/safe/trainer/configs/default_config.json`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/trainer/data_utils.py` & `safe_mol-0.1.8/safe/trainer/data_utils.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/trainer/model.py` & `safe_mol-0.1.8/safe/trainer/model.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/trainer/trainer_utils.py` & `safe_mol-0.1.8/safe/trainer/trainer_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,17 @@
     """
     Custom trainer for training SAFE model.
 
     This custom trainer changes the loss function to support the property head
 
     """
 
-    def __init__(
-        self, *args, prop_loss_coeff: float = 1e-3, dispatch_batches: bool = False, **kwargs
-    ):
+    def __init__(self, *args, prop_loss_coeff: float = 1e-3, **kwargs):
         super().__init__(*args, **kwargs)
         self.prop_loss_coeff = prop_loss_coeff
-        self.accelerator.dispatch_batches = dispatch_batches
 
     def compute_loss(self, model, inputs, return_outputs=False):
         """
         How the loss is computed by Trainer. By default, all models return the loss in the first element.
         """
         labels = (
             inputs.pop("labels") if self.label_smoother is not None and "labels" in inputs else None
```

### Comparing `safe_mol-0.1.7/safe/utils.py` & `safe_mol-0.1.8/safe/utils.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe/viz.py` & `safe_mol-0.1.8/safe/viz.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/safe_mol.egg-info/PKG-INFO` & `safe_mol-0.1.8/safe_mol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-mol
-Version: 0.1.7
+Version: 0.1.8
 Summary: Implementation of the 'Gotta be SAFE: a new framework for molecular design' paper
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/datamol-io/safe
 Project-URL: Bug Tracker, https://github.com/datamol-io/safe/issues
 Project-URL: Documentation, https://safe-docs.datamol.io/
 Keywords: safe,smiles,de novo,design,molecules
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: safe-mol Version: 0.1.7 Summary: Implementation of
+Metadata-Version: 2.1 Name: safe-mol Version: 0.1.8 Summary: Implementation of
 the 'Gotta be SAFE: a new framework for molecular design' paper Author-email:
 Emmanuel Noutahi
 gmail.com> License: Apache-2.0 Project-URL: Source Code, https://github.com/
 datamol-io/safe Project-URL: Bug Tracker, https://github.com/datamol-io/safe/
 issues Project-URL: Documentation, https://safe-docs.datamol.io/ Keywords:
 safe,smiles,de novo,design,molecules Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
```

### Comparing `safe_mol-0.1.7/safe_mol.egg-info/SOURCES.txt` & `safe_mol-0.1.8/safe_mol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/tests/test_hgf_load.py` & `safe_mol-0.1.8/tests/test_hgf_load.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/tests/test_notebooks.py` & `safe_mol-0.1.8/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `safe_mol-0.1.7/tests/test_safe.py` & `safe_mol-0.1.8/tests/test_safe.py`

 * *Files identical despite different names*

