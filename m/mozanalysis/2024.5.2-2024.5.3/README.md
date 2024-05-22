# Comparing `tmp/mozanalysis-2024.5.2.tar.gz` & `tmp/mozanalysis-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozanalysis-2024.5.2.tar", last modified: Wed May 15 17:24:51 2024, max compression
+gzip compressed data, was "mozanalysis-2024.5.3.tar", last modified: Wed May 22 16:16:06 2024, max compression
```

## Comparing `mozanalysis-2024.5.2.tar` & `mozanalysis-2024.5.3.tar`

### file list

```diff
@@ -1,106 +1,95 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.605057 mozanalysis-2024.5.2/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.593057 mozanalysis-2024.5.2/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4142 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1238 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      985 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2024-05-15 17:24:51.605057 mozanalysis-2024.5.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2627 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.593057 mozanalysis-2024.5.2/docs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.593057 mozanalysis-2024.5.2/docs/_ext/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/_ext/metrics_docstrings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/about.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.593057 mozanalysis-2024.5.2/docs/adrs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4532 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/adrs/adr-0001-dependency_management.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.597056 mozanalysis-2024.5.2/docs/api/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.597056 mozanalysis-2024.5.2/docs/api/bayesian_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/bayesian_stats/bayesian_bootstrap.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/bayesian_stats/binary.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/bayesian_stats/survival_func.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/bayesian_stats.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/bq.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/config.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/experiment.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/exposure.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.597056 mozanalysis-2024.5.2/docs/api/frequentist_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/frequentist_stats/bootstrap.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/frequentist_stats/sample_size.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.597056 mozanalysis-2024.5.2/docs/api/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/metrics/desktop.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/metrics/fenix.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/metrics/firefox_ios.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/metrics.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.597056 mozanalysis-2024.5.2/docs/api/segments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/segments/desktop.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/segments.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api/sizing.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5711 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15311 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      231 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/ruff.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2024-05-15 17:24:51.609057 mozanalysis-2024.5.2/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1318 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.593057 mozanalysis-2024.5.2/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.597056 mozanalysis-2024.5.2/src/mozanalysis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.601056 mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9493 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11573 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8539 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/binary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5892 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/survival_func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3172 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/bq.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8771 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    57151 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/experiment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3557 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/exposure.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.601056 mozanalysis-2024.5.2/src/mozanalysis/frequentist_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/frequentist_stats/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10768 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/frequentist_stats/bootstrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17262 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/frequentist_stats/linear_models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34453 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/frequentist_stats/sample_size.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.601056 mozanalysis-2024.5.2/src/mozanalysis/metrics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14870 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/metrics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/metrics/desktop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1033 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/metrics/fenix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      829 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/metrics/firefox_ios.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/metrics/focus_android.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/metrics/focus_ios.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      836 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/metrics/klar_android.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/metrics/klar_ios.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.601056 mozanalysis-2024.5.2/src/mozanalysis/segments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8362 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/segments/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/segments/desktop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25702 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/sizing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4039 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/src/mozanalysis/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.605057 mozanalysis-2024.5.2/src/mozanalysis.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2024-05-15 17:24:51.000000 mozanalysis-2024.5.2/src/mozanalysis.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2537 2024-05-15 17:24:51.000000 mozanalysis-2024.5.2/src/mozanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-15 17:24:51.000000 mozanalysis-2024.5.2/src/mozanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2024-05-15 17:24:51.000000 mozanalysis-2024.5.2/src/mozanalysis.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-05-15 17:24:51.000000 mozanalysis-2024.5.2/src/mozanalysis.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.605057 mozanalysis-2024.5.2/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.605057 mozanalysis-2024.5.2/tests/bayesian_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/bayesian_stats/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7054 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/bayesian_stats/test_bayesian_bootstrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2287 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/bayesian_stats/test_binary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5514 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/bayesian_stats/test_consistency.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3358 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/bayesian_stats/test_init.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3990 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/bayesian_stats/test_survival_func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.605057 mozanalysis-2024.5.2/tests/frequentist_stats/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/frequentist_stats/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9479 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/frequentist_stats/test_bootstrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20560 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/frequentist_stats/test_linear_models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9096 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/frequentist_stats/test_sample_size_calc.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 17:24:51.605057 mozanalysis-2024.5.2/tests/helpers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/helpers/cheap_lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5117 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26177 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/test_experiment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1523 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/test_metric_libraries.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1282 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/test_metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2584 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/test_segment_libraries.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7936 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/test_sizing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1106 2024-05-15 17:24:40.000000 mozanalysis-2024.5.2/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.726232 mozanalysis-2024.5.3/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.714232 mozanalysis-2024.5.3/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4120 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/.circleci/config.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.714232 mozanalysis-2024.5.3/.github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/.github/dependabot.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1238 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      985 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5041 2024-05-22 16:16:06.726232 mozanalysis-2024.5.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3597 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.714232 mozanalysis-2024.5.3/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.714232 mozanalysis-2024.5.3/docs/_ext/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/_ext/metrics_docstrings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/about.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.714232 mozanalysis-2024.5.3/docs/adrs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4532 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/adrs/adr-0001-dependency_management.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.714232 mozanalysis-2024.5.3/docs/api/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.714232 mozanalysis-2024.5.3/docs/api/bayesian_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/bayesian_stats/bayesian_bootstrap.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/bayesian_stats/binary.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/bayesian_stats/survival_func.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/bayesian_stats.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/bq.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/config.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/experiment.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/exposure.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.718232 mozanalysis-2024.5.3/docs/api/frequentist_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/frequentist_stats/bootstrap.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/frequentist_stats/sample_size.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/metrics.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/segments.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api/sizing.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5711 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15311 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      231 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9439 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/requirements-dev.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102507 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/requirements-dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5600 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/requirements.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    99277 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.718232 mozanalysis-2024.5.3/script/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      413 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/script/update_deps
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-22 16:16:06.726232 mozanalysis-2024.5.3/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.710231 mozanalysis-2024.5.3/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.718232 mozanalysis-2024.5.3/src/mozanalysis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.718232 mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9493 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11573 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8539 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/binary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5892 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/survival_func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3172 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/bq.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8771 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57290 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/experiment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3557 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/exposure.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.718232 mozanalysis-2024.5.3/src/mozanalysis/frequentist_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/frequentist_stats/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10768 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/frequentist_stats/bootstrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18398 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/frequentist_stats/linear_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34453 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/frequentist_stats/sample_size.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14290 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7706 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/segments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26053 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/sizing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4039 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/src/mozanalysis/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.722232 mozanalysis-2024.5.3/src/mozanalysis.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5041 2024-05-22 16:16:06.000000 mozanalysis-2024.5.3/src/mozanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2161 2024-05-22 16:16:06.000000 mozanalysis-2024.5.3/src/mozanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-22 16:16:06.000000 mozanalysis-2024.5.3/src/mozanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      361 2024-05-22 16:16:06.000000 mozanalysis-2024.5.3/src/mozanalysis.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-05-22 16:16:06.000000 mozanalysis-2024.5.3/src/mozanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.722232 mozanalysis-2024.5.3/tests/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.722232 mozanalysis-2024.5.3/tests/bayesian_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/bayesian_stats/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7054 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/bayesian_stats/test_bayesian_bootstrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2287 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/bayesian_stats/test_binary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5514 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/bayesian_stats/test_consistency.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3358 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/bayesian_stats/test_init.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3990 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/bayesian_stats/test_survival_func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.722232 mozanalysis-2024.5.3/tests/frequentist_stats/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/frequentist_stats/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9479 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/frequentist_stats/test_bootstrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22576 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/frequentist_stats/test_linear_models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9254 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/frequentist_stats/test_sample_size_calc.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 16:16:06.722232 mozanalysis-2024.5.3/tests/helpers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/helpers/cheap_lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2729 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/helpers/config_loader_lists.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5146 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25326 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/test_experiment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1282 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/test_metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8084 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/test_sizing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1165 2024-05-22 16:15:21.000000 mozanalysis-2024.5.3/tox.ini
```

### Comparing `mozanalysis-2024.5.2/.circleci/config.yml` & `mozanalysis-2024.5.3/.circleci/config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -57,19 +57,19 @@
     docker:
       - image: cimg/python:3.10
     steps:
       - checkout
       - run:
           name: Install deployment tools
           command: |
