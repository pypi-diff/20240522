# Comparing `tmp/ifk-smhi-0.1.2.tar.gz` & `tmp/ifk_smhi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifk-smhi-0.1.2.tar", last modified: Fri Jan 26 06:46:29 2024, max compression
+gzip compressed data, was "ifk_smhi-0.2.0.tar", last modified: Wed May 22 17:59:30 2024, max compression
```

## Comparing `ifk-smhi-0.1.2.tar` & `ifk_smhi-0.2.0.tar`

### file list

```diff
@@ -1,83 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.367879 ifk-smhi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.bandit
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.351879 ifk-smhi-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.355879 ifk-smhi-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.github/workflows/github-action-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.github/workflows/github-action-lint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.github/workflows/github-action-md-lint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.github/workflows/github-action-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.github/workflows/github-action-test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.github/workflows/github-action-type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.markdownlintignore
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-01-26 06:46:29.367879 ifk-smhi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.359879 ifk-smhi-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.359879 ifk-smhi-0.1.2/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/assets/ifk_logo_black.png
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/assets/ifk_logo_white.png
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/mesan-example.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/mesan-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/metfcts-example.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/metfcts-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/metobs-example.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/metobs-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/strang-example.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/docs/strang-reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.351879 ifk-smhi-0.1.2/material/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.359879 ifk-smhi-0.1.2/material/partials/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/material/partials/copyright.html
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 06:46:29.367879 ifk-smhi-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.351879 ifk-smhi-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.363879 ifk-smhi-0.1.2/src/ifk_smhi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-01-26 06:46:29.000000 ifk-smhi-0.1.2/src/ifk_smhi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-26 06:46:29.000000 ifk-smhi-0.1.2/src/ifk_smhi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 06:46:29.000000 ifk-smhi-0.1.2/src/ifk_smhi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-26 06:46:29.000000 ifk-smhi-0.1.2/src/ifk_smhi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-26 06:46:29.000000 ifk-smhi-0.1.2/src/ifk_smhi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.359879 ifk-smhi-0.1.2/src/smhi/
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/src/smhi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/src/smhi/mesan.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/src/smhi/metfcts.py
--rw-r--r--   0 runner    (1001) docker     (127)    20168 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/src/smhi/metobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/src/smhi/smhi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/src/smhi/strang.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.355879 ifk-smhi-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.363879 ifk-smhi-0.1.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/STRANG_NONE.csv
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/STRANG_RESULT_DAILY_2020_01_01_2020_01_02.csv
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/STRANG_RESULT_HOURLY_2020_01_01_2020_01_02.csv
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/STRANG_RESULT_MONTHLY_2020_01_01_2020_02_01.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/STRANG_RESULT_MULTIPOINT_2020_01_01_MONTHLY_10.csv
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/metobs_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/metobs_integration_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/metobs_integration_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/metobs_integration_22.json
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/metobs_unit_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/metobs_unit_2.json
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/unit_mesan_multipoint_format.json
--rw-r--r--   0 runner    (1001) docker     (127)   121790 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/unit_mesan_multipoint_format_result.csv
--rw-r--r--   0 runner    (1001) docker     (127)    49270 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/unit_mesan_point_format.json
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/unit_mesan_point_format_result.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/fixtures/unit_metobs_data.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.363879 ifk-smhi-0.1.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/integration/test_integration_mesan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/integration/test_integration_metobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/integration/test_integration_smhi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/integration/test_integration_strang.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 06:46:29.363879 ifk-smhi-0.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/unit/test_unit_mesan.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/unit/test_unit_metfcts.py
--rw-r--r--   0 runner    (1001) docker     (127)    30780 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/unit/test_unit_metobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/unit/test_unit_smhi.py
--rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tests/unit/test_unit_strang.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-26 06:46:20.000000 ifk-smhi-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.584736 ifk_smhi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.556736 ifk_smhi-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.560736 ifk_smhi-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.github/workflows/github-action-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.github/workflows/github-action-lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.github/workflows/github-action-md-lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.github/workflows/github-action-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.github/workflows/github-action-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.github/workflows/github-action-type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.markdownlintignore
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-22 17:59:30.580736 ifk_smhi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3400 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/create_pydantic_models.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.564736 ifk_smhi-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.564736 ifk_smhi-0.2.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/assets/ifk_logo_black.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/assets/ifk_logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1012815 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/assets/kiruna_snodjup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/mesan-example.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/mesan-model.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/mesan-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/metfcts-example.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/metfcts-model.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/metfcts-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/metobs-example.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/metobs-model.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/metobs-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/smhi-example.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/smhi-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/strang-example.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/strang-model.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/docs/strang-reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.556736 ifk_smhi-0.2.0/material/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.564736 ifk_smhi-0.2.0/material/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/material/partials/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:59:30.584736 ifk_smhi-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.556736 ifk_smhi-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.580736 ifk_smhi-0.2.0/src/ifk_smhi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-22 17:59:30.000000 ifk_smhi-0.2.0/src/ifk_smhi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-22 17:59:30.000000 ifk_smhi-0.2.0/src/ifk_smhi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:59:30.000000 ifk_smhi-0.2.0/src/ifk_smhi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-22 17:59:30.000000 ifk_smhi-0.2.0/src/ifk_smhi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 17:59:30.000000 ifk_smhi-0.2.0/src/ifk_smhi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.568736 ifk_smhi-0.2.0/src/smhi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/mesan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/metfcts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16223 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/metobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.568736 ifk_smhi-0.2.0/src/smhi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/models/mesan_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/models/metfcts_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/models/metobs_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/models/strang_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/models/variable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/smhi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/strang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/src/smhi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.560736 ifk_smhi-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.560736 ifk_smhi-0.2.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.572736 ifk_smhi-0.2.0/tests/fixtures/mesan/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/mesan/multipoint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/mesan/multipoint_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/mesan/point.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/mesan/point_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/mesan/point_data_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.576736 ifk_smhi-0.2.0/tests/fixtures/metobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/data_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/data_parameter.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/data_period.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/data_station.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/metobs_integration_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/metobs_integration_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/metobs_integration_22.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/parameters.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/parameters_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/periods.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/periods_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/periods_data_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/periods_set.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/stations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/stations_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/metobs/versions.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.576736 ifk_smhi-0.2.0/tests/fixtures/strang/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/multipoint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/multipoint_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/point.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/point_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/strang_none.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/strang_result_daily_2020_01_01_2020_01_02.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/strang_result_hourly_2020_01_01_2020_01_02.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/strang_result_monthly_2020_01_01_2020_02_01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/fixtures/strang/strang_result_multipoint_2020_01_01_monthly_10.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.576736 ifk_smhi-0.2.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/integration/test_integration_mesan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/integration/test_integration_metobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/integration/test_integration_smhi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/integration/test_integration_strang.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:59:30.580736 ifk_smhi-0.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)    14059 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/unit/test_unit_mesan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/unit/test_unit_metfcts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/unit/test_unit_metobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/unit/test_unit_smhi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/unit/test_unit_strang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/unit/text_unit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-22 17:59:26.000000 ifk_smhi-0.2.0/tests/unit/utils.py
```

### Comparing `ifk-smhi-0.1.2/.github/workflows/github-action-docs.yaml` & `ifk_smhi-0.2.0/.github/workflows/github-action-docs.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: Deploy docs to GitHub Pages
 
 on:
-  push:
-    branches: ["main"]
+  release:
+    types: [published]
 
   workflow_dispatch:
 
 permissions:
   contents: read
   pages: write
   id-token: write
@@ -16,15 +16,15 @@
   cancel-in-progress: true
 
 jobs:
   build-docs:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9"]
+        python-version: ["3.11"]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `ifk-smhi-0.1.2/.github/workflows/github-action-lint.yaml` & `ifk_smhi-0.2.0/.github/workflows/github-action-lint.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Lint
 on: [push]
 jobs:
   lint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9"]
+        python-version: ["3.11"]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `ifk-smhi-0.1.2/.github/workflows/github-action-md-lint.yaml` & `ifk_smhi-0.2.0/.github/workflows/github-action-md-lint.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Markdown Lint
 on: [push]
 jobs:
   mdlint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9"]
+        python-version: ["3.11"]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `ifk-smhi-0.1.2/.github/workflows/github-action-pypi.yaml` & `ifk_smhi-0.2.0/.github/workflows/github-action-pypi.yaml`

 * *Files identical despite different names*

### Comparing `ifk-smhi-0.1.2/.github/workflows/github-action-test.yaml` & `ifk_smhi-0.2.0/.github/workflows/github-action-test.yaml`

 * *Files identical despite different names*

### Comparing `ifk-smhi-0.1.2/.gitignore` & `ifk_smhi-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ifk-smhi-0.1.2/.pre-commit-config.yaml` & `ifk_smhi-0.2.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 repos:
-- repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v2.3.0
-  hooks:
-  - id: check-yaml
-  - id: end-of-file-fixer
-  - id: trailing-whitespace
-- repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.1.5
-  hooks:
-    - id: ruff
-      types_or: [ python, pyi, jupyter ]
-      args: [ --fix ]
-    - id: ruff-format
-      types_or: [ python, pyi, jupyter ]
-- repo: https://github.com/pre-commit/mirrors-mypy
-  rev: "586b4f0"
-  hooks:
-  - id: mypy
-    args: [--no-strict-optional, --ignore-missing-imports]
-- repo: https://github.com/igorshubovych/markdownlint-cli
-  rev: v0.32.2
-  hooks:
-  - id: markdownlint
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v2.3.0
+    hooks:
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.4
+    hooks:
+      - id: ruff
+        types_or: [python, pyi, jupyter]
+        args: [--fix]
+      - id: ruff-format
+        types_or: [python, pyi, jupyter]
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: "586b4f0"
+    hooks:
+      - id: mypy
+        args: [--no-strict-optional, --ignore-missing-imports]
+  - repo: https://github.com/igorshubovych/markdownlint-cli
+    rev: v0.32.2
+    hooks:
+      - id: markdownlint
```

### Comparing `ifk-smhi-0.1.2/LICENSE` & `ifk_smhi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ifk-smhi-0.1.2/PKG-INFO` & `ifk_smhi-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: ifk-smhi
-Version: 0.1.2
+Version: 0.2.0
 Summary: Inspect and get SMHI data.
 Author-email: Anders Nord <dr.anders.nord@gmail.com>, Mladen Gibanica <11275336+mgcth@users.noreply.github.com>
 License: MIT
 Project-URL: homepage, https://ingenjorsarbeteforklimatet.se/ifk-smhi/
 Project-URL: documentation, https://ingenjorsarbeteforklimatet.se/ifk-smhi/
 Project-URL: repository, https://github.com/Ingenjorsarbete-For-Klimatet/ifk-smhi
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.28
-Requires-Dist: pandas~=1.5
+Requires-Dist: pandas~=2.2
 Requires-Dist: geopy~=2.2
 Requires-Dist: arrow~=1.2
+Requires-Dist: shapely~=2.0
+Requires-Dist: pydantic~=2.6
+Requires-Dist: pandera[mypy]~=0.18
 Provides-Extra: lint
-Requires-Dist: ruff~=0.1; extra == "lint"
+Requires-Dist: ruff~=0.3; extra == "lint"
 Provides-Extra: type
 Requires-Dist: mypy~=1.7; extra == "type"
-Requires-Dist: types-requests~=2.28; extra == "type"
+Requires-Dist: types-requests~=2.31; extra == "type"
 Requires-Dist: pandas-stubs~=1.5; extra == "type"
 Provides-Extra: test
 Requires-Dist: pytest~=7.1; extra == "test"
 Requires-Dist: coverage~=6.5; extra == "test"
 Requires-Dist: pytest-cov~=4.0; extra == "test"
 Provides-Extra: doc
 Requires-Dist: mkdocs~=1.4; extra == "doc"
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: ifk-smhi Version: 0.1.2 Summary: Inspect and get
+Metadata-Version: 2.1 Name: ifk-smhi Version: 0.2.0 Summary: Inspect and get
 SMHI data. Author-email: Anders Nord
 gmail.com>, Mladen Gibanica <11275336+mgcth@users.noreply.github.com> License:
 MIT Project-URL: homepage, https://ingenjorsarbeteforklimatet.se/ifk-smhi/
 Project-URL: documentation, https://ingenjorsarbeteforklimatet.se/ifk-smhi/
 Project-URL: repository, https://github.com/Ingenjorsarbete-For-Klimatet/ifk-
 smhi Requires-Python: >=3.9 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests~=2.28 Requires-Dist: pandas~=1.5
