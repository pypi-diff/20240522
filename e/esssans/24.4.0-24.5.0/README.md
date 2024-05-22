# Comparing `tmp/esssans-24.4.0.tar.gz` & `tmp/esssans-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esssans-24.4.0.tar", last modified: Fri Apr  5 12:59:02 2024, max compression
+gzip compressed data, was "esssans-24.5.0.tar", last modified: Wed May 22 05:43:07 2024, max compression
```

## Comparing `esssans-24.4.0.tar` & `esssans-24.5.0.tar`

### file list

```diff
@@ -1,138 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.142093 esssans-24.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 12:58:52.000000 esssans-24.4.0/.copier-answers.ess.yml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-05 12:58:52.000000 esssans-24.4.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/ISSUE_TEMPLATE/high-level-requirement.yml
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 12:58:52.000000 esssans-24.4.0/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 12:58:52.000000 esssans-24.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 12:58:52.000000 esssans-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-05 12:58:52.000000 esssans-24.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 12:58:52.000000 esssans-24.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-05 12:58:52.000000 esssans-24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 12:58:52.000000 esssans-24.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-05 12:59:02.142093 esssans-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-05 12:58:52.000000 esssans-24.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-05 12:58:52.000000 esssans-24.4.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.122093 esssans-24.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_static/anaconda-icon.js
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    18596 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18379 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/_templates/module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/developer/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/user-guide/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/user-guide/common/
--rw-r--r--   0 runner    (1001) docker     (127)    19765 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/common/beam-center-finder.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/common/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/user-guide/isis/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/isis/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/isis/sans2d.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/isis/zoom.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.126093 esssans-24.4.0/docs/user-guide/loki/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/loki/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    20783 2024-04-05 12:58:52.000000 esssans-24.4.0/docs/user-guide/loki/loki-direct-beam.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-05 12:58:52.000000 esssans-24.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.130093 esssans-24.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 12:58:52.000000 esssans-24.4.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.130093 esssans-24.4.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-04-05 12:58:52.000000 esssans-24.4.0/resources/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 12:59:02.142093 esssans-24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.118093 esssans-24.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.118093 esssans-24.4.0/src/ess/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.134093 esssans-24.4.0/src/ess/isissans/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/mantidio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/sans2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/isissans/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.134093 esssans-24.4.0/src/ess/loki/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/loki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/loki/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/loki/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/loki/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.138093 esssans-24.4.0/src/ess/sans/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/beam_center_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/direct_beam.py
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/i_of_q.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-05 12:58:52.000000 esssans-24.4.0/src/ess/sans/uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.142093 esssans-24.4.0/src/esssans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 12:59:02.000000 esssans-24.4.0/src/esssans.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.138093 esssans-24.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/common_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/i_of_q_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/io_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.138093 esssans-24.4.0/tests/isissans/
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/isissans/sans2d_reduction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/isissans/zoom_reduction_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:59:02.138093 esssans-24.4.0/tests/loki/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/loki/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/loki/directbeam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13227 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/loki/iofq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-05 12:58:52.000000 esssans-24.4.0/tests/uncertainty_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-05 12:58:52.000000 esssans-24.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.092584 esssans-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-22 05:43:02.000000 esssans-24.5.0/.copier-answers.ess.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-22 05:43:02.000000 esssans-24.5.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.076584 esssans-24.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.076584 esssans-24.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/ISSUE_TEMPLATE/high-level-requirement.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.076584 esssans-24.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/copier.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-22 05:43:02.000000 esssans-24.5.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-22 05:43:02.000000 esssans-24.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-22 05:43:02.000000 esssans-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-22 05:43:02.000000 esssans-24.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 05:43:02.000000 esssans-24.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-22 05:43:02.000000 esssans-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 05:43:02.000000 esssans-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-22 05:43:07.092584 esssans-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 05:43:02.000000 esssans-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.076584 esssans-24.5.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-22 05:43:02.000000 esssans-24.5.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.076584 esssans-24.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.076584 esssans-24.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    18596 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18379 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.076584 esssans-24.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/_templates/module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.076584 esssans-24.5.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.080584 esssans-24.5.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.080584 esssans-24.5.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.080584 esssans-24.5.0/docs/user-guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.080584 esssans-24.5.0/docs/user-guide/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    20397 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/common/beam-center-finder.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/common/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.080584 esssans-24.5.0/docs/user-guide/isis/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/isis/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14048 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/isis/sans2d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/isis/zoom.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.080584 esssans-24.5.0/docs/user-guide/loki/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/loki/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20967 2024-05-22 05:43:02.000000 esssans-24.5.0/docs/user-guide/loki/loki-direct-beam.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-22 05:43:02.000000 esssans-24.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.084584 esssans-24.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 05:43:02.000000 esssans-24.5.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.084584 esssans-24.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-05-22 05:43:02.000000 esssans-24.5.0/resources/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 05:43:07.092584 esssans-24.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.072584 esssans-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.072584 esssans-24.5.0/src/ess/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.084584 esssans-24.5.0/src/ess/isissans/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/mantidio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/sans2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/isissans/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.084584 esssans-24.5.0/src/ess/loki/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/loki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/loki/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/loki/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/loki/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/loki/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.088584 esssans-24.5.0/src/ess/sans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/beam_center_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9485 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/direct_beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/i_of_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17686 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-22 05:43:02.000000 esssans-24.5.0/src/ess/sans/uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.092584 esssans-24.5.0/src/esssans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-22 05:43:07.000000 esssans-24.5.0/src/esssans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-22 05:43:07.000000 esssans-24.5.0/src/esssans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 05:43:07.000000 esssans-24.5.0/src/esssans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-22 05:43:07.000000 esssans-24.5.0/src/esssans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 05:43:07.000000 esssans-24.5.0/src/esssans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 05:43:07.000000 esssans-24.5.0/src/esssans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.092584 esssans-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/i_of_q_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/io_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.092584 esssans-24.5.0/tests/isissans/
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/isissans/sans2d_reduction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/isissans/zoom_reduction_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:43:07.092584 esssans-24.5.0/tests/loki/
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/loki/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/loki/directbeam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/loki/iofq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/loki/live_reduction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-22 05:43:02.000000 esssans-24.5.0/tests/uncertainty_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-22 05:43:02.000000 esssans-24.5.0/tox.ini
```

### Comparing `esssans-24.4.0/.github/ISSUE_TEMPLATE/high-level-requirement.yml` & `esssans-24.5.0/.github/ISSUE_TEMPLATE/high-level-requirement.yml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/.github/workflows/ci.yml` & `esssans-24.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/.github/workflows/docs.yml` & `esssans-24.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/.github/workflows/nightly_at_main.yml` & `esssans-24.5.0/.github/workflows/nightly_at_main.yml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/.github/workflows/nightly_at_release.yml` & `esssans-24.5.0/.github/workflows/nightly_at_release.yml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/.github/workflows/release.yml` & `esssans-24.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/.github/workflows/test.yml` & `esssans-24.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/.github/workflows/unpinned.yml` & `esssans-24.5.0/.github/workflows/unpinned.yml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/.pre-commit-config.yaml` & `esssans-24.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/CODE_OF_CONDUCT.md` & `esssans-24.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/CONTRIBUTING.md` & `esssans-24.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/LICENSE` & `esssans-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/PKG-INFO` & `esssans-24.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esssans
-Version: 24.4.0
+Version: 24.5.0
 Summary: SANS data reduction for the European Spallation Source
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `esssans-24.4.0/README.md` & `esssans-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/conda/meta.yaml` & `esssans-24.5.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/_static/anaconda-icon.js` & `esssans-24.5.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/_static/favicon.ico` & `esssans-24.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/_static/logo-dark.svg` & `esssans-24.5.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/_static/logo.svg` & `esssans-24.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/_templates/class-template.rst` & `esssans-24.5.0/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/_templates/module-template.rst` & `esssans-24.5.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/about/index.md` & `esssans-24.5.0/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/api-reference/index.md` & `esssans-24.5.0/docs/api-reference/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,22 @@
    :recursive:
 
    data
    general
    io
 ```
 
+```{eval-rst}
+.. autosummary::
+   :toctree: ../generated/functions
+   :recursive:
+
+   ess.loki.LokiAtLarmorWorkflow
+```
+
 ## ISIS sans
 
 ```{eval-rst}
 .. currentmodule:: ess.isissans
 
 .. autosummary::
    :toctree: ../generated/modules
@@ -70,8 +78,9 @@
    components
    data
    general
    io
    mantidio
    sans2d
    visualization
+   zoom
 ```
```

### Comparing `esssans-24.4.0/docs/conf.py` & `esssans-24.5.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import doctest
 import os
 import sys
-
-from ess import sans
+from importlib.metadata import version as get_version
 
 sys.path.insert(0, os.path.abspath('.'))
 
 # General information about the project.
 project = u'ESSsans'
 copyright = u'2024 Scipp contributors'
 author = u'Scipp contributors'
@@ -107,18 +106,16 @@
 master_doc = 'index'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 
-# The short X.Y version.
-version = sans.__version__
-# The full version, including alpha/beta/rc tags.
-release = sans.__version__
+release = get_version("esssans")
+version = ".".join(release.split('.')[:3])  # CalVer
 
 warning_is_error = True
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `esssans-24.4.0/docs/developer/coding-conventions.md` & `esssans-24.5.0/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/developer/dependency-management.md` & `esssans-24.5.0/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/developer/getting-started.md` & `esssans-24.5.0/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/index.md` & `esssans-24.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/docs/user-guide/common/beam-center-finder.ipynb` & `esssans-24.5.0/docs/user-guide/common/beam-center-finder.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.982192893911644%*

 * *Differences: {"'cells'": "{1: {'source': {delete: [2]}}, 2: {'source': {insert: [(0, '## Create and configure "*

 * *            "the workflow\\n'), (2, 'We begin by setting creating a workflow and set some "*

 * *            "parameters,\\n')], delete: [2, 0]}}, 3: {'id': '6bfb29ae', 'source': ['workflow = "*

 * *            "isis.sans2d.Sans2dTutorialWorkflow()\\n', '# For real data use:\\n', '# workflow = "*

 * *            "isis.sans2d.Sans2dWorkflow()\\n', 'workflow[Filename[SampleRun]] = "*

 * *            'isis.data.sans2d_tutorial_sampl […]*

```diff
@@ -23,45 +23,41 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
                 "import plopp as pp\n",
-                "import sciline\n",
                 "from ess import sans\n",
                 "from ess import isissans as isis\n",
                 "from ess.sans.types import *"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e84bd5a5-8bed-459b-ad8c-0d04aa6117e0",
             "metadata": {},
             "source": [
-                "## Setting up the pipeline\n",
+                "## Create and configure the workflow\n",
                 "\n",
-                "We begin by setting some parameters for the pipeline,\n",
+                "We begin by setting creating a workflow and set some parameters,\n",
                 "as well as the name of the data file we wish to use."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "327a8b3c-fdde-45cd-9f29-dc33f9bb101d",
+            "id": "6bfb29ae",
             "metadata": {},
             "outputs": [],
             "source": [
-                "params = {Filename[SampleRun]: 'SANS2D00063114.nxs'}\n",
-                "\n",
-                "# Build the pipeline\n",
-                "providers = list(\n",
-                "    sans.providers + isis.providers + isis.data.providers + isis.sans2d.providers\n",
-                ")\n",
-                "pipeline = sciline.Pipeline(providers, params=params)"
+                "workflow = isis.sans2d.Sans2dTutorialWorkflow()\n",
+                "# For real data use:\n",
+                "# workflow = isis.sans2d.Sans2dWorkflow()\n",
+                "workflow[Filename[SampleRun]] = isis.data.sans2d_tutorial_sample_run()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1ae3315b-ab76-4fbc-9d6e-594b31d2fae6",
             "metadata": {},
             "source": [
@@ -75,15 +71,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fdc562a4-7cd5-43fa-8921-5f12a062ecfb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "raw = pipeline.compute(RawData[SampleRun])['spectrum', :61440]\n",
+                "raw = workflow.compute(RawData[SampleRun])['spectrum', :61440]\n",
                 "\n",
                 "p = isis.plot_flat_detector_xy(raw.hist(), norm='log')\n",
                 "p.ax.plot(0, 0, '+', color='k', ms=10)\n",
                 "p"
             ]
         },
         {
@@ -127,15 +123,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7bf3c65d-09b4-4e17-97d0-d2039bb1b05d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "masked = pipeline.compute(MaskedData[SampleRun])['spectrum', :61440].copy()\n",
+                "masked = workflow.compute(MaskedData[SampleRun])['spectrum', :61440].copy()\n",
                 "masked.masks['low_counts'] = masked.hist().data < sc.scalar(80.0, unit='counts')\n",
                 "\n",
                 "p = isis.plot_flat_detector_xy(masked.hist(), norm='log')\n",
                 "p.ax.plot(0, 0, '+', color='k', ms=10)\n",
                 "p"
             ]
         },