-            pip install --upgrade setuptools wheel twine
+            pip install -r requirements.txt
       - run:
           name: Create the distribution files
           command: |
-            python setup.py sdist bdist_wheel
+            python3 -m build --sdist
       - run:
           name: Upload to PyPI
           command: |
             # Relies on the TWINE_USERNAME and TWINE_PASSWORD environment variables configured at:
             #   https://circleci.com/gh/mozilla/mozanalysis/edit#env-vars
             # For more on twine, see:
             #   https://twine.readthedocs.io/en/latest/
```

### Comparing `mozanalysis-2024.5.2/.gitignore` & `mozanalysis-2024.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/CHANGELOG.rst` & `mozanalysis-2024.5.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/CODE_OF_CONDUCT.md` & `mozanalysis-2024.5.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/LICENSE` & `mozanalysis-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/README.md` & `mozanalysis-2024.5.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,30 +10,39 @@
 
 ##  Installation from pypi
 - To install this package from pypi run:
 ```
 pip install mozanalysis
 ```
 
+## Local Installation
+### Dependencies
+Dependencies are specified in the `requirements.txt` and `requirements-dev.txt` files, which are used for testing and development respecitvely.
+To create a virtualenv and set up the package execute the following, replacing `requirements.txt` with `requirements-dev.txt` if you plan on contributing to the package.
+```bash
+# Create and activate a python virtual environment.
+python3 -m venv venv/
+source venv/bin/activate
+pip install -r requirements.txt
+pip install -e . --no-dependencies
+```
+
 ## Development
 Linting and Formatting are done with Ruff.
 