-Requires-Dist: geopy~=2.2 Requires-Dist: arrow~=1.2 Provides-Extra: lint
-Requires-Dist: ruff~=0.1; extra == "lint" Provides-Extra: type Requires-Dist:
-mypy~=1.7; extra == "type" Requires-Dist: types-requests~=2.28; extra == "type"
-Requires-Dist: pandas-stubs~=1.5; extra == "type" Provides-Extra: test
+File: LICENSE Requires-Dist: requests~=2.28 Requires-Dist: pandas~=2.2
+Requires-Dist: geopy~=2.2 Requires-Dist: arrow~=1.2 Requires-Dist: shapely~=2.0
+Requires-Dist: pydantic~=2.6 Requires-Dist: pandera[mypy]~=0.18 Provides-Extra:
+lint Requires-Dist: ruff~=0.3; extra == "lint" Provides-Extra: type Requires-
+Dist: mypy~=1.7; extra == "type" Requires-Dist: types-requests~=2.31; extra ==
+"type" Requires-Dist: pandas-stubs~=1.5; extra == "type" Provides-Extra: test
 Requires-Dist: pytest~=7.1; extra == "test" Requires-Dist: coverage~=6.5; extra
 == "test" Requires-Dist: pytest-cov~=4.0; extra == "test" Provides-Extra: doc
 Requires-Dist: mkdocs~=1.4; extra == "doc" Requires-Dist: mkdocs-material~=8.5;
 extra == "doc" Requires-Dist: mkdocstrings[python]~=0.19; extra == "doc"
 Provides-Extra: dev Requires-Dist: ifk-smhi[lint]; extra == "dev" Requires-
 Dist: ifk-smhi[type]; extra == "dev" Requires-Dist: ifk-smhi[test]; extra ==
 "dev" Requires-Dist: ifk-smhi[doc]; extra == "dev" Requires-Dist: pre-
```

### Comparing `ifk-smhi-0.1.2/README.md` & `ifk_smhi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ifk-smhi-0.1.2/docs/assets/favicon.png` & `ifk_smhi-0.2.0/docs/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `ifk-smhi-0.1.2/docs/assets/ifk_logo_black.png` & `ifk_smhi-0.2.0/docs/assets/ifk_logo_black.png`

 * *Files identical despite different names*

### Comparing `ifk-smhi-0.1.2/docs/assets/ifk_logo_white.png` & `ifk_smhi-0.2.0/docs/assets/ifk_logo_white.png`

 * *Files identical despite different names*

### Comparing `ifk-smhi-0.1.2/mkdocs.yml` & `ifk_smhi-0.2.0/mkdocs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 site_name: ifk-smhi
 repo_url: https://github.com/Ingenjorsarbete-For-Klimatet/smhi
 site_author: Mladen Gibanica
 site_url: https://ingenjorsarbete-for-klimatet.github.io/ifk-smhi/
 repo_name: Ingenjorsarbete-For-Klimatet/ifk-smhi
 
 nav:
-- Home: index.md
-- Examples:
-  - "Metobs": metobs-example.md
-  - "Metfcts": metfcts-example.md
-  - "Mesan": mesan-example.md
-  - "Strang": strang-example.md
-- Reference:
-  - "Metobs reference": metobs-reference.md
-  - "Metfcts reference": metfcts-reference.md
-  - "Mesan reference": mesan-reference.md
-  - "Strang reference": strang-reference.md
+  - Home: index.md
+  - Examples:
+      - "Metobs": metobs-example.md
+      - "Metfcts": metfcts-example.md
+      - "Mesan": mesan-example.md
+      - "Strang": strang-example.md
+      - "SMHI": smhi-example.md
+  - Reference:
+      - "Clients":
+          - "Metobs reference": metobs-reference.md
+          - "Metfcts reference": metfcts-reference.md
+          - "Mesan reference": mesan-reference.md
+          - "Strang reference": strang-reference.md
+          - "SMHI reference": smhi-reference.md
+      - "Models":
+          - "Metobs model": metobs-model.md
+          - "Metfcts model": metfcts-model.md
+          - "Mesan model": mesan-model.md
+          - "Strang model": strang-model.md
 
 watch:
-- src/smhi
+  - src/smhi
 
 theme:
   name: material
   custom_dir: material
   palette:
     scheme: default
     primary: black
@@ -32,16 +40,21 @@
     repo: fontawesome/brands/git-alt
   logo: assets/ifk_logo_white.png
   favicon: assets/favicon.png
   features:
     - navigation.tabs
 
 plugins:
-- search
-- mkdocstrings
+  - search
+  - mkdocstrings:
+      handlers:
+        python:
+          options:
+            show_root_heading: true
+            heading_level: 2
 
 markdown_extensions:
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
```

### Comparing `ifk-smhi-0.1.2/pyproject.toml` & `ifk_smhi-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifk-smhi"
-version = "0.1.2"
+version = "0.2.0"
 description = "Inspect and get SMHI data."
 license = { text = "MIT" }
 readme = "README.md"
 authors = [
     { name = "Anders Nord", email = "dr.anders.nord@gmail.com" },
     { name = "Mladen Gibanica", email = "11275336+mgcth@users.noreply.github.com" },
 ]
 requires-python = ">=3.9"
 dependencies = [
     "requests ~= 2.28",
-    "pandas ~= 1.5",
+    "pandas ~= 2.2",
     "geopy ~= 2.2",
     "arrow ~= 1.2",
+    "shapely ~= 2.0",
+    "pydantic ~= 2.6",
+    "pandera[mypy] ~= 0.18"
 ]
 
 [project.urls]
 homepage = "https://ingenjorsarbeteforklimatet.se/ifk-smhi/"
 documentation = "https://ingenjorsarbeteforklimatet.se/ifk-smhi/"
 repository = "https://github.com/Ingenjorsarbete-For-Klimatet/ifk-smhi"
 
 [project.optional-dependencies]