@@ -156,26 +152,26 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "c0e4b26a-4143-4e8d-9061-bb5f25d5553a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Insert the provider that computes the center-of-mass of the pixels\n",
-                "pipeline.insert(sans.beam_center_finder.beam_center_from_center_of_mass)\n",
-                "pipeline.visualize(BeamCenter, graph_attr={'rankdir': 'LR'})"
+                "workflow.insert(sans.beam_center_finder.beam_center_from_center_of_mass)\n",
+                "workflow.visualize(BeamCenter, graph_attr={'rankdir': 'LR'})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "36107cf1-da94-43c4-a1c3-68f168a07e37",
             "metadata": {},
             "outputs": [],
             "source": [
-                "com = pipeline.compute(BeamCenter)\n",
+                "com = workflow.compute(BeamCenter)\n",
                 "com"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b4b958ad-c03c-47ea-8464-567b64ccde96",
             "metadata": {},
@@ -212,15 +208,15 @@
             "source": [
                 "The procedure is the following:\n",
                 "\n",
                 "1. Divide the panel into 4 quadrants\n",
                 "1. Compute $I(Q)$ inside each quadrant and compute the residual difference between all 4 quadrants\n",
                 "1. Iteratively move the center position and repeat 1. and 2. until all 4 $I(Q)$ curves lie on top of each other\n",
                 "\n",
-                "For this, we need to set-up a fully-fledged pipeline that can compute $I(Q)$,\n",
+                "For this, we need to set-up a fully-fledged workflow that can compute $I(Q)$,\n",
                 "which requires some additional parameters (see the [SANS2D reduction workflow](../isis/sans2d.ipynb) for more details)."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5e8700d8-27b7-44e5-bc7e-616bb4850329",
             "metadata": {},
@@ -237,47 +233,78 @@
                 "\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "eadbb74f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "workflow = isis.sans2d.Sans2dTutorialWorkflow()\n",
+                "# For real data use:\n",
+                "# workflow = isis.sans2d.Sans2dWorkflow()\n",
+                "\n",
+                "workflow.insert(isis.data.transmission_from_sample_run)\n",
+                "# Insert the provider that computes the center from I(Q) curves\n",
+                "workflow.insert(sans.beam_center_finder.beam_center_from_iofq)\n",
+                "workflow.visualize(BeamCenter, graph_attr={'rankdir': 'LR'})"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "6e1c7413",
+            "metadata": {},
+            "source": [
+                "We set the missing input parameters:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "f43d6ddd-6106-4b8e-bc81-5f7b98b58078",
             "metadata": {},
             "outputs": [],
             "source": [
-                "params[WavelengthBins] = sc.linspace(\n",
+                "workflow[WavelengthBins] = sc.linspace(\n",
                 "    'wavelength', start=2.0, stop=16.0, num=141, unit='angstrom'\n",
                 ")\n",
-                "params[Filename[EmptyBeamRun]] = 'SANS2D00063091.nxs'\n",
+                "workflow[Filename[EmptyBeamRun]] = isis.data.sans2d_tutorial_empty_beam_run()\n",
                 "\n",
-                "params[NeXusMonitorName[Incident]] = 'monitor2'\n",
-                "params[NeXusMonitorName[Transmission]] = 'monitor4'\n",
+                "workflow[NeXusMonitorName[Incident]] = 'monitor2'\n",
+                "workflow[NeXusMonitorName[Transmission]] = 'monitor4'\n",
                 "\n",
-                "params[isis.SampleOffset] = sc.vector([0.0, 0.0, 0.053], unit='m')\n",
-                "params[isis.MonitorOffset[Transmission]] = sc.vector([0.0, 0.0, -6.719], unit='m')\n",
+                "workflow[isis.SampleOffset] = sc.vector([0.0, 0.0, 0.053], unit='m')\n",
+                "workflow[isis.MonitorOffset[Transmission]] = sc.vector([0.0, 0.0, -6.719], unit='m')\n",
                 "\n",
-                "params[CorrectForGravity] = True\n",
-                "params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
-                "params[sans.beam_center_finder.BeamCenterFinderQBins] = sc.linspace(\n",
+                "workflow[CorrectForGravity] = True\n",
+                "workflow[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
+                "workflow[sans.beam_center_finder.BeamCenterFinderQBins] = sc.linspace(\n",
                 "    'Q', 0.02, 0.25, 71, unit='1/angstrom'\n",
-                ")\n",
-                "\n",
-                "providers.append(isis.data.transmission_from_sample_run)\n",
-                "\n",
-                "# Build the pipeline\n",
-                "pipeline = sciline.Pipeline(providers, params=params)\n",
-                "\n",
-                "# Insert the provider that computes the center from I(Q) curves\n",
-                "pipeline.insert(sans.beam_center_finder.beam_center_from_iofq)\n",
-                "\n",
-                "# Override with data that contains the new mask\n",
-                "pipeline[MaskedData[SampleRun]] = masked\n",
-                "\n",
-                "pipeline.visualize(BeamCenter, graph_attr={'rankdir': 'LR'})"
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "641be8e9",
+            "metadata": {},
+            "source": [
+                "Finally, we set the data to be used, including overriding with data that contains the new mask defined earlier:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "3f772512",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "workflow[Filename[SampleRun]] = isis.data.sans2d_tutorial_sample_run()\n",
+                "workflow[MaskedData[SampleRun]] = masked"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bfe7784a-dd05-48c5-b74c-a006c82d235c",
             "metadata": {},
             "source": [
@@ -291,15 +318,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c087798a-fc33-4292-924c-eed8e3baf36a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "iofq_center = pipeline.compute(BeamCenter)\n",
+                "iofq_center = workflow.compute(BeamCenter)\n",
                 "iofq_center"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "76811e12-cf19-41ec-8791-8733c9bb69f2",
             "metadata": {},
@@ -400,20 +427,20 @@
             "execution_count": null,
             "id": "56960e8c-511b-45c6-b068-ff6a3905e2e4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "kwargs = dict(\n",
                 "    data=masked,\n",
-                "    norm=pipeline.compute(NormWavelengthTerm[SampleRun]),\n",
-                "    graph=pipeline.compute(sans.conversions.ElasticCoordTransformGraph),\n",
-                "    q_bins=params[sans.beam_center_finder.BeamCenterFinderQBins],\n",
-                "    wavelength_bins=params[WavelengthBins],\n",
-                "    transform=pipeline.compute(LabFrameTransform[SampleRun]),\n",
-                "    pixel_shape=pipeline.compute(DetectorPixelShape[SampleRun]),\n",
+                "    norm=workflow.compute(NormWavelengthTerm[SampleRun]),\n",
+                "    graph=workflow.compute(sans.conversions.ElasticCoordTransformGraph),\n",
+                "    q_bins=workflow.compute(sans.beam_center_finder.BeamCenterFinderQBins),\n",
+                "    wavelength_bins=workflow.compute(WavelengthBins),\n",
+                "    transform=workflow.compute(LabFrameTransform[SampleRun]),\n",
+                "    pixel_shape=workflow.compute(DetectorPixelShape[SampleRun]),\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6c335c02-7f17-48fe-9369-f4ed7daacdf3",
             "metadata": {},
@@ -567,18 +594,18 @@
             "id": "3bcc446a-1f04-4161-8f8d-ca782e48ecf7",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-info\">\n",
                 "\n",
                 "*Note*\n",
                 "\n",
-                "The result obtained just above is slightly different from the one obtained earlier [using the pipeline](#Method-2:-computing-I(Q)-inside-4-quadrants).\n",
+                "The result obtained just above is slightly different from the one obtained earlier [using the workflow](#Method-2:-computing-I(Q)-inside-4-quadrants).\n",
                 "\n",
                 "This is because in our example, we used `x=0, y=0` as our initial guess,\n",
-                "while the pipeline uses an additional optimization where it first computes a better initial guess using method 1 (center-of-mass).\n",
+                "while the workflow uses an additional optimization where it first computes a better initial guess using method 1 (center-of-mass).\n",
                 "This allows it to converge faster, with fewer iterations, and produce a slightly more accurate result.\n",
                 "\n",
                 "</div>"
             ]
         }
     ],
     "metadata": {
@@ -592,13 +619,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `esssans-24.4.0/docs/user-guide/isis/sans2d.ipynb` & `esssans-24.5.0/docs/user-guide/isis/sans2d.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9514533403822055%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Sans2d Data Reduction\\n'), (4, 'This notebook gives "*

 * *            'an overview of how to use the `esssans` package with Sciline, on the example of the '*

 * *            "data reduction of a Sans2d experiment.\\n')], delete: [4, 0]}}, 1: {'source': "*

 * *            "{delete: [1]}}, 2: {'source': {insert: [(0, '## Create and configure the "*

 * *            "workflow\\n'), (2, 'We begin by creating the Sans2d workflow object (this is a "*

 * *            '[sciline.Pipeline](https: […]*

```diff
@@ -1,161 +1,196 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "9a935df3-c816-4829-99c3-2afa979b7611",
             "metadata": {},
             "source": [
-                "# Sans2d data reduction\n",
+                "# Sans2d Data Reduction\n",
                 "\n",
                 "## Introduction\n",
                 "\n",
-                "This notebook gives a concise overview of how to use the `esssans` package with Sciline, on the example of the data reduction of a Sans2d experiment.\n",
+                "This notebook gives an overview of how to use the `esssans` package with Sciline, on the example of the data reduction of a Sans2d experiment.\n",
                 "We begin with relevant imports:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8c7f7cf7-0582-4953-a772-a0f87d1cf0e2",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
-                "import sciline\n",
                 "import plopp as pp\n",
                 "from ess import sans\n",
                 "from ess import isissans as isis\n",
                 "from ess.sans.types import *"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3da2d397-6206-4ed1-a98f-11b3aaf7e5b0",
             "metadata": {},
             "source": [
-                "## Define reduction parameters\n",
+                "## Create and configure the workflow\n",
                 "\n",
-                "We define the reduction parameters, with keys and types given by aliases or types defined in `ess.sans.types`:"
+                "We begin by creating the Sans2d workflow object (this is a [sciline.Pipeline](https://scipp.github.io/sciline/generated/classes/sciline.Pipeline.html) which can be consulted for advanced usage).\n",
+                "The Sans2d workflow uses Mantid to load files.\n",
+                "This tutorial comes with files that do not require Mantid, so we use a slightly modified workflow that does not require Mantid.\n",
+                "The workflow is otherwise identical to the full Mantid-based workflow:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d3f5e1ee-bd80-4301-9ff9-15c8ada3cf57",
             "metadata": {},
             "outputs": [],
             "source": [
-                "params = {}\n",
-                "\n",
-                "params[DirectBeamFilename] = 'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat'\n",
-                "params[Filename[SampleRun]] = 'SANS2D00063114.nxs'\n",
-                "params[Filename[BackgroundRun]] = 'SANS2D00063159.nxs'\n",
-                "params[Filename[EmptyBeamRun]] = 'SANS2D00063091.nxs'\n",
-                "params[OutFilename] = 'reduced.nxs'\n",
-                "\n",
-                "params[NeXusMonitorName[Incident]] = 'monitor2'\n",
-                "params[NeXusMonitorName[Transmission]] = 'monitor4'\n",
-                "\n",
-                "params[isis.SampleOffset] = sc.vector([0.0, 0.0, 0.053], unit='m')\n",
-                "params[isis.MonitorOffset[Transmission]] = sc.vector([0.0, 0.0, -6.719], unit='m')\n",
-                "\n",
-                "params[WavelengthBins] = sc.linspace(\n",
-                "    'wavelength', start=2.0, stop=16.0, num=141, unit='angstrom'\n",
-                ")\n",
-                "\n",
-                "params[isis.sans2d.LowCountThreshold] = sc.scalar(100, unit='counts')\n",
-                "\n",
-                "mask_interval = sc.array(dims=['wavelength'], values=[2.21, 2.59], unit='angstrom')\n",
-                "params[WavelengthMask] = sc.DataArray(\n",
-                "    sc.array(dims=['wavelength'], values=[True]),\n",
-                "    coords={'wavelength': mask_interval},\n",
-                ")\n",
-                "\n",
-                "params[QBins] = sc.linspace(dim='Q', start=0.01, stop=0.6, num=141, unit='1/angstrom')\n",
-                "params[NonBackgroundWavelengthRange] = sc.array(\n",
-                "    dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'\n",
-                ")\n",
-                "params[CorrectForGravity] = True\n",
-                "params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
-                "params[ReturnEvents] = True"
+                "workflow = isis.sans2d.Sans2dTutorialWorkflow()\n",
+                "# For real data use:\n",
+                "# workflow = isis.sans2d.Sans2dWorkflow()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c21564a8-e742-4183-9edc-2c70c51d5863",
+            "id": "6e08fb56",
             "metadata": {},
             "source": [
-                "## Create pipeline using Sciline\n",
-                "\n",
-                "We use all providers available in `ess.sans` as well as the `isis` and `sans2d`-specific providers, which include I/O and mask setup specific to the [Sans2d](https://www.isis.stfc.ac.uk/Pages/sans2d.aspx) instrument:"
+                "We can insert steps for configuring the workflow.\n",
+                "In this case, we would like to use the transmission monitor from the regular background and sample runs since there was no separate transmission run.\n",
+                "We also want to compute the beam center using a simple center-of-mass estimation:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "bb55a3d4",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "workflow.insert(isis.data.transmission_from_background_run)\n",
+                "workflow.insert(isis.data.transmission_from_sample_run)\n",
+                "workflow.insert(sans.beam_center_from_center_of_mass)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "d0dfa507",
+            "metadata": {},
+            "source": [
+                "The workflow can be visualized as a graph.\n",
+                "For readability we show only sub-workflow for computing `IofQ[Sample]`.\n",
+                "The workflow can actually compute the full `BackgroundSubtractedIofQ`, which applies and equivalent workflow to the background run, before a subtraction step:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "85b955ba-a54d-4760-bb35-af9cbe1ada90",
+            "id": "89212ffd",
             "metadata": {},
             "outputs": [],
             "source": [
-                "providers = (\n",
-                "    sans.providers + isis.providers + isis.data.providers + isis.sans2d.providers\n",
+                "# left-right layout works better for this graph\n",
+                "workflow.visualize(IofQ[SampleRun], graph_attr={'rankdir': 'LR'})"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "82319158",
+            "metadata": {},
+            "source": [
+                "Note the red boxes which indicate missing input parameters.\n",
+                "We can set these missing parameters, as well as parameters where we do not want to use the defaults:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4a2df47b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "workflow[OutFilename] = 'reduced.nxs'\n",
+                "\n",
+                "workflow[NeXusMonitorName[Incident]] = 'monitor2'\n",
+                "workflow[NeXusMonitorName[Transmission]] = 'monitor4'\n",
+                "\n",
+                "workflow[isis.SampleOffset] = sc.vector([0.0, 0.0, 0.053], unit='m')\n",
+                "workflow[isis.MonitorOffset[Transmission]] = sc.vector([0.0, 0.0, -6.719], unit='m')\n",
+                "\n",
+                "workflow[WavelengthBins] = sc.linspace(\n",
+                "    'wavelength', start=2.0, stop=16.0, num=141, unit='angstrom'\n",
                 ")\n",
-                "providers = providers + (\n",
-                "    isis.data.transmission_from_background_run,\n",
-                "    isis.data.transmission_from_sample_run,\n",
-                "    sans.beam_center_from_center_of_mass,\n",
+                "\n",
+                "workflow[isis.sans2d.LowCountThreshold] = sc.scalar(100, unit='counts')\n",
+                "\n",
+                "mask_interval = sc.array(dims=['wavelength'], values=[2.21, 2.59], unit='angstrom')\n",
+                "workflow[WavelengthMask] = sc.DataArray(\n",
+                "    sc.array(dims=['wavelength'], values=[True]),\n",
+                "    coords={'wavelength': mask_interval},\n",
                 ")\n",
                 "\n",
-                "pipeline = sciline.Pipeline(providers=providers, params=params)"
+                "workflow[QBins] = sc.linspace(dim='Q', start=0.01, stop=0.6, num=141, unit='1/angstrom')\n",
+                "workflow[NonBackgroundWavelengthRange] = sc.array(\n",
+                "    dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'\n",
+                ")\n",
+                "workflow[CorrectForGravity] = True\n",
+                "workflow[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
+                "workflow[ReturnEvents] = True"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "39f70669-0771-4a59-8e10-95c9120d0e9e",
+            "id": "67b18b0d",
             "metadata": {},
             "source": [
-                "## Visualize the pipeline\n",
+                "## Configuring data to load\n",
                 "\n",
-                "Before we begin computations, we can visualize the pipeline:"
+                "We have not configured which files we want to load.\n",
+                "In this tutorial, we use helpers to fetch the tutorial data which return the filenames of the cached files.\n",
+                "In a real use case, you would set these parameters manually:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d71780b8-56d5-445f-9d43-635d3d5f406b",
+            "id": "ff1658c5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# left-right layout works better for this graph\n",
-                "pipeline.visualize(BackgroundSubtractedIofQ, graph_attr={'rankdir': 'LR'})"
+                "workflow[DirectBeamFilename] = isis.data.sans2d_tutorial_direct_beam()\n",
+                "workflow[Filename[SampleRun]] = isis.data.sans2d_tutorial_sample_run()\n",
+                "workflow[Filename[BackgroundRun]] = isis.data.sans2d_tutorial_background_run()\n",
+                "workflow[Filename[EmptyBeamRun]] = isis.data.sans2d_tutorial_empty_beam_run()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c19eeaf0",
             "metadata": {},
             "source": [
-                "## Use the pipeline\n",
+                "## Use the workflow\n",
                 "\n",
                 "### Compute final result\n",
                 "\n",
                 "We can now compute the background-subtracted $I(Q)$:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c8cf57ce",
             "metadata": {},
             "outputs": [],
             "source": [
-                "result = pipeline.compute(BackgroundSubtractedIofQ)\n",
+                "result = workflow.compute(BackgroundSubtractedIofQ)\n",
                 "result.hist().plot(scale={'Q': 'log'}, norm='log')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "28532aa7",
             "metadata": {},
@@ -186,18 +221,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6a8e0b6b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.drop\n",
-                "result_drop = pipeline.compute(BackgroundSubtractedIofQ)\n",
+                "workflow[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.drop\n",
+                "result_drop = workflow.compute(BackgroundSubtractedIofQ)\n",
                 "# Reset the UnsertaintyBroadcastMode to the old value\n",
-                "pipeline[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
+                "workflow[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
                 "sc.DataGroup(upper_bound=result, dropped=result_drop).hist().plot(norm='log')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "53ce1e48-b8a9-475a-b0ec-9ad204541543",
             "metadata": {},
@@ -214,15 +249,15 @@
             "execution_count": null,
             "id": "b83c7580-fba7-43d8-b9d0-1aeeebbe0301",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ess.sans.io import save_background_subtracted_iofq\n",
                 "\n",
-                "pipeline.bind_and_call(save_background_subtracted_iofq)"
+                "workflow.bind_and_call(save_background_subtracted_iofq)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f39206c6",
             "metadata": {},
             "source": [
@@ -246,25 +281,25 @@
                 "    WavelengthMonitor[BackgroundRun, Incident],\n",
                 "    WavelengthMonitor[BackgroundRun, Transmission],\n",
                 ")\n",
                 "parts = (CleanSummedQ[SampleRun, Numerator], CleanSummedQ[SampleRun, Denominator])\n",
                 "iofqs = (IofQ[SampleRun], IofQ[BackgroundRun], BackgroundSubtractedIofQ)\n",
                 "keys = monitors + (MaskedData[SampleRun],) + parts + iofqs\n",
                 "\n",
-                "results = pipeline.compute(keys)\n",
+                "results = workflow.compute(keys)\n",
                 "\n",
                 "display(sc.plot({str(key): results[key] for key in monitors}, norm='log'))\n",
                 "\n",
                 "display(\n",
                 "    isis.plot_flat_detector_xy(\n",
                 "        results[MaskedData[SampleRun]]['spectrum', :61440].hist(), norm='log'\n",
                 "    )\n",
                 ")\n",
                 "\n",
-                "wavelength = pipeline.compute(WavelengthBins)\n",
+                "wavelength = workflow.compute(WavelengthBins)\n",
                 "display(\n",
                 "    results[CleanSummedQ[SampleRun, Numerator]]\n",
                 "    .hist(wavelength=wavelength)\n",
                 "    .transpose()\n",
                 "    .plot(norm='log')\n",
                 ")\n",
                 "display(results[CleanSummedQ[SampleRun, Denominator]].plot(norm='log'))\n",
@@ -306,16 +341,16 @@
                 "        UncertaintyBroadcastMode: [\n",
                 "            UncertaintyBroadcastMode.upper_bound,\n",
                 "            UncertaintyBroadcastMode.drop,\n",
                 "        ]\n",
                 "    },\n",
                 "    index=[Mode('upper_bound'), Mode('drop')],\n",
                 ")\n",
-                "pipeline.set_param_table(param_table)\n",
-                "results = pipeline.compute(sciline.Series[Mode, BackgroundSubtractedIofQ])\n",
+                "workflow.set_param_table(param_table)\n",
+                "results = workflow.compute(sciline.Series[Mode, BackgroundSubtractedIofQ])\n",
                 "sc.DataGroup(results).hist().plot(norm='log')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "94062d33-04cb-4a4d-aef1-e5ec58c228c4",
             "metadata": {},
@@ -332,15 +367,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "27068e8a-350f-4ea4-b4a4-2b13926905b5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[WavelengthBands] = sc.linspace(\n",
+                "workflow[WavelengthBands] = sc.linspace(\n",
                 "    'wavelength', start=2.0, stop=16.0, num=11, unit='angstrom'\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "cc3cac02-2cb4-4da5-a83d-8e6fb3d2c929",
@@ -352,15 +387,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6bd670f9-85db-4257-ab67-e296a7e8ecdf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "result = pipeline.compute(BackgroundSubtractedIofQ)\n",
+                "result = workflow.compute(BackgroundSubtractedIofQ)\n",
                 "result"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "601d2a4f-1295-4918-8177-d2dca0b839f9",
             "metadata": {},
@@ -373,108 +408,14 @@
             "execution_count": null,
             "id": "d5df969d-79d1-443a-a71b-88faf8b57a37",
             "metadata": {},
             "outputs": [],
             "source": [
                 "pp.plot(sc.collapse(result.hist(), keep='Q'), norm='log')"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "0977a3dc-eb5f-4067-80c5-cc19137cc915",
-            "metadata": {},
-            "source": [
-                "## Loading local files\n",
-                "\n",
-                "The data files used above are hosted on an external server, and downloaded on-the-fly (and cached) when computing the result.\n",
-                "\n",
-                "It is also possible to load local files from your hard drive, by using the `DataFolder` parameter.\n",
-                "We also need to insert the `isis.io.to_path` provider which supplies the file paths to the files in the folder.\n",
-                "\n",
-                "As an example, we will save our current direct beam to disk, and then re-load it using a pipeline that reads local files.\n",
-                "\n",
-                "**Note** that is it not currently possible to mix local and cloud files in the same pipeline with the present setup."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "871743bf-32d0-4df1-a285-ba722a4198ef",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Direct beam computation currently uses the `get_path` provider which\n",
-                "# fetches files from the remote server\n",
-                "direct_beam = pipeline.get(DirectBeam)\n",
-                "direct_beam.visualize()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f35f4d14-58f2-437f-826c-b9ac74570e52",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Save the direct beam to disk\n",
-                "db_filename = 'my_local_direct_beam_file.h5'\n",
-                "direct_beam.compute().save_hdf5(db_filename)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "8f712a5d-cab9-4878-9b74-5a6c9751e403",
-            "metadata": {},
-            "source": [
-                "We now modify our pipeline by setting the `DataFolder` parameter,\n",
-                "as well as our new direct beam filename. Finally, we insert the local file provider `to_path`."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "27432974-0f06-4549-8ea5-4f75ff42fbc5",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pipeline[DataFolder] = '.'\n",
-                "pipeline[DirectBeamFilename] = db_filename\n",
-                "\n",
-                "# Insert provider for local files\n",
-                "pipeline.insert(isis.io.to_path)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "37be7d9a-92ec-468c-a36e-1c73682b1bda",
-            "metadata": {},
-            "source": [
-                "We can now see that `to_path` uses both the file name and the local folder to create a file path:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "a5647adf-5606-4efa-9e18-2c2943d8250d",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "db_local = pipeline.get(DirectBeam)\n",
-                "db_local.visualize()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "446ef2a3-bf7d-404b-b493-0c65f71c1a03",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "db_local.compute().plot()"
-            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -484,13 +425,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `esssans-24.4.0/docs/user-guide/isis/zoom.ipynb` & `esssans-24.5.0/docs/user-guide/isis/zoom.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9720526903195489%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, '- Position corrections from user file (not "*

 * *            "automatically, have manual sample and detector bank offsets)\\n'), (4, '\\n'), (5, "*

 * *            "'We begin with relevant imports:')], delete: [3]}}, 2: {'source': {delete: [1]}}, 3: "*

 * *            "{'id': 'd1bb87a9', 'source': ['## Create and configure the workflow\\n', '\\n', 'We "*

 * *            'begin by creating the Zoom workflow object (this is a '*

 * *            '[sciline.Pipeline](https://scipp.github.io/sc […]*

```diff
@@ -18,213 +18,190 @@
             "cell_type": "markdown",
             "id": "53e2278d",
             "metadata": {},
             "source": [
                 "There are a few things that are not yet handled:\n",
                 "\n",
                 "- TOF or wavelength masks\n",
-                "- Position corrections from user file (not automatically, have manual sample and detector bank offsets)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "09234b87",
-            "metadata": {},
-            "source": [
-                "## Setup\n",
+                "- Position corrections from user file (not automatically, have manual sample and detector bank offsets)\n",
                 "\n",
-                "### Imports and configuration"
+                "We begin with relevant imports:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "319162e9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
-                "import sciline\n",
                 "from ess import sans\n",
                 "from ess import isissans as isis\n",
                 "from ess.sans.types import *"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "64783c51",
+            "id": "d1bb87a9",
             "metadata": {},
             "source": [
-                "### Setup input files"
+                "## Create and configure the workflow\n",
+                "\n",
+                "We begin by creating the Zoom workflow object (this is a [sciline.Pipeline](https://scipp.github.io/sciline/generated/classes/sciline.Pipeline.html) which can be consulted for advanced usage).\n",
+                "The Zoom workflow uses Mantid to load files.\n",
+                "This tutorial comes with files that do not require Mantid, so we use a slightly modified workflow that does not require Mantid.\n",
+                "The workflow is otherwise identical to the full Mantid-based workflow:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9e7cfc82",
+            "id": "955bbc91",
             "metadata": {},
             "outputs": [],
             "source": [
-                "params = {\n",
-                "    DirectBeamFilename: 'Direct_Zoom_4m_8mm_100522.txt',\n",
-                "    isis.CalibrationFilename: '192tubeCalibration_11-02-2019_r5_10lines.nxs',\n",
-                "    Filename[SampleRun]: 'ZOOM00034786.nxs',\n",
-                "    Filename[EmptyBeamRun]: 'ZOOM00034787.nxs',\n",
-                "    isis.SampleOffset: sc.vector([0.0, 0.0, 0.11], unit='m'),\n",
-                "    isis.DetectorBankOffset: sc.vector([0.0, 0.0, 0.5], unit='m'),\n",
-                "}\n",
-                "masks = [\n",
-                "    'andru_test.xml',\n",
-                "    'left_beg_18_2.xml',\n",
-                "    'right_beg_18_2.xml',\n",
-                "    'small_bs_232.xml',\n",
-                "    'small_BS_31032023.xml',\n",
-                "    'tube_1120_bottom.xml',\n",
-                "    'tubes_beg_18_2.xml',\n",
-                "]"
+                "workflow = isis.zoom.ZoomTutorialWorkflow()\n",
+                "# For real data use:\n",
+                "# workflow = isis.zoom.ZoomWorkflow()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8a8a4e01",
+            "id": "be9f1b06",
             "metadata": {},
             "source": [
-                "### Setup reduction parameters"
+                "We can insert steps for configuring the workflow.\n",
+                "In this case, we would like to use the transmission monitor from the regular background and sample runs since there was no separate transmission run.\n",
+                "We also want to compute the beam center using a simple center-of-mass estimation:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "50f11eb2",
+            "id": "0f199e59",
             "metadata": {},
             "outputs": [],
             "source": [
-                "params[NeXusMonitorName[Incident]] = 'monitor3'\n",
-                "params[NeXusMonitorName[Transmission]] = 'monitor5'\n",
-                "\n",
-                "params[WavelengthBins] = sc.geomspace(\n",
-                "    'wavelength', start=1.75, stop=16.5, num=141, unit='angstrom'\n",
-                ")\n",
-                "\n",
-                "params[QBins] = sc.geomspace(dim='Q', start=0.004, stop=0.8, num=141, unit='1/angstrom')\n",
-                "\n",
-                "params[NonBackgroundWavelengthRange] = sc.array(\n",
-                "    dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'\n",
-                ")\n",
-                "params[CorrectForGravity] = True\n",
-                "params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
-                "params[ReturnEvents] = False"
+                "workflow.insert(isis.data.transmission_from_background_run)\n",
+                "workflow.insert(isis.data.transmission_from_sample_run)\n",
+                "workflow.insert(sans.beam_center_from_center_of_mass)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0b47024f",
+            "id": "b2a3c480",
             "metadata": {},
             "source": [
-                "### Setup reduction pipeline"
+                "The workflow lacks some input parameters, as well as parameters where we do not want to use the defaults, which we can set now:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fdcaec37",
+            "id": "50f11eb2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "providers = sans.providers + isis.providers + (isis.io.read_xml_detector_masking,)\n",
-                "providers = providers + (\n",
-                "    isis.data.transmission_from_background_run,\n",
-                "    isis.data.transmission_from_sample_run,\n",
-                "    sans.beam_center_from_center_of_mass,\n",
+                "workflow[NeXusMonitorName[Incident]] = 'monitor3'\n",
+                "workflow[NeXusMonitorName[Transmission]] = 'monitor5'\n",
+                "\n",
+                "workflow[WavelengthBins] = sc.geomspace(\n",
+                "    'wavelength', start=1.75, stop=16.5, num=141, unit='angstrom'\n",
+                ")\n",
+                "\n",
+                "workflow[QBins] = sc.geomspace(\n",
+                "    dim='Q', start=0.004, stop=0.8, num=141, unit='1/angstrom'\n",
+                ")\n",
+                "\n",
+                "workflow[NonBackgroundWavelengthRange] = sc.array(\n",
+                "    dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'\n",
                 ")\n",
-                "pipeline = sciline.Pipeline(providers, params=params)\n",
-                "pipeline.set_param_series(PixelMaskFilename, masks)"
+                "workflow[CorrectForGravity] = True\n",
+                "workflow[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
+                "workflow[ReturnEvents] = False"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "951aec10",
+            "id": "1f22567f",
             "metadata": {},
             "source": [
-                "If Mantid is available, we can use it to load data files.\n",
-                "**You must configure the** `DataFolder` **below to point to the directory containing the data files.**\n",
-                "Otherwise, we fall back to load intermediate data files that have been prepared for the concrete example in this notebook.\n",
-                "If you want to use the workflow with different files you must have Mantid installed:"
+                "## Configuring data to load\n",
+                "\n",
+                "We have not configured which files we want to load.\n",
+                "In this tutorial, we use helpers to fetch the tutorial data which return the filenames of the cached files.\n",
+                "In a real use case, you would set these parameters manually:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "66237b3e",
+            "id": "9e7cfc82",
             "metadata": {},
             "outputs": [],
             "source": [
-                "try:\n",
-                "    from mantid import ConfigService\n",
-                "    import ess.isissans.mantidio\n",
-                "\n",
-                "    cfg = ConfigService.Instance()\n",
-                "    cfg.setLogLevel(3)  # Silence verbose load via Mantid\n",
-                "\n",
-                "    pipeline[DataFolder] = 'zoom_data'\n",
-                "    for provider in isis.mantidio.providers:\n",
-                "        pipeline.insert(provider)\n",
-                "except ImportError:\n",
-                "    import ess.isissans.io\n",
-                "\n",
-                "    for provider in isis.data.providers:\n",
-                "        pipeline.insert(provider)"
+                "workflow[DirectBeamFilename] = isis.data.zoom_tutorial_direct_beam()\n",
+                "workflow[isis.CalibrationFilename] = isis.data.zoom_tutorial_calibration()\n",
+                "workflow[Filename[SampleRun]] = isis.data.zoom_tutorial_sample_run()\n",
+                "workflow[Filename[EmptyBeamRun]] = isis.data.zoom_tutorial_empty_beam_run()\n",
+                "workflow[isis.SampleOffset] = sc.vector([0.0, 0.0, 0.11], unit='m')\n",
+                "workflow[isis.DetectorBankOffset] = sc.vector([0.0, 0.0, 0.5], unit='m')\n",
+                "masks = isis.data.zoom_tutorial_mask_filenames()\n",
+                "workflow.set_param_series(PixelMaskFilename, masks)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "703ffc1e",
+            "id": "a75ee3ca",
             "metadata": {},
             "source": [
-                "## Reduction\n",
-                "\n",
-                "### The reduction workflow"
+                "The workflow can be visualized as a graph:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "029e7c10-3428-4c10-8a5d-fa49b807a785",
+            "id": "cb572094",
             "metadata": {},
             "outputs": [],
             "source": [
-                "iofq = pipeline.get(IofQ[SampleRun])\n",
-                "iofq.visualize(graph_attr={'rankdir': 'LR'}, compact=True)"
+                "# left-right layout works better for this graph\n",
+                "workflow.visualize(IofQ[SampleRun], graph_attr={'rankdir': 'LR'})"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "77687728",
+            "id": "02c5969c",
             "metadata": {},
             "source": [
-                "### Running the workflow"
+                "## Use the workflow\n",
+                "\n",
+                "### Compute final result\n",
+                "\n",
+                "We can now compute $I(Q)$:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "558327ff",
             "metadata": {},
             "outputs": [],
             "source": [
-                "da = iofq.compute()\n",
+                "da = workflow.compute(IofQ[SampleRun])\n",
                 "da.plot(norm='log', scale={'Q': 'log'})"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5a7526fc",
             "metadata": {},
             "source": [
-                "### Inspecting intermediate results"
+                "### Compute intermediate results"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bb922379",
             "metadata": {},
@@ -234,25 +211,25 @@
                 "    WavelengthMonitor[SampleRun, Incident],\n",
                 "    WavelengthMonitor[SampleRun, Transmission],\n",
                 ")\n",
                 "parts = (CleanSummedQ[SampleRun, Numerator], CleanSummedQ[SampleRun, Denominator])\n",
                 "iofqs = (IofQ[SampleRun],)\n",
                 "keys = monitors + (MaskedData[SampleRun],) + parts + iofqs\n",
                 "\n",
-                "results = pipeline.compute(keys)\n",
+                "results = workflow.compute(keys)\n",
                 "\n",
                 "display(sc.plot({str(key): results[key] for key in monitors}, norm='log'))\n",
                 "\n",
                 "display(\n",
                 "    isis.plot_flat_detector_xy(\n",
                 "        results[MaskedData[SampleRun]], norm='log', figsize=(6, 10)\n",
                 "    )\n",
                 ")\n",
                 "\n",
-                "wavelength = pipeline.compute(WavelengthBins)\n",
+                "wavelength = workflow.compute(WavelengthBins)\n",
                 "display(\n",
                 "    results[CleanSummedQ[SampleRun, Numerator]]\n",
                 "    .hist(wavelength=wavelength)\n",
                 "    .transpose()\n",
                 "    .plot(norm='log')\n",
                 ")\n",
                 "display(results[CleanSummedQ[SampleRun, Denominator]].plot(norm='log'))\n",
@@ -271,31 +248,29 @@
         {
             "cell_type": "markdown",
             "id": "e63318c7-4d63-4133-97c3-feb56707caba",
             "metadata": {},
             "source": [
                 "## Computing Qx/Qy\n",
                 "\n",
-                "To compute $I(Q_{x}, Q_{y})$ instead of the one-dimensional $I(Q)$,\n",
-                "we can simply define some `QxyBins` in our parameters:"
+                "To compute $I(Q_{x}, Q_{y})$ instead of the one-dimensional $I(Q)$, we can compute `IofQxy` instead of `IofQ`.\n",
+                "For this to work, we need to define `QxBins` and `QyBins` in our parameters:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3879702d-424a-462f-8475-6056116d7d35",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[QxyBins] = {\n",
-                "    'Qx': sc.linspace(dim='Qx', start=-0.5, stop=0.5, num=101, unit='1/angstrom'),\n",
-                "    'Qy': sc.linspace(dim='Qy', start=-0.8, stop=0.8, num=101, unit='1/angstrom'),\n",
-                "}\n",
+                "workflow[QxBins] = sc.linspace('Qx', start=-0.5, stop=0.5, num=101, unit='1/angstrom')\n",
+                "workflow[QyBins] = sc.linspace('Qy', start=-0.8, stop=0.8, num=101, unit='1/angstrom')\n",
                 "\n",
-                "iqxqy = pipeline.compute(IofQ[SampleRun])\n",
+                "iqxqy = workflow.compute(IofQxy[SampleRun])\n",
                 "iqxqy.plot(norm='log', aspect='equal')"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
@@ -307,13 +282,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `esssans-24.4.0/docs/user-guide/loki/loki-direct-beam.ipynb` & `esssans-24.5.0/docs/user-guide/loki/loki-direct-beam.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.983803582241034%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'This notebook is used to compute the direct beam "*

 * *            'function for the [LoKI](https://europeanspallationsource.se/instruments/loki) '*

 * *            "detectors.\\n'), (15, '1. Create a workflow to compute $I(Q)$ inside a set of "*

 * *            'wavelength bands (the number of wavelength bands will be the number of data points in '*

 * *            "the final direct beam function)\\n'), (18, '   (we compute the full-range data by "*

 * *            'making a copy of the  […]*

```diff
@@ -5,29 +5,29 @@
             "id": "9a935df3-c816-4829-99c3-2afa979b7611",
             "metadata": {},
             "source": [
                 "# Direct beam iterations for LoKI\n",
                 "\n",
                 "## Introduction\n",
                 "\n",
-                "This notebook is used to compute the direct beam function for the LoKI detectors.\n",
+                "This notebook is used to compute the direct beam function for the [LoKI](https://europeanspallationsource.se/instruments/loki) detectors.\n",
                 "It uses data recorded during the detector test at the Larmor instrument.\n",
                 "\n",
                 "**Description of the procedure:**\n",
                 "\n",
                 "The idea behind the direct beam iterations is to determine an efficiency of the detectors as a function of wavelength.\n",
                 "To calculate this, it is possible to compute $I(Q)$ for the full wavelength range, and for individual slices (bands) of the wavelength range.\n",
                 "If the direct beam function used in the $I(Q)$ computation is correct, then $I(Q)$ curves for the full wavelength range and inside the bands should overlap.\n",
                 "\n",
                 "In the following notebook, we will:\n",
                 "\n",
-                "1. Create a pipeline to compute $I(Q)$ inside a set of wavelength bands (the number of wavelength bands will be the number of data points in the final direct beam function)\n",
+                "1. Create a workflow to compute $I(Q)$ inside a set of wavelength bands (the number of wavelength bands will be the number of data points in the final direct beam function)\n",
                 "1. Create a flat direct beam function, as a function of wavelength, with wavelength bins corresponding to the wavelength bands\n",
                 "1. Calculate inside each band by how much one would have to multiply the final $I(Q)$ so that the curve would overlap with the full-range curve\n",
-                "   (we compute the full-range data by making a copy of the pipeline but setting only a single wavelength band that contains all wavelengths)\n",
+                "   (we compute the full-range data by making a copy of the workflow but setting only a single wavelength band that contains all wavelengths)\n",
                 "1. Multiply the direct beam values inside each wavelength band by this factor\n",
                 "1. Compare the full-range $I(Q)$ to a theoretical reference and add the corresponding additional scaling to the direct beam function\n",
                 "1. Iterate until the changes to the direct beam function become small"
             ]
         },
         {
             "cell_type": "code",
@@ -47,155 +47,182 @@
                 "from ess import loki\n",
                 "from ess import isissans as isis\n",
                 "from ess.sans.types import *"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c21564a8-e742-4183-9edc-2c70c51d5863",
+            "id": "446d14b9",
             "metadata": {},
             "source": [
-                "## Define reduction parameters\n",
+                "## Create and configure the workflow\n",
                 "\n",
-                "We define a dictionary containing the reduction parameters, with keys and types given by aliases or types defined in `ess.sans.types`:"
+                "We begin by creating the Loki workflow object (this is a [sciline.Pipeline](https://scipp.github.io/sciline/generated/classes/sciline.Pipeline.html) which can be consulted for advanced usage).\n",
+                "The files we use here come from a Loki detector test at Larmor, so we use the corresponding workflow:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ce2841f0-bd9e-43c3-8cc5-52bb45f392ad",
+            "id": "63ceda7f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "params = loki.default_parameters.copy()\n",
-                "\n",
-                "# File names\n",
-                "params[Filename[SampleRun]] = '60339-2022-02-28_2215.nxs'\n",
-                "params[Filename[BackgroundRun]] = '60393-2022-02-28_2215.nxs'\n",
-                "params[Filename[TransmissionRun[SampleRun]]] = '60394-2022-02-28_2215.nxs'\n",
-                "params[Filename[TransmissionRun[BackgroundRun]]] = '60392-2022-02-28_2215.nxs'\n",
-                "params[Filename[EmptyBeamRun]] = '60392-2022-02-28_2215.nxs'\n",
-                "\n",
-                "# Wavelength binning parameters\n",
-                "wavelength_min = sc.scalar(1.0, unit='angstrom')\n",
-                "wavelength_max = sc.scalar(13.0, unit='angstrom')\n",
-                "n_wavelength_bins = 50\n",
-                "n_wavelength_bands = 50\n",
-                "\n",
-                "params[WavelengthBins] = sc.linspace(\n",
-                "    'wavelength', wavelength_min, wavelength_max, n_wavelength_bins + 1\n",
-                ")\n",
-                "params[WavelengthBands] = sc.linspace(\n",
-                "    'wavelength', wavelength_min, wavelength_max, n_wavelength_bands + 1\n",
-                ")\n",
-                "\n",
-                "masks = ['mask_new_July2022.xml']\n",
+                "workflow = loki.LokiAtLarmorWorkflow()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "d8fe14da",
+            "metadata": {},
+            "source": [
+                "We configure the workflow be defining the series of masks filenames and bank names to reduce.\n",
+                "In this case there is just a single bank:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "b8f42605",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "masks = loki.data.loki_tutorial_mask_filenames()\n",
                 "banks = ['larmor_detector']\n",
-                "\n",
-                "params[CorrectForGravity] = True\n",
-                "params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
-                "params[ReturnEvents] = False\n",
-                "\n",
-                "params[QBins] = sc.linspace(dim='Q', start=0.01, stop=0.3, num=101, unit='1/angstrom')"
+                "workflow.insert(sans.merge_banks)\n",
+                "workflow.set_param_series(PixelMaskFilename, masks)\n",
+                "workflow.set_param_series(NeXusDetectorName, banks)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "f2c3b542",
+            "id": "eb90e677",
             "metadata": {},
             "source": [
-                "## Create pipeline using Sciline\n",
-                "\n",
-                "We use all providers available in `esssans` as well as the `loki`-specific providers,\n",
-                "which include I/O and mask setup specific to the [LoKI](https://europeanspallationsource.se/instruments/loki) instrument.\n",
-                "\n",
-                "We then build the pipeline which can be used to compute the (background subtracted) $I(Q)$."
+                "The workflow can be visualized as a graph.\n",
+                "For readability we show only sub-workflow for computing `IofQ[Sample]`.\n",
+                "The workflow can actually compute the full `BackgroundSubtractedIofQ`, which applies and equivalent workflow to the background run, before a subtraction step:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "dc988a34",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "workflow.visualize(IofQ[SampleRun], compact=True, graph_attr={'rankdir': 'LR'})"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "abde8696",
+            "metadata": {},
+            "source": [
+                "Note the red boxes which indicate missing input parameters.\n",
+                "We can set these missing parameters, as well as parameters where we do not want to use the defaults:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0c1e0e90-da33-45e7-a464-4799f4fbc657",
+            "id": "ce2841f0-bd9e-43c3-8cc5-52bb45f392ad",
             "metadata": {},
             "outputs": [],
             "source": [
-                "providers = sans.providers + loki.providers + (isis.io.read_xml_detector_masking,)\n",
+                "# Wavelength binning parameters\n",
+                "wavelength_min = sc.scalar(1.0, unit='angstrom')\n",
+                "wavelength_max = sc.scalar(13.0, unit='angstrom')\n",
+                "n_wavelength_bins = 50\n",
+                "n_wavelength_bands = 50\n",
+                "\n",
+                "workflow[WavelengthBins] = sc.linspace(\n",
+                "    'wavelength', wavelength_min, wavelength_max, n_wavelength_bins + 1\n",
+                ")\n",
+                "workflow[WavelengthBands] = sc.linspace(\n",
+                "    'wavelength', wavelength_min, wavelength_max, n_wavelength_bands + 1\n",
+                ")\n",
                 "\n",
-                "pipeline = sciline.Pipeline(providers, params=params)\n",
-                "pipeline.insert(sans.merge_banks)\n",
-                "pipeline.set_param_series(PixelMaskFilename, masks)\n",
-                "pipeline.set_param_series(NeXusDetectorName, banks)\n",
                 "\n",
-                "# Add providers that fetch data from online resource\n",
-                "for provider in loki.data.providers:\n",
-                "    pipeline.insert(provider)\n",
+                "workflow[CorrectForGravity] = True\n",
+                "workflow[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound\n",
+                "workflow[ReturnEvents] = False\n",
                 "\n",
-                "# In the present file, there is no sample information so we use a dummy sample provider\n",
-                "pipeline.insert(loki.io.dummy_load_sample)"
+                "workflow[QBins] = sc.linspace(dim='Q', start=0.01, stop=0.3, num=101, unit='1/angstrom')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "805c22ea-216f-4ae4-bcbb-9eb31656cfef",
+            "id": "11e6d962",
             "metadata": {},
             "source": [
-                "Before we begin computations, we can visualize the pipeline:"
+                "## Configuring data to load\n",
+                "\n",
+                "We have not configured which files we want to load.\n",
+                "In this tutorial, we use helpers to fetch the tutorial data which return the filenames of the cached files.\n",
+                "In a real use case, you would set these parameters manually:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6eca12c4-e28c-4e45-8d3d-c5869746086b",
+            "id": "153ae0ca",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline.visualize(BackgroundSubtractedIofQ, compact=True, graph_attr={'rankdir': 'LR'})"
+                "workflow[Filename[SampleRun]] = loki.data.loki_tutorial_sample_run_60339()\n",
+                "workflow[Filename[BackgroundRun]] = loki.data.loki_tutorial_background_run_60393()\n",
+                "workflow[Filename[TransmissionRun[SampleRun]]] = (\n",
+                "    loki.data.loki_tutorial_sample_transmission_run()\n",
+                ")\n",
+                "workflow[Filename[TransmissionRun[BackgroundRun]]] = loki.data.loki_tutorial_run_60392()\n",
+                "workflow[Filename[EmptyBeamRun]] = loki.data.loki_tutorial_run_60392()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "632e3c82-89d6-4899-b1c2-f9a318899c33",
             "metadata": {},
             "source": [
                 "## Finding the beam center\n",
                 "\n",
-                "Looking carefully at the pipeline above,\n",
-                "one will notice that there is a missing parameter from the pipeline: the red box that contains the `BeamCenter` type.\n",
+                "Looking carefully at the workflow above,\n",
+                "one will notice that there is a missing parameter from the workflow: the red box that contains the `BeamCenter` type.\n",
                 "Before we can proceed with computing the direct beam function,\n",
                 "we therefore have to first determine the center of the beam.\n",
                 "\n",
                 "There are more details on how this is done in the [beam center finder notebook](../common/beam-center-finder.ipynb),\n",
-                "but for now we simply reuse the pipeline (by making a copy),\n",
+                "but for now we simply reuse the workflow (by making a copy),\n",
                 "and inserting the provider that will compute the beam center.\n",
                 "\n",
                 "For now, we compute the beam center only for the rear detector (named 'larmor_detector') but apply it to all banks (currently there is only one bank).\n",
                 "The beam center may need to be computed or applied differently to each bank, see [scipp/esssans#28](https://github.com/scipp/esssans/issues/28)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bdc15ab4-6ec6-4a29-81dc-1d00a8e890dc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "bc_pipeline = pipeline.copy()\n",
-                "bc_pipeline.del_param_table(NeXusDetectorName)\n",
-                "bc_pipeline[NeXusDetectorName] = 'larmor_detector'\n",
-                "bc_pipeline.insert(sans.beam_center_from_center_of_mass)"
+                "bc_workflow = workflow.copy()\n",
+                "bc_workflow.del_param_table(NeXusDetectorName)\n",
+                "bc_workflow[NeXusDetectorName] = 'larmor_detector'\n",
+                "bc_workflow.insert(sans.beam_center_from_center_of_mass)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7cc2cf3b-973e-4425-93ea-deb30b12c956",
             "metadata": {},
             "outputs": [],
             "source": [
-                "bc_pipeline.visualize(BeamCenter, compact=True, graph_attr={'rankdir': 'LR'})"
+                "bc_workflow.visualize(BeamCenter, compact=True, graph_attr={'rankdir': 'LR'})"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b6bf5342-6768-4b65-882b-aefc9b583724",
             "metadata": {},
             "source": [
@@ -205,34 +232,34 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6a17ac7c-de17-49c9-a02c-ca078eb7f023",
             "metadata": {},
             "outputs": [],
             "source": [
-                "center = bc_pipeline.compute(BeamCenter)\n",
+                "center = bc_workflow.compute(BeamCenter)\n",
                 "center"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0814805a-9611-4951-a015-c12ae254b099",
             "metadata": {},
             "source": [
-                "and set that value onto our original pipeline"
+                "and set that value onto our original workflow"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e79181de-1de8-43a0-a934-e9407ebcd740",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[BeamCenter] = center"
+                "workflow[BeamCenter] = center"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3756cd2e-d402-4ed0-8dcb-682eef769c00",
             "metadata": {},
             "source": [
@@ -249,19 +276,18 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "e8951c82-e726-49b3-b102-66bfb9cc53e1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scipp.scipy.interpolate import interp1d\n",
-                "from ess.loki.data import get_path\n",
                 "\n",
-                "Iq_theory = sc.io.load_hdf5(get_path('PolyGauss_I0-50_Rg-60.h5'))\n",
+                "Iq_theory = sc.io.load_hdf5(loki.data.loki_tutorial_poly_gauss_I0())\n",
                 "f = interp1d(Iq_theory, 'Q')\n",
-                "I0 = f(sc.midpoints(params[QBins])).data[0]\n",
+                "I0 = f(sc.midpoints(workflow.compute(QBins))).data[0]\n",
                 "I0"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "078fb21e-c4d5-49e7-bcca-7bacf93fbd19",
             "metadata": {},
@@ -278,15 +304,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6ffa0b31-a43c-4f73-a568-5fa1ab2d61bf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "results = sans.direct_beam(pipeline=pipeline, I0=I0, niter=6)\n",
+                "results = sans.direct_beam(workflow=workflow, I0=I0, niter=6)\n",
                 "# Unpack the final result\n",
                 "iofq_full = results[-1]['iofq_full']\n",
                 "iofq_bands = results[-1]['iofq_bands']\n",
                 "direct_beam_function = results[-1]['direct_beam']"
             ]
         },
         {
@@ -374,15 +400,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "64682705-3322-4003-8a56-f52f2523c8d4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline[DimsToKeep] = ['layer']"
+                "workflow[DimsToKeep] = ['layer']"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "92691c97-4883-41b4-b880-17e0359191a2",
             "metadata": {},
             "source": [
@@ -392,15 +418,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7e039618-d8c9-4201-9a9f-59738034786b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "results_layers = sans.direct_beam(pipeline=pipeline, I0=I0, niter=6)\n",
+                "results_layers = sans.direct_beam(workflow=workflow, I0=I0, niter=6)\n",
                 "# Unpack the final result\n",
                 "iofq_full_layers = results_layers[-1]['iofq_full']\n",
                 "iofq_bands_layers = results_layers[-1]['iofq_bands']\n",
                 "direct_beam_function_layers = results_layers[-1]['direct_beam']"
             ]
         },
         {
@@ -499,75 +525,69 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bf5f23b0-e4b6-48d8-b98a-99ec5e56be4e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "del params[Filename[SampleRun]]\n",
-                "del params[Filename[BackgroundRun]]\n",
-                "\n",
-                "sample_runs = ['60250-2022-02-28_2215.nxs', '60339-2022-02-28_2215.nxs']\n",
-                "background_runs = ['60248-2022-02-28_2215.nxs', '60393-2022-02-28_2215.nxs']"
+                "sample_runs = [\n",
+                "    loki.data.loki_tutorial_sample_run_60250(),\n",
+                "    loki.data.loki_tutorial_sample_run_60339(),\n",
+                "]\n",
+                "background_runs = [\n",
+                "    loki.data.loki_tutorial_background_run_60248(),\n",
+                "    loki.data.loki_tutorial_background_run_60393(),\n",
+                "]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c3e2ff3d-2b3d-4ba7-b4ca-f0a5617d22dc",
             "metadata": {},
             "source": [
-                "We now construct a new pipeline, inserting parameter series and merging providers:"
+                "We update the workflow, inserting parameter series and merging providers:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2a39bd50-5d63-4183-9afe-6d990548bc11",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Same as original pipeline, but without sample and background run file names\n",
-                "params[BeamCenter] = center\n",
-                "pipeline = sciline.Pipeline(providers, params=params)\n",
-                "for provider in loki.data.providers:\n",
-                "    pipeline.insert(provider)\n",
-                "pipeline.insert(sans.merge_banks)\n",
-                "pipeline.set_param_series(PixelMaskFilename, masks)\n",
-                "pipeline.set_param_series(NeXusDetectorName, banks)\n",
+                "# Reset workflow\n",
+                "workflow[DimsToKeep] = []\n",
                 "\n",
                 "# Set parameter series for file names\n",
-                "pipeline.set_param_series(Filename[SampleRun], sample_runs)\n",
-                "pipeline.set_param_series(Filename[BackgroundRun], background_runs)\n",
+                "workflow.set_param_series(Filename[SampleRun], sample_runs)\n",
+                "workflow.set_param_series(Filename[BackgroundRun], background_runs)\n",
                 "\n",
                 "# Add event merging provider\n",
-                "pipeline.insert(sans.merge_runs)\n",
-                "\n",
-                "# Add dummy sample provider\n",
-                "pipeline.insert(loki.io.dummy_load_sample)"
+                "workflow.insert(sans.merge_runs)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6a50ef4f-a15c-4ae4-a8e7-666483a93da0",
             "metadata": {},
             "source": [
-                "If we now visualize the pipeline,\n",
+                "If we now visualize the workflow,\n",
                 "we can see that every step for the `SampleRun` and `BackgroundRun` branches are now series of types (3D-looking boxes instead of flat rectangles).\n",
                 "There is also the new `merge_multiple_runs` step that combines the events from the two runs,\n",
                 "just before the normalization."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4ab8426a-d7b9-4ffe-aa9b-e029b5888ae0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pipeline.visualize(BackgroundSubtractedIofQ, compact=True, graph_attr={'rankdir': 'LR'})"
+                "workflow.visualize(BackgroundSubtractedIofQ, compact=True, graph_attr={'rankdir': 'LR'})"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1c674237-c85e-4e1f-b136-1d9f53494572",
             "metadata": {},
             "source": [
@@ -577,15 +597,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0c132101-9dfc-4896-bb68-56a0878bfcef",
             "metadata": {},
             "outputs": [],
             "source": [
-                "results = sans.direct_beam(pipeline=pipeline, I0=I0, niter=6)\n",
+                "results = sans.direct_beam(workflow=workflow, I0=I0, niter=6)\n",
                 "# Unpack the final result\n",
                 "iofq_full_new = results[-1]['iofq_full']\n",
                 "iofq_bands_new = results[-1]['iofq_bands']\n",
                 "direct_beam_function_new = results[-1]['direct_beam']"
             ]
         },
         {
```

### Comparing `esssans-24.4.0/pyproject.toml` & `esssans-24.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -83,7 +83,11 @@
 enable_error_code = [
     "ignore-without-code",
     "redundant-expr",
     "truthy-bool",
 ]
 show_error_codes = true
 warn_unreachable = true
+
+[project.entry-points."beamlime.stateless"]
+ess-loki-monitor = "ess.loki.workflow:loki_monitor_workflow"
+ess-loki-iofq = "ess.loki.workflow:loki_iofq_workflow"
```

### Comparing `esssans-24.4.0/requirements/base.txt` & `esssans-24.5.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/requirements/ci.txt` & `esssans-24.5.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/requirements/dev.txt` & `esssans-24.5.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/requirements/docs.txt` & `esssans-24.5.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/requirements/make_base.py` & `esssans-24.5.0/requirements/make_base.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/requirements/nightly.txt` & `esssans-24.5.0/requirements/nightly.txt`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/requirements/static.txt` & `esssans-24.5.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/resources/logo.svg` & `esssans-24.5.0/resources/logo.svg`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/src/ess/isissans/__init__.py` & `esssans-24.5.0/src/ess/isissans/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 
 import importlib.metadata
 
-from . import components, data, general, io, sans2d
+from . import components, data, general, io, sans2d, zoom
 from .components import DetectorBankOffset, MonitorOffset, SampleOffset
+from .general import default_parameters
 from .io import CalibrationFilename
 from .visualization import plot_flat_detector_xy
 
 try:
     __version__ = importlib.metadata.version(__package__ or __name__)
 except importlib.metadata.PackageNotFoundError:
     __version__ = "0.0.0"
@@ -16,16 +17,17 @@
 providers = components.providers + general.providers + io.providers
 
 del importlib
 
 __all__ = [
     'CalibrationFilename',
     'DetectorBankOffset',
-    'apply_component_user_offsets_to_raw_data',
     'data',
     'io',
     'MonitorOffset',
     'providers',
     'SampleOffset',
     'plot_flat_detector_xy',
     'sans2d',
+    'default_parameters',
+    'zoom',
 ]
```

### Comparing `esssans-24.4.0/src/ess/isissans/components.py` & `esssans-24.5.0/src/ess/isissans/components.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
-from typing import NewType, Optional
+from typing import NewType
 
 import sciline
 import scipp as sc
 
 from ..sans.types import (
     ConfiguredReducibleDataData,
     ConfiguredReducibleMonitor,
@@ -22,60 +22,53 @@
 
 SampleOffset = NewType('SampleOffset', sc.Variable)
 DetectorBankOffset = NewType('DetectorBankOffset', sc.Variable)
 
 
 def apply_component_user_offsets_to_raw_data(
     data: RawData[ScatteringRunType],
-    sample_offset: Optional[SampleOffset],
-    detector_bank_offset: Optional[DetectorBankOffset],
+    sample_offset: SampleOffset,
+    detector_bank_offset: DetectorBankOffset,
 ) -> ConfiguredReducibleDataData[ScatteringRunType]:
     """Apply user offsets to raw data.
 
     Parameters
     ----------
     data:
         Raw data.
     sample_offset:
         Sample offset.
     detector_bank_offset:
         Detector bank offset.
     """
     data = data.copy(deep=False)
-    if sample_offset is not None:
-        sample_pos = data.coords['sample_position']
-        data.coords['sample_position'] = sample_pos + sample_offset.to(
-            unit=sample_pos.unit, copy=False
-        )
-    if detector_bank_offset is not None:
-        pos = data.coords['position']
-        data.coords['position'] = pos + detector_bank_offset.to(
-            unit=pos.unit, copy=False
-        )
+    sample_pos = data.coords['sample_position']
+    data.coords['sample_position'] = sample_pos + sample_offset.to(
+        unit=sample_pos.unit, copy=False
+    )
+    pos = data.coords['position']
+    data.coords['position'] = pos + detector_bank_offset.to(unit=pos.unit, copy=False)
     return ConfiguredReducibleDataData[ScatteringRunType](data)
 
 
 def apply_component_user_offsets_to_raw_monitor(
     monitor_data: RawMonitor[RunType, MonitorType],
-    monitor_offset: Optional[MonitorOffset[MonitorType]],
+    monitor_offset: MonitorOffset[MonitorType],
 ) -> ConfiguredReducibleMonitor[RunType, MonitorType]:
     """Apply user offsets to raw monitor.
     Parameters
     ----------
     monitor_data:
         Raw monitor data.
     monitor_offset:
         Offset to apply to monitor position.
     """
     monitor_data = monitor_data.copy(deep=False)
-    if monitor_offset is not None:
-        pos = monitor_data.coords['position']
-        monitor_data.coords['position'] = pos + monitor_offset.to(
-            unit=pos.unit, copy=False
-        )
+    pos = monitor_data.coords['position']
+    monitor_data.coords['position'] = pos + monitor_offset.to(unit=pos.unit, copy=False)
     return ConfiguredReducibleMonitor[RunType, MonitorType](monitor_data)
 
 
 providers = (
     apply_component_user_offsets_to_raw_data,
     apply_component_user_offsets_to_raw_monitor,
 )
```

### Comparing `esssans-24.4.0/src/ess/isissans/data.py` & `esssans-24.5.0/src/ess/isissans/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,137 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
-
-from dataclasses import dataclass
-from typing import Dict
-
 import sciline
 import scipp as sc
 
-from ..sans.data import Registry
-from ..sans.types import (
+from ess.sans.data import Registry
+from ess.sans.types import (
     BackgroundRun,
     DirectBeam,
     DirectBeamFilename,
+    EmptyBeamRun,
     Filename,
-    FilenameType,
-    FilePath,
+    PixelMaskFilename,
     RunType,
     SampleRun,
     TransmissionRun,
 )
 
+from .io import CalibrationFilename
 
-@dataclass
-class IsisRegistry:
-    registry: Registry
-    mapping: Dict[str, str]
-
-
-_sans2d_registry = IsisRegistry(
-    registry=Registry(
-        instrument='sans2d',
-        files={
-            # Direct beam file (efficiency of detectors as a function of wavelength)
-            'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat.h5': 'md5:43f4188301d709aa49df0631d03a67cb',  # noqa: E501
-            # Empty beam run (no sample and no sample holder/can)
-            'SANS2D00063091.nxs.h5': 'md5:ec7f78d51a4abc643bbe1965b7a876b9',
-            # Sample run (sample and sample holder/can)
-            'SANS2D00063114.nxs.h5': 'md5:d0701afe88c09e6a714b31ecfbd79c0c',
-            # Background run (no sample, sample holder/can only)
-            'SANS2D00063159.nxs.h5': 'md5:8d740b29d8965c8d9ca4f20f1e68ec15',
-            # Solid angles of the SANS2D detector pixels computed by Mantid (for tests)
-            'SANS2D00063091.SolidAngle_from_mantid.h5': 'md5:d57b82db377cb1aea0beac7202713861',  # noqa: E501
-        },
-        version='1',
-    ),
-    mapping={
-        'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat': 'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat.h5',  # noqa: E501
-        'SANS2D00063091.nxs': 'SANS2D00063091.nxs.h5',
-        'SANS2D00063114.nxs': 'SANS2D00063114.nxs.h5',
-        'SANS2D00063159.nxs': 'SANS2D00063159.nxs.h5',
+_sans2d_registry = Registry(
+    instrument='sans2d',
+    files={
+        # Direct beam file (efficiency of detectors as a function of wavelength)
+        'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat.h5': 'md5:43f4188301d709aa49df0631d03a67cb',  # noqa: E501
+        # Empty beam run (no sample and no sample holder/can)
+        'SANS2D00063091.nxs.h5': 'md5:ec7f78d51a4abc643bbe1965b7a876b9',
+        # Sample run (sample and sample holder/can)
+        'SANS2D00063114.nxs.h5': 'md5:d0701afe88c09e6a714b31ecfbd79c0c',
+        # Background run (no sample, sample holder/can only)
+        'SANS2D00063159.nxs.h5': 'md5:8d740b29d8965c8d9ca4f20f1e68ec15',
+        # Solid angles of the SANS2D detector pixels computed by Mantid (for tests)
+        'SANS2D00063091.SolidAngle_from_mantid.h5': 'md5:d57b82db377cb1aea0beac7202713861',  # noqa: E501
     },
+    version='1',
 )
 
 
-_zoom_registry = IsisRegistry(
-    registry=Registry(
-        instrument='zoom',
-        files={
-            # Sample run (sample and sample holder/can) with applied 192tubeCalibration_11-02-2019_r5_10lines.nxs  # noqa: E501
-            'ZOOM00034786.nxs.h5.zip': 'md5:e1c53bf826dd87545df1b3629f424762',
-            # Empty beam run (no sample and no sample holder/can) - Scipp-hdf5 format
-            'ZOOM00034787.nxs.h5': 'md5:27e563d4e57621518658307acbbc3413',
-            # Calibration file, Mantid processed NeXus
-            '192tubeCalibration_11-02-2019_r5_10lines.nxs': 'md5:ca1e0e3c387903be445d0dfd0a784ed6',  # noqa: E501
-            # Direct beam file (efficiency of detectors as a function of wavelength)
-            'Direct_Zoom_4m_8mm_100522.txt.h5': 'md5:bbe813580676a9ad170934ffb7c99617',
-            # Moderator file (used for computing Q-resolution)
-            'ModeratorStdDev_TS2_SANS_LETexptl_07Aug2015.txt': 'md5:5fc389340d453b9095a5dfcc33608dae',  # noqa: E501
-            # ISIS user file configuring the data reduction
-            'USER_ZOOM_Cabral_4m_TJump_233G_8x8mm_Small_BEAMSTOP_v1_M5.toml': 'md5:4423ecb7d924c79711aba5b0a30a23e7',  # noqa: E501
-            # 7 pixel mask files for the ZOOM00034786.nxs run
-            'andru_test.xml': 'md5:c59e0c4a80640a387df7beca4857e66f',
-            'left_beg_18_2.xml': 'md5:5b24a8954d4d8a291f59f5392cd61681',
-            'right_beg_18_2.xml': 'md5:fae95a5056e5f5ba4996c8dff83ec109',
-            'small_bs_232.xml': 'md5:6d67dea9208193c9f0753ffcbb50ed83',
-            'small_BS_31032023.xml': 'md5:3c644e8c75105809ab521773f9c0c85b',
-            'tube_1120_bottom.xml': 'md5:fe577bf73c16bf5ac909516fa67360e9',
-            'tubes_beg_18_2.xml': 'md5:2debde8d82c383cc3d592ea000552300',
-        },
-        version='2',
-    ),
-    mapping={
-        'Direct_Zoom_4m_8mm_100522.txt': 'Direct_Zoom_4m_8mm_100522.txt.h5',
-        'ZOOM00034786.nxs': 'ZOOM00034786.nxs.h5.zip',
-        'ZOOM00034787.nxs': 'ZOOM00034787.nxs.h5',
+def sans2d_solid_angle_reference() -> str:
+    """Solid angles of the SANS2D detector pixels computed by Mantid (for tests)"""
+    return _sans2d_registry.get_path('SANS2D00063091.SolidAngle_from_mantid.h5')
+
+
+_zoom_registry = Registry(
+    instrument='zoom',
+    files={
+        # Sample run (sample and sample holder/can) with applied 192tubeCalibration_11-02-2019_r5_10lines.nxs  # noqa: E501
+        'ZOOM00034786.nxs.h5.zip': 'md5:e1c53bf826dd87545df1b3629f424762',
+        # Empty beam run (no sample and no sample holder/can) - Scipp-hdf5 format
+        'ZOOM00034787.nxs.h5': 'md5:27e563d4e57621518658307acbbc3413',
+        # Calibration file, Mantid processed NeXus
+        '192tubeCalibration_11-02-2019_r5_10lines.nxs': 'md5:ca1e0e3c387903be445d0dfd0a784ed6',  # noqa: E501
+        # Direct beam file (efficiency of detectors as a function of wavelength)
+        'Direct_Zoom_4m_8mm_100522.txt.h5': 'md5:bbe813580676a9ad170934ffb7c99617',
+        # Moderator file (used for computing Q-resolution)
+        'ModeratorStdDev_TS2_SANS_LETexptl_07Aug2015.txt': 'md5:5fc389340d453b9095a5dfcc33608dae',  # noqa: E501
+        # ISIS user file configuring the data reduction
+        'USER_ZOOM_Cabral_4m_TJump_233G_8x8mm_Small_BEAMSTOP_v1_M5.toml': 'md5:4423ecb7d924c79711aba5b0a30a23e7',  # noqa: E501
+        # 7 pixel mask files for the ZOOM00034786.nxs run
+        'andru_test.xml': 'md5:c59e0c4a80640a387df7beca4857e66f',
+        'left_beg_18_2.xml': 'md5:5b24a8954d4d8a291f59f5392cd61681',
+        'right_beg_18_2.xml': 'md5:fae95a5056e5f5ba4996c8dff83ec109',
+        'small_bs_232.xml': 'md5:6d67dea9208193c9f0753ffcbb50ed83',
+        'small_BS_31032023.xml': 'md5:3c644e8c75105809ab521773f9c0c85b',
+        'tube_1120_bottom.xml': 'md5:fe577bf73c16bf5ac909516fa67360e9',
+        'tubes_beg_18_2.xml': 'md5:2debde8d82c383cc3d592ea000552300',
     },
+    version='2',
 )
 
 
-_registries = (_sans2d_registry, _zoom_registry)
+def sans2d_tutorial_direct_beam() -> DirectBeamFilename:
+    return DirectBeamFilename(
+        _sans2d_registry.get_path('DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat.h5')
+    )
+
+
+def sans2d_tutorial_sample_run() -> Filename[SampleRun]:
+    return Filename[SampleRun](_sans2d_registry.get_path('SANS2D00063114.nxs.h5'))
+
+
+def sans2d_tutorial_background_run() -> Filename[BackgroundRun]:
+    return Filename[BackgroundRun](_sans2d_registry.get_path('SANS2D00063159.nxs.h5'))
+
+
+def sans2d_tutorial_empty_beam_run() -> Filename[EmptyBeamRun]:
+    return Filename[EmptyBeamRun](_sans2d_registry.get_path('SANS2D00063091.nxs.h5'))
+
 
+def zoom_tutorial_direct_beam() -> DirectBeamFilename:
+    return DirectBeamFilename(
+        _zoom_registry.get_path('Direct_Zoom_4m_8mm_100522.txt.h5')
+    )
 
-def get_path(filename: FilenameType) -> FilePath[FilenameType]:
-    """Translate any filename to a path to the file obtained from pooch registries."""
-    for reg in _registries:
-        filename = reg.mapping.get(filename, filename)
-        if filename in reg.registry:
-            if filename.endswith('.zip'):
-                return reg.registry.get_path(filename, unzip=True)[0]
-            return reg.registry.get_path(filename)
+
+def zoom_tutorial_calibration() -> Filename[CalibrationFilename]:
+    return Filename[CalibrationFilename](
+        _zoom_registry.get_path('192tubeCalibration_11-02-2019_r5_10lines.nxs')
+    )
+
+
+def zoom_tutorial_sample_run() -> Filename[SampleRun]:
+    return _zoom_registry.get_path('ZOOM00034786.nxs.h5.zip', unzip=True)[0]
+
+
+def zoom_tutorial_empty_beam_run() -> Filename[EmptyBeamRun]:
+    return Filename[EmptyBeamRun](_zoom_registry.get_path('ZOOM00034787.nxs.h5'))
+
+
+def zoom_tutorial_mask_filenames() -> list[PixelMaskFilename]:
+    return [
+        PixelMaskFilename(_zoom_registry.get_path('andru_test.xml')),
+        PixelMaskFilename(_zoom_registry.get_path('left_beg_18_2.xml')),
+        PixelMaskFilename(_zoom_registry.get_path('right_beg_18_2.xml')),
+        PixelMaskFilename(_zoom_registry.get_path('small_bs_232.xml')),
+        PixelMaskFilename(_zoom_registry.get_path('small_BS_31032023.xml')),
+        PixelMaskFilename(_zoom_registry.get_path('tube_1120_bottom.xml')),
+        PixelMaskFilename(_zoom_registry.get_path('tubes_beg_18_2.xml')),
+    ]
 
 
 class LoadedFileContents(sciline.Scope[RunType, sc.DataGroup], sc.DataGroup):
     """Contents of a loaded file."""
 
 
-def load_run(filename: FilePath[Filename[RunType]]) -> LoadedFileContents[RunType]:
+def load_tutorial_run(filename: Filename[RunType]) -> LoadedFileContents[RunType]:
     return LoadedFileContents[RunType](sc.io.load_hdf5(filename))
 
 
-def load_direct_beam(filename: FilePath[DirectBeamFilename]) -> DirectBeam:
+def load_tutorial_direct_beam(filename: DirectBeamFilename) -> DirectBeam:
     return DirectBeam(sc.io.load_hdf5(filename))
 
 
 def transmission_from_sample_run(
     data: LoadedFileContents[SampleRun],
 ) -> LoadedFileContents[TransmissionRun[SampleRun]]:
     """
@@ -125,10 +143,7 @@
 def transmission_from_background_run(
     data: LoadedFileContents[BackgroundRun],
 ) -> LoadedFileContents[TransmissionRun[BackgroundRun]]:
     """
     Use transmission from a background run, instead of dedicated run.
     """
     return LoadedFileContents[TransmissionRun[BackgroundRun]](data)
-
-
-providers = (get_path, load_run, load_direct_beam)
```

### Comparing `esssans-24.4.0/src/ess/isissans/general.py` & `esssans-24.5.0/src/ess/isissans/general.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,31 +4,47 @@
 Providers for the ISIS instruments.
 """
 import scipp as sc
 
 from ..sans.types import (
     ConfiguredReducibleDataData,
     ConfiguredReducibleMonitor,
+    CorrectForGravity,
     DetectorPixelShape,
+    DimsToKeep,
+    Incident,
     LabFrameTransform,
     MonitorType,
     NeXusMonitorName,
     RawData,
     RawMonitor,
     RunNumber,
     RunTitle,
     RunType,
     SampleRun,
     ScatteringRunType,
     TofData,
     TofMonitor,
+    Transmission,
 )
+from .components import DetectorBankOffset, MonitorOffset, SampleOffset
 from .data import LoadedFileContents
 
 
+def default_parameters() -> dict:
+    return {
+        CorrectForGravity: False,
+        DimsToKeep: tuple(),
+        MonitorOffset[Incident]: MonitorOffset(sc.vector([0, 0, 0], unit='m')),
+        MonitorOffset[Transmission]: MonitorOffset(sc.vector([0, 0, 0], unit='m')),
+        DetectorBankOffset: DetectorBankOffset(sc.vector([0, 0, 0], unit='m')),
+        SampleOffset: SampleOffset(sc.vector([0, 0, 0], unit='m')),
+    }
+
+
 def get_detector_data(
     dg: LoadedFileContents[RunType],
 ) -> RawData[RunType]:
     return RawData[RunType](dg['data'])
 
 
 def get_monitor_data(
```

### Comparing `esssans-24.4.0/src/ess/isissans/io.py` & `esssans-24.5.0/src/ess/isissans/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,32 +3,20 @@
 """
 File loading functions for ISIS data, NOT using Mantid.
 """
 from typing import NewType
 
 import scipp as sc
 
-from ..sans.types import (
-    DataFolder,
-    FilenameType,
-    FilePath,
-    MaskedDetectorIDs,
-    PixelMaskFilename,
-)
+from ess.sans.types import MaskedDetectorIDs, PixelMaskFilename
 
 CalibrationFilename = NewType('CalibrationFilename', str)
 
 
-def to_path(filename: FilenameType, path: DataFolder) -> FilePath[FilenameType]:
-    return f'{path}/{filename}'
-
-
-def read_xml_detector_masking(
-    filename: FilePath[PixelMaskFilename],
-) -> MaskedDetectorIDs:
+def read_xml_detector_masking(filename: PixelMaskFilename) -> MaskedDetectorIDs:
     """Read a pixel mask from an XML file.
 
     The format is as follows, where the detids are inclusive ranges of detector IDs:
 
     .. code-block:: xml
 
         <?xml version="1.0"?>
@@ -60,8 +48,8 @@
                     masked_detids.append(int(detid))
 
     return MaskedDetectorIDs(
         sc.array(dims=['detector_id'], values=masked_detids, unit=None, dtype='int32')
     )
 
 
-providers = (read_xml_detector_masking, to_path)
+providers = (read_xml_detector_masking,)
```

### Comparing `esssans-24.4.0/src/ess/isissans/mantidio.py` & `esssans-24.5.0/src/ess/isissans/mantidio.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from typing import NewType, NoReturn, Optional
 
 import sciline
 import scipp as sc
 import scippneutron as scn
 from scipp.constants import g
 
-from ..sans.types import DirectBeam, DirectBeamFilename, Filename, RunType, SampleRun
+from ess.sans.types import DirectBeam, DirectBeamFilename, Filename, RunType, SampleRun
+
 from .data import LoadedFileContents
-from .io import CalibrationFilename, FilePath
+from .io import CalibrationFilename
 
 try:
     import mantid.api as _mantid_api
     import mantid.simpleapi as _mantid_simpleapi
     from mantid.api import MatrixWorkspace
 except ModuleNotFoundError:
     # Catch runtime usages of Mantid
@@ -27,14 +28,16 @@
             ) from None
 
     _mantid_api = _MantidFallback()
     _mantid_simpleapi = _MantidFallback
     # Needed for type annotations
     MatrixWorkspace = object
 
+Period = NewType('Period', int)
+"""Period number of the events."""
 
 CalibrationWorkspace = NewType('CalibrationWorkspace', MatrixWorkspace)
 
 
 class DataWorkspace(sciline.Scope[RunType, MatrixWorkspace], MatrixWorkspace):
     """Workspace containing data"""
 
@@ -53,33 +56,32 @@
         da.coords[dim],
         sc.arange('detector', da.sizes['detector'], dtype='int32', unit=None),
     ):
         raise ValueError("Spectrum-detector mapping is not 1:1, this is not supported.")
     return da.data.rename_dims(detector='spectrum')
 
 
-def load_calibration(filename: FilePath[CalibrationFilename]) -> CalibrationWorkspace:
+def load_calibration(filename: CalibrationFilename) -> CalibrationWorkspace:
     ws = _mantid_simpleapi.Load(Filename=str(filename), StoreInADS=False)
     return CalibrationWorkspace(ws)
 
 
-def load_direct_beam(filename: FilePath[DirectBeamFilename]) -> DirectBeam:
+def load_direct_beam(filename: DirectBeamFilename) -> DirectBeam:
     dg = scn.load_with_mantid(
         filename=filename,
         mantid_alg="LoadRKH",
         mantid_args={"FirstColumnValue": "Wavelength"},
     )
     da = dg['data']
     del da.coords['spectrum']
     return DirectBeam(da)
 
 
 def from_data_workspace(
-    ws: DataWorkspace[RunType],
-    calibration: Optional[CalibrationWorkspace],
+    ws: DataWorkspace[RunType], calibration: Optional[CalibrationWorkspace]
 ) -> LoadedFileContents[RunType]:
     if calibration is not None:
         _mantid_simpleapi.CopyInstrumentParameters(
             InputWorkspace=calibration, OutputWorkspace=ws, StoreInADS=False
         )
     up = ws.getInstrument().getReferenceFrame().vecPointingUp()
     dg = scn.from_mantid(ws)
@@ -92,24 +94,36 @@
     if (dg['data'].bins is not None) and ('tof' in dg['data'].coords):
         del dg['data'].coords['tof']
     dg['data'].coords['detector_id'] = det_ids
     dg['data'].coords['gravity'] = sc.vector(value=-up) * g
     return LoadedFileContents[RunType](dg)
 
 
-def load_run(filename: FilePath[Filename[RunType]]) -> DataWorkspace[RunType]:
+def load_run(
+    filename: Filename[RunType], period: Optional[Period]
+) -> DataWorkspace[RunType]:
     loaded = _mantid_simpleapi.Load(
         Filename=str(filename), LoadMonitors=True, StoreInADS=False
     )
     if isinstance(loaded, _mantid_api.Workspace):
         # A single workspace
         data_ws = loaded
     else:
         # Separate data and monitor workspaces
         data_ws = loaded.OutputWorkspace
+        if isinstance(data_ws, _mantid_api.WorkspaceGroup):
+            if period is None:
+                raise ValueError(
+                    f'Needs {Period} to be set to know what '
+                    'section of the event data to load'
+                )
+            data_ws = data_ws.getItem(period)
+            data_ws.setMonitorWorkspace(loaded.MonitorWorkspace.getItem(period))
+        else:
+            data_ws.setMonitorWorkspace(loaded.MonitorWorkspace)
     return DataWorkspace[RunType](data_ws)
 
 
 providers = (
     from_data_workspace,
     load_calibration,
     load_direct_beam,
```

### Comparing `esssans-24.4.0/src/ess/isissans/sans2d.py` & `esssans-24.5.0/src/ess/isissans/sans2d.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
 from typing import NewType, Optional
 
+import sciline
 import scipp as sc
 
-from ..sans.types import MaskedData, SampleRun, ScatteringRunType, TofData
+from ess.sans import providers as sans_providers
+from ess.sans.types import MaskedData, SampleRun, ScatteringRunType, TofData
+
+from .data import load_tutorial_direct_beam, load_tutorial_run
+from .general import default_parameters
+from .mantidio import providers as mantid_providers
 
 DetectorEdgeMask = NewType('DetectorEdgeMask', sc.Variable)
 """Detector edge mask"""
 
 LowCountThreshold = NewType('LowCountThreshold', sc.Variable)
 """Threshold below which detector pixels should be masked
 (low-counts on the edges of the detector panel, and the beam stop)"""
@@ -62,7 +68,29 @@
         da.masks['edges'] = edge_mask
     if holder_mask is not None:
         da.masks['holder_mask'] = holder_mask
     return MaskedData[ScatteringRunType](da)
 
 
 providers = (detector_edge_mask, sample_holder_mask, mask_detectors)
+
+
+def Sans2dWorkflow() -> sciline.Pipeline:
+    """Create Sans2d workflow with default parameters."""
+    from . import providers as isis_providers
+
+    params = default_parameters()
+    sans2d_providers = sans_providers + isis_providers + mantid_providers + providers
+    return sciline.Pipeline(providers=sans2d_providers, params=params)
+
+
+def Sans2dTutorialWorkflow() -> sciline.Pipeline:
+    """
+    Create Sans2d tutorial workflow.
+
+    Equivalent to :func:`Sans2dWorkflow`, but with loaders for tutorial data instead
+    of Mantid-based loaders.
+    """
+    workflow = Sans2dWorkflow()
+    workflow.insert(load_tutorial_run)
+    workflow.insert(load_tutorial_direct_beam)
+    return workflow
```

### Comparing `esssans-24.4.0/src/ess/isissans/visualization.py` & `esssans-24.5.0/src/ess/isissans/visualization.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/src/ess/loki/general.py` & `esssans-24.5.0/src/ess/loki/general.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """
 Default parameters, providers and utility functions for the loki workflow.
 """
 from typing import Optional
 
+import sciline
 import scipp as sc
 from ess.reduce import nexus
 
+from ess.sans import providers as sans_providers
+
 from ..sans.common import gravity_vector
 from ..sans.types import (
     ConfiguredReducibleDataData,
     ConfiguredReducibleMonitor,
+    CorrectForGravity,
     DetectorPixelShape,
+    DimsToKeep,
     Incident,
     LabFrameTransform,
     LoadedNeXusDetector,
     LoadedNeXusMonitor,
     MonitorType,
     NeXusDetectorName,
     NeXusMonitorName,
@@ -30,21 +35,53 @@
     ScatteringRunType,
     SourcePosition,
     TofData,
     TofMonitor,
     TransformationPath,
     Transmission,
 )
+from .io import dummy_load_sample
 
-default_parameters = {
-    NeXusMonitorName[Incident]: 'monitor_1',
-    NeXusMonitorName[Transmission]: 'monitor_2',
-    TransformationPath: 'transform',
-    PixelShapePath: 'pixel_shape',
-}
+
+def default_parameters() -> dict:
+    return {
+        CorrectForGravity: False,
+        DimsToKeep: tuple(),
+        NeXusMonitorName[Incident]: 'monitor_1',
+        NeXusMonitorName[Transmission]: 'monitor_2',
+        TransformationPath: 'transform',
+        PixelShapePath: 'pixel_shape',
+    }
+
+
+def LokiAtLarmorWorkflow() -> sciline.Pipeline:
+    """
+    Workflow with default parameters for Loki test at Larmor.
+
+    This version of the Loki workflow:
+
+    - Uses ISIS XML files to define masks.
+    - Sets a dummy sample position [0,0,0] since files do not contain this information.
+
+    Returns
+    -------
+    :
+        Loki workflow as a sciline.Pipeline
+    """
+    from ess.isissans.io import read_xml_detector_masking
+
+    from . import providers as loki_providers
+
+    params = default_parameters()
+    loki_providers = sans_providers + loki_providers
+    workflow = sciline.Pipeline(providers=loki_providers, params=params)
+    workflow.insert(read_xml_detector_masking)
+    # No sample information in the Loki@Larmor files, so we use a dummy sample provider
+    workflow.insert(dummy_load_sample)
+    return workflow
 
 
 DETECTOR_BANK_RESHAPING = {
     'larmor_detector': lambda x: x.fold(
         dim='detector_number', sizes=dict(layer=4, tube=32, straw=7, pixel=512)
     )
 }
```

### Comparing `esssans-24.4.0/src/ess/loki/io.py` & `esssans-24.5.0/src/ess/loki/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,66 +2,58 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """
 Loading and merging of LoKI data.
 """
 import scipp as sc
 from ess.reduce import nexus
 
-from ..sans.types import (
-    DataFolder,
+from ess.sans.types import (
     Filename,
-    FilenameType,
-    FilePath,
     LoadedNeXusDetector,
     LoadedNeXusMonitor,
     MonitorType,
     NeXusDetectorName,
     NeXusMonitorName,
     RawSample,
     RawSource,
     RunType,
 )
 
 
-def load_nexus_sample(file_path: FilePath[Filename[RunType]]) -> RawSample[RunType]:
+def load_nexus_sample(file_path: Filename[RunType]) -> RawSample[RunType]:
     return RawSample[RunType](nexus.load_sample(file_path))
 
 
-def dummy_load_sample(file_path: FilePath[Filename[RunType]]) -> RawSample[RunType]:
+def dummy_load_sample(file_path: Filename[RunType]) -> RawSample[RunType]:
     return RawSample[RunType](
         sc.DataGroup({'position': sc.vector(value=[0, 0, 0], unit='m')})
     )
 
 
-def load_nexus_source(file_path: FilePath[Filename[RunType]]) -> RawSource[RunType]:
+def load_nexus_source(file_path: Filename[RunType]) -> RawSource[RunType]:
     return RawSource[RunType](nexus.load_source(file_path))
 
 
 def load_nexus_detector(
-    file_path: FilePath[Filename[RunType]], detector_name: NeXusDetectorName
+    file_path: Filename[RunType], detector_name: NeXusDetectorName
 ) -> LoadedNeXusDetector[RunType]:
     return LoadedNeXusDetector[RunType](
         nexus.load_detector(file_path=file_path, detector_name=detector_name)
     )
 
 
 def load_nexus_monitor(
-    file_path: FilePath[Filename[RunType]],
+    file_path: Filename[RunType],
     monitor_name: NeXusMonitorName[MonitorType],
 ) -> LoadedNeXusMonitor[RunType, MonitorType]:
     return LoadedNeXusMonitor[RunType, MonitorType](
         nexus.load_monitor(file_path=file_path, monitor_name=monitor_name)
     )
 
 
-def to_path(filename: FilenameType, path: DataFolder) -> FilePath[FilenameType]:
-    return FilePath[FilenameType](f'{path}/{filename}')
-
-
 providers = (
     load_nexus_detector,
     load_nexus_monitor,
     load_nexus_sample,
     load_nexus_source,
-    to_path,
 )
 """Providers for loading single files."""
```

### Comparing `esssans-24.4.0/src/ess/sans/__init__.py` & `esssans-24.5.0/src/ess/sans/__init__.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/src/ess/sans/beam_center_finder.py` & `esssans-24.5.0/src/ess/sans/beam_center_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,23 @@
     detector_to_wavelength,
     mask_wavelength,
 )
 from .i_of_q import bin_in_q, no_bank_merge, no_run_merge
 from .logging import get_logger
 from .normalization import (
     iofq_denominator,
-    normalize,
+    normalize_q,
     process_wavelength_bands,
     solid_angle,
 )
 from .types import (
     BeamCenter,
     CalibratedMaskedData,
     DetectorPixelShape,
+    DimsToKeep,
     IofQ,
     LabFrameTransform,
     MaskedData,
     NormWavelengthTerm,
     QBins,
     ReturnEvents,
     SampleRun,
@@ -169,15 +170,15 @@
     quadrants = ['south-west', 'south-east', 'north-east', 'north-west']
 
     providers = [
         compute_Q,
         bin_in_q,
         no_run_merge,
         no_bank_merge,
-        normalize,
+        normalize_q,
         iofq_denominator,
         mask_wavelength,
         detector_to_wavelength,
         solid_angle,
         calibrate_positions,
         process_wavelength_bands,
     ]
@@ -186,14 +187,15 @@
     params[ReturnEvents] = False
     params[WavelengthBins] = wavelength_bins
     params[QBins] = q_bins
     params[DetectorPixelShape[SampleRun]] = pixel_shape
     params[LabFrameTransform[SampleRun]] = transform
     params[ElasticCoordTransformGraph] = graph
     params[BeamCenter] = _offsets_to_vector(data=data, xy=xy, graph=graph)
+    params[DimsToKeep] = tuple()
 
     pipeline = sciline.Pipeline(providers, params=params)
     pipeline[MaskedData[SampleRun]] = data
     calibrated = pipeline.compute(CalibratedMaskedData[SampleRun])
     with_phi = calibrated.transform_coords(
         'phi', graph=graph, keep_intermediate=False, keep_inputs=False
     )
```

### Comparing `esssans-24.4.0/src/ess/sans/common.py` & `esssans-24.5.0/src/ess/sans/common.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/src/ess/sans/conversions.py` & `esssans-24.5.0/src/ess/sans/conversions.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from scippneutron.conversion.graph import beamline, tof
 
 from .common import mask_range
 from .types import (
     BeamCenter,
     CalibratedMaskedData,
     CleanQ,
+    CleanQxy,
     CleanWavelength,
     CleanWavelengthMasked,
     CorrectForGravity,
     IofQPart,
     MaskedData,
     MonitorType,
     Numerator,
-    QxyBins,
     RunType,
     ScatteringRunType,
     TofMonitor,
     WavelengthMask,
     WavelengthMonitor,
 )
 
@@ -140,15 +140,15 @@
     return {'Qx': Qx, 'Qy': Qy}
 
 
 ElasticCoordTransformGraph = NewType('ElasticCoordTransformGraph', dict)
 MonitorCoordTransformGraph = NewType('MonitorCoordTransformGraph', dict)
 
 
-def sans_elastic(gravity: Optional[CorrectForGravity]) -> ElasticCoordTransformGraph:
+def sans_elastic(gravity: CorrectForGravity) -> ElasticCoordTransformGraph:
     """
     Generate a coordinate transformation graph for SANS elastic scattering.
 
     It is based on classical conversions from ``tof`` and pixel ``position`` to
     :math:`\\lambda` (``wavelength``), :math:`\\theta` (``theta``) and
     :math:`Q` (``Q``), but can take into account the Earth's gravitational field,
     which bends the flight path of the neutrons, to compute the scattering angle
@@ -237,35 +237,55 @@
     da: CleanWavelength[ScatteringRunType, IofQPart], mask: Optional[WavelengthMask]
 ) -> CleanWavelengthMasked[ScatteringRunType, IofQPart]:
     if mask is not None:
         da = mask_range(da, mask=mask)
     return CleanWavelengthMasked[ScatteringRunType, IofQPart](da)
 
 
+def _compute_Q(
+    data: sc.DataArray, graph: ElasticCoordTransformGraph, target: tuple[str, ...]
+) -> sc.DataArray:
+    # Keep naming of wavelength dim, subsequent steps use a (Q[xy], wavelength) binning.
+    return CleanQ[ScatteringRunType, IofQPart](
+        data.transform_coords(
+            target,
+            graph=graph,
+            keep_intermediate=False,
+            rename_dims=False,
+        )
+    )
+
+
 def compute_Q(
     data: CleanWavelengthMasked[ScatteringRunType, IofQPart],
     graph: ElasticCoordTransformGraph,
-    compute_Qxy: Optional[QxyBins],
 ) -> CleanQ[ScatteringRunType, IofQPart]:
     """
     Convert a data array from wavelength to Q.
     """
-    # Keep naming of wavelength dim, subsequent steps use a (Q[xy], wavelength) binning.
     return CleanQ[ScatteringRunType, IofQPart](
-        data.transform_coords(
-            ('Qx', 'Qy') if compute_Qxy else 'Q',
-            graph=graph,
-            keep_intermediate=False,
-            rename_dims=False,
-        )
+        _compute_Q(data=data, graph=graph, target=('Q',))
+    )
+
+
+def compute_Qxy(
+    data: CleanWavelengthMasked[ScatteringRunType, IofQPart],
+    graph: ElasticCoordTransformGraph,
+) -> CleanQxy[ScatteringRunType, IofQPart]:
+    """
+    Convert a data array from wavelength to Qx and Qy.
+    """
+    return CleanQxy[ScatteringRunType, IofQPart](
+        _compute_Q(data=data, graph=graph, target=('Qx', 'Qy'))
     )
 
 
 providers = (
     sans_elastic,
     sans_monitor,
     calibrate_positions,
     monitor_to_wavelength,
     detector_to_wavelength,
     mask_wavelength,
     compute_Q,
+    compute_Qxy,
 )
```

### Comparing `esssans-24.4.0/src/ess/sans/data.py` & `esssans-24.5.0/src/ess/sans/data.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/src/ess/sans/direct_beam.py` & `esssans-24.5.0/src/ess/sans/direct_beam.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     scaling = sc.values(iofq_full['Q', 0].data) / I0
     # Note: do not use a `set` here because the order of dimensions is important
     dims = [dim for dim in iofq_bands.dims if dim != 'Q']
     out = sc.array(dims=dims, values=eff) * scaling
     return out.rename_dims({wavelength_band_dim: 'wavelength'})
 
 
-def direct_beam(pipeline: Pipeline, I0: sc.Variable, niter: int = 5) -> List[dict]:
+def direct_beam(*, workflow: Pipeline, I0: sc.Variable, niter: int = 5) -> List[dict]:
     """
     Compute the direct beam function.
 
     Procedure:
 
     The idea behind the direct beam iterations is to determine an efficiency of the
     detectors as a function of wavelength.
@@ -92,54 +92,54 @@
     I0:
         The intensity of the I(Q) for the known sample at the lowest Q value.
     niter:
         The number of iterations to perform.
     """
 
     direct_beam_function = None
-    bands = pipeline.compute(ProcessedWavelengthBands)
+    bands = workflow.compute(ProcessedWavelengthBands)
     band_dim = (set(bands.dims) - {'wavelength'}).pop()
     full_wavelength_range = sc.concat([bands.min(), bands.max()], dim='wavelength')
 
-    pipeline = pipeline.copy()
+    workflow = workflow.copy()
 
-    wavelength_bins = pipeline.compute(WavelengthBins)
+    wavelength_bins = workflow.compute(WavelengthBins)
     parts = (
         FinalSummedQ[SampleRun, Numerator],
         FinalSummedQ[SampleRun, Denominator],
         FinalSummedQ[BackgroundRun, Numerator],
         FinalSummedQ[BackgroundRun, Denominator],
     )
-    parts = pipeline.compute(parts)
+    parts = workflow.compute(parts)
     # Convert events to histograms to make normalization (in every iteration) cheap
     for key in [
         FinalSummedQ[SampleRun, Numerator],
         FinalSummedQ[BackgroundRun, Numerator],
     ]:
         parts[key] = parts[key].hist(wavelength=wavelength_bins)
 
     # For now we simply strip all uncertainties, since direct beam function is
     # computed without variances anyway.
     parts = {key: sc.values(result) for key, result in parts.items()}
     for key, part in parts.items():
-        pipeline[key] = part
+        workflow[key] = part
     sample0 = parts[FinalSummedQ[SampleRun, Denominator]]
     background0 = parts[FinalSummedQ[BackgroundRun, Denominator]]
 
     results = []
 
     for _it in range(niter):
         # The first time we compute I(Q), the direct beam function is not in the
         # parameters, nor given by any providers, so it will be considered flat.
         # TODO: Should we have a check that DirectBeam cannot be computed from the
         # pipeline?
-        pipeline[WavelengthBands] = full_wavelength_range
-        iofq_full = pipeline.compute(BackgroundSubtractedIofQ)
-        pipeline[WavelengthBands] = bands
-        iofq_bands = pipeline.compute(BackgroundSubtractedIofQ)
+        workflow[WavelengthBands] = full_wavelength_range
+        iofq_full = workflow.compute(BackgroundSubtractedIofQ)
+        workflow[WavelengthBands] = bands
+        iofq_bands = workflow.compute(BackgroundSubtractedIofQ)
 
         if direct_beam_function is None:
             # Make a flat direct beam
             dims = [dim for dim in iofq_bands.dims if dim != 'Q']
             direct_beam_function = sc.DataArray(
                 data=sc.ones(sizes={dim: iofq_bands.sizes[dim] for dim in dims}),
                 coords={band_dim: sc.midpoints(bands, dim='wavelength').squeeze()},
@@ -157,16 +157,16 @@
         db = resample_direct_beam(
             direct_beam=direct_beam_function,
             wavelength_bins=wavelength_bins,
         )
         db.coords['wavelength'] = sc.midpoints(
             db.coords['wavelength'], dim='wavelength'
         )
-        pipeline[FinalSummedQ[SampleRun, Denominator]] = sample0 * db
-        pipeline[FinalSummedQ[BackgroundRun, Denominator]] = background0 * db
+        workflow[FinalSummedQ[SampleRun, Denominator]] = sample0 * db
+        workflow[FinalSummedQ[BackgroundRun, Denominator]] = background0 * db
 
         results.append(
             {
                 'iofq_full': iofq_full,
                 'iofq_bands': iofq_bands,
                 'direct_beam': direct_beam_function,
             }
```

### Comparing `esssans-24.4.0/src/ess/sans/i_of_q.py` & `esssans-24.5.0/src/ess/sans/i_of_q.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 import uuid
 from typing import Optional
 
 import sciline
 import scipp as sc
 from scipp.scipy.interpolate import interp1d
 
 from .common import mask_range
 from .logging import get_logger
 from .types import (
     BackgroundRun,
     BackgroundSubtractedIofQ,
+    BackgroundSubtractedIofQxy,
     CleanDirectBeam,
     CleanMonitor,
     CleanQ,
+    CleanQxy,
     CleanSummedQ,
     CleanSummedQMergedBanks,
+    CleanSummedQxy,
+    CleanSummedQxyMergedBanks,
     DimsToKeep,
     DirectBeam,
     Filename,
     FinalSummedQ,
+    FinalSummedQxy,
     IofQ,
     IofQPart,
+    IofQxy,
     MonitorType,
     NeXusDetectorName,
     NonBackgroundWavelengthRange,
     QBins,
-    QxyBins,
+    QxBins,
+    QyBins,
     ReturnEvents,
     RunType,
     SampleRun,
     ScatteringRunType,
     UncertaintyBroadcastMode,
     WavelengthBins,
     WavelengthMonitor,
@@ -135,17 +141,16 @@
         bounds_error=False,
     )
     return CleanDirectBeam(func(wavelength_bins, midpoints=True))
 
 
 def bin_in_q(
     data: CleanQ[ScatteringRunType, IofQPart],
-    q_bins: Optional[QBins],
-    qxy_bins: Optional[QxyBins],
-    dims_to_keep: Optional[DimsToKeep],
+    q_bins: QBins,
+    dims_to_keep: DimsToKeep,
 ) -> CleanSummedQ[ScatteringRunType, IofQPart]:
     """
     Merges data from all pixels into a single I(Q) spectrum:
 
     * In the case of event data, events in all bins are concatenated
     * In the case of dense data, counts in all spectra are summed
 
@@ -160,24 +165,63 @@
         I(Q) result (this is typically the layer dimension).
 
     Returns
     -------
     :
         The input data converted to Q and then summed over all detector pixels.
     """
+    out = _bin_in_q(data=data, edges={'Q': q_bins}, dims_to_keep=dims_to_keep)
+    return CleanSummedQ[ScatteringRunType, IofQPart](out)
+
+
+def bin_in_qxy(
+    data: CleanQxy[ScatteringRunType, IofQPart],
+    qx_bins: QxBins,
+    qy_bins: QyBins,
+    dims_to_keep: DimsToKeep,
+) -> CleanSummedQxy[ScatteringRunType, IofQPart]:
+    """
+    Merges data from all pixels into a single I(Q) spectrum:
+
+    * In the case of event data, events in all bins are concatenated
+    * In the case of dense data, counts in all spectra are summed
+
+    Parameters
+    ----------
+    data:
+        A DataArray containing the data that is to be converted to Q.
+    qx_bins:
+        The binning in Qx to be used.
+    qy_bins:
+        The binning in Qy to be used.
+    dims_to_keep:
+        Dimensions that should not be reduced and thus still be present in the final
+        I(Q) result (this is typically the layer dimension).
+
+    Returns
+    -------
+    :
+        The input data converted to Qx and Qy and then summed over all detector pixels.
+    """
+    # We make Qx the inner dim, such that plots naturally show Qx on the x-axis.
+    out = _bin_in_q(
+        data=data,
+        edges={'Qy': qy_bins, 'Qx': qx_bins},
+        dims_to_keep=dims_to_keep,
+    )
+    return CleanSummedQxy[ScatteringRunType, IofQPart](out)
+
+
+def _bin_in_q(
+    data: sc.DataArray, edges: dict[str, sc.Variable], dims_to_keep: tuple[str, ...]
+) -> sc.DataArray:
     dims_to_reduce = set(data.dims) - {'wavelength'}
     if dims_to_keep is not None:
         dims_to_reduce -= set(dims_to_keep)
 
-    if qxy_bins:
-        # We make Qx the inner dim, such that plots naturally show Qx on the x-axis.
-        edges = {'Qy': qxy_bins['Qy'], 'Qx': qxy_bins['Qx']}
-    else:
-        edges = {'Q': q_bins}
-
     if data.bins is not None:
         q_all_pixels = data.bins.concat(dims_to_reduce)
         # q_all_pixels may just have a single bin now, which currently yields
         # inferior performance when binning (no/bad multi-threading?).
         # We operate on the content buffer for better multi-threaded performance.
         if q_all_pixels.ndim == 0:
             content = q_all_pixels.bins.constituents['data']
@@ -220,29 +264,41 @@
                     flat.coords[dim] = sc.arange(dim, flat.sizes[dim])
             out = (
                 flat.flatten(to=str(uuid.uuid4()))
                 .group(*[flat.coords[dim] for dim in flat.dims if dim != helper_dim])
                 .drop_coords(dims_to_keep or ())
                 .hist(**edges)
             )
-    return CleanSummedQ[ScatteringRunType, IofQPart](out.squeeze())
+    return out.squeeze()
 
 
 def no_bank_merge(
     data: CleanSummedQ[ScatteringRunType, IofQPart]
 ) -> CleanSummedQMergedBanks[ScatteringRunType, IofQPart]:
     return CleanSummedQMergedBanks[ScatteringRunType, IofQPart](data)
 
 
+def no_bank_merge_xy(
+    data: CleanSummedQxy[ScatteringRunType, IofQPart]
+) -> CleanSummedQxyMergedBanks[ScatteringRunType, IofQPart]:
+    return CleanSummedQxyMergedBanks[ScatteringRunType, IofQPart](data)
+
+
 def no_run_merge(
     data: CleanSummedQMergedBanks[ScatteringRunType, IofQPart]
 ) -> FinalSummedQ[ScatteringRunType, IofQPart]:
     return FinalSummedQ[ScatteringRunType, IofQPart](data)
 
 
+def no_run_merge_xy(
+    data: CleanSummedQxyMergedBanks[ScatteringRunType, IofQPart]
+) -> FinalSummedQxy[ScatteringRunType, IofQPart]:
+    return FinalSummedQxy[ScatteringRunType, IofQPart](data)
+
+
 def _merge_contributions(data: list[sc.DataArray]) -> sc.DataArray:
     if len(data) == 1:
         return data[0]
     reducer = sc.reduce(data)
     return reducer.bins.concat() if data[0].bins is not None else reducer.sum()
 
 
@@ -254,14 +310,28 @@
     denominator, before the normalization step.
     """
     return CleanSummedQMergedBanks[ScatteringRunType, IofQPart](
         _merge_contributions(list(banks.values()))
     )
 
 
+def merge_banks_xy(
+    banks: sciline.Series[
+        NeXusDetectorName, CleanSummedQxy[ScatteringRunType, IofQPart]
+    ]
+) -> CleanSummedQxyMergedBanks[ScatteringRunType, IofQPart]:
+    """
+    Merge the events or counts from multiple detector banks into a single numerator or
+    denominator, before the normalization step.
+    """
+    return CleanSummedQxyMergedBanks[ScatteringRunType, IofQPart](
+        _merge_contributions(list(banks.values()))
+    )
+
+
 def merge_runs(
     runs: sciline.Series[
         Filename[ScatteringRunType],
         CleanSummedQMergedBanks[ScatteringRunType, IofQPart],
     ],
 ) -> FinalSummedQ[ScatteringRunType, IofQPart]:
     """
@@ -269,29 +339,72 @@
     denominator, before the normalization step.
     """
     return FinalSummedQ[ScatteringRunType, IofQPart](
         _merge_contributions(list(runs.values()))
     )
 
 
-def subtract_background(
-    sample: IofQ[SampleRun],
-    background: IofQ[BackgroundRun],
+def merge_runs_xy(
+    runs: sciline.Series[
+        Filename[ScatteringRunType],
+        CleanSummedQxyMergedBanks[ScatteringRunType, IofQPart],
+    ],
+) -> FinalSummedQxy[ScatteringRunType, IofQPart]:
+    """
+    Merge the events or counts from multiple runs into a single numerator or
+    denominator, before the normalization step.
+    """
+    return FinalSummedQxy[ScatteringRunType, IofQPart](
+        _merge_contributions(list(runs.values()))
+    )
+
+
+def _subtract_background(
+    sample: sc.DataArray,
+    background: sc.DataArray,
     return_events: ReturnEvents,
-) -> BackgroundSubtractedIofQ:
+) -> sc.DataArray:
     if return_events and sample.bins is not None and background.bins is not None:
         return sample.bins.concatenate(-background)
     if sample.bins is not None:
         sample = sample.bins.sum()
     if background.bins is not None:
         background = background.bins.sum()
-    return BackgroundSubtractedIofQ(sample - background)
+    return sample - background
+
+
+def subtract_background(
+    sample: IofQ[SampleRun],
+    background: IofQ[BackgroundRun],
+    return_events: ReturnEvents,
+) -> BackgroundSubtractedIofQ:
+    return BackgroundSubtractedIofQ(
+        _subtract_background(
+            sample=sample, background=background, return_events=return_events
+        )
+    )
+
+
+def subtract_background_xy(
+    sample: IofQxy[SampleRun],
+    background: IofQxy[BackgroundRun],
+    return_events: ReturnEvents,
+) -> BackgroundSubtractedIofQxy:
+    return BackgroundSubtractedIofQxy(
+        _subtract_background(
+            sample=sample, background=background, return_events=return_events
+        )
+    )
 
 
 providers = (
     preprocess_monitor_data,
     resample_direct_beam,
     bin_in_q,
+    bin_in_qxy,
     subtract_background,
+    subtract_background_xy,
     no_bank_merge,
+    no_bank_merge_xy,
     no_run_merge,
+    no_run_merge_xy,
 )
```

### Comparing `esssans-24.4.0/src/ess/sans/io.py` & `esssans-24.5.0/src/ess/sans/io.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/src/ess/sans/logging.py` & `esssans-24.5.0/src/ess/sans/logging.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/src/ess/sans/masking.py` & `esssans-24.5.0/src/ess/sans/masking.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """
 Masking functions for the loki workflow.
 """
-from typing import Optional
-
 import numpy as np
 import sciline
 import scipp as sc
 
 from .types import (
     MaskedData,
     MaskedDetectorIDs,
@@ -16,15 +14,15 @@
     ScatteringRunType,
     TofData,
 )
 
 
 def apply_pixel_masks(
     data: TofData[ScatteringRunType],
-    masked_ids: Optional[sciline.Series[PixelMaskFilename, MaskedDetectorIDs]],
+    masked_ids: sciline.Series[PixelMaskFilename, MaskedDetectorIDs],
 ) -> MaskedData[ScatteringRunType]:
     """Apply pixel-specific masks to raw data.
     The masks are based on detector IDs stored in XML files.
 
     Parameters
     ----------
     data:
```

### Comparing `esssans-24.4.0/src/ess/sans/normalization.py` & `esssans-24.5.0/src/ess/sans/normalization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 from typing import Optional
 
 import scipp as sc
 from scipp.core import concepts
 
 from .types import (
     CalibratedMaskedData,
     CleanDirectBeam,
     CleanMonitor,
     CleanWavelength,
     Denominator,
     DetectorPixelShape,
     EmptyBeamRun,
     FinalSummedQ,
+    FinalSummedQxy,
     Incident,
     IofQ,
+    IofQxy,
     LabFrameTransform,
     NormWavelengthTerm,
     Numerator,
     ProcessedWavelengthBands,
     ReturnEvents,
     ScatteringRunType,
     SolidAngle,
@@ -334,21 +335,21 @@
             'Wavelength_bands must have a size of 2 in the wavelength dimension, '
             'defining a start and an end wavelength, '
             f'got {wavelength_bands.sizes["wavelength"]}.'
         )
     return wavelength_bands
 
 
-def normalize(
-    numerator: FinalSummedQ[ScatteringRunType, Numerator],
-    denominator: FinalSummedQ[ScatteringRunType, Denominator],
+def _normalize(
+    numerator: sc.DataArray,
+    denominator: sc.DataArray,
     return_events: ReturnEvents,
     uncertainties: UncertaintyBroadcastMode,
     wavelength_bands: ProcessedWavelengthBands,
-) -> IofQ[ScatteringRunType]:
+) -> sc.DataArray:
     """
     Perform normalization of counts as a function of Q.
     If the numerator contains events, we use the sc.lookup function to perform the
     division.
 
     Parameters
     ----------
@@ -409,18 +410,59 @@
                     denominator, events=numerator
                 )
     elif numerator.bins is not None:
         numerator = numerator.hist()
     numerator /= denominator.drop_coords(
         [name for name in denominator.coords if name not in denominator.dims]
     )
-    return IofQ[ScatteringRunType](numerator)
+    return numerator
+
+
+def normalize_q(
+    numerator: FinalSummedQ[ScatteringRunType, Numerator],
+    denominator: FinalSummedQ[ScatteringRunType, Denominator],
+    return_events: ReturnEvents,
+    uncertainties: UncertaintyBroadcastMode,
+    wavelength_bands: ProcessedWavelengthBands,
+) -> IofQ[ScatteringRunType]:
+    return IofQ[ScatteringRunType](
+        _normalize(
+            numerator=numerator,
+            denominator=denominator,
+            return_events=return_events,
+            uncertainties=uncertainties,
+            wavelength_bands=wavelength_bands,
+        )
+    )
+
+
+def normalize_qxy(
+    numerator: FinalSummedQxy[ScatteringRunType, Numerator],
+    denominator: FinalSummedQxy[ScatteringRunType, Denominator],
+    return_events: ReturnEvents,
+    uncertainties: UncertaintyBroadcastMode,
+    wavelength_bands: ProcessedWavelengthBands,
+) -> IofQxy[ScatteringRunType]:
+    return IofQxy[ScatteringRunType](
+        _normalize(
+            numerator=numerator,
+            denominator=denominator,
+            return_events=return_events,
+            uncertainties=uncertainties,
+            wavelength_bands=wavelength_bands,
+        )
+    )
+
+
+normalize_q.__doc__ = _normalize.__doc__
+normalize_qxy.__doc__ = _normalize.__doc__
 
 
 providers = (
     transmission_fraction,
     iofq_norm_wavelength_term,
     iofq_denominator,
-    normalize,
+    normalize_q,
+    normalize_qxy,
     process_wavelength_bands,
     solid_angle,
 )
```

### Comparing `esssans-24.4.0/src/ess/sans/types.py` & `esssans-24.5.0/src/ess/sans/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,18 +116,21 @@
 ProcessedWavelengthBands = NewType('ProcessedWavelengthBands', sc.Variable)
 """Processed wavelength bands, as a two-dimensional variable, with the first dimension
 being the band index and the second dimension being the wavelength. For each band, there
 must be two wavelength values defining the start and end wavelength of the band."""
 
 
 QBins = NewType('QBins', sc.Variable)
-"""Q binning"""
+"""Q binning used when computing IofQ"""
 
-QxyBins = NewType('QxyBins', dict[str, sc.Variable])
-"""Binning for 'Qx' and 'Qy'. If set this overrides QBins."""
+QxBins = NewType('QxBins', sc.Variable)
+"""Qx binning used when computing IofQxy"""
+
+QyBins = NewType('QyBins', sc.Variable)
+"""Qy binning used when computing IofQxy"""
 
 NonBackgroundWavelengthRange = NewType('NonBackgroundWavelengthRange', sc.Variable)
 """Range of wavelengths that are not considered background in the monitor"""
 
 DirectBeamFilename = NewType('DirectBeamFilename', str)
 """Filename of direct beam correction"""
 
@@ -153,21 +156,14 @@
 
 
 PixelMaskFilename = NewType('PixelMaskFilename', str)
 
 FilenameType = TypeVar('FilenameType', bound=str)
 
 
-DataFolder = NewType('DataFolder', str)
-
-
-class FilePath(sciline.Scope[FilenameType, str], str):
-    """Path to a file"""
-
-
 class Filename(sciline.Scope[RunType, str], str):
     """Filename of a run"""
 
 
 MaskedDetectorIDs = NewType('MaskedDetectorIDs', sc.Variable)
 """1-D variable listing all masked detector IDs."""
 
@@ -289,39 +285,71 @@
 
 class CleanQ(
     sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
 ):
     """Result of converting :py:class:`CleanWavelengthMasked` to Q"""
 
 
+class CleanQxy(
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
+):
+    """Result of converting :py:class:`CleanWavelengthMasked` to Qx and Qy"""
+
+
 class CleanSummedQ(
     sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
 ):
     """Result of histogramming/binning :py:class:`CleanQ` over all pixels into Q bins"""
 
 
+class CleanSummedQxy(
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
+):
+    """Result of histogramming/binning :py:class:`CleanQxy` over all pixels into Qx and
+    Qy bins"""
+
+
 class CleanSummedQMergedBanks(
     sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
 ):
     """CleanSummedQ with merged banks"""
 
 
+class CleanSummedQxyMergedBanks(
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
+):
+    """CleanSummedQxy with merged banks"""
+
+
 class FinalSummedQ(
     sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
 ):
     """Final data into Q bins, in a state that is ready to be normalized."""
 
 
+class FinalSummedQxy(
+    sciline.ScopeTwoParams[ScatteringRunType, IofQPart, sc.DataArray], sc.DataArray
+):
+    """Final data into Qx and Qy bins, in a state that is ready to be normalized."""
+
+
 class IofQ(sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray):
     """I(Q)"""
 
 
+class IofQxy(sciline.Scope[ScatteringRunType, sc.DataArray], sc.DataArray):
+    """I(Qx, Qy)"""
+
+
 BackgroundSubtractedIofQ = NewType('BackgroundSubtractedIofQ', sc.DataArray)
 """I(Q) with background (given by I(Q) of the background run) subtracted"""
 
+BackgroundSubtractedIofQxy = NewType('BackgroundSubtractedIofQxy', sc.DataArray)
+"""I(Qx, Qy) with background (given by I(Qx, Qy) of the background run) subtracted"""
+
 
 class RawMonitor(
     sciline.ScopeTwoParams[RunType, MonitorType, sc.DataArray], sc.DataArray
 ):
     """Raw monitor data"""
```

### Comparing `esssans-24.4.0/src/ess/sans/uncertainty.py` & `esssans-24.5.0/src/ess/sans/uncertainty.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/src/esssans.egg-info/PKG-INFO` & `esssans-24.5.0/src/esssans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esssans
-Version: 24.4.0
+Version: 24.5.0
 Summary: SANS data reduction for the European Spallation Source
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `esssans-24.4.0/src/esssans.egg-info/SOURCES.txt` & `esssans-24.5.0/src/esssans.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/high-level-requirement.yml
 .github/workflows/ci.yml
+.github/workflows/copier.yml
 .github/workflows/docs.yml
 .github/workflows/nightly_at_main.yml
 .github/workflows/nightly_at_release.yml
 .github/workflows/python-version-ci
 .github/workflows/release.yml
 .github/workflows/test.yml
 .github/workflows/unpinned.yml
@@ -71,18 +72,20 @@
 src/ess/isissans/components.py
 src/ess/isissans/data.py
 src/ess/isissans/general.py
 src/ess/isissans/io.py
 src/ess/isissans/mantidio.py
 src/ess/isissans/sans2d.py
 src/ess/isissans/visualization.py
+src/ess/isissans/zoom.py
 src/ess/loki/__init__.py
 src/ess/loki/data.py
 src/ess/loki/general.py
 src/ess/loki/io.py
+src/ess/loki/workflow.py
 src/ess/sans/__init__.py
 src/ess/sans/beam_center_finder.py
 src/ess/sans/common.py
 src/ess/sans/conversions.py
 src/ess/sans/data.py
 src/ess/sans/direct_beam.py
 src/ess/sans/i_of_q.py
@@ -92,20 +95,22 @@
 src/ess/sans/normalization.py
 src/ess/sans/py.typed
 src/ess/sans/types.py
 src/ess/sans/uncertainty.py
 src/esssans.egg-info/PKG-INFO
 src/esssans.egg-info/SOURCES.txt
 src/esssans.egg-info/dependency_links.txt
+src/esssans.egg-info/entry_points.txt
 src/esssans.egg-info/requires.txt
 src/esssans.egg-info/top_level.txt
 tests/common_test.py
 tests/i_of_q_test.py
 tests/io_test.py
 tests/normalization_test.py
 tests/package_test.py
 tests/uncertainty_test.py
 tests/isissans/sans2d_reduction_test.py
 tests/isissans/zoom_reduction_test.py
 tests/loki/common.py
 tests/loki/directbeam_test.py
-tests/loki/iofq_test.py
+tests/loki/iofq_test.py
+tests/loki/live_reduction_test.py
```

### Comparing `esssans-24.4.0/tests/common_test.py` & `esssans-24.5.0/tests/common_test.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/tests/i_of_q_test.py` & `esssans-24.5.0/tests/i_of_q_test.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/tests/io_test.py` & `esssans-24.5.0/tests/io_test.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/tests/isissans/sans2d_reduction_test.py` & `esssans-24.5.0/tests/isissans/sans2d_reduction_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ess import sans
 from ess.isissans import MonitorOffset, SampleOffset, sans2d
 from ess.sans.types import (
     BackgroundRun,
     BackgroundSubtractedIofQ,
     BeamCenter,
     CorrectForGravity,
+    DimsToKeep,
     DirectBeam,
     DirectBeamFilename,
     EmptyBeamRun,
     Filename,
     Incident,
     IofQ,
     MaskedData,
@@ -33,15 +34,15 @@
     WavelengthBands,
     WavelengthBins,
     WavelengthMask,
 )
 
 
 def make_params() -> dict:
-    params = {}
+    params = isis.default_parameters()
     params[WavelengthBins] = sc.linspace(
         'wavelength', start=2.0, stop=16.0, num=141, unit='angstrom'
     )
     params[WavelengthMask] = sc.DataArray(
         data=sc.array(dims=['wavelength'], values=[True]),
         coords={
             'wavelength': sc.array(
@@ -50,42 +51,45 @@
         },
     )
     params[sans2d.LowCountThreshold] = sc.scalar(100.0, unit='counts')
 
     params[QBins] = sc.linspace(
         dim='Q', start=0.01, stop=0.55, num=141, unit='1/angstrom'
     )
-    params[DirectBeamFilename] = 'DIRECT_SANS2D_REAR_34327_4m_8mm_16Feb16.dat'
-    params[Filename[SampleRun]] = 'SANS2D00063114.nxs'
-    params[Filename[BackgroundRun]] = 'SANS2D00063159.nxs'
-    params[Filename[EmptyBeamRun]] = 'SANS2D00063091.nxs'
+    params[DirectBeamFilename] = isis.data.sans2d_tutorial_direct_beam()
+    params[Filename[SampleRun]] = isis.data.sans2d_tutorial_sample_run()
+    params[Filename[BackgroundRun]] = isis.data.sans2d_tutorial_background_run()
+    params[Filename[EmptyBeamRun]] = isis.data.sans2d_tutorial_empty_beam_run()
 
     params[NeXusMonitorName[Incident]] = 'monitor2'
     params[NeXusMonitorName[Transmission]] = 'monitor4'
     params[SampleOffset] = sc.vector([0.0, 0.0, 0.053], unit='m')
     params[MonitorOffset[Transmission]] = sc.vector([0.0, 0.0, -6.719], unit='m')
 
     params[NonBackgroundWavelengthRange] = sc.array(
         dims=['wavelength'], values=[0.7, 17.1], unit='angstrom'
     )
     params[CorrectForGravity] = True
     params[UncertaintyBroadcastMode] = UncertaintyBroadcastMode.upper_bound
     params[ReturnEvents] = False
+    params[DimsToKeep] = tuple()
     return params
 
 
 def sans2d_providers():
     return list(
         sans.providers
         + isis.providers
-        + isis.data.providers
         + isis.sans2d.providers
+        + isis.mantidio.providers
         + (
             isis.data.transmission_from_background_run,
             isis.data.transmission_from_sample_run,
+            isis.data.load_tutorial_direct_beam,
+            isis.data.load_tutorial_run,
             sans.beam_center_finder.beam_center_from_center_of_mass,
         )
     )
 
 
 def test_can_create_pipeline():
     sciline.Pipeline(sans2d_providers(), params=make_params())
@@ -180,15 +184,15 @@
 
     return dict(zip([get_type_hints(func)['return'] for func in funcs], funcs))
 
 
 def pixel_dependent_direct_beam(
     filename: DirectBeamFilename, shape: RawData[SampleRun]
 ) -> DirectBeam:
-    direct_beam = isis.data.load_direct_beam(isis.data.get_path(filename))
+    direct_beam = isis.data.load_tutorial_direct_beam(filename)
     sizes = {'spectrum': shape.sizes['spectrum'], **direct_beam.sizes}
     return DirectBeam(direct_beam.broadcast(sizes=sizes).copy())
 
 
 @pytest.mark.parametrize(
     'uncertainties',
     [UncertaintyBroadcastMode.drop, UncertaintyBroadcastMode.upper_bound],
```

### Comparing `esssans-24.4.0/tests/loki/directbeam_test.py` & `esssans-24.5.0/tests/loki/directbeam_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,29 @@
 import sys
 from pathlib import Path
 
 import sciline
 import scipp as sc
 from scipp.scipy.interpolate import interp1d
 
-from ess import sans
-from ess.loki.data import get_path
-from ess.sans.types import DimsToKeep, QBins, WavelengthBands, WavelengthBins
+from ess import loki, sans
+from ess.sans.types import (
+    DimsToKeep,
+    PixelMaskFilename,
+    QBins,
+    WavelengthBands,
+    WavelengthBins,
+)
 
 sys.path.insert(0, str(Path(__file__).resolve().parent))
 from common import loki_providers, make_params  # noqa: E402
 
 
 def _get_I0(qbins: sc.Variable) -> sc.Variable:
-    Iq_theory = sc.io.load_hdf5(get_path('PolyGauss_I0-50_Rg-60.h5'))
+    Iq_theory = sc.io.load_hdf5(loki.data.loki_tutorial_poly_gauss_I0())
     f = interp1d(Iq_theory, 'Q')
     return f(sc.midpoints(qbins)).data[0]
 
 
 def test_can_compute_direct_beam_for_all_pixels():
     n_wavelength_bands = 10
     params = make_params()
@@ -28,17 +33,18 @@
         'wavelength',
         params[WavelengthBins].min(),
         params[WavelengthBins].max(),
         n_wavelength_bands + 1,
     )
     providers = loki_providers()
     pipeline = sciline.Pipeline(providers, params=params)
+    pipeline.set_param_series(PixelMaskFilename, [])
     I0 = _get_I0(qbins=params[QBins])
 
-    results = sans.direct_beam(pipeline=pipeline, I0=I0, niter=4)
+    results = sans.direct_beam(workflow=pipeline, I0=I0, niter=4)
     iofq_full = results[-1]['iofq_full']
     iofq_bands = results[-1]['iofq_bands']
     direct_beam_function = results[-1]['direct_beam']
 
     assert iofq_full.dims == ('Q',)
     assert iofq_bands.dims == ('band', 'Q')
     assert iofq_bands.sizes['band'] == n_wavelength_bands
@@ -57,17 +63,18 @@
     )
     params[WavelengthBands] = sc.concat(
         [edges[:-2], edges[2::]], dim='wavelength'
     ).transpose()
 
     providers = loki_providers()
     pipeline = sciline.Pipeline(providers, params=params)
+    pipeline.set_param_series(PixelMaskFilename, [])
     I0 = _get_I0(qbins=params[QBins])
 
-    results = sans.direct_beam(pipeline=pipeline, I0=I0, niter=4)
+    results = sans.direct_beam(workflow=pipeline, I0=I0, niter=4)
     iofq_full = results[-1]['iofq_full']
     iofq_bands = results[-1]['iofq_bands']
     direct_beam_function = results[-1]['direct_beam']
 
     assert iofq_full.dims == ('Q',)
     assert iofq_bands.dims == ('band', 'Q')
     assert iofq_bands.sizes['band'] == n_wavelength_bands
@@ -82,17 +89,18 @@
         params[WavelengthBins].min(),
         params[WavelengthBins].max(),
         n_wavelength_bands + 1,
     )
     params[DimsToKeep] = ['layer']
     providers = loki_providers()
     pipeline = sciline.Pipeline(providers, params=params)
+    pipeline.set_param_series(PixelMaskFilename, [])
     I0 = _get_I0(qbins=params[QBins])
 
-    results = sans.direct_beam(pipeline=pipeline, I0=I0, niter=4)
+    results = sans.direct_beam(workflow=pipeline, I0=I0, niter=4)
     iofq_full = results[-1]['iofq_full']
     iofq_bands = results[-1]['iofq_bands']
     direct_beam_function = results[-1]['direct_beam']
 
     assert iofq_full.dims == ('layer', 'Q')
     assert iofq_bands.dims == ('band', 'layer', 'Q')
     assert iofq_bands.sizes['band'] == n_wavelength_bands
@@ -106,20 +114,21 @@
     params = make_params()
     params[WavelengthBands] = sc.linspace(
         'wavelength',
         params[WavelengthBins].min(),
         params[WavelengthBins].max(),
         n_wavelength_bands + 1,
     )
-    params[DimsToKeep] = ['layer', 'straw']
+    params[DimsToKeep] = ('layer', 'straw')
     providers = loki_providers()
     pipeline = sciline.Pipeline(providers, params=params)
+    pipeline.set_param_series(PixelMaskFilename, [])
     I0 = _get_I0(qbins=params[QBins])
 
-    results = sans.direct_beam(pipeline=pipeline, I0=I0, niter=4)
+    results = sans.direct_beam(workflow=pipeline, I0=I0, niter=4)
     iofq_full = results[-1]['iofq_full']
     iofq_bands = results[-1]['iofq_bands']
     direct_beam_function = results[-1]['direct_beam']
 
     assert iofq_full.dims == ('layer', 'straw', 'Q')
     assert iofq_bands.dims == ('band', 'layer', 'straw', 'Q')
     assert iofq_bands.sizes['band'] == n_wavelength_bands
```

### Comparing `esssans-24.4.0/tests/normalization_test.py` & `esssans-24.5.0/tests/normalization_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import numpy as np
 import pytest
 import scipp as sc
 
-from ess.isissans.data import get_path
+from ess.isissans.data import sans2d_solid_angle_reference
 from ess.sans import normalization
 
 # See https://github.com/mantidproject/mantid/blob/main/instrument/SANS2D_Definition_Tubes.xml  # noqa: E501
 _SANS2D_PIXEL_RADIUS = 0.00405 * sc.Unit('m')
 _SANS2D_PIXEL_LENGTH = 0.002033984375 * sc.Unit('m')
-_SANS2D_SOLID_ANGLE_REFERENCE_FILE = 'SANS2D00063091.SolidAngle_from_mantid.h5'
 
 
 def _sans2d_geometry():
     R = _SANS2D_PIXEL_RADIUS.value
     L = _SANS2D_PIXEL_LENGTH.value
     pixel_shape = {
         'vertices': sc.vectors(
@@ -33,15 +32,15 @@
     return dict(pixel_shape=pixel_shape, transform=transform)
 
 
 def _mantid_sans2d_solid_angle_data():
     simpleapi = pytest.importorskip("mantid.simpleapi")
     scippneutron = pytest.importorskip("scippneutron")
 
-    ws = simpleapi.Load(get_path('SANS2D00063091.nxs'))
+    ws = simpleapi.Load('SANS2D00063091.nxs')
     radius = _SANS2D_PIXEL_RADIUS
     length = _SANS2D_PIXEL_LENGTH
 
     simpleapi.SetInstrumentParameter(
         ws,
         ParameterName='x-pixel-size',
         ParameterType='Number',
@@ -52,16 +51,16 @@
         ParameterName='y-pixel-size',
         ParameterType='Number',
         Value=str(length.to(unit='mm').value),
     )
     outWs = simpleapi.SolidAngle(ws, method='HorizontalTube')
     da = scippneutron.from_mantid(outWs)['data']['spectrum', :120000:100]
     # Create new reference file:
-    # sc.io.hdf5.save_hdf5(da, _SANS2D_SOLID_ANGLE_REFERENCE_FILE)
-    # Note, also update the name, don't overwrite old reference files.
+    # sc.io.hdf5.save_hdf5(da, 'SANS2D00063091.SolidAngle_from_mantid.h5')
+    # Note, also update the registry version, don't overwrite old reference files.
     # Overwriting reference files breaks old versions of the repository.
     return da
 
 
 @pytest.mark.filterwarnings("ignore:.*")
 def test_solid_angle_compare_to_mantid():
     da = _mantid_sans2d_solid_angle_data()
@@ -71,15 +70,15 @@
     ).data
     assert sc.allclose(
         da.data['tof', 0], solid_angle, atol=0.0 * sc.Unit('dimensionless')
     )
 
 
 def test_solid_angle_compare_to_reference_file():
-    da = sc.io.load_hdf5(filename=get_path(_SANS2D_SOLID_ANGLE_REFERENCE_FILE))
+    da = sc.io.load_hdf5(filename=sans2d_solid_angle_reference())
     solid_angle = normalization.solid_angle(
         da,
         **_sans2d_geometry(),
     ).data
     assert sc.allclose(
         da.data['tof', 0], solid_angle, atol=0.0 * sc.Unit('dimensionless')
     )
```

### Comparing `esssans-24.4.0/tests/uncertainty_test.py` & `esssans-24.5.0/tests/uncertainty_test.py`

 * *Files identical despite different names*

### Comparing `esssans-24.4.0/tox.ini` & `esssans-24.5.0/tox.ini`

 * *Files identical despite different names*