+When adding new dependencies, add them to the `pyproject.toml` `dependencies` list.  Then generate updated requirements files using the script `script/update_deps`.  [`pip-compile` is called](https://pypi.org/project/pip-tools/) in this script, which uses the specified dependencies to create the `requirements.txt` and `requirements-dev.txt` files.  Finally, you'll want to update the requirements in your virtual env by running `pip install -r requirements-dev.txt`
+
 ## Testing locally
 
 ### With pytest
-First one must ensure that all the test dependencies are installed.  To do so, navigate to the root of the repo and run
-```
-pip install -e ".[testing]"
-```
-
-Then run `pytest` on the commandline
+Run `pytest` on the commandline from the root of the package file structure.
 
 ### with Tox
 
-Install tox into your global Python environment and run `tox`.
+Tox is included in the dev dependencies.  If you want to run with tox, install the dev dependencies in the `requirements-dev.txt` as detailed above.
 
 You can pass flags to tox to limit the different environments you test in
 or the tests you run. Options after `--` or positional arguments are forwarded to pytest.
 
 For example, you can run:
 
 * `tox -e lint` to lint
```

### Comparing `mozanalysis-2024.5.2/docs/_ext/metrics_docstrings.py` & `mozanalysis-2024.5.3/docs/_ext/metrics_docstrings.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/docs/adrs/adr-0001-dependency_management.md` & `mozanalysis-2024.5.3/docs/adrs/adr-0001-dependency_management.md`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/docs/conf.py` & `mozanalysis-2024.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/docs/guide.rst` & `mozanalysis-2024.5.3/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/setup.py` & `mozanalysis-2024.5.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,71 @@
-#!/usr/bin/env python
+[build-system]
+requires = ["setuptools>=64", "setuptools_scm>=8", "pytest-runner", "setuptools_scm"]
+build-backend = "setuptools.build_meta"
 
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at http://mozilla.org/MPL/2.0/.
-from setuptools import find_packages, setup
+[project]
+name= "mozanalysis"
+dynamic = ["version"]
+authors=[{name = "Mozilla Corporation", email="fx-data-dev@mozilla.org"}]
+description="A library for Mozilla experiments analysis"
+requires-python=">=3.10,<=3.11"
+dependencies=[
+    "attrs",
+    "mozilla-metric-config-parser>=2024.4.1",
+    "numpy",
+    "pandas",
+    "pyarrow",
+    "scipy",
+    "google-cloud-bigquery",
+    "google-cloud-bigquery-storage",
+    "statsmodels",
+    "marginaleffects==0.0.11",
+    "matplotlib",
+    "SecretStorage"
+]
+readme = "README.md"
+
+[project.urls]
+Repository = "https://github.com/mozilla/mozanalysis"
+Documentation = "https://mozilla.github.io/mozanalysis/"
 
-tests_require = [
+[project.optional-dependencies]
+docs = ["Sphinx", "sphinx-autobuild", "sphinx-rtd-theme"]
+testing = [
     "mock",
     "pytest",
     "pytest-ruff",
     "pytest-cov",
     "pytest-timeout",
-    "ruff==0.3.1",
+    "ruff==0.4.4",
+    'build',
+    'twine'
 ]
+dev = ['pip-tools', 'tox', "mozanalysis[testing]"]
+
+[tool.setuptools_scm]
 
-docs_require = ["Sphinx", "sphinx-autobuild", "sphinx-rtd-theme"]
+[tool.ruff]
+line-length=88
+exclude = [".git","__pycache__"]
+target-version = "py310"
+
+[tool.ruff.lint]
+ignore= ["E741", "RUF005"]
+select = [
+    "E", # pycodestyle
+    "W", # pycodestyle
+    "F", # Pyflakes
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
+    "I", # isort
+    "SIM", # flake8-simplify
+    "TCH", # flake8-type-checking
+    "TID", # flake8-tidy-imports
+    "Q", # flake8-quotes
+    "UP", # pyupgrade
+    "PT", # flake8-pytest-style
+    "RUF", # Ruff-specific rules
+]
 
-setup(
-    name="mozanalysis",
-    use_scm_version=True,
-    author="Mozilla Corporation",
-    author_email="fx-data-dev@mozilla.org",
-    description="A library for Mozilla experiments analysis",
-    url="https://github.com/mozilla/mozanalysis",
-    packages=find_packages(where="src"),
-    package_dir={"": "src"},
-    python_requires=">=3.10,<=3.11",
-    install_requires=[
-        "attrs",
-        "mozilla-metric-config-parser>=2024.4.1",
-        "numpy",
-        "pandas",
-        "pyarrow",
-        "scipy",
-        "google-cloud-bigquery",
-        "google-cloud-bigquery-storage",
-        "statsmodels",
-        "marginaleffects==0.0.11",
-        "matplotlib",
-    ],
-    setup_requires=["pytest-runner", "setuptools_scm"],
-    extras_require={
-        "testing": tests_require,
-        "docs": docs_require,
-    },
-    tests_require=tests_require,
-)
+[tool.pytest.ini_options]
+norecursedirs = "tests/helpers"
```

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/__init__.py` & `mozanalysis-2024.5.3/src/mozanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/__init__.py` & `mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py` & `mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/bayesian_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/binary.py` & `mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/binary.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/bayesian_stats/survival_func.py` & `mozanalysis-2024.5.3/src/mozanalysis/bayesian_stats/survival_func.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/bq.py` & `mozanalysis-2024.5.3/src/mozanalysis/bq.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/config.py` & `mozanalysis-2024.5.3/src/mozanalysis/config.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/experiment.py` & `mozanalysis-2024.5.3/src/mozanalysis/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,18 @@
 
         from google.colab import auth
         auth.authenticate_user()
         print('Authenticated')
 
         from mozanalysis.experiment import Experiment
         from mozanalysis.bq import BigQueryContext
-        from mozanalysis.metrics.desktop import active_hours, uri_count
+        from mozanalysis.config import ConfigLoader
+
+        active_hours = ConfigLoader.get_metric("active_hours", "firefox_desktop")
+        uri_count = ConfigLoader.get_metric("uri_count", "firefox_desktop")
 
         bq_context = BigQueryContext(
             dataset_id='your-dataset-id',  # e.g. mine's flawrence
             project_id='moz-fx-data-bq-data-science'  # this is the default anyway
         )
 
         experiment = Experiment(
```

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/exposure.py` & `mozanalysis-2024.5.3/src/mozanalysis/exposure.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/frequentist_stats/bootstrap.py` & `mozanalysis-2024.5.3/src/mozanalysis/frequentist_stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/frequentist_stats/linear_models.py` & `mozanalysis-2024.5.3/src/mozanalysis/frequentist_stats/linear_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 import re
+import warnings
 
 import numpy as np
 import pandas as pd
 import statsmodels.formula.api as smf
 from marginaleffects import avg_comparisons
 from statsmodels.regression.linear_model import RegressionResults
 from statsmodels.stats.weightstats import DescrStatsW
@@ -140,15 +141,14 @@
     if pattern.findall(target):
         raise ValueError(f"Target variable {target} contains invalid character")
     if pattern.findall(ref_branch):
         raise ValueError(f"Reference branch {ref_branch} contains invalid character")
     if covariate is not None and pattern.findall(covariate):
         raise ValueError(f"Covariate {covariate} contains invalid character")
 
-
     formula = f"{target} ~ C(branch, Treatment(reference='{ref_branch}'))"
     if covariate is not None:
         formula += f" + {covariate}"
 
     return formula
 
 
@@ -255,26 +255,55 @@
         output.loc[("rel_uplift", high_str)] = ac["conf_high"][0] - 1
         output.loc[("rel_uplift", "0.5")] = ac["estimate"][0] - 1
         output.loc[("rel_uplift", "exp")] = ac["estimate"][0] - 1
 
     return output
 
 
-def fit_model(formula: str, df: pd.DataFrame) -> RegressionResults:
+def fit_model(
+    df: pd.DataFrame,
+    target: str,
+    ref_branch: str,
+    treatment_branches: list[str],
+    covariate: str | None = None,
+) -> RegressionResults | None:
     """Fits a linear regression model to `df` using the provided formula. See
     `_make_formula` for a more in-depth discussion on the model structure.
 
     Parameters:
     - formula (str): the model formula (such as the output of `_make_formula`)
     - df (pd.DataFrame): the model data (such as the output of `make_model_df`)
 
     Returns:
     - results (RegressionResults): the fitted model results object.
     """
-    results = smf.ols(formula, df).fit()
+    formula = _make_formula(target, ref_branch, covariate)
+    try:
+        results = smf.ols(formula, df).fit(method="qr")
+    except np.linalg.LinAlgError as lae:
+        if covariate is None:
+            # nothing we can do about this
+            raise lae
+        else:
+            # maybe covariate is bad (e.g., pre-treatment covariate in
+            # onboarding experiment is always zero), try falling back to
+            # unadjusted inferences
+            formula = _make_formula(target, ref_branch, None)
+            results = smf.ols(formula, df).fit(method="qr")
+            warnings.warn("Fell back to unadjusted inferences", stacklevel=1)
+
+    if not np.isfinite(results.llf):
+        raise Exception("Error fitting model")
+
+    for branch in treatment_branches:
+        param_name = f"C(branch, Treatment(reference='{ref_branch}'))[T.{branch}]"
+        if param_name not in results.params:
+            # this can occur if a branch does not have any non-null data
+            raise Exception(f"Effect for branch {branch} not found in model!")
+
     return results
 
 
 def summarize_joint(
     df: pd.DataFrame,
     col_label: str,
     alphas: list[float],
@@ -315,17 +344,17 @@
 
     """
 
     branch_list = _infer_branch_list(df.branch, branch_list)
 
     treatment_branches = [b for b in branch_list if b != ref_branch_label]
 
-    formula = _make_formula(col_label, ref_branch_label, covariate_col_label)
-
-    results = fit_model(formula, df)
+    results = fit_model(
+        df, col_label, ref_branch_label, treatment_branches, covariate_col_label
+    )
 
     output = {}
 
     for branch in treatment_branches:
         rel_uplifts = _extract_absolute_uplifts(
             results, branch, ref_branch_label, alphas
         )
```

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/frequentist_stats/sample_size.py` & `mozanalysis-2024.5.3/src/mozanalysis/frequentist_stats/sample_size.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/metrics/__init__.py` & `mozanalysis-2024.5.3/src/mozanalysis/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,38 +6,19 @@
 from enum import Enum
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from mozanalysis.experiment import TimeLimits
 
 import logging
-import warnings
 
 import attr
 
 logger = logging.getLogger(__name__)
 
-warnings.simplefilter("default")
-warnings.warn(
-    """
-    metrics and data sources created in mozanalysis are deprecated
-    please create directly from metric-hub with ConfigLoader like
-
-    from mozanalysis.config import ConfigLoader
-    metric=ConfigLoader.get_metric(metric_slug="active_hours",app_name="firefox_desktop")
-
-    and data sources like
-    data_source=ConfigLoader.get_data_source(data_source_slug="active_hours",
-                                                app_name="firefox_desktop")
-
-    """,
-    DeprecationWarning,
-    stacklevel=1,
-)
-
 
 class AnalysisBasis(Enum):
     """Determines what the population used for the analysis will be based on."""
 
     ENROLLMENTS = "enrollments"
     EXPOSURES = "exposures"
```

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/segments/__init__.py` & `mozanalysis-2024.5.3/src/mozanalysis/segments.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,13 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-import warnings
-
 import attr
 
-warnings.simplefilter("default")
-warnings.warn(
-    """
-    segments and segment data source objects created in mozanalysis are deprecated
-    please create directly from metric-hub with ConfigLoader like
-
-    from mozanalysis.config import ConfigLoader
-    segment=ConfigLoader.get_segment(segment_slug="regular_users_v3",
-                                        app_name="firefox_desktop")
-
-    and data sources like
-    segment_data_source=ConfigLoader.get_segment_data_source("clients_last_seen",
-                                                                "firefox_desktop")
-
-    """,
-    DeprecationWarning,
-    stacklevel=1,
-)
-
 
 @attr.s(frozen=True, slots=True)
 class SegmentDataSource:
     """Represents a table or view, from which segments may be defined.
 
     ``window_start`` and ``window_end`` define the window of data used
     to determine whether each client fits a segment. Ideally this
```

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/sizing.py` & `mozanalysis-2024.5.3/src/mozanalysis/sizing.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,23 @@
 
     Example usage (in a colab notebook)::
 
         from google.colab import auth
         auth.authenticate_user()
         print('Authenticated')
 
-        from mozanalysis.metrics.desktop import active_hours, uri_count
-        from mozanalysis.segments.desktop import allweek_regular_v1, \
-            new_or_resurrected_v3
+        from mozanalysis.config import ConfigLoader
+
+        active_hours = ConfigLoader.get_metric("active_hours", "firefox_desktop")
+        uri_count = ConfigLoader.get_metric("uri_count", "firefox_desktop")
+
+        new_or_resurrected_v3 = ConfigLoader.get_segment("new_or_resurrected_v3",
+                                                            "firefox_desktop")
+        allweek_regular_v1 = ConfigLoader.get_segment("allweek_regular_v1",
+                                                            "firefox_desktop")
 
         bq_context = BigQueryContext(
             dataset_id='mbowerman',  # e.g. mine's mbowerman
             project_id='moz-fx-data-bq-data-science'  # this is the default anyway
         )
 
         ht = HistoricalTarget(
```

### Comparing `mozanalysis-2024.5.2/src/mozanalysis/utils.py` & `mozanalysis-2024.5.3/src/mozanalysis/utils.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/src/mozanalysis.egg-info/SOURCES.txt` & `mozanalysis-2024.5.3/src/mozanalysis.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 .gitignore
 CHANGELOG.rst
 CODE_OF_CONDUCT.md
 LICENSE
 README.md
-ruff.toml
-setup.cfg
-setup.py
+pyproject.toml
+requirements-dev.in
+requirements-dev.txt
+requirements.in
+requirements.txt
 tox.ini
 .circleci/config.yml
+.github/dependabot.yml
 docs/about.rst
 docs/api.rst
 docs/conf.py
 docs/guide.rst
 docs/index.rst
 docs/_ext/metrics_docstrings.py
 docs/adrs/adr-0001-dependency_management.md
@@ -24,23 +27,22 @@
 docs/api/segments.rst
 docs/api/sizing.rst
 docs/api/bayesian_stats/bayesian_bootstrap.rst
 docs/api/bayesian_stats/binary.rst
 docs/api/bayesian_stats/survival_func.rst
 docs/api/frequentist_stats/bootstrap.rst
 docs/api/frequentist_stats/sample_size.rst
-docs/api/metrics/desktop.rst
-docs/api/metrics/fenix.rst
-docs/api/metrics/firefox_ios.rst
-docs/api/segments/desktop.rst
+script/update_deps
 src/mozanalysis/__init__.py
 src/mozanalysis/bq.py
 src/mozanalysis/config.py
 src/mozanalysis/experiment.py
 src/mozanalysis/exposure.py
+src/mozanalysis/metrics.py
+src/mozanalysis/segments.py
 src/mozanalysis/sizing.py
 src/mozanalysis/utils.py
 src/mozanalysis.egg-info/PKG-INFO
 src/mozanalysis.egg-info/SOURCES.txt
 src/mozanalysis.egg-info/dependency_links.txt
 src/mozanalysis.egg-info/requires.txt
 src/mozanalysis.egg-info/top_level.txt
@@ -48,37 +50,25 @@
 src/mozanalysis/bayesian_stats/bayesian_bootstrap.py
 src/mozanalysis/bayesian_stats/binary.py
 src/mozanalysis/bayesian_stats/survival_func.py
 src/mozanalysis/frequentist_stats/__init__.py
 src/mozanalysis/frequentist_stats/bootstrap.py
 src/mozanalysis/frequentist_stats/linear_models.py
 src/mozanalysis/frequentist_stats/sample_size.py
-src/mozanalysis/metrics/__init__.py
-src/mozanalysis/metrics/desktop.py
-src/mozanalysis/metrics/fenix.py
-src/mozanalysis/metrics/firefox_ios.py
-src/mozanalysis/metrics/focus_android.py
-src/mozanalysis/metrics/focus_ios.py
-src/mozanalysis/metrics/klar_android.py
-src/mozanalysis/metrics/klar_ios.py
-src/mozanalysis/segments/__init__.py
-src/mozanalysis/segments/desktop.py
-tests/__init__.py
 tests/conftest.py
 tests/test_config.py
 tests/test_experiment.py
-tests/test_metric_libraries.py
 tests/test_metrics.py
-tests/test_segment_libraries.py
 tests/test_sizing.py
 tests/test_utils.py
 tests/bayesian_stats/__init__.py
 tests/bayesian_stats/test_bayesian_bootstrap.py
 tests/bayesian_stats/test_binary.py
 tests/bayesian_stats/test_consistency.py
 tests/bayesian_stats/test_init.py
 tests/bayesian_stats/test_survival_func.py
 tests/frequentist_stats/__init__.py
 tests/frequentist_stats/test_bootstrap.py
 tests/frequentist_stats/test_linear_models.py
 tests/frequentist_stats/test_sample_size_calc.py
-tests/helpers/cheap_lint.py
+tests/helpers/cheap_lint.py
+tests/helpers/config_loader_lists.py
```

### Comparing `mozanalysis-2024.5.2/tests/bayesian_stats/test_bayesian_bootstrap.py` & `mozanalysis-2024.5.3/tests/bayesian_stats/test_bayesian_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/tests/bayesian_stats/test_binary.py` & `mozanalysis-2024.5.3/tests/bayesian_stats/test_binary.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/tests/bayesian_stats/test_consistency.py` & `mozanalysis-2024.5.3/tests/bayesian_stats/test_consistency.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/tests/bayesian_stats/test_init.py` & `mozanalysis-2024.5.3/tests/bayesian_stats/test_init.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/tests/bayesian_stats/test_survival_func.py` & `mozanalysis-2024.5.3/tests/bayesian_stats/test_survival_func.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/tests/frequentist_stats/test_bootstrap.py` & `mozanalysis-2024.5.3/tests/frequentist_stats/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/tests/frequentist_stats/test_linear_models.py` & `mozanalysis-2024.5.3/tests/frequentist_stats/test_linear_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     ref_branch = "treatment-a"
     alphas = [0.01, 0.05]
     branches = ["control"] * 100 + ["treatment-a"] * 100 + ["treatment-b"] * 100
     searches = list(range(100)) + list(range(100, 200)) + list(range(200, 300))
     model_df = pd.DataFrame({"search_count": searches, "branch": branches})
     formula = "search_count ~ C(branch, Treatment(reference='treatment-a'))"
     results = smf.ols(formula, model_df).fit()
-
-    return results, alphas, ref_branch, model_df, "search_count"
+    treatment_branches = ["control", "treatment-b"]
+    return results, alphas, ref_branch, model_df, "search_count", treatment_branches
 
 
 def _make_test_model_covariate():
     np.random.seed(42)
     ref_branch = "treatment-a"
     alphas = [0.01, 0.05]
+    treatment_branches = ["control", "treatment-b"]
     branches = ["control"] * 100 + ["treatment-a"] * 100 + ["treatment-b"] * 100
     y_base = np.random.normal(loc=2, scale=0.1, size=300)
     y_pre_adj = np.random.normal(loc=0, scale=0.02, size=300)
     te = np.concatenate(
         [
             np.random.normal(loc=0, scale=0.05, size=100),
             np.random.normal(loc=0.1, scale=0.05, size=100),
@@ -40,15 +41,23 @@
             "search_count_pre": y_base + y_pre_adj,
         }
     )
     formula = "search_count ~ C(branch, Treatment(reference='treatment-a')) + search_count_pre"  # noqa: E501
 
     results = smf.ols(formula, model_df).fit()
 
-    return results, alphas, ref_branch, model_df, "search_count", "search_count_pre"
+    return (
+        results,
+        alphas,
+        ref_branch,
+        model_df,
+        "search_count",
+        "search_count_pre",
+        treatment_branches,
+    )
 
 
 def test_stringify_alpha():
     for bad_alphas in [-1, 0, 1, 2]:
         with pytest.raises(ValueError, match=r"alpha must be in \(0.002,1\)"):
             mafslm.stringify_alpha(bad_alphas)
 
@@ -189,15 +198,15 @@
     for key in expected_keys:
         assert key in out.index
 
     assert len(out.index) == len(expected_keys)
 
 
 def test__extract_absolute_uplifts():
-    results, alphas, ref_branch, model_df, column_label = _make_test_model()
+    results, alphas, ref_branch, model_df, column_label, _ = _make_test_model()
 
     bootstrap_results = mafsb.compare_branches(
         model_df, column_label, ref_branch_label=ref_branch
     )
 
     # control vs treatment-a
     out = mafslm._extract_absolute_uplifts(results, "control", ref_branch, alphas)
@@ -254,15 +263,15 @@
             out[("abs_uplift", a_str_high)],
             boot_df[("abs_uplift", a_str_high)],
             atol=1.0,
         )
 
 
 def test__extract_absolute_uplifts_covariate():
-    results, alphas, ref_branch, model_df, column_label, _ = (
+    results, alphas, ref_branch, model_df, column_label, _, _ = (
         _make_test_model_covariate()
     )
 
     bootstrap_results = mafsb.compare_branches(
         model_df, column_label, ref_branch_label=ref_branch
     )
 
@@ -300,15 +309,15 @@
             boot_df[("abs_uplift", a_str_high)] - boot_df[("abs_uplift", a_str_low)]
         )
         ci_width_lm = out[("abs_uplift", a_str_high)] - out[("abs_uplift", a_str_low)]
         assert ci_width_lm < ci_width_boot
 
 
 def test__extract_relative_uplifts():
-    results, alphas, ref_branch, model_df, column_label = _make_test_model()
+    results, alphas, ref_branch, model_df, column_label, _ = _make_test_model()
 
     bootstrap_results = mafsb.compare_branches(
         model_df, column_label, ref_branch_label=ref_branch
     )
 
     # control vs treatment-a
     out = mafslm._extract_relative_uplifts(results, "control", ref_branch, alphas)
@@ -351,15 +360,15 @@
             out[("rel_uplift", a_str_high)],
             boot_df[("rel_uplift", a_str_high)],
             atol=0.01,
         )
 
 
 def test__extract_relative_uplifts_covariate():
-    results, alphas, ref_branch, model_df, column_label, _ = (
+    results, alphas, ref_branch, model_df, column_label, _, _ = (
         _make_test_model_covariate()
     )
 
     bootstrap_results = mafsb.compare_branches(
         model_df, column_label, ref_branch_label=ref_branch
     )
 
@@ -400,15 +409,15 @@
         assert ci_width_lm < ci_width_boot
 
 
 def test_summarize_joint():
     """Validates the structure of the comparative results object,
     tests for accuracy of reported values are found above, in the
     test__extract_<>_uplifts tests"""
-    _, alphas, _, model_df, column_label = _make_test_model()
+    _, alphas, _, model_df, column_label, _ = _make_test_model()
 
     actual = mafslm.summarize_joint(
         model_df,
         column_label,
         alphas,
         ref_branch_label="treatment-a",
     )
@@ -485,15 +494,15 @@
 
 
 def test_compare_branches_lm():
     """This is an integration type test, testing only that the
     format of the output object is correct. Functionality testing
     of specific elements of the object is covered by other tests"""
     branches = ["control", "treatment-a", "treatment-b"]
-    _, alphas, _, model_df, column_label = _make_test_model()
+    _, alphas, _, model_df, column_label, _ = _make_test_model()
 
     out = mafslm.compare_branches_lm(
         model_df, column_label, "treatment-a", alphas=alphas
     )
 
     assert list(out.keys()) == ["individual", "comparative"]
 
@@ -529,36 +538,97 @@
     ]
 
     for branch in comparative_branches:
         assert sorted(out["comparative"][branch].index) == expected_index
 
 
 def test_fit_model():
-    expected_results, _, ref_branch, model_df, column_label = _make_test_model()
-
-    formula = f"{column_label} ~ C(branch, Treatment(reference='{ref_branch}'))"
+    expected_results, _, ref_branch, model_df, column_label, treatment_branches = (
+        _make_test_model()
+    )
 
-    actual_results = mafslm.fit_model(formula, model_df)
+    actual_results = mafslm.fit_model(
+        model_df, column_label, ref_branch, treatment_branches
+    )
 
     pd.testing.assert_series_equal(actual_results.params, expected_results.params)
 
     alpha = 0.05
     pd.testing.assert_frame_equal(
         actual_results.conf_int(alpha), expected_results.conf_int(alpha)
     )
 
 
 def test_fit_model_covariate():
-    expected_results, _, ref_branch, model_df, column_label, column_label_pre = (
+    (
+        expected_results,
+        _,
+        ref_branch,
+        model_df,
+        column_label,
+        column_label_pre,
+        treatment_branches,
+    ) = _make_test_model_covariate()
+
+    actual_results = mafslm.fit_model(
+        model_df, column_label, ref_branch, treatment_branches, column_label_pre
+    )
+
+    pd.testing.assert_series_equal(actual_results.params, expected_results.params)
+
+    alpha = 0.05
+    pd.testing.assert_frame_equal(
+        actual_results.conf_int(alpha), expected_results.conf_int(alpha)
+    )
+
+
+def test_fit_model_covariate_robust_to_bad_covariate():
+    _, _, ref_branch, model_df, column_label, column_label_pre, treatment_branches = (
         _make_test_model_covariate()
     )
 
-    formula = f"{column_label} ~ C(branch, Treatment(reference='{ref_branch}')) + {column_label_pre}"  # noqa: E501
+    model_df.loc[:, column_label_pre] = [0] * model_df.shape[0]
 
-    actual_results = mafslm.fit_model(formula, model_df)
+    expected_formula = (
+        f"{column_label} ~ C(branch, Treatment(reference='{ref_branch}'))"
+    )
+    expected_results = smf.ols(expected_formula, model_df).fit()
+
+    with pytest.warns(Warning, match="Fell back to unadjusted inferences"):
+        actual_results = mafslm.fit_model(
+            model_df, column_label, ref_branch, treatment_branches, column_label_pre
+        )
 
     pd.testing.assert_series_equal(actual_results.params, expected_results.params)
 
     alpha = 0.05
     pd.testing.assert_frame_equal(
         actual_results.conf_int(alpha), expected_results.conf_int(alpha)
     )
+
+
+def test_fit_model_covariate_fails_on_bad_data():
+    _, _, ref_branch, model_df, column_label, column_label_pre, treatment_branches = (
+        _make_test_model_covariate()
+    )
+
+    model_df.loc[:, column_label] = [0] * model_df.shape[0]
+
+    with pytest.raises(Exception, match="Error fitting model"):
+        mafslm.fit_model(
+            model_df, column_label, ref_branch, treatment_branches, column_label_pre
+        )
+
+
+def test_fit_model_covariate_fails_on_bad_branch():
+    _, _, ref_branch, model_df, column_label, column_label_pre, treatment_branches = (
+        _make_test_model_covariate()
+    )
+
+    model_df.loc[:, "branch"] = ["treatment-a"] * model_df.shape[0]
+
+    with pytest.raises(
+        Exception, match="Effect for branch control not found in model!"
+    ):
+        mafslm.fit_model(
+            model_df, column_label, ref_branch, treatment_branches, column_label_pre
+        )
```

### Comparing `mozanalysis-2024.5.2/tests/frequentist_stats/test_sample_size_calc.py` & `mozanalysis-2024.5.3/tests/frequentist_stats/test_sample_size_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 import pytest
+from mozanalysis.config import ConfigLoader
 from mozanalysis.frequentist_stats.sample_size import (
     empirical_effect_size_sample_size_calc,
     sample_size_curves,
     z_or_t_ind_sample_size_calc,
 )
-from mozanalysis.metrics.desktop import search_clients_daily, uri_count
+
+search_clients_daily = ConfigLoader.get_data_source(
+    "search_clients_engines_sources_daily", "firefox_desktop"
+)
+uri_count = ConfigLoader.get_metric("uri_count", "firefox_desktop")
 
 
 @pytest.fixture()
 def fake_ts_result():
     class FakeTimeSeriesResult:
         def get_aggregated_data(self, metric_list, aggregate_function, **kwargs):
             periods = [0, 7, 14]
```

### Comparing `mozanalysis-2024.5.2/tests/test_config.py` & `mozanalysis-2024.5.3/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import pytest
-from cheap_lint import sql_lint
+from helpers.cheap_lint import sql_lint  # local helper file
 from mozanalysis.config import ConfigLoader
 from mozanalysis.metrics import DataSource, Metric
 from mozanalysis.segments import Segment, SegmentDataSource
 
 
 def test_get_metric():
     m = ConfigLoader.get_metric("active_hours", "firefox_desktop")
```

### Comparing `mozanalysis-2024.5.2/tests/test_experiment.py` & `mozanalysis-2024.5.3/tests/test_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import mozanalysis.metrics.desktop as mad
-import mozanalysis.metrics.fenix
-import mozanalysis.metrics.firefox_ios
-import mozanalysis.metrics.klar_android
-import mozanalysis.metrics.klar_ios
-import mozanalysis.segments.desktop as msd
 import pytest
-from cheap_lint import sql_lint
+from helpers.cheap_lint import sql_lint  # local helper file
+from helpers.config_loader_lists import (
+    desktop_metrics,
+    desktop_segments,
+    fenix_metrics,
+    firefox_ios_metrics,
+    klar_android_metrics,
+    klar_ios_metrics,
+)
+from mozanalysis.config import ConfigLoader
 from mozanalysis.experiment import (
     AnalysisWindow,
     EnrollmentsQueryType,
     Experiment,
     TimeLimits,
 )
 from mozanalysis.exposure import ExposureSignal
@@ -315,15 +318,15 @@
     enrollments_sql = exp.build_enrollments_query(
         time_limits=tl, enrollments_query_type=EnrollmentsQueryType.NORMANDY
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[m for m in mad.__dict__.values() if isinstance(m, Metric)],
+        metric_list=desktop_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
     )
 
     sql_lint(metrics_sql)
 
 
@@ -335,22 +338,22 @@
         last_date_full_data="2019-03-01",
         time_series_period="weekly",
         num_dates_enrollment=8,
     )
 
     enrollments_sql = exp.build_enrollments_query(
         time_limits=tl,
-        segment_list=[s for s in msd.__dict__.values() if isinstance(s, Segment)],
+        segment_list=desktop_segments,
         enrollments_query_type=EnrollmentsQueryType.NORMANDY,
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[m for m in mad.__dict__.values() if isinstance(m, Metric)],
+        metric_list=desktop_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
     )
 
     sql_lint(metrics_sql)
 
 
@@ -381,19 +384,15 @@
         segment_list=[segment],
         enrollments_query_type=EnrollmentsQueryType.FENIX_FALLBACK,
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[
-            m
-            for m in mozanalysis.metrics.fenix.__dict__.values()
-            if isinstance(m, Metric)
-        ],
+        metric_list=fenix_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
     )
 
     sql_lint(metrics_sql)
 
     assert "org_mozilla_firefox" not in enrollments_sql