-lint = ["ruff ~= 0.1"]
-type = ["mypy ~= 1.7", "types-requests ~= 2.28", "pandas-stubs ~= 1.5"]
+lint = ["ruff ~= 0.3"]
+type = ["mypy ~= 1.7", "types-requests ~= 2.31", "pandas-stubs ~= 1.5"]
 test = ["pytest ~= 7.1", "coverage ~= 6.5", "pytest-cov ~= 4.0"]
 doc = [
     "mkdocs ~= 1.4",
     "mkdocs-material ~= 8.5",
     "mkdocstrings[python] ~= 0.19",
 ]
 dev = [
@@ -41,7 +44,22 @@
     "ifk-smhi[doc]",
     "pre-commit ~= 2.20",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 exclude = ["material"]
+
+[tool.ruff.lint]
+select = ["E4", "E7", "E9", "F", "N", "I"]
+
+[tool.mypy]
+plugins = [
+  "pydantic.mypy"
+]
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = [
+    "arrow"
+]
+ignore_missing_imports = true
```

### Comparing `ifk-smhi-0.1.2/src/ifk_smhi.egg-info/PKG-INFO` & `ifk_smhi-0.2.0/src/ifk_smhi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: ifk-smhi
-Version: 0.1.2
+Version: 0.2.0
 Summary: Inspect and get SMHI data.
 Author-email: Anders Nord <dr.anders.nord@gmail.com>, Mladen Gibanica <11275336+mgcth@users.noreply.github.com>
 License: MIT
 Project-URL: homepage, https://ingenjorsarbeteforklimatet.se/ifk-smhi/
 Project-URL: documentation, https://ingenjorsarbeteforklimatet.se/ifk-smhi/
 Project-URL: repository, https://github.com/Ingenjorsarbete-For-Klimatet/ifk-smhi
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.28
-Requires-Dist: pandas~=1.5
+Requires-Dist: pandas~=2.2
 Requires-Dist: geopy~=2.2
 Requires-Dist: arrow~=1.2
+Requires-Dist: shapely~=2.0
+Requires-Dist: pydantic~=2.6
+Requires-Dist: pandera[mypy]~=0.18
 Provides-Extra: lint
-Requires-Dist: ruff~=0.1; extra == "lint"
+Requires-Dist: ruff~=0.3; extra == "lint"
 Provides-Extra: type
 Requires-Dist: mypy~=1.7; extra == "type"
-Requires-Dist: types-requests~=2.28; extra == "type"
+Requires-Dist: types-requests~=2.31; extra == "type"
 Requires-Dist: pandas-stubs~=1.5; extra == "type"
 Provides-Extra: test
 Requires-Dist: pytest~=7.1; extra == "test"
 Requires-Dist: coverage~=6.5; extra == "test"
 Requires-Dist: pytest-cov~=4.0; extra == "test"
 Provides-Extra: doc
 Requires-Dist: mkdocs~=1.4; extra == "doc"
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: ifk-smhi Version: 0.1.2 Summary: Inspect and get
+Metadata-Version: 2.1 Name: ifk-smhi Version: 0.2.0 Summary: Inspect and get
 SMHI data. Author-email: Anders Nord
 gmail.com>, Mladen Gibanica <11275336+mgcth@users.noreply.github.com> License:
 MIT Project-URL: homepage, https://ingenjorsarbeteforklimatet.se/ifk-smhi/
 Project-URL: documentation, https://ingenjorsarbeteforklimatet.se/ifk-smhi/
 Project-URL: repository, https://github.com/Ingenjorsarbete-For-Klimatet/ifk-
 smhi Requires-Python: >=3.9 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests~=2.28 Requires-Dist: pandas~=1.5
-Requires-Dist: geopy~=2.2 Requires-Dist: arrow~=1.2 Provides-Extra: lint
-Requires-Dist: ruff~=0.1; extra == "lint" Provides-Extra: type Requires-Dist:
-mypy~=1.7; extra == "type" Requires-Dist: types-requests~=2.28; extra == "type"
-Requires-Dist: pandas-stubs~=1.5; extra == "type" Provides-Extra: test
+File: LICENSE Requires-Dist: requests~=2.28 Requires-Dist: pandas~=2.2
+Requires-Dist: geopy~=2.2 Requires-Dist: arrow~=1.2 Requires-Dist: shapely~=2.0
+Requires-Dist: pydantic~=2.6 Requires-Dist: pandera[mypy]~=0.18 Provides-Extra:
+lint Requires-Dist: ruff~=0.3; extra == "lint" Provides-Extra: type Requires-
+Dist: mypy~=1.7; extra == "type" Requires-Dist: types-requests~=2.31; extra ==
+"type" Requires-Dist: pandas-stubs~=1.5; extra == "type" Provides-Extra: test
 Requires-Dist: pytest~=7.1; extra == "test" Requires-Dist: coverage~=6.5; extra
 == "test" Requires-Dist: pytest-cov~=4.0; extra == "test" Provides-Extra: doc
 Requires-Dist: mkdocs~=1.4; extra == "doc" Requires-Dist: mkdocs-material~=8.5;
 extra == "doc" Requires-Dist: mkdocstrings[python]~=0.19; extra == "doc"
 Provides-Extra: dev Requires-Dist: ifk-smhi[lint]; extra == "dev" Requires-
 Dist: ifk-smhi[type]; extra == "dev" Requires-Dist: ifk-smhi[test]; extra ==
 "dev" Requires-Dist: ifk-smhi[doc]; extra == "dev" Requires-Dist: pre-
```

### Comparing `ifk-smhi-0.1.2/src/smhi/smhi.py` & `ifk_smhi-0.2.0/src/smhi/smhi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,193 @@
 """Read SMHI data."""
+
 import logging
+import time
+from typing import Any, List, Optional, Tuple
+
 import pandas as pd
-from geopy.geocoders import Nominatim
 from geopy import distance
-from typing import Optional, Any, List, Tuple
-from smhi.metobs import Metobs
-from smhi.constants import TYPE_MAP
+from geopy.extra.rate_limiter import RateLimiter
+from geopy.geocoders import Nominatim
+from smhi.metobs import Data, Parameters, Periods, Stations
+from smhi.models.metobs_model import MetobsLinks
+
+logger = logging.getLogger(__name__)
 
 
 class SMHI:
     """SMHI class with high-level functions."""
 
-    def __init__(self, type: str = "json", version: str = "1.0") -> None:
+    def __init__(self) -> None:
         """Initialise SMHI class.
 
-        Args:
-            type: API type
-            version: API version
+        Raises:
+            ValueError
         """
-        self.type = TYPE_MAP[type]
-        self.client = Metobs(type)
-        self.client.get_parameters()
+        self.parameters = Parameters()
 
-    @property
-    def parameters(self):
-        """Get available parameters.
+        if self.parameters is None:
+            raise ValueError("No parameters available.")
 
-        Returns:
-            parameters
-        """
-        return self.client.parameters.data
-
-    def get_stations(self, parameter: Optional[int] = None):
+    def get_stations(self, parameter: Optional[int] = None) -> List[MetobsLinks]:
         """Get stations from parameter.
 
         Args:
             parameter: station parameter
 
         Returns:
             stations
         """
-        if self.client.parameters is None:
-            logging.info("No parameters available.")
-            return None
-
-        self.client.get_stations(parameter)
-        return self.client.stations.data
+        return Stations(self.parameters, parameter).data
 
-    def get_stations_from_title(self, title: Optional[str] = None):
+    def get_stations_from_title(self, title: Optional[str] = None) -> List[MetobsLinks]:
         """Get stations from title.
 
         Args:
             title: station title
 
         Returns:
             stations
         """
-        if self.client.stations is None:
-            logging.info("No stations available.")
-            return None
-
-        self.client.get_stations(None, title)
-        return self.client.stations.data
-
-    def find_stations_from_gps(
-        self, parameter: int, latitude: float, longitude: float, dist: float = 0
-    ) -> None:
+        return Stations(self.parameters, parameter_title=title).data
+
+    def get_data(
+        self,
+        parameter: int,
+        station: int,
+        distance: int = 0,
+    ) -> Tuple[Any, Any]:
+        """Get data from station.
+
+        Args:
+            parameter: data parameter
+            station: station id
+            distance: station distance in km (for interpolation)
+
+        Returns:
+            data
+        """
+        stations = Stations(Parameters(), parameter)
+        periods = Periods(stations, station)
+        data = Data(periods)
+
+        return self._interpolate(distance, stations, periods, data)
+
+    def get_data_by_city(
+        self,
+        parameter: int,
+        city: str,
+        distance: int = 0,
+    ) -> Tuple[Any, Any]:
+        """Get data from station.
+
+        Args:
+            parameter: data parameter
+            city: user provided city
+            distance: station distance in km
+
+        Returns:
+            data
+        """
+        stations = Stations(Parameters(), parameter)
+        station = self._find_stations_by_city(stations, city, distance)[0][0]
+        periods = Periods(stations, station)
+        data = Data(periods)
+
+        return self._interpolate(distance, stations, periods, data)
+
+    def _find_stations_from_gps(
+        self,
+        station_response: Stations,
+        latitude: float,
+        longitude: float,
+        dist: float = 0,
+    ) -> List[Tuple[int, str, float]]:
         """Find stations for parameter from gps location.
 
         Args:
             parameter: station parameter
             latitude: latitude
             longitude: longitude
-            dist: distance from gps location. If zero (default), chooses closest.
+            dist: distance from gps location. If zero (default), chooses closest
 
+        Returns:
+            nearby stations
         """
-        if parameter is None:
-            logging.info("Parameter needed.")
-            return None
+        if not dist:
+            dist = 0
+
+        user_pos = (latitude, longitude)
+        all_stations = station_response.station
+        nearby_stations = [
+            (s.id, s.name, distance.distance(user_pos, (s.latitude, s.longitude)).km)
+            for s in all_stations
+        ]
 
-        user_position = (latitude, longitude)
-        self.get_stations(parameter)
-        self.nearby_stations: List[Tuple[Any, Any, Any]]
-        all_stations = self.client.stations.stations
         if dist == 0:
-            stations = [
-                (
-                    s["id"],
-                    s["name"],
-                    distance.distance(
-                        user_position, (s["latitude"], s["longitude"])
-                    ).km,
-                )
-                for s in all_stations
-            ]
-            self.nearby_stations = min(stations, key=lambda x: x[2])
-
-        else:
-            self.nearby_stations = [
-                (
-                    s["id"],
-                    s["name"],
-                    distance.distance(
-                        user_position, (s["latitude"], s["longitude"])
-                    ).km,
-                )
-                for s in all_stations
-                if distance.distance(user_position, (s["latitude"], s["longitude"]))
-                <= dist
-            ]
-            self.nearby_stations = sorted(self.nearby_stations, key=lambda x: x[2])
+            return [min(nearby_stations, key=lambda x: x[2])]
 
-    def find_stations_by_city(self, parameter: int, city: str, dist: float = 0) -> None:
+        nearby_stations = [x for x in nearby_stations if x[2] <= dist]
+
+        return sorted(nearby_stations, key=lambda x: x[2])
+
+    def _find_stations_by_city(
+        self, station_response: Stations, city: str, dist: float = 0
+    ) -> List[Tuple[int, str, float]]:
         """Find stations for parameter from city name.
 
         Args:
             parameter: station parameter
-            dist: distance from city
+            dist: distance from city in km
             city: name of city
+
+        Returns:
+            nearby stations
         """
         geolocator = Nominatim(user_agent="ifk-smhi")
-        loc = geolocator.geocode(city)
-        self.find_stations_from_gps(
-            parameter=parameter,
-            dist=dist,
-            latitude=loc.latitude,
-            longitude=loc.longitude,
-        )
-
-    def get_data(
-        self,
-        parameter: int,
-        station: int,
-        period: str = "corrected-archive",
-        interpolate: int = 0,
-    ) -> Tuple[Any, Any]:
-        """Get data from station.
+        geocode = RateLimiter(geolocator.geocode, min_delay_seconds=1)
+        loc = geocode(city)
 
-        Args:
-            parameter: data parameter
-            station: station id
-            period: period to get
-        """
-        data, header = self.client.get_data_from_selection(
-            parameter=parameter, station=station, period=period
+        return self._find_stations_from_gps(
+            station_response, latitude=loc.latitude, longitude=loc.longitude, dist=dist
         )
-        if interpolate > 0:
-            # Find the station latitude and longitude information from Metobs
-            stat = next(
-                item for item in self.client.stations.stations if item["id"] == station
-            )
-            latitude = stat["latitude"]
-            longitude = stat["longitude"]
-
-            holes_to_fill = data[
-                data.index.to_series().diff() > data.index.to_series().diff().median()
-            ]
-            # Find stations within a given radius - set in "interpolate".
-            self.find_stations_from_gps(
-                parameter=parameter,
-                latitude=latitude,
-                longitude=longitude,
-                dist=interpolate,
-            )
-
-            # Iterate over nearby stations, starting with the closest
-            for nearby_station in self.nearby_stations[1:]:
-                tmpdata, _ = self.get_data(parameter, nearby_station[0])
-                for time, _ in holes_to_fill.iterrows():
-                    earliertime = data[data.index < time].index.max()
-
-                    if (
-                        len(
-                            tmpdata[
-                                (tmpdata.index > earliertime) & (tmpdata.index < time)
-                            ]
-                        )
-                        > 0
-                    ):
-                        data = pd.concat([data, tmpdata], axis=0, join="outer")
-
-                # Re-check how many holes remain
-                holes_to_fill = data[
-                    data.index.to_series().diff()
-                    > data.index.to_series().diff().median()
-                ]
-        data = data.sort_index()
-        return data, header
+
+    def _interpolate(
+        self, distance: float, stations: Stations, periods: Periods, data: Data
+    ) -> Data:
+        """Interpolate data from several stations based on allowed distance."""
+        if not distance:
+            return data
+
+        if distance <= 0:
+            return data
+
+        lat, lon = (periods.position[0].latitude, periods.position[0].longitude)
+        missing_df = self._find_missing_data(data.df)
+        all_nearby_stations = self._find_stations_from_gps(stations, lat, lon, distance)
+
+        for nearby_station in all_nearby_stations[1:]:
+            time.sleep(1)
+            nearby_data = Data(Periods(stations, nearby_station[0]))
+            data.df = self._iterate_over_time(data.df, nearby_data.df, missing_df)
+            missing_df = self._find_missing_data(data.df)
+
+        data.df = data.df.sort_index()
+
+        return data
+
+    def _iterate_over_time(
+        self, df: pd.DataFrame, nearby_df: pd.DataFrame, missing_df: pd.DataFrame
+    ) -> pd.DataFrame:
+        """Iterate over time."""
+        for tajm, _ in missing_df.iterrows():
+            earliertime = df[df.index < tajm].index.max()
+            condition = (nearby_df.index > earliertime) & (nearby_df.index < tajm)
+
+            if len(nearby_df[condition]) > 0:
+                df = pd.concat([df, nearby_df], axis=0, join="outer")
+
+        return df
+
+    def _find_missing_data(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Find missing data."""
+        return df[df.index.to_series().diff() > df.index.to_series().diff().median()]
```

### Comparing `ifk-smhi-0.1.2/src/smhi/strang.py` & `ifk_smhi-0.2.0/src/smhi/strang.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,221 +1,245 @@
 """SMHI Strang client.
 
 See validation of model: https://strang.smhi.se/validation/validation.html
 """
+
 import json
-import arrow
-import requests
 import logging
-import pandas as pd
-from functools import partial
 from collections import defaultdict
-from typing import Optional, Any
+from enum import Enum
+from functools import partial
+from typing import Any, Optional
+
+import arrow
+import pandas as pd
 from requests.structures import CaseInsensitiveDict
 from smhi.constants import (
-    STRANG,
-    STRANG_EMPTY,
-    STRANG_POINT_URL,
-    STRANG_PARAMETERS,
     STRANG_MULTIPOINT_URL,
+    STRANG_PARAMETERS,
+    STRANG_POINT_URL,
     STRANG_TIME_INTERVALS,
 )
+from smhi.models.strang_model import (
+    StrangMultiPoint,
+    StrangParameter,
+    StrangPoint,
+)
+from smhi.utils import format_datetime, get_request
+
+logger = logging.getLogger(__name__)
+
+
+class RequestType(Enum):
+    POINT = 1
+    MULTIPOINT = 2
 
 
 class Strang:
     """SMHI Strang class. Only supports category strang1g and version 1."""
 
     def __init__(self) -> None:
         """Initialise Strang object."""
         self._category = "strang1g"
         self._version = 1
 
-        self.latitude: Optional[float] = None
-        self.longitude: Optional[float] = None
-        self.parameter: STRANG = STRANG_EMPTY
-        self.time_from: Optional[str] = None
-        self.time_to: Optional[str] = None
-        self.valid_time: Optional[str] = None
-        self.time_interval: Optional[str] = None
-        self.status: Optional[bool] = None
-        self.header: Optional[CaseInsensitiveDict[str]] = None
-        self.available_parameters: defaultdict[int, STRANG] = STRANG_PARAMETERS
-        self.point_raw_url: partial[str] = partial(
+        self._point_raw_url: partial[str] = partial(
             STRANG_POINT_URL.format, category=self._category, version=self._version
         )
-        self.multipoint_raw_url: partial[str] = partial(
+        self._multipoint_raw_url: partial[str] = partial(
             STRANG_MULTIPOINT_URL.format, category=self._category, version=self._version
         )
-        self.point_url: Optional[str] = None
-        self.multipoint_url: Optional[str] = None
+        self._point_url: Optional[str] = None
+        self._multipoint_url: Optional[str] = None
+        self._available_parameters: defaultdict[int, StrangParameter] = (
+            STRANG_PARAMETERS
+        )
 
     @property
     def parameters(
         self,
     ) -> list[int]:
         """Get parameters property.
 
         Returns:
             available parameters
         """
-        for key, value in self.available_parameters.items():
-            logging.info(
+        for key, value in self._available_parameters.items():
+            logger.info(
                 "parameter: {parameter}, info: {meaning}".format(
                     parameter=key, meaning=value.meaning
                 )
             )
 
-        return list(self.available_parameters.keys())
+        return list(self._available_parameters.keys())
 
     def get_point(
         self,
         latitude: float,
         longitude: float,
         parameter: int,
         time_from: Optional[str] = None,
         time_to: Optional[str] = None,
         time_interval: Optional[str] = None,
-    ) -> Any:
+    ) -> StrangPoint:
         """Get data for given lon, lat and parameter.
 
         Args:
             latitude: latitude
             longitude: longitude
             parameter: parameter
             time_from: get data from (optional),
             time_to: get data to (optional),
             time_interval: interval of data
                            [valid values: hourly, daily, monthly] (optional)
 
         Returns:
-            data: data
+            strange point model
 
         Raises:
-            TypeError: wrong type of latitude and/or longitude
+            ValueError: wrong value of latitude and/or longitude
             NotImplementedError: parameter not supported
         """
-        strang_parameter = self.available_parameters[parameter]
-        if strang_parameter.parameter is None:
+        strang_parameter = self._available_parameters[parameter]
+        if strang_parameter.key is None:
             raise NotImplementedError(
                 "Parameter not implemented."
                 + " Try client.parameters to list available parameters."
             )
 
         if longitude is None or latitude is None:
-            raise TypeError("Wrong type of latitude and/or longitude provided.")
+            raise ValueError("Wrong value of latitude and/or longitude provided.")
 
-        self.longitude = longitude
-        self.latitude = latitude
-        self.parameter = strang_parameter
-        self.time_from = time_from
-        self.time_to = time_to
-        self.time_interval = time_interval
-
-        url = self.point_raw_url
-        url = self._build_base_point_url(url)
-        url = self._build_time_point_url(url)
-        data, header, status = self._get_and_load_data(url)
-        self.header = header
-        self.status = status
-        self.point_url = url
+        time_from = self._parse_datetime(time_from, strang_parameter)
+        time_to = self._parse_datetime(time_to, strang_parameter)
 
-        return data
+        raw_url = self._point_raw_url
+        url = self._build_base_point_url(raw_url, strang_parameter, longitude, latitude)
+        url = self._build_time_point_url(url, time_from, time_to, time_interval)
+        data, header, status = self._get_and_load_data(url, RequestType["POINT"])
+
+        return StrangPoint(
+            parameter_key=strang_parameter.key,
+            parameter_meaning=strang_parameter.meaning,
+            longitude=longitude,
+            latitude=latitude,
+            time_from=time_from,
+            time_to=time_to,
+            time_interval=time_interval,
+            url=url,
+            status=status,
+            headers=header,
+            df=data,
+        )
 
     def get_multipoint(
         self, parameter: int, valid_time: str, time_interval: Optional[str] = None
-    ) -> Any:
+    ) -> StrangMultiPoint:
         """Get full spatial data for given parameter and time.
 
         Args:
             parameter: parameter
             valid_time: valid time
             time_interval: interval of data
                            [valid values: hourly,
                             daily, monthly] (optional)
 
         Returns:
-            data: data
+            strange multipoint model
 
         Raises:
             TypeError: wrong type of valid time
             NotImplementedError: parameter not supported
         """
-        parameter = self.available_parameters[parameter]
-        if parameter.parameter is None:
+        strang_parameter = self._available_parameters[parameter]
+        if strang_parameter.key is None:
             raise NotImplementedError(
                 "Parameter not implemented."
                 + " Try client.parameters to list available parameters."
             )
 
         try:
             valid_time = arrow.get(valid_time).isoformat()
         except TypeError:
             raise TypeError("Wrong type of valid time provided. Check valid time.")
 
-        self.parameter = parameter
-        self.valid_time = arrow.get(valid_time).isoformat()
-        self.time_interval = time_interval
-
-        url = self.multipoint_raw_url
-        url = self._build_base_multipoint_url(url)
-        url = self._build_time_multipoint_url(url)
-        data, header, status = self._get_and_load_data(url)
-        self.header = header
-        self.status = status
-        self.multipoint_url = url
-
-        return data
+        raw_url = self._multipoint_raw_url
+        url = self._build_base_multipoint_url(raw_url, strang_parameter, valid_time)
+        url = self._build_time_multipoint_url(url, time_interval)
+        data, header, status = self._get_and_load_data(url, RequestType["MULTIPOINT"])
+
+        return StrangMultiPoint(
+            parameter_key=strang_parameter.key,
+            parameter_meaning=strang_parameter.meaning,
+            valid_time=valid_time,
+            time_interval=time_interval,
+            url=url,
+            status=status,
+            headers=header,
+            df=data,
+        )
 
-    def _build_base_point_url(self, url: partial[str]) -> str:
+    def _build_base_point_url(
+        self,
+        url: partial[str],
+        parameter: StrangParameter,
+        longitude: float,
+        latitude: float,
+    ) -> str:
         """Build base point url.
 
         Args:
             url: url to format
+            parameter: strang parameter
+            longitude: longitude
+            latitude: latitude
 
         Returns:
             formatted url string
         """
-        return url(
-            lon=self.longitude,
-            lat=self.latitude,
-            parameter=self.parameter.parameter,
-        )
+        return url(lon=longitude, lat=latitude, parameter=parameter.key)
 
-    def _build_base_multipoint_url(self, url: partial[str]) -> str:
+    def _build_base_multipoint_url(
+        self, url: partial[str], parameter: StrangParameter, valid_time: str
+    ) -> str:
         """
         Build base point url.
 
         Args:
             url: url to format
+            parameter: strang parameter
+            valid_time: valid time for call
 
         Returns:
             formatted url string
         """
-        return url(
-            validtime=self.valid_time,
-            parameter=self.parameter.parameter,
-        )
+        return url(validtime=valid_time, parameter=parameter.key)
 
-    def _build_time_point_url(self, url: str) -> str:
+    def _build_time_point_url(
+        self,
+        url: str,
+        time_from: Optional[str],
+        time_to: Optional[str],
+        time_interval: Optional[str],
+    ) -> str:
         """Build date part of the API url.
 
         Args:
             url: formatted url string
+            time_from: from time
+            time_to: to time
+            time_interval: interval
 
         Returns:
             url string
 
         Raises:
             ValueError: time_interval not valid
             NotImplementedError: date out of bounds
         """
-        time_from = self._parse_datetime(self.time_from)
-        time_to = self._parse_datetime(self.time_to)
-        time_interval = self.time_interval
-
         if any([time_from, time_to, time_interval]) is True:
             url += "?"
 
         if time_from is not None:
             url += "from={time_from}".format(time_from=time_from)
 
         if time_to is not None:
@@ -231,125 +255,113 @@
         if time_interval is not None and (time_from is not None or time_to is not None):
             if time_interval not in STRANG_TIME_INTERVALS:
                 raise ValueError("Time interval must be hourly, daily or monthly.")
             url += "&interval={interval}".format(interval=time_interval)
 
         return url
 
-    def _build_time_multipoint_url(self, url: str) -> str:
+    def _build_time_multipoint_url(self, url: str, time_interval: Optional[str]) -> str:
         """Build date part of the API url.
 
         Args:
             url: formatted url string
+            time_interval: time interval
 
         Returns:
             url string
 
         Raises:
             ValueError
         """
-        time_interval = self.time_interval
-
         if time_interval is not None:
             if time_interval not in STRANG_TIME_INTERVALS:
                 raise ValueError("Time interval must be hourly, daily or monthly.")
             url += "?interval={interval}".format(interval=time_interval)
 
         return url
 
     def _get_and_load_data(
-        self, url: str
-    ) -> tuple[pd.DataFrame, CaseInsensitiveDict[str], bool]:
+        self, url: str, request: RequestType
+    ) -> tuple[pd.DataFrame, CaseInsensitiveDict[str], int]:
         """Fetch requested point data and parse it with datetime.
 
         Args:
             url: url to fetch from
 
         Returns:
             data
             header
-            status
+            status code
         """
-        response = requests.get(url)
-        status = response.ok
-        header = response.headers
-
-        if status is True:
-            data = json.loads(response.content)
-
-            if "date_time" in data[0]:
-                data = self._parse_point_data(data)
-            else:
-                data = self._parse_multipoint_data(data)
+        response = get_request(url)
+        data = df = json.loads(response.content)
 
-            return data, header, status
+        if request == RequestType.POINT:
+            df = self._parse_point_data(data)
         else:
-            logging.info("No data returned.")
+            df = self._parse_multipoint_data(data)
 
-            return pd.DataFrame(), header, status
+        return df, response.headers, response.status_code
 
-    def _parse_datetime(self, date_time: Optional[str]) -> Optional[str]:
+    def _parse_datetime(
+        self, date_time: Optional[str], parameter: StrangParameter
+    ) -> Optional[str]:
         """Parse date into a datetime format given as string and check bounds.
 
         Args:
             date_time: date as string
+            parameter: strang parameter
 
         Returns:
             parsed date
 
         Raises:
             ValueError
         """
         if date_time is None:
             return date_time
 
         try:
-            date_time_arrow = arrow.get(date_time)
+            date_time_arrow = arrow.get(format_datetime(date_time))
         except ValueError:
             raise ValueError("Wrong format of date.")
 
-        if self.parameter.time_from < date_time_arrow < self.parameter.time_to():
+        if parameter.time_from < date_time_arrow < parameter.time_to():
             return date_time_arrow.isoformat()
         else:
             raise ValueError(
                 "Time not in allowed interval: {time_from} to {time_to}.".format(
-                    time_from=self.parameter.time_from, time_to=self.parameter.time_to()
+                    time_from=parameter.time_from, time_to=parameter.time_to()
                 )
             )
 
-    def _parse_point_data(self, data: list) -> pd.DataFrame:
+    def _parse_point_data(
+        self, data: list[CaseInsensitiveDict[Any]]
+    ) -> Optional[pd.DataFrame]:
         """Parse point data into a pandas DataFrame.
 
         Args:
-            data: data as a list
+            url: url of request
 
         Returns
-            data_pd: pandas dataframe
+            pandas dataframe
         """
         for entry in data:
             entry["date_time"] = arrow.get(entry["date_time"]).datetime
 
         data_pd = pd.DataFrame(data)
         data_pd.set_index("date_time", inplace=True)
-        data_pd.rename(columns={"value": self.parameter[1]}, inplace=True)
 
         return data_pd
 
-    def _parse_multipoint_data(self, data: list) -> pd.DataFrame:
+    def _parse_multipoint_data(
+        self, data: list[CaseInsensitiveDict[Any]]
+    ) -> pd.DataFrame:
         """Parse multipoint data into a pandas DataFrame.
 
         Args:
             data: data as a list
 
         Returns
             data_pd: pandas dataframe
         """
-        data_pd = pd.DataFrame(data)
-        data_pd.rename(
-            columns={
-                "value": str(self.parameter[1])
-                + " {0} {1}".format(self.valid_time, self.time_interval)
-            },
-            inplace=True,
-        )
-
-        return data_pd
+        return pd.DataFrame(data)
```

### Comparing `ifk-smhi-0.1.2/tests/fixtures/STRANG_RESULT_HOURLY_2020_01_01_2020_01_02.csv` & `ifk_smhi-0.2.0/tests/fixtures/strang/strang_result_hourly_2020_01_01_2020_01_02.csv`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-date_time,Direct normal irradiance [W/m²]
+date_time,value
 2020-01-01 00:00:00+00:00,0.0
 2020-01-01 01:00:00+00:00,0.0
 2020-01-01 02:00:00+00:00,0.0
 2020-01-01 03:00:00+00:00,0.0
 2020-01-01 04:00:00+00:00,0.0
 2020-01-01 05:00:00+00:00,0.0
 2020-01-01 06:00:00+00:00,0.0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