@@ -456,19 +455,15 @@
         segment_list=[segment],
         enrollments_query_type=EnrollmentsQueryType.GLEAN_EVENT,
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[
-            m
-            for m in mozanalysis.metrics.firefox_ios.__dict__.values()
-            if isinstance(m, Metric)
-        ],
+        metric_list=firefox_ios_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
     )
 
     sql_lint(metrics_sql)
 
     assert "org_mozilla_ios_firefox" not in enrollments_sql
@@ -504,19 +499,15 @@
         segment_list=[segment],
         enrollments_query_type=EnrollmentsQueryType.GLEAN_EVENT,
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[
-            m
-            for m in mozanalysis.metrics.klar_android.__dict__.values()
-            if isinstance(m, Metric)
-        ],
+        metric_list=klar_android_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
     )
 
     sql_lint(metrics_sql)
 
     assert "org_mozilla_klar" not in enrollments_sql
@@ -552,19 +543,15 @@
         segment_list=[segment],
         enrollments_query_type=EnrollmentsQueryType.GLEAN_EVENT,
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[
-            m
-            for m in mozanalysis.metrics.klar_ios.__dict__.values()
-            if isinstance(m, Metric)
-        ],
+        metric_list=klar_ios_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
     )
 
     sql_lint(metrics_sql)
 
     assert "org_mozilla_ios_klar" not in enrollments_sql
@@ -627,15 +614,15 @@
     )
 
     enrollment_sql = exp.build_enrollments_query(
         time_limits=tl,
         enrollments_query_type=EnrollmentsQueryType.GLEAN_EVENT,
         exposure_signal=ExposureSignal(
             name="exposures",
-            data_source=mozanalysis.metrics.fenix.baseline,
+            data_source=ConfigLoader.get_data_source("baseline", "fenix"),
             select_expr="metrics.counter.events_total_uri_count > 0",
             friendly_name="URI visited exposure",
             description="Exposed when URI visited",
         ),
     )
 
     sql_lint(enrollment_sql)
@@ -655,15 +642,15 @@
     )
 
     enrollment_sql = exp.build_enrollments_query(
         time_limits=tl,
         enrollments_query_type=EnrollmentsQueryType.GLEAN_EVENT,
         exposure_signal=ExposureSignal(
             name="exposures",
-            data_source=mozanalysis.metrics.fenix.baseline,
+            data_source=ConfigLoader.get_data_source("baseline", "fenix"),
             select_expr="metrics.counter.events_total_uri_count > 0",
             friendly_name="URI visited exposure",
             description="Exposed when URI visited",
             window_start=1,
             window_end=3,
         ),
     )
@@ -689,19 +676,15 @@
     enrollments_sql = exp.build_enrollments_query(
         time_limits=tl, enrollments_query_type=EnrollmentsQueryType.FENIX_FALLBACK
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[
-            m
-            for m in mozanalysis.metrics.fenix.__dict__.values()
-            if isinstance(m, Metric)
-        ],
+        metric_list=fenix_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
         analysis_basis=AnalysisBasis.EXPOSURES,
     )
 
     sql_lint(metrics_sql)
 
@@ -721,25 +704,21 @@
     enrollments_sql = exp.build_enrollments_query(
         time_limits=tl, enrollments_query_type=EnrollmentsQueryType.FENIX_FALLBACK
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[
-            m
-            for m in mozanalysis.metrics.fenix.__dict__.values()
-            if isinstance(m, Metric)
-        ],
+        metric_list=fenix_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
         analysis_basis=AnalysisBasis.EXPOSURES,
         exposure_signal=ExposureSignal(
             name="exposures",
-            data_source=mozanalysis.metrics.fenix.baseline,
+            data_source=ConfigLoader.get_data_source("baseline", "fenix"),
             select_expr="metrics.counter.events_total_uri_count > 0",
             friendly_name="URI visited exposure",
             description="Exposed when URI visited",
             window_start=1,
             window_end=3,
         ),
     )
@@ -763,25 +742,21 @@
     enrollments_sql = exp.build_enrollments_query(
         time_limits=tl, enrollments_query_type=EnrollmentsQueryType.FENIX_FALLBACK
     )
 
     sql_lint(enrollments_sql)
 
     metrics_sql = exp.build_metrics_query(
-        metric_list=[
-            m
-            for m in mozanalysis.metrics.fenix.__dict__.values()
-            if isinstance(m, Metric)
-        ],
+        metric_list=fenix_metrics,
         time_limits=tl,
         enrollments_table="enrollments",
         analysis_basis=AnalysisBasis.EXPOSURES,
         exposure_signal=ExposureSignal(
             name="exposures",
-            data_source=mozanalysis.metrics.fenix.baseline,
+            data_source=ConfigLoader.get_data_source("baseline", "fenix"),
             select_expr="metrics.counter.events_total_uri_count > 0",
             friendly_name="URI visited exposure",
             description="Exposed when URI visited",
         ),
     )
 
     sql_lint(metrics_sql)
```

### Comparing `mozanalysis-2024.5.2/tests/test_metrics.py` & `mozanalysis-2024.5.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/tests/test_sizing.py` & `mozanalysis-2024.5.3/tests/test_sizing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import mozanalysis.metrics.desktop as mad
-import mozanalysis.segments.desktop as msd
 import pandas as pd
 import pytest
-from cheap_lint import sql_lint
+from helpers.cheap_lint import sql_lint  # local helper file
+from helpers.config_loader_lists import desktop_metrics, desktop_segments
 from mozanalysis.config import ConfigLoader
 from mozanalysis.experiment import TimeLimits
 from mozanalysis.metrics import DataSource, Metric
 from mozanalysis.segments import Segment, SegmentDataSource
 from mozanalysis.sizing import HistoricalTarget
 
 
@@ -135,15 +134,19 @@
         analysis_length_dates=3,
     )
 
     test_sds = SegmentDataSource("test_ds", "test_table")
     test_seg = Segment("test_seg", test_sds, "TEST AGG SELECT STATEMENT", "", "")
 
     target_sql = test_target.build_targets_query(
-        time_limits=tl, target_list=[msd.new_unique_profiles, test_seg]
+        time_limits=tl,
+        target_list=[
+            ConfigLoader.get_segment("new_unique_profiles", "firefox_desktop"),
+            test_seg,
+        ],
     )
 
     sql_lint(target_sql)
 
     assert "ds_1" in target_sql
 
 
@@ -154,15 +157,18 @@
         first_enrollment_date="2022-01-01",
         last_date_full_data="2022-01-04",
         analysis_start_days=0,
         analysis_length_dates=3,
     )
 
     target_sql = test_target.build_targets_query(
-        time_limits=tl, target_list=[msd.new_unique_profiles]
+        time_limits=tl,
+        target_list=[
+            ConfigLoader.get_segment("new_unique_profiles", "firefox_desktop")
+        ],
     )
 
     sql_lint(target_sql)
 
     metrics_sql = test_target.build_metrics_query(
         time_limits=tl, metric_list=[], targets_table="targets"
     )
@@ -178,26 +184,26 @@
         last_date_full_data="2022-01-04",
         analysis_start_days=0,
         analysis_length_dates=3,
     )
 
     target_sql = test_target.build_targets_query(
         time_limits=tl,
-        target_list=[s for s in msd.__dict__.values() if isinstance(s, Segment)],
+        target_list=desktop_segments,
     )
 
     sql_lint(target_sql)
 
+    desktop_metrics_no_experiment_slug = [
+        m for m in desktop_metrics if "experiment_slug" not in m.select_expr
+    ]
+
     metrics_sql = test_target.build_metrics_query(
         time_limits=tl,
-        metric_list=[
-            m
-            for m in mad.__dict__.values()
-            if isinstance(m, Metric) and "experiment_slug" not in m.select_expr
-        ],
+        metric_list=desktop_metrics_no_experiment_slug,
         targets_table="targets",
     )
 
     sql_lint(metrics_sql)
 
 
 def test_custom_query_override_target():
```

### Comparing `mozanalysis-2024.5.2/tests/test_utils.py` & `mozanalysis-2024.5.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mozanalysis-2024.5.2/tox.ini` & `mozanalysis-2024.5.3/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # Tox (https://tox.readthedocs.io/) is a tool for maintaining
 # multiple virtualenv environments for different python versions.
 # This file is referenced when tox is invoked in bin/test or .circleci/config.yml
 
 [tox]
 envlist = py310,docs,lint  # CircleCI jobs override the envlist; see .circleci/config.yml
 
-[pytest]
-addopts =
-    -rsxX
-    --verbose
-    --showlocals
-    --ruff-format
-    --tb=native
-    --timeout=120
-    --capture=no
-    --cov=src/
-    --cov-report=xml
-
 [testenv]
+deps = -rrequirements.txt
 skipsdist = True
 usedevelop = True
 extras = testing
-commands = pytest {posargs:tests/}
+commands = pytest tests \
+    -rsxX \
+    --verbose \
+    --showlocals \
+    --ruff-format \
+    --tb=native \
+    --timeout=120 \
+    --capture=no \
+    --cov=src/ \
+    --cov-report=xml \
+    {posargs}
 setenv = OBJC_DISABLE_INITIALIZE_FORK_SAFETY = YES
 
 [testenv:lint]
 skip_install = True
 deps =
     ruff
 commands =
@@ -40,7 +39,10 @@
 commands =
     # -j4: use 4 processes
     # -T: show full tracebacks on exception
     # -W: warnings are errors
     # -b: format to build
     # -d: where to cache files during the build
     sphinx-build -j4 -T -W -b html -d {envtmpdir}/doctrees docs docs/_build/html
+
+[coverage:run]
+source = src/
```

