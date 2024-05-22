# Comparing `tmp/dbt_artifacts_parser-0.6.0.tar.gz` & `tmp/dbt_artifacts_parser-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_artifacts_parser-0.6.0.tar", last modified: Tue May 21 09:33:13 2024, max compression
+gzip compressed data, was "dbt_artifacts_parser-0.7.0.tar", last modified: Wed May 22 00:39:33 2024, max compression
```

## Comparing `dbt_artifacts_parser-0.6.0.tar` & `dbt_artifacts_parser-0.7.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    11357 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/LICENSE
--rw-r--r--   0        0        0    10523 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/README.md
--rw-r--r--   0        0        0      859 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/__init__.py
--rw-r--r--   0        0        0    14365 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parser.py
--rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/__init__.py
--rw-r--r--   0        0        0      977 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/base.py
--rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/catalog/__init__.py
--rw-r--r--   0        0        0     1887 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
--rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/__init__.py
--rw-r--r--   0        0        0    39709 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
--rw-r--r--   0        0        0    47940 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v10.py
--rw-r--r--   0        0        0    44179 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v11.py
--rw-r--r--   0        0        0   162546 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v12.py
--rw-r--r--   0        0        0    40546 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
--rw-r--r--   0        0        0    41294 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
--rw-r--r--   0        0        0    46633 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
--rw-r--r--   0        0        0    47752 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
--rw-r--r--   0        0        0    48520 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
--rw-r--r--   0        0        0    52862 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
--rw-r--r--   0        0        0    35032 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
--rw-r--r--   0        0        0    39343 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
--rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/__init__.py
--rw-r--r--   0        0        0     1719 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
--rw-r--r--   0        0        0     1755 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
--rw-r--r--   0        0        0     3346 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
--rw-r--r--   0        0        0     3458 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
--rw-r--r--   0        0        0     1839 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v5.py
--rw-r--r--   0        0        0     1759 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v6.py
--rw-r--r--   0        0        0      796 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/__init__.py
--rw-r--r--   0        0        0     2044 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v1.py
--rw-r--r--   0        0        0     2327 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v2.py
--rw-r--r--   0        0        0     2441 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v3.py
--rw-r--r--   0        0        0     2348 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/utils.py
--rw-r--r--   0        0        0     5202 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/version_map.py
--rw-r--r--   0        0        0     5968 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json
--rw-r--r--   0        0        0   129577 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json
--rw-r--r--   0        0        0   148278 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v10.json
--rw-r--r--   0        0        0   130575 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v11.json
--rw-r--r--   0        0        0   724056 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v12.json
--rw-r--r--   0        0        0   135379 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json
--rw-r--r--   0        0        0   138302 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json
--rw-r--r--   0        0        0   157235 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json
--rw-r--r--   0        0        0   159203 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json
--rw-r--r--   0        0        0   163791 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json
--rw-r--r--   0        0        0   174833 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json
--rw-r--r--   0        0        0   115570 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json
--rw-r--r--   0        0        0   129190 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json
--rw-r--r--   0        0        0     4622 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json
--rw-r--r--   0        0        0     4777 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json
--rw-r--r--   0        0        0     9817 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json
--rw-r--r--   0        0        0    10272 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json
--rw-r--r--   0        0        0     4690 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v5.json
--rw-r--r--   0        0        0     4820 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v6.json
--rw-r--r--   0        0        0     5568 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v1.json
--rw-r--r--   0        0        0     6790 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v2.json
--rw-r--r--   0        0        0     7249 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v3.json
--rw-r--r--   0        0        0     1017 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/utils.py
--rw-r--r--   0        0        0     1828 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      830 2024-05-21 09:33:13.000000 dbt_artifacts_parser-0.6.0/setup.py
--rw-r--r--   0        0        0    12383 1970-01-01 00:00:00.000000 dbt_artifacts_parser-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/LICENSE
+-rw-r--r--   0        0        0    11811 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/README.md
+-rw-r--r--   0        0        0      859 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/__init__.py
+-rw-r--r--   0        0        0    14510 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parser.py
+-rw-r--r--   0        0        0      796 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/base.py
+-rw-r--r--   0        0        0      796 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/catalog/__init__.py
+-rw-r--r--   0        0        0     1814 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
+-rw-r--r--   0        0        0      796 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/__init__.py
+-rw-r--r--   0        0        0    44817 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
+-rw-r--r--   0        0        0    49003 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v10.py
+-rw-r--r--   0        0        0    43278 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v11.py
+-rw-r--r--   0        0        0   117364 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v12.py
+-rw-r--r--   0        0        0    45698 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
+-rw-r--r--   0        0        0    46324 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
+-rw-r--r--   0        0        0    52225 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
+-rw-r--r--   0        0        0    52797 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
+-rw-r--r--   0        0        0    54267 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
+-rw-r--r--   0        0        0    58602 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
+-rw-r--r--   0        0        0    38032 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
+-rw-r--r--   0        0        0    43066 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
+-rw-r--r--   0        0        0      796 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/__init__.py
+-rw-r--r--   0        0        0     1691 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
+-rw-r--r--   0        0        0     1717 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
+-rw-r--r--   0        0        0     3324 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
+-rw-r--r--   0        0        0     3408 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
+-rw-r--r--   0        0        0     1951 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v5.py
+-rw-r--r--   0        0        0     1797 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v6.py
+-rw-r--r--   0        0        0      796 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/sources/__init__.py
+-rw-r--r--   0        0        0     2021 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/sources/sources_v1.py
+-rw-r--r--   0        0        0     2306 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/sources/sources_v2.py
+-rw-r--r--   0        0        0     2392 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/sources/sources_v3.py
+-rw-r--r--   0        0        0     2348 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/utils.py
+-rw-r--r--   0        0        0     5202 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/version_map.py
+-rw-r--r--   0        0        0     5968 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json
+-rw-r--r--   0        0        0   129577 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json
+-rw-r--r--   0        0        0   148279 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v10.json
+-rw-r--r--   0        0        0   130575 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v11.json
+-rw-r--r--   0        0        0   724056 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v12.json
+-rw-r--r--   0        0        0   135379 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json
+-rw-r--r--   0        0        0   138302 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json
+-rw-r--r--   0        0        0   157235 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json
+-rw-r--r--   0        0        0   159203 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json
+-rw-r--r--   0        0        0   163791 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json
+-rw-r--r--   0        0        0   174833 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json
+-rw-r--r--   0        0        0   115570 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json
+-rw-r--r--   0        0        0   129190 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json
+-rw-r--r--   0        0        0     4622 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json
+-rw-r--r--   0        0        0     4777 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json
+-rw-r--r--   0        0        0     9817 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json
+-rw-r--r--   0        0        0    10272 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json
+-rw-r--r--   0        0        0     4690 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v5.json
+-rw-r--r--   0        0        0     4820 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v6.json
+-rw-r--r--   0        0        0     5568 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/sources/sources_v1.json
+-rw-r--r--   0        0        0     6790 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/sources/sources_v2.json
+-rw-r--r--   0        0        0     7249 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/sources/sources_v3.json
+-rw-r--r--   0        0        0     1017 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/utils.py
+-rw-r--r--   0        0        0     1824 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2024-05-22 00:39:33.000000 dbt_artifacts_parser-0.7.0/setup.py
+-rw-r--r--   0        0        0    13667 1970-01-01 00:00:00.000000 dbt_artifacts_parser-0.7.0/PKG-INFO
```

### Comparing `dbt_artifacts_parser-0.6.0/LICENSE` & `dbt_artifacts_parser-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/README.md` & `dbt_artifacts_parser-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,33 @@
 <a href="https://pypi.org/project/dbt-artifacts-parser" target="_blank">
 <img src="https://img.shields.io/pypi/v/dbt-artifacts-parser?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/dbt-artifacts-parser" target="_blank">
 <img src="https://img.shields.io/pypi/pyversions/dbt-artifacts-parser.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 
-
 # dbt-artifacts-parser
+
 This is a dbt artifacts parse in python.
 It enables us to deal with `catalog.json`, `manifest.json`, `run-results.json` and `sources.json` as python objects.
 
+## Supported Versions and Compatibility
+
+> **⚠️ Important Note:**
+>
+> - **Pydantic v1 will not be supported for dbt 1.9 or later.**
+> - **To parse dbt 1.9 or later, please migrate your code to pydantic v2.**
+> - **We will reassess version compatibility upon the release of pydantic v3.**
+
+| Version | Supported dbt Version | Supported pydantic Version |
+|---------|-----------------------|----------------------------|
+|  0.7    | dbt 1.5 to 1.8        | pydantic v2                |
+|  0.6    | dbt 1.5 to 1.8        | pydantic v1                |
+|  0.5    | dbt 1.5 to 1.7        | pydantic v1                |
+
 ## Installation
 
 ```bash
 pip install -U dbt-artifacts-parser
 ```
 
 ## Python classes
@@ -31,21 +45,23 @@
 - [ManifestV5](dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for manifest.json v5
 - [ManifestV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for manifest.json v6
 - [ManifestV7](dbt_artifacts_parser/parsers/manifest/manifest_v7.py) for manifest.json v7
 - [ManifestV8](dbt_artifacts_parser/parsers/manifest/manifest_v8.py) for manifest.json v8
 - [ManifestV9](dbt_artifacts_parser/parsers/manifest/manifest_v9.py) for manifest.json v9
 - [ManifestV10](dbt_artifacts_parser/parsers/manifest/manifest_v10.py) for manifest.json v10
 - [ManifestV11](dbt_artifacts_parser/parsers/manifest/manifest_v11.py) for manifest.json v11
+- [ManifestV12](dbt_artifacts_parser/parsers/manifest/manifest_v12.py) for manifest.json v12
 
 ### Run Results
 - [RunResultsV1](dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for run_results.json v1
 - [RunResultsV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for run_results.json v2
 - [RunResultsV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for run_results.json v3
 - [RunResultsV4](dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for run_results.json v4
 - [RunResultsV5](dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for run_results.json v5
+- [RunResultsV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for run_results.json v6
 
 ### Sources
 - [SourcesV1](dbt_artifacts_parser/parsers/sources/sources_v1.py) for sources.json v1
 - [SourcesV2](dbt_artifacts_parser/parsers/sources/sources_v2.py) for sources.json v2
 - [SourcesV3](dbt_artifacts_parser/parsers/sources/sources_v3.py) for sources.json v3
 
 ## Examples
@@ -153,14 +169,21 @@
 
 # parse manifest.json v11
 from dbt_artifacts_parser.parser import parse_manifest_v11
 
 with open("path/to/manifest.json", "r") as fp:
     manifest_dict = json.load(fp)
     manifest_obj = parse_manifest_v11(manifest=manifest_dict)
+
+# parse manifest.json v12
+from dbt_artifacts_parser.parser import parse_manifest_v12
+
+with open("path/to/manifest.json", "r") as fp:
+    manifest_dict = json.load(fp)
+    manifest_obj = parse_manifest_v12(manifest=manifest_dict)
 ```
 
 ### Parse run-results.json
 
 ```python
 import json
 
@@ -201,14 +224,21 @@
 
 # parse run-results.json v5
 from dbt_artifacts_parser.parser import parse_run_results_v5
 
 with open("path/to/run-results.json", "r") as fp:
     run_results_dict = json.load(fp)
     run_results_obj = parse_run_results_v5(run_results=run_results_dict)
+
+# parse run-results.json v6
+from dbt_artifacts_parser.parser import parse_run_results_v6
+
+with open("path/to/run-results.json", "r") as fp:
+    run_results_dict = json.load(fp)
+    run_results_obj = parse_run_results_v6(run_results=run_results_dict)
 ```
 
 ### Parse sources.json
 
 ```python
 import json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,13 +1,20 @@
 [![Test python](https://github.com/yu-iskw/dbt-artifacts-parser/actions/
 workflows/test.yml/badge.svg)](https://github.com/yu-iskw/dbt-artifacts-parser/
 actions/workflows/test.yml) _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]# dbt-
 artifacts-parser This is a dbt artifacts parse in python. It enables us to deal
 with `catalog.json`, `manifest.json`, `run-results.json` and `sources.json` as
-python objects. ## Installation ```bash pip install -U dbt-artifacts-parser ```
+python objects. ## Supported Versions and Compatibility > **â ï¸ Important
+Note:** > > - **Pydantic v1 will not be supported for dbt 1.9 or later.** > -
+**To parse dbt 1.9 or later, please migrate your code to pydantic v2.** > -
+**We will reassess version compatibility upon the release of pydantic v3.** |
+Version | Supported dbt Version | Supported pydantic Version | |---------|-----
+------------------|----------------------------| | 0.7 | dbt 1.5 to 1.8 |
+pydantic v2 | | 0.6 | dbt 1.5 to 1.8 | pydantic v1 | | 0.5 | dbt 1.5 to 1.7 |
+pydantic v1 | ## Installation ```bash pip install -U dbt-artifacts-parser ```
 ## Python classes Those are the classes to parse dbt artifacts. ### Catalog -
 [CatalogV1](dbt_artifacts_parser/parsers/catalog/catalog_v1.py) for
 catalog.json v1 ### Manifest - [ManifestV1](dbt_artifacts_parser/parsers/
 manifest/manifest_v1.py) for manifest.json v1 - [ManifestV2]
 (dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for manifest.json v2 -
 [ManifestV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for
 manifest.json v3 - [ManifestV4](dbt_artifacts_parser/parsers/manifest/
@@ -16,28 +23,30 @@
 (dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for manifest.json v6 -
 [ManifestV7](dbt_artifacts_parser/parsers/manifest/manifest_v7.py) for
 manifest.json v7 - [ManifestV8](dbt_artifacts_parser/parsers/manifest/
 manifest_v8.py) for manifest.json v8 - [ManifestV9](dbt_artifacts_parser/
 parsers/manifest/manifest_v9.py) for manifest.json v9 - [ManifestV10]
 (dbt_artifacts_parser/parsers/manifest/manifest_v10.py) for manifest.json v10 -
 [ManifestV11](dbt_artifacts_parser/parsers/manifest/manifest_v11.py) for
-manifest.json v11 ### Run Results - [RunResultsV1](dbt_artifacts_parser/
-parsers/manifest/manifest_v1.py) for run_results.json v1 - [RunResultsV2]
-(dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for run_results.json v2
-- [RunResultsV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for
-run_results.json v3 - [RunResultsV4](dbt_artifacts_parser/parsers/manifest/
-manifest_v4.py) for run_results.json v4 - [RunResultsV5](dbt_artifacts_parser/
-parsers/manifest/manifest_v5.py) for run_results.json v5 ### Sources -
-[SourcesV1](dbt_artifacts_parser/parsers/sources/sources_v1.py) for
-sources.json v1 - [SourcesV2](dbt_artifacts_parser/parsers/sources/
-sources_v2.py) for sources.json v2 - [SourcesV3](dbt_artifacts_parser/parsers/
-sources/sources_v3.py) for sources.json v3 ## Examples ### Parse catalog.json
-```python import json # parse any version of catalog.json from
-dbt_artifacts_parser.parser import parse_catalog with open("path/to/
-catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
+manifest.json v11 - [ManifestV12](dbt_artifacts_parser/parsers/manifest/
+manifest_v12.py) for manifest.json v12 ### Run Results - [RunResultsV1]
+(dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for run_results.json v1
+- [RunResultsV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for
+run_results.json v2 - [RunResultsV3](dbt_artifacts_parser/parsers/manifest/
+manifest_v3.py) for run_results.json v3 - [RunResultsV4](dbt_artifacts_parser/
+parsers/manifest/manifest_v4.py) for run_results.json v4 - [RunResultsV5]
+(dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for run_results.json v5
+- [RunResultsV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for
+run_results.json v6 ### Sources - [SourcesV1](dbt_artifacts_parser/parsers/
+sources/sources_v1.py) for sources.json v1 - [SourcesV2](dbt_artifacts_parser/
+parsers/sources/sources_v2.py) for sources.json v2 - [SourcesV3]
+(dbt_artifacts_parser/parsers/sources/sources_v3.py) for sources.json v3 ##
+Examples ### Parse catalog.json ```python import json # parse any version of
+catalog.json from dbt_artifacts_parser.parser import parse_catalog with open
+("path/to/catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog(catalog=catalog_dict) # parse catalog.json v1 from
 dbt_artifacts_parser.parser import parse_catalog_v1 with open("path/to/
 catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog_v1(catalog=catalog_dict) ``` ### Parse manifest.json ```python
 import json # parse any version of manifest.json from
 dbt_artifacts_parser.parser import parse_manifest with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
@@ -70,15 +79,18 @@
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
 parse_manifest_v9(manifest=manifest_dict) # parse manifest.json v10 from
 dbt_artifacts_parser.parser import parse_manifest_v10 with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
 parse_manifest_v10(manifest=manifest_dict) # parse manifest.json v11 from
 dbt_artifacts_parser.parser import parse_manifest_v11 with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
-parse_manifest_v11(manifest=manifest_dict) ``` ### Parse run-results.json
+parse_manifest_v11(manifest=manifest_dict) # parse manifest.json v12 from
+dbt_artifacts_parser.parser import parse_manifest_v12 with open("path/to/
+manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
+parse_manifest_v12(manifest=manifest_dict) ``` ### Parse run-results.json
 ```python import json # parse any version of run-results.json from
 dbt_artifacts_parser.parser import parse_run_results with open("path/to/run-
 resultsjson", "r") as fp: run_results_dict = json.load(fp) run_results_obj =
 parse_run_results(run_results=run_results_dict) # parse run-results.json v1
 from dbt_artifacts_parser.parser import parse_run_results_v1 with open("path/
 to/run-results.json", "r") as fp: run_results_dict = json.load(fp)
 run_results_obj = parse_run_results_v1(run_results=run_results_dict) # parse
@@ -91,22 +103,26 @@
 parse_run_results_v3(run_results=run_results_dict) # parse run-results.json v4
 from dbt_artifacts_parser.parser import parse_run_results_v4 with open("path/
 to/run-results.json", "r") as fp: run_results_dict = json.load(fp)
 run_results_obj = parse_run_results_v4(run_results=run_results_dict) # parse
 run-results.json v5 from dbt_artifacts_parser.parser import
 parse_run_results_v5 with open("path/to/run-results.json", "r") as fp:
 run_results_dict = json.load(fp) run_results_obj = parse_run_results_v5
-(run_results=run_results_dict) ``` ### Parse sources.json ```python import json
-# parse any version of sources.json from dbt_artifacts_parser.parser import
-parse_sources with open("path/to/sources.json", "r") as fp: sources_dict =
-json.load(fp) sources_obj = parse_sources(sources=sources_dict) # parse
-sources.json v1 from dbt_artifacts_parser.parser import parse_sources_v1 with
-open("path/to/sources.json", "r") as fp: sources_dict = json.load(fp)
-sources_obj = parse_sources_v1(sources=sources_dict) # parse sources.json v2
-from dbt_artifacts_parser.parser import parse_sources_v2 with open("path/to/
+(run_results=run_results_dict) # parse run-results.json v6 from
+dbt_artifacts_parser.parser import parse_run_results_v6 with open("path/to/run-
+results.json", "r") as fp: run_results_dict = json.load(fp) run_results_obj =
+parse_run_results_v6(run_results=run_results_dict) ``` ### Parse sources.json
+```python import json # parse any version of sources.json from
+dbt_artifacts_parser.parser import parse_sources with open("path/to/
+sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
+parse_sources(sources=sources_dict) # parse sources.json v1 from
+dbt_artifacts_parser.parser import parse_sources_v1 with open("path/to/
+sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
+parse_sources_v1(sources=sources_dict) # parse sources.json v2 from
+dbt_artifacts_parser.parser import parse_sources_v2 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v2(sources=sources_dict) # parse sources.json v3 from
 dbt_artifacts_parser.parser import parse_sources_v3 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v3(sources=sources_dict) ``` ## Contributors
   _[_y_u_-_i_s_k_w_]   _[_d_l_a_w_i_n_]  _[_b_b_r_e_w_i_n_g_t_o_n_]   _[_j_u_d_a_h_r_a_n_d_]   _[_n_a_b_i_l_m_]     _[_O_n_k_a_r_V_O_7_]
  _YY_uu_ _II_ss_hh_ii_kk_aa_ww_aa    _NN_uu_ll_ll   _BB_rr_ee_nn_tt_ _BB_rr_ee_ww_ii_nn_gg_tt_oo_nn _JJ_uu_dd_aa_hh_ _RR_aa_nn_dd  _MM_oo_hh_aa_mm_ee_dd_ _NN_aa_bb_ii_ll _OO_nn_kk_aa_rr_ _RR_aa_vv_gg_aa_nn
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/__init__.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 """
 A dbt artifacts parser in python
 """
-__version__ = "0.6.0"
+__version__ = "0.7.0"
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parser.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,19 @@
 ]:
     """Parse manifest.json
 
     Args:
         manifest: A dict of manifest.json
 
     Returns:
-       Union[ManifestV1, ManifestV2, ManifestV3, ManifestV4]
+       Union[
+           ManifestV1, ManifestV2, ManifestV3, ManifestV4, ManifestV5,
+           ManifestV6, ManifestV7, ManifestV8, ManifestV9, ManifestV10,
+           ManifestV11, ManifestV12,
+        ]
     """
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V1.value.dbt_schema_version:
         return ManifestV1(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V2.value.dbt_schema_version:
         return ManifestV2(**manifest)
     elif dbt_schema_version == ArtifactTypes.MANIFEST_V3.value.dbt_schema_version:
@@ -167,46 +171,46 @@
     """Parse manifest.json ver.6"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V6.value.dbt_schema_version:
         return ManifestV6(**manifest)
     raise ValueError("Not a manifest.json v6")
 
 
-def parse_manifest_v7(manifest: dict) -> ManifestV6:
+def parse_manifest_v7(manifest: dict) -> ManifestV7:
     """Parse manifest.json ver.7"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V7.value.dbt_schema_version:
         return ManifestV7(**manifest)
     raise ValueError("Not a manifest.json v7")
 
 
-def parse_manifest_v8(manifest: dict) -> ManifestV6:
+def parse_manifest_v8(manifest: dict) -> ManifestV8:
     """Parse manifest.json ver.8"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V8.value.dbt_schema_version:
         return ManifestV8(**manifest)
     raise ValueError("Not a manifest.json v8")
 
 
-def parse_manifest_v9(manifest: dict) -> ManifestV6:
+def parse_manifest_v9(manifest: dict) -> ManifestV9:
     """Parse manifest.json ver.9"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V9.value.dbt_schema_version:
         return ManifestV9(**manifest)
     raise ValueError("Not a manifest.json v9")
 
-def parse_manifest_v10(manifest: dict) -> ManifestV6:
+def parse_manifest_v10(manifest: dict) -> ManifestV10:
     """Parse manifest.json ver.10"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V10.value.dbt_schema_version:
         return ManifestV10(**manifest)
     raise ValueError("Not a manifest.json v10")
 
 
-def parse_manifest_v11(manifest: dict) -> ManifestV6:
+def parse_manifest_v11(manifest: dict) -> ManifestV11:
     """Parse manifest.json ver.11"""
     dbt_schema_version = get_dbt_schema_version(artifact_json=manifest)
     if dbt_schema_version == ArtifactTypes.MANIFEST_V11.value.dbt_schema_version:
         return ManifestV11(**manifest)
     raise ValueError("Not a manifest.json v11")
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/__init__.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/base.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/catalog/__init__.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/catalog/catalog_v1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,74 @@
 # generated by datamodel-codegen:
 #   filename:  catalog_v1.json
-#   timestamp: 2022-03-01T06:21:30+00:00
 
 from __future__ import annotations
 
-from datetime import datetime
 from typing import Dict, List, Optional, Union
 
-from pydantic import Extra, Field
+from pydantic import AwareDatetime, ConfigDict, Field
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class CatalogMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    dbt_schema_version: Optional[
-        str] = 'https://schemas.getdbt.com/dbt/catalog/v1.json'
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: Optional[str] = 'https://schemas.getdbt.com/dbt/catalog/v1.json'
     dbt_version: Optional[str] = '0.19.0'
-    generated_at: Optional[datetime] = '2021-02-10T04:42:33.680487Z'
-    invocation_id: Optional[Optional[str]] = None
+    generated_at: Optional[AwareDatetime] = '2021-02-10T04:42:33.680487Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class TableMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     type: str
-    database: Optional[Optional[str]] = None
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
-    comment: Optional[Optional[str]] = None
-    owner: Optional[Optional[str]] = None
+    comment: Optional[str] = None
+    owner: Optional[str] = None
 
 
 class ColumnMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     type: str
-    comment: Optional[Optional[str]] = None
+    comment: Optional[str] = None
     index: int
     name: str
 
 
 class StatsItem(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     id: str
     label: str
-    value: Optional[Optional[Union[bool, str, float]]] = None
-    description: Optional[Optional[str]] = None
+    value: Optional[Union[bool, str, float]] = None
+    description: Optional[str] = None
     include: bool
 
 
 class CatalogTable(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: TableMetadata
     columns: Dict[str, ColumnMetadata]
     stats: Dict[str, StatsItem]
-    unique_id: Optional[Optional[str]] = None
+    unique_id: Optional[str] = None
 
 
 class CatalogV1(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: CatalogMetadata
     nodes: Dict[str, CatalogTable]
     sources: Dict[str, CatalogTable]
-    errors: Optional[Optional[List[str]]] = None
+    errors: Optional[List[str]] = None
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/__init__.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v1.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v11.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1439 +1,1454 @@
 # generated by datamodel-codegen:
-#   filename:  manifest_v1.json
-#   timestamp: 2022-03-01T06:21:31+00:00
+#   filename:  manifest_v11.json
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, Union
+from uuid import UUID
 
-# pylint: disable=no-name-in-module
-from pydantic import Extra, Field, constr
+from pydantic import ConfigDict, Field, constr
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class ManifestMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    dbt_schema_version: Optional[
-        str] = 'https://schemas.getdbt.com/dbt/manifest/v1.json'
-    dbt_version: Optional[str] = '0.19.0'
-    generated_at: Optional[datetime] = '2021-02-10T04:42:33.683996Z'
-    invocation_id: Optional[Optional[str]] = None
-    env: Optional[Dict[str, str]] = {}
-    project_id: Optional[Optional[str]] = Field(
-        None, description='A unique identifier for the project')
-    user_id: Optional[Optional[constr(
-        regex=r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
-    )]] = Field(None, description='A unique identifier for the user')
-    send_anonymous_usage_stats: Optional[Optional[bool]] = Field(
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: Optional[str] = None
+    dbt_version: Optional[str] = '1.8.0a1'
+    generated_at: Optional[str] = None
+    invocation_id: Optional[str] = None
+    env: Optional[Dict[str, str]] = None
+    project_name: Optional[str] = Field(None, description='Name of the root project')
+    project_id: Optional[str] = Field(
         None,
-        description=
-        'Whether dbt is configured to send anonymous usage statistics')
-    adapter_type: Optional[Optional[str]] = Field(
-        None, description='The type name of the adapter')
-
-
-class ResourceType(Enum):
-    analysis = 'analysis'
+        description='A unique identifier for the project, hashed from the project name',
+    )
+    user_id: Optional[UUID] = Field(
+        None, description='A unique identifier for the user'
+    )
+    send_anonymous_usage_stats: Optional[bool] = Field(
+        None, description='Whether dbt is configured to send anonymous usage statistics'
+    )
+    adapter_type: Optional[str] = Field(
+        None, description='The type name of the adapter'
+    )
 
 
 class FileHash(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     checksum: str
 
 
 class Hook(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     sql: str
     transaction: Optional[bool] = True
-    index: Optional[Optional[int]] = None
-
-
-class DependsOn(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    macros: Optional[List[str]] = []
-    nodes: Optional[List[str]] = []
-
-
-class ColumnInfo(BaseParserModel):
-
-    class Config:
-        extra = Extra.allow
-
-    name: str
-    description: Optional[str] = ''
-    meta: Optional[Dict[str, Any]] = {}
-    data_type: Optional[Optional[str]] = None
-    quote: Optional[Optional[bool]] = None
-    tags: Optional[List[str]] = []
+    index: Optional[int] = None
 
 
 class Docs(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     show: Optional[bool] = True
+    node_color: Optional[str] = None
 
 
-class InjectedCTE(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    id: str
-    sql: str
-
+class ContractConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    enforced: Optional[bool] = False
+    alias_types: Optional[bool] = True
 
-class ResourceType1(Enum):
-    test = 'test'
 
+class OnConfigurationChange(Enum):
+    apply = 'apply'
+    continue_ = 'continue'
+    fail = 'fail'
 
-class TestConfig(BaseParserModel):
-
-    class Config:
-        extra = Extra.allow
 
+class NodeConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
     enabled: Optional[bool] = True
-    materialized: Optional[str] = 'test'
-    persist_docs: Optional[Dict[str, Any]] = {}
-    post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
-    pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
-    vars: Optional[Dict[str, Any]] = {}
-    quoting: Optional[Dict[str, Any]] = {}
-    column_types: Optional[Dict[str, Any]] = {}
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
-    tags: Optional[Union[List[str], str]] = []
-    full_refresh: Optional[Optional[bool]] = None
-    severity: Optional[constr(
-        regex=r'^([Ww][Aa][Rr][Nn]|[Ee][Rr][Rr][Oo][Rr])$')] = 'ERROR'
-
-
-class ResourceType2(Enum):
-    model = 'model'
-
-
-class ResourceType3(Enum):
-    operation = 'operation'
-
-
-class ResourceType4(Enum):
-    rpc = 'rpc'
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field(None, alias='schema')
+    database: Optional[str] = None
+    tags: Optional[Union[List[str], str]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    materialized: Optional[str] = 'view'
+    incremental_strategy: Optional[str] = None
+    persist_docs: Optional[Dict[str, Any]] = None
+    post_hook: Optional[List[Hook]] = Field(None, alias='post-hook')
+    pre_hook: Optional[List[Hook]] = Field(None, alias='pre-hook')
+    quoting: Optional[Dict[str, Any]] = None
+    column_types: Optional[Dict[str, Any]] = None
+    full_refresh: Optional[bool] = None
+    unique_key: Optional[Union[str, List[str]]] = None
+    on_schema_change: Optional[str] = 'ignore'
+    on_configuration_change: Optional[OnConfigurationChange] = None
+    grants: Optional[Dict[str, Any]] = None
+    packages: Optional[List[str]] = None
+    docs: Optional[Docs] = None
+    contract: Optional[ContractConfig] = None
 
 
-class ResourceType5(Enum):
-    test = 'test'
+class Type(Enum):
+    check = 'check'
+    not_null = 'not_null'
+    unique = 'unique'
+    primary_key = 'primary_key'
+    foreign_key = 'foreign_key'
+    custom = 'custom'
 
 
-class TestMetadata(BaseParserModel):
+class ColumnLevelConstraint(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    type: Type
+    name: Optional[str] = None
+    expression: Optional[str] = None
+    warn_unenforced: Optional[bool] = True
+    warn_unsupported: Optional[bool] = True
 
-    class Config:
-        extra = Extra.forbid
 
-    namespace: Optional[Optional[str]] = None
+class ColumnInfo(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
     name: str
-    kwargs: Dict[str, Any]
-
-
-class ResourceType6(Enum):
-    seed = 'seed'
-
-
-class SeedConfig(BaseParserModel):
-
-    class Config:
-        extra = Extra.allow
-
-    enabled: Optional[bool] = True
-    materialized: Optional[str] = 'seed'
-    persist_docs: Optional[Dict[str, Any]] = {}
-    post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
-    pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
-    vars: Optional[Dict[str, Any]] = {}
-    quoting: Optional[Dict[str, Any]] = {}
-    column_types: Optional[Dict[str, Any]] = {}
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
-    tags: Optional[Union[List[str], str]] = []
-    full_refresh: Optional[Optional[bool]] = None
-    quote_columns: Optional[Optional[bool]] = None
+    description: Optional[str] = ''
+    meta: Optional[Dict[str, Any]] = None
+    data_type: Optional[str] = None
+    constraints: Optional[List[ColumnLevelConstraint]] = None
+    quote: Optional[bool] = None
+    tags: Optional[List[str]] = None
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
 
 
-class ResourceType7(Enum):
-    snapshot = 'snapshot'
+class RefArgs(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    package: Optional[str] = None
+    version: Optional[Union[str, float]] = None
 
 
-class ResourceType8(Enum):
-    analysis = 'analysis'
+class DependsOn(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    macros: Optional[List[str]] = None
+    nodes: Optional[List[str]] = None
 
 
-class ResourceType9(Enum):
-    test = 'test'
+class InjectedCTE(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    id: str
+    sql: str
 
 
-class ParsedDataTestNode(BaseParserModel):
+class Contract(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    enforced: Optional[bool] = False
+    alias_types: Optional[bool] = True
+    checksum: Optional[str] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    database: Optional[Optional[str]] = None
+class AnalysisNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
+    name: str
+    resource_type: Literal['analysis']
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
-    name: str
-    resource_type: ResourceType9
+    unique_id: str
+    fqn: List[str]
     alias: str
     checksum: FileHash
-    config: Optional[TestConfig] = {
-        'enabled': True,
-        'materialized': 'test',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-        'severity': 'ERROR',
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    config: Optional[NodeConfig] = None
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-
-
-class ResourceType10(Enum):
-    operation = 'operation'
-
-
-class ResourceType11(Enum):
-    model = 'model'
-
-
-class ResourceType12(Enum):
-    rpc = 'rpc'
-
-
-class ResourceType13(Enum):
-    test = 'test'
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    language: Optional[str] = 'sql'
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    compiled_path: Optional[str] = None
+    compiled: Optional[bool] = False
+    compiled_code: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = None
+    field_pre_injected_sql: Optional[str] = Field(None, alias='_pre_injected_sql')
+    contract: Optional[Contract] = None
 
 
-class ParsedSchemaTestNode(BaseParserModel):
+class TestConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
+    enabled: Optional[bool] = True
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field('dbt_test__audit', alias='schema')
+    database: Optional[str] = None
+    tags: Optional[Union[List[str], str]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    materialized: Optional[str] = 'test'
+    severity: Optional[
+        constr(pattern=r'^([Ww][Aa][Rr][Nn]|[Ee][Rr][Rr][Oo][Rr])$')
+    ] = 'ERROR'
+    store_failures: Optional[bool] = None
+    store_failures_as: Optional[str] = None
+    where: Optional[str] = None
+    limit: Optional[int] = None
+    fail_calc: Optional[str] = 'count(*)'
+    warn_if: Optional[str] = '!= 0'
+    error_if: Optional[str] = '!= 0'
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    test_metadata: TestMetadata
-    database: Optional[Optional[str]] = None
+class SingularTestNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
+    name: str
+    resource_type: Literal['test']
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
-    name: str
-    resource_type: ResourceType13
+    unique_id: str
+    fqn: List[str]
     alias: str
     checksum: FileHash
-    config: Optional[TestConfig] = {
-        'enabled': True,
-        'materialized': 'test',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-        'severity': 'ERROR',
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    config: Optional[TestConfig] = None
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    column_name: Optional[Optional[str]] = None
-
-
-class ResourceType14(Enum):
-    seed = 'seed'
-
-
-class ParsedSeedNode(BaseParserModel):
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    language: Optional[str] = 'sql'
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    compiled_path: Optional[str] = None
+    compiled: Optional[bool] = False
+    compiled_code: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = None
+    field_pre_injected_sql: Optional[str] = Field(None, alias='_pre_injected_sql')
+    contract: Optional[Contract] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    database: Optional[Optional[str]] = None
+class HookNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
+    name: str
+    resource_type: Literal['operation']
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
-    name: str
-    resource_type: ResourceType14
+    unique_id: str
+    fqn: List[str]
     alias: str
     checksum: FileHash
-    config: Optional[SeedConfig] = {
-        'enabled': True,
-        'materialized': 'seed',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-        'quote_columns': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    config: Optional[NodeConfig] = None
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-
-
-class ResourceType15(Enum):
-    snapshot = 'snapshot'
-
-
-class Strategy(Enum):
-    timestamp = 'timestamp'
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    language: Optional[str] = 'sql'
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    compiled_path: Optional[str] = None
+    compiled: Optional[bool] = False
+    compiled_code: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = None
+    field_pre_injected_sql: Optional[str] = Field(None, alias='_pre_injected_sql')
+    contract: Optional[Contract] = None
+    index: Optional[int] = None
 
 
-class TimestampSnapshotConfig(BaseParserModel):
+class Access(Enum):
+    private = 'private'
+    protected = 'protected'
+    public = 'public'
 
-    class Config:
-        extra = Extra.allow
 
+class ModelConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
     enabled: Optional[bool] = True
-    materialized: Optional[str] = 'snapshot'
-    persist_docs: Optional[Dict[str, Any]] = {}
-    post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
-    pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
-    vars: Optional[Dict[str, Any]] = {}
-    quoting: Optional[Dict[str, Any]] = {}
-    column_types: Optional[Dict[str, Any]] = {}
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
-    tags: Optional[Union[List[str], str]] = []
-    full_refresh: Optional[Optional[bool]] = None
-    unique_key: str
-    target_schema: str
-    target_database: Optional[Optional[str]] = None
-    strategy: Strategy
-    updated_at: str
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field(None, alias='schema')
+    database: Optional[str] = None
+    tags: Optional[Union[List[str], str]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    materialized: Optional[str] = 'view'
+    incremental_strategy: Optional[str] = None
+    persist_docs: Optional[Dict[str, Any]] = None
+    post_hook: Optional[List[Hook]] = Field(None, alias='post-hook')
+    pre_hook: Optional[List[Hook]] = Field(None, alias='pre-hook')
+    quoting: Optional[Dict[str, Any]] = None
+    column_types: Optional[Dict[str, Any]] = None
+    full_refresh: Optional[bool] = None
+    unique_key: Optional[Union[str, List[str]]] = None
+    on_schema_change: Optional[str] = 'ignore'
+    on_configuration_change: Optional[OnConfigurationChange] = None
+    grants: Optional[Dict[str, Any]] = None
+    packages: Optional[List[str]] = None
+    docs: Optional[Docs] = None
+    contract: Optional[ContractConfig] = None
+    access: Optional[Access] = 'protected'
+
+
+class ModelLevelConstraint(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    type: Type
+    name: Optional[str] = None
+    expression: Optional[str] = None
+    warn_unenforced: Optional[bool] = True
+    warn_unsupported: Optional[bool] = True
+    columns: Optional[List[str]] = None
 
 
-class Strategy1(Enum):
-    check = 'check'
+class DeferRelation(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    alias: str
+    relation_name: Optional[str] = None
 
 
-class CheckCol(Enum):
-    all = 'all'
+class ModelNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    name: str
+    resource_type: Literal['model']
+    package_name: str
+    path: str
+    original_file_path: str
+    unique_id: str
+    fqn: List[str]
+    alias: str
+    checksum: FileHash
+    config: Optional[ModelConfig] = None
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    language: Optional[str] = 'sql'
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    compiled_path: Optional[str] = None
+    compiled: Optional[bool] = False
+    compiled_code: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = None
+    field_pre_injected_sql: Optional[str] = Field(None, alias='_pre_injected_sql')
+    contract: Optional[Contract] = None
+    access: Optional[Access] = 'protected'
+    constraints: Optional[List[ModelLevelConstraint]] = None
+    version: Optional[Union[str, float]] = None
+    latest_version: Optional[Union[str, float]] = None
+    deprecation_date: Optional[str] = None
+    defer_relation: Optional[DeferRelation] = None
 
 
-class CheckSnapshotConfig(BaseParserModel):
+class RPCNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    name: str
+    resource_type: Literal['rpc']
+    package_name: str
+    path: str
+    original_file_path: str
+    unique_id: str
+    fqn: List[str]
+    alias: str
+    checksum: FileHash
+    config: Optional[NodeConfig] = None
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    language: Optional[str] = 'sql'
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    compiled_path: Optional[str] = None
+    compiled: Optional[bool] = False
+    compiled_code: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = None
+    field_pre_injected_sql: Optional[str] = Field(None, alias='_pre_injected_sql')
+    contract: Optional[Contract] = None
 
-    class Config:
-        extra = Extra.allow
 
-    enabled: Optional[bool] = True
-    materialized: Optional[str] = 'snapshot'
-    persist_docs: Optional[Dict[str, Any]] = {}
-    post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
-    pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
-    vars: Optional[Dict[str, Any]] = {}
-    quoting: Optional[Dict[str, Any]] = {}
-    column_types: Optional[Dict[str, Any]] = {}
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
-    tags: Optional[Union[List[str], str]] = []
-    full_refresh: Optional[Optional[bool]] = None
-    unique_key: str
-    target_schema: str
-    target_database: Optional[Optional[str]] = None
-    strategy: Strategy1
-    check_cols: Union[CheckCol, List[str]]
+class SqlNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    name: str
+    resource_type: Literal['sql_operation']
+    package_name: str
+    path: str
+    original_file_path: str
+    unique_id: str
+    fqn: List[str]
+    alias: str
+    checksum: FileHash
+    config: Optional[NodeConfig] = None
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    language: Optional[str] = 'sql'
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    compiled_path: Optional[str] = None
+    compiled: Optional[bool] = False
+    compiled_code: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = None
+    field_pre_injected_sql: Optional[str] = Field(None, alias='_pre_injected_sql')
+    contract: Optional[Contract] = None
 
 
-class Strategy2(BaseParserModel):
-    pass
+class TestMetadata(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    kwargs: Optional[Dict[str, Any]] = None
+    namespace: Optional[str] = None
 
 
-class GenericSnapshotConfig(BaseParserModel):
+class GenericTestNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    test_metadata: TestMetadata
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    name: str
+    resource_type: Literal['test']
+    package_name: str
+    path: str
+    original_file_path: str
+    unique_id: str
+    fqn: List[str]
+    alias: str
+    checksum: FileHash
+    config: Optional[TestConfig] = None
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    language: Optional[str] = 'sql'
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    compiled_path: Optional[str] = None
+    compiled: Optional[bool] = False
+    compiled_code: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = None
+    field_pre_injected_sql: Optional[str] = Field(None, alias='_pre_injected_sql')
+    contract: Optional[Contract] = None
+    column_name: Optional[str] = None
+    file_key_name: Optional[str] = None
+    attached_node: Optional[str] = None
 
-    class Config:
-        extra = Extra.allow
 
+class SnapshotConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
     enabled: Optional[bool] = True
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field(None, alias='schema')
+    database: Optional[str] = None
+    tags: Optional[Union[List[str], str]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
     materialized: Optional[str] = 'snapshot'
-    persist_docs: Optional[Dict[str, Any]] = {}
-    post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
-    pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
-    vars: Optional[Dict[str, Any]] = {}
-    quoting: Optional[Dict[str, Any]] = {}
-    column_types: Optional[Dict[str, Any]] = {}
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
-    tags: Optional[Union[List[str], str]] = []
-    full_refresh: Optional[Optional[bool]] = None
-    unique_key: str
-    target_schema: str
-    target_database: Optional[Optional[str]] = None
-    strategy: Strategy2
-
-
-class ResourceType16(Enum):
-    source = 'source'
-
-
-class Quoting(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[Optional[bool]] = None
-    schema_: Optional[Optional[bool]] = Field(None, alias='schema')
-    identifier: Optional[Optional[bool]] = None
-    column: Optional[Optional[bool]] = None
-
-
-class FreshnessMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    dbt_schema_version: Optional[
-        str] = 'https://schemas.getdbt.com/dbt/sources/v1.json'
-    dbt_version: Optional[str] = '0.19.0'
-    generated_at: Optional[datetime] = '2021-02-10T04:42:33.675309Z'
-    invocation_id: Optional[Optional[str]] = None
-    env: Optional[Dict[str, str]] = {}
+    incremental_strategy: Optional[str] = None
+    persist_docs: Optional[Dict[str, Any]] = None
+    post_hook: Optional[List[Hook]] = Field(None, alias='post-hook')
+    pre_hook: Optional[List[Hook]] = Field(None, alias='pre-hook')
+    quoting: Optional[Dict[str, Any]] = None
+    column_types: Optional[Dict[str, Any]] = None
+    full_refresh: Optional[bool] = None
+    unique_key: Optional[str] = None
+    on_schema_change: Optional[str] = 'ignore'
+    on_configuration_change: Optional[OnConfigurationChange] = None
+    grants: Optional[Dict[str, Any]] = None
+    packages: Optional[List[str]] = None
+    docs: Optional[Docs] = None
+    contract: Optional[ContractConfig] = None
+    strategy: Optional[str] = None
+    target_schema: Optional[str] = None
+    target_database: Optional[str] = None
+    updated_at: Optional[str] = None
+    check_cols: Optional[Union[str, List[str]]] = None
+
+
+class SnapshotNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    name: str
+    resource_type: Literal['snapshot']
+    package_name: str
+    path: str
+    original_file_path: str
+    unique_id: str
+    fqn: List[str]
+    alias: str
+    checksum: FileHash
+    config: SnapshotConfig
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    language: Optional[str] = 'sql'
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    compiled_path: Optional[str] = None
+    compiled: Optional[bool] = False
+    compiled_code: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = None
+    field_pre_injected_sql: Optional[str] = Field(None, alias='_pre_injected_sql')
+    contract: Optional[Contract] = None
+    defer_relation: Optional[DeferRelation] = None
 
 
-class Status(Enum):
-    runtime_error = 'runtime error'
+class SeedConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
+    enabled: Optional[bool] = True
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field(None, alias='schema')
+    database: Optional[str] = None
+    tags: Optional[Union[List[str], str]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    materialized: Optional[str] = 'seed'
+    incremental_strategy: Optional[str] = None
+    persist_docs: Optional[Dict[str, Any]] = None
+    post_hook: Optional[List[Hook]] = Field(None, alias='post-hook')
+    pre_hook: Optional[List[Hook]] = Field(None, alias='pre-hook')
+    quoting: Optional[Dict[str, Any]] = None
+    column_types: Optional[Dict[str, Any]] = None
+    full_refresh: Optional[bool] = None
+    unique_key: Optional[Union[str, List[str]]] = None
+    on_schema_change: Optional[str] = 'ignore'
+    on_configuration_change: Optional[OnConfigurationChange] = None
+    grants: Optional[Dict[str, Any]] = None
+    packages: Optional[List[str]] = None
+    docs: Optional[Docs] = None
+    contract: Optional[ContractConfig] = None
+    delimiter: Optional[str] = ','
+    quote_columns: Optional[bool] = None
 
 
-class SourceFreshnessRuntimeError(BaseParserModel):
+class MacroDependsOn(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    macros: Optional[List[str]] = None
 
-    class Config:
-        extra = Extra.forbid
 
+class SeedNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    name: str
+    resource_type: Literal['seed']
+    package_name: str
+    path: str
+    original_file_path: str
     unique_id: str
-    error: Optional[Optional[Union[str, int]]] = None
-    status: Status
+    fqn: List[str]
+    alias: str
+    checksum: FileHash
+    config: Optional[SeedConfig] = None
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    tags: Optional[List[str]] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = None
+    created_at: Optional[float] = None
+    config_call_dict: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    raw_code: Optional[str] = ''
+    root_path: Optional[str] = None
+    depends_on: Optional[MacroDependsOn] = None
+    defer_relation: Optional[DeferRelation] = None
 
 
-class Status1(Enum):
-    pass_ = 'pass'
-    warn = 'warn'
-    error = 'error'
-    runtime_error = 'runtime error'
+class Quoting(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[bool] = None
+    schema_: Optional[bool] = Field(None, alias='schema')
+    identifier: Optional[bool] = None
+    column: Optional[bool] = None
 
 
 class Period(Enum):
     minute = 'minute'
     hour = 'hour'
     day = 'day'
 
 
 class Time(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    count: Optional[int] = None
+    period: Optional[Period] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    count: int
-    period: Period
+class FreshnessThreshold(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    warn_after: Optional[Time] = None
+    error_after: Optional[Time] = None
+    filter: Optional[str] = None
 
 
 class ExternalPartition(BaseParserModel):
-
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
     name: Optional[str] = ''
     description: Optional[str] = ''
     data_type: Optional[str] = ''
-    meta: Optional[Dict[str, Any]] = {}
+    meta: Optional[Dict[str, Any]] = None
 
 
-class SourceConfig(BaseParserModel):
+class ExternalTable(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
+    location: Optional[str] = None
+    file_format: Optional[str] = None
+    row_format: Optional[str] = None
+    tbl_properties: Optional[str] = None
+    partitions: Optional[Union[List[str], List[ExternalPartition]]] = None
 
-    class Config:
-        extra = Extra.allow
 
+class SourceConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
     enabled: Optional[bool] = True
 
 
-class ResourceType17(Enum):
-    macro = 'macro'
-
-
-class MacroDependsOn(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    macros: Optional[List[str]] = []
+class SourceDefinition(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    name: str
+    resource_type: Literal['source']
+    package_name: str
+    path: str
+    original_file_path: str
+    unique_id: str
+    fqn: List[str]
+    source_name: str
+    source_description: str
+    loader: str
+    identifier: str
+    field_event_status: Optional[Dict[str, Any]] = Field(None, alias='_event_status')
+    quoting: Optional[Quoting] = None
+    loaded_at_field: Optional[str] = None
+    freshness: Optional[FreshnessThreshold] = None
+    external: Optional[ExternalTable] = None
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = None
+    meta: Optional[Dict[str, Any]] = None
+    source_meta: Optional[Dict[str, Any]] = None
+    tags: Optional[List[str]] = None
+    config: Optional[SourceConfig] = None
+    patch_path: Optional[str] = None
+    unrendered_config: Optional[Dict[str, Any]] = None
+    relation_name: Optional[str] = None
+    created_at: Optional[float] = None
 
 
 class MacroArgument(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    type: Optional[Optional[str]] = None
+    type: Optional[str] = None
     description: Optional[str] = ''
 
 
-class ParsedDocumentation(BaseParserModel):
+class SupportedLanguage(Enum):
+    python = 'python'
+    sql = 'sql'
 
-    class Config:
-        extra = Extra.forbid
 
-    unique_id: str
+class Macro(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    resource_type: Literal['macro']
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
+    unique_id: str
+    macro_sql: str
+    depends_on: Optional[MacroDependsOn] = None
+    description: Optional[str] = ''
+    meta: Optional[Dict[str, Any]] = None
+    docs: Optional[Docs] = None
+    patch_path: Optional[str] = None
+    arguments: Optional[List[MacroArgument]] = None
+    created_at: Optional[float] = None
+    supported_languages: Optional[List[SupportedLanguage]] = None
+
+
+class Documentation(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
+    resource_type: Literal['doc']
+    package_name: str
+    path: str
+    original_file_path: str
+    unique_id: str
     block_contents: str
 
 
-class Type(Enum):
+class Owner(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
+    email: Optional[str] = None
+    name: Optional[str] = None
+
+
+class ExposureConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
+    enabled: Optional[bool] = True
+
+
+class Type2(Enum):
     dashboard = 'dashboard'
     notebook = 'notebook'
     analysis = 'analysis'
     ml = 'ml'
     application = 'application'
 
 
-class ResourceType18(Enum):
-    model = 'model'
-    analysis = 'analysis'
-    test = 'test'
-    snapshot = 'snapshot'
-    operation = 'operation'
-    seed = 'seed'
-    rpc = 'rpc'
-    docs = 'docs'
-    source = 'source'
-    macro = 'macro'
-    exposure = 'exposure'
-
-
-class MaturityEnum(Enum):
+class Maturity(Enum):
     low = 'low'
     medium = 'medium'
     high = 'high'
 
 
-class ExposureOwner(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    email: str
-    name: Optional[Optional[str]] = None
-
-
-class NodeConfig(BaseParserModel):
-
-    class Config:
-        extra = Extra.allow
-
-    enabled: Optional[bool] = True
-    materialized: Optional[str] = 'view'
-    persist_docs: Optional[Dict[str, Any]] = {}
-    post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
-    pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
-    vars: Optional[Dict[str, Any]] = {}
-    quoting: Optional[Dict[str, Any]] = {}
-    column_types: Optional[Dict[str, Any]] = {}
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
-    tags: Optional[Union[List[str], str]] = []
-    full_refresh: Optional[Optional[bool]] = None
-
-
-class CompiledDataTestNode(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    raw_sql: str
-    compiled: bool
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
+class Exposure(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    resource_type: Literal['exposure']
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
-    name: str
-    resource_type: ResourceType1
-    alias: str
-    checksum: FileHash
-    config: Optional[TestConfig] = {
-        'enabled': True,
-        'materialized': 'test',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-        'severity': 'ERROR',
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
+    unique_id: str
+    fqn: List[str]
+    type: Type2
+    owner: Owner
     description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    compiled_sql: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    relation_name: Optional[Optional[str]] = None
+    label: Optional[str] = None
+    maturity: Optional[Maturity] = None
+    meta: Optional[Dict[str, Any]] = None
+    tags: Optional[List[str]] = None
+    config: Optional[ExposureConfig] = None
+    unrendered_config: Optional[Dict[str, Any]] = None
+    url: Optional[str] = None
+    depends_on: Optional[DependsOn] = None
+    refs: Optional[List[RefArgs]] = None
+    sources: Optional[List[List[str]]] = None
+    metrics: Optional[List[List[str]]] = None
+    created_at: Optional[float] = None
+
+
+class WhereFilter(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    where_sql_template: str
 
 
-class CompiledModelNode(BaseParserModel):
+class WhereFilterIntersection(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    where_filters: List[WhereFilter]
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    compiled: bool
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
+class MetricInputMeasure(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    resource_type: ResourceType2
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    compiled_sql: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    relation_name: Optional[Optional[str]] = None
+    filter: Optional[WhereFilterIntersection] = None
+    alias: Optional[str] = None
+    join_to_timespine: Optional[bool] = False
+    fill_nulls_with: Optional[int] = None
 
 
-class CompiledHookNode(BaseParserModel):
+class Granularity(Enum):
+    day = 'day'
+    week = 'week'
+    month = 'month'
+    quarter = 'quarter'
+    year = 'year'
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    compiled: bool
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
-    name: str
-    resource_type: ResourceType3
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    compiled_sql: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    relation_name: Optional[Optional[str]] = None
-    index: Optional[Optional[int]] = None
+class MetricTimeWindow(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    count: int
+    granularity: Granularity
 
 
-class CompiledRPCNode(BaseParserModel):
+class OffsetToGrain(Enum):
+    day = 'day'
+    week = 'week'
+    month = 'month'
+    quarter = 'quarter'
+    year = 'year'
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    compiled: bool
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
+class MetricInput(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    resource_type: ResourceType4
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    compiled_sql: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    relation_name: Optional[Optional[str]] = None
-
+    filter: Optional[WhereFilterIntersection] = None
+    alias: Optional[str] = None
+    offset_window: Optional[MetricTimeWindow] = None
+    offset_to_grain: Optional[OffsetToGrain] = None
 
-class CompiledSchemaTestNode(BaseParserModel):
 
-    class Config:
-        extra = Extra.forbid
-
-    raw_sql: str
-    test_metadata: TestMetadata
-    compiled: bool
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
-    name: str
-    resource_type: ResourceType5
-    alias: str
-    checksum: FileHash
-    config: Optional[TestConfig] = {
-        'enabled': True,
-        'materialized': 'test',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-        'severity': 'ERROR',
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    compiled_sql: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    relation_name: Optional[Optional[str]] = None
-    column_name: Optional[Optional[str]] = None
+class GrainToDate(Enum):
+    day = 'day'
+    week = 'week'
+    month = 'month'
+    quarter = 'quarter'
+    year = 'year'
 
 
-class CompiledSeedNode(BaseParserModel):
+class MetricTypeParams(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    measure: Optional[MetricInputMeasure] = None
+    input_measures: Optional[List[MetricInputMeasure]] = None
+    numerator: Optional[MetricInput] = None
+    denominator: Optional[MetricInput] = None
+    expr: Optional[str] = None
+    window: Optional[MetricTimeWindow] = None
+    grain_to_date: Optional[GrainToDate] = None
+    metrics: Optional[List[MetricInput]] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    compiled: bool
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
-    name: str
-    resource_type: ResourceType6
-    alias: str
-    checksum: FileHash
-    config: Optional[SeedConfig] = {
-        'enabled': True,
-        'materialized': 'seed',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-        'quote_columns': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    compiled_sql: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    relation_name: Optional[Optional[str]] = None
+class FileSlice(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    filename: str
+    content: str
+    start_line_number: int
+    end_line_number: int
 
 
-class CompiledSnapshotNode(BaseParserModel):
+class SourceFileMetadata(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    repo_file_path: str
+    file_slice: FileSlice
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    compiled: bool
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
-    name: str
-    resource_type: ResourceType7
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    compiled_sql: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    relation_name: Optional[Optional[str]] = None
+class MetricConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
+    enabled: Optional[bool] = True
+    group: Optional[str] = None
 
 
-class ParsedAnalysisNode(BaseParserModel):
+class Type3(Enum):
+    simple = 'simple'
+    ratio = 'ratio'
+    cumulative = 'cumulative'
+    derived = 'derived'
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
+class Metric(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    resource_type: Literal['metric']
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
-    name: str
-    resource_type: ResourceType8
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-
-
-class ParsedHookNode(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    raw_sql: str
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
     unique_id: str
+    fqn: List[str]
+    description: str
+    label: str
+    type: Type3
+    type_params: MetricTypeParams
+    filter: Optional[WhereFilterIntersection] = None
+    metadata: Optional[SourceFileMetadata] = None
+    meta: Optional[Dict[str, Any]] = None
+    tags: Optional[List[str]] = None
+    config: Optional[MetricConfig] = None
+    unrendered_config: Optional[Dict[str, Any]] = None
+    sources: Optional[List[List[str]]] = None
+    depends_on: Optional[DependsOn] = None
+    refs: Optional[List[RefArgs]] = None
+    metrics: Optional[List[List[str]]] = None
+    created_at: Optional[float] = None
+    group: Optional[str] = None
+
+
+class Group(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    resource_type: Literal['group']
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
-    name: str
-    resource_type: ResourceType10
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    index: Optional[Optional[int]] = None
+    unique_id: str
+    owner: Owner
 
 
-class ParsedModelNode(BaseParserModel):
+class QueryParams(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    metrics: List[str]
+    group_by: List[str]
+    where: Optional[WhereFilterIntersection] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
-    name: str
-    resource_type: ResourceType11
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
+class ExportAs(Enum):
+    table = 'table'
+    view = 'view'
 
 
-class ParsedRPCNode(BaseParserModel):
+class ExportConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    export_as: ExportAs
+    schema_name: Optional[str] = None
+    alias: Optional[str] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
+class Export(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    resource_type: ResourceType12
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
+    config: ExportConfig
 
 
-class ParsedSnapshotNode(BaseParserModel):
+class SavedQueryConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
+    enabled: Optional[bool] = True
+    group: Optional[str] = None
+    meta: Optional[Dict[str, Any]] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
+class ResourceType(Enum):
+    model = 'model'
+    analysis = 'analysis'
+    test = 'test'
+    snapshot = 'snapshot'
+    operation = 'operation'
+    seed = 'seed'
+    rpc = 'rpc'
+    sql_operation = 'sql_operation'
+    doc = 'doc'
+    source = 'source'
+    macro = 'macro'
+    exposure = 'exposure'
+    metric = 'metric'
+    group = 'group'
+    saved_query = 'saved_query'
+    semantic_model = 'semantic_model'
+
+
+class SavedQuery(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    resource_type: ResourceType
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
-    name: str
-    resource_type: ResourceType15
+    unique_id: str
+    fqn: List[str]
+    query_params: QueryParams
+    exports: List[Export]
+    description: Optional[str] = None
+    label: Optional[str] = None
+    metadata: Optional[SourceFileMetadata] = None
+    config: Optional[SavedQueryConfig] = None
+    unrendered_config: Optional[Dict[str, Any]] = None
+    group: Optional[str] = None
+    depends_on: Optional[DependsOn] = None
+    created_at: Optional[float] = None
+    refs: Optional[List[RefArgs]] = None
+
+
+class NodeRelation(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     alias: str
-    checksum: FileHash
-    config: Union[TimestampSnapshotConfig, CheckSnapshotConfig,
-                  GenericSnapshotConfig]
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
+    schema_name: str
+    database: Optional[str] = None
+    relation_name: Optional[str] = None
 
 
-class FreshnessThreshold(BaseParserModel):
+class Defaults(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    agg_time_dimension: Optional[str] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    warn_after: Optional[Optional[Time]] = None
-    error_after: Optional[Optional[Time]] = None
-    filter: Optional[Optional[str]] = None
+class Type4(Enum):
+    foreign = 'foreign'
+    natural = 'natural'
+    primary = 'primary'
+    unique = 'unique'
 
 
-class SourceFreshnessOutput(BaseParserModel):
+class Entity(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    type: Type4
+    description: Optional[str] = None
+    label: Optional[str] = None
+    role: Optional[str] = None
+    expr: Optional[str] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    unique_id: str
-    max_loaded_at: datetime
-    snapshotted_at: datetime
-    max_loaded_at_time_ago_in_s: float
-    status: Status1
-    criteria: FreshnessThreshold
-    adapter_response: Dict[str, Any]
+class MeasureAggregationParameters(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    percentile: Optional[float] = None
+    use_discrete_percentile: Optional[bool] = False
+    use_approximate_percentile: Optional[bool] = False
+
+
+class WindowChoice(Enum):
+    sum = 'sum'
+    min = 'min'
+    max = 'max'
+    count_distinct = 'count_distinct'
+    sum_boolean = 'sum_boolean'
+    average = 'average'
+    percentile = 'percentile'
+    median = 'median'
+    count = 'count'
+
+
+class NonAdditiveDimension(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    window_choice: WindowChoice
+    window_groupings: List[str]
 
 
-class ExternalTable(BaseParserModel):
+class Agg(Enum):
+    sum = 'sum'
+    min = 'min'
+    max = 'max'
+    count_distinct = 'count_distinct'
+    sum_boolean = 'sum_boolean'
+    average = 'average'
+    percentile = 'percentile'
+    median = 'median'
+    count = 'count'
+
+
+class Measure(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    agg: Agg
+    description: Optional[str] = None
+    label: Optional[str] = None
+    create_metric: Optional[bool] = False
+    expr: Optional[str] = None
+    agg_params: Optional[MeasureAggregationParameters] = None
+    non_additive_dimension: Optional[NonAdditiveDimension] = None
+    agg_time_dimension: Optional[str] = None
 
-    class Config:
-        extra = Extra.allow
 
-    location: Optional[Optional[str]] = None
-    file_format: Optional[Optional[str]] = None
-    row_format: Optional[Optional[str]] = None
-    tbl_properties: Optional[Optional[str]] = None
-    partitions: Optional[Optional[List[ExternalPartition]]] = None
+class DimensionValidityParams(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    is_start: Optional[bool] = False
+    is_end: Optional[bool] = False
 
 
-class ParsedMacro(BaseParserModel):
+class TimeGranularity(Enum):
+    day = 'day'
+    week = 'week'
+    month = 'month'
+    quarter = 'quarter'
+    year = 'year'
 
-    class Config:
-        extra = Extra.forbid
 
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
-    name: str
-    macro_sql: str
-    resource_type: ResourceType17
-    tags: Optional[List[str]] = []
-    depends_on: Optional[MacroDependsOn] = {'macros': []}
-    description: Optional[str] = ''
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    arguments: Optional[List[MacroArgument]] = []
+class DimensionTypeParams(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    time_granularity: TimeGranularity
+    validity_params: Optional[DimensionValidityParams] = None
 
 
-class ParsedExposure(BaseParserModel):
+class Type5(Enum):
+    categorical = 'categorical'
+    time = 'time'
 
-    class Config:
-        extra = Extra.forbid
 
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
+class Dimension(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    type: Type
-    owner: ExposureOwner
-    resource_type: Optional[ResourceType18] = 'exposure'
-    description: Optional[str] = ''
-    maturity: Optional[Optional[MaturityEnum]] = None
-    url: Optional[Optional[str]] = None
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List[str]]] = []
+    type: Type5
+    description: Optional[str] = None
+    label: Optional[str] = None
+    is_partition: Optional[bool] = False
+    type_params: Optional[DimensionTypeParams] = None
+    expr: Optional[str] = None
+    metadata: Optional[SourceFileMetadata] = None
 
 
-class CompiledAnalysisNode(BaseParserModel):
+class SemanticModelConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    field_extra: Optional[Dict[str, Any]] = Field(None, alias='_extra')
+    enabled: Optional[bool] = True
+    group: Optional[str] = None
+    meta: Optional[Dict[str, Any]] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    raw_sql: str
-    compiled: bool
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    fqn: List[str]
-    unique_id: str
-    package_name: str
-    root_path: str
-    path: str
-    original_file_path: str
+class SemanticModel(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     resource_type: ResourceType
-    alias: str
-    checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'materialized': 'view',
-        'persist_docs': {},
-        'post-hook': [],
-        'pre-hook': [],
-        'vars': {},
-        'quoting': {},
-        'column_types': {},
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'full_refresh': None,
-    }
-    tags: Optional[List[str]] = []
-    refs: Optional[List[List[str]]] = []
-    sources: Optional[List[List]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
-    deferred: Optional[bool] = False
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    compiled_sql: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    relation_name: Optional[Optional[str]] = None
-
-
-class ParsedSourceDefinition(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    fqn: List[str]
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
-    unique_id: str
     package_name: str
-    root_path: str
     path: str
     original_file_path: str
-    name: str
-    source_name: str
-    source_description: str
-    loader: str
-    identifier: str
-    resource_type: ResourceType16
-    quoting: Optional[Quoting] = {
-        'database': None,
-        'schema': None,
-        'identifier': None,
-        'column': None,
-    }
-    loaded_at_field: Optional[Optional[str]] = None
-    freshness: Optional[Optional[FreshnessThreshold]] = None
-    external: Optional[Optional[ExternalTable]] = None
-    description: Optional[str] = ''
-    columns: Optional[Dict[str, ColumnInfo]] = {}
-    meta: Optional[Dict[str, Any]] = {}
-    source_meta: Optional[Dict[str, Any]] = {}
-    tags: Optional[List[str]] = []
-    config: Optional[SourceConfig] = {'enabled': True}
-    patch_path: Optional[Optional[str]] = None
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-
-
-class ManifestV1(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    metadata: ManifestMetadata = Field(
-        ..., description='Metadata about the manifest')
+    unique_id: str
+    fqn: List[str]
+    model: str
+    node_relation: Optional[NodeRelation] = None
+    description: Optional[str] = None
+    label: Optional[str] = None
+    defaults: Optional[Defaults] = None
+    entities: Optional[List[Entity]] = None
+    measures: Optional[List[Measure]] = None
+    dimensions: Optional[List[Dimension]] = None
+    metadata: Optional[SourceFileMetadata] = None
+    depends_on: Optional[DependsOn] = None
+    refs: Optional[List[RefArgs]] = None
+    created_at: Optional[float] = None
+    config: Optional[SemanticModelConfig] = None
+    unrendered_config: Optional[Dict[str, Any]] = None
+    primary_entity: Optional[str] = None
+    group: Optional[str] = None
+
+
+class ManifestV11(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    metadata: ManifestMetadata = Field(..., description='Metadata about the manifest')
     nodes: Dict[
-        str, Union[CompiledAnalysisNode, CompiledDataTestNode,
-                   CompiledModelNode, CompiledHookNode, CompiledRPCNode,
-                   CompiledSchemaTestNode, CompiledSeedNode,
-                   CompiledSnapshotNode, ParsedAnalysisNode, ParsedDataTestNode,
-                   ParsedHookNode, ParsedModelNode, ParsedRPCNode,
-                   ParsedSchemaTestNode, ParsedSeedNode, ParsedSnapshotNode,],
+        str,
+        Union[
+            AnalysisNode,
+            SingularTestNode,
+            HookNode,
+            ModelNode,
+            RPCNode,
+            SqlNode,
+            GenericTestNode,
+            SnapshotNode,
+            SeedNode,
+        ],
     ] = Field(
-        ...,
-        description='The nodes defined in the dbt project and its dependencies')
-    sources: Dict[str, ParsedSourceDefinition] = Field(
-        ...,
-        description='The sources defined in the dbt project and its dependencies'
-    )
-    macros: Dict[str, ParsedMacro] = Field(
-        ...,
-        description='The macros defined in the dbt project and its dependencies'
-    )
-    docs: Dict[str, ParsedDocumentation] = Field(
-        ...,
-        description='The docs defined in the dbt project and its dependencies')
-    exposures: Dict[str, ParsedExposure] = Field(
-        ...,
-        description=
-        'The exposures defined in the dbt project and its dependencies')
+        ..., description='The nodes defined in the dbt project and its dependencies'
+    )
+    sources: Dict[str, SourceDefinition] = Field(
+        ..., description='The sources defined in the dbt project and its dependencies'
+    )
+    macros: Dict[str, Macro] = Field(
+        ..., description='The macros defined in the dbt project and its dependencies'
+    )
+    docs: Dict[str, Documentation] = Field(
+        ..., description='The docs defined in the dbt project and its dependencies'
+    )
+    exposures: Dict[str, Exposure] = Field(
+        ..., description='The exposures defined in the dbt project and its dependencies'
+    )
+    metrics: Dict[str, Metric] = Field(
+        ..., description='The metrics defined in the dbt project and its dependencies'
+    )
+    groups: Dict[str, Group] = Field(
+        ..., description='The groups defined in the dbt project'
+    )
     selectors: Dict[str, Any] = Field(
-        ..., description='The selectors defined in selectors.yml')
-    disabled: Optional[Optional[List[
-        Union[CompiledAnalysisNode, CompiledDataTestNode, CompiledModelNode,
-              CompiledHookNode, CompiledRPCNode, CompiledSchemaTestNode,
-              CompiledSeedNode, CompiledSnapshotNode, ParsedAnalysisNode,
-              ParsedDataTestNode, ParsedHookNode, ParsedModelNode,
-              ParsedRPCNode, ParsedSchemaTestNode, ParsedSeedNode,
-              ParsedSnapshotNode, ParsedSourceDefinition,]]]] = Field(
-                  None,
-                  description='A list of the disabled nodes in the target')
-    parent_map: Optional[Optional[Dict[str, List[str]]]] = Field(
-        None, description='A mapping from\xa0child nodes to their dependencies')
-    child_map: Optional[Optional[Dict[str, List[str]]]] = Field(
-        None, description='A mapping from parent nodes to their dependents')
+        ..., description='The selectors defined in selectors.yml'
+    )
+    disabled: Optional[
+        Dict[
+            str,
+            List[
+                Union[
+                    AnalysisNode,
+                    SingularTestNode,
+                    HookNode,
+                    ModelNode,
+                    RPCNode,
+                    SqlNode,
+                    GenericTestNode,
+                    SnapshotNode,
+                    SeedNode,
+                    SourceDefinition,
+                    Exposure,
+                    Metric,
+                    SavedQuery,
+                    SemanticModel,
+                ]
+            ],
+        ]
+    ] = Field(..., description='A mapping of the disabled nodes in the target')
+    parent_map: Optional[Dict[str, List[str]]] = Field(
+        ..., description='A mapping from\xa0child nodes to their dependencies'
+    )
+    child_map: Optional[Dict[str, List[str]]] = Field(
+        ..., description='A mapping from parent nodes to their dependents'
+    )
+    group_map: Optional[Dict[str, List[str]]] = Field(
+        ..., description='A mapping from group names to their nodes'
+    )
+    saved_queries: Dict[str, SavedQuery] = Field(
+        ..., description='The saved queries defined in the dbt project'
+    )
+    semantic_models: Dict[str, SemanticModel] = Field(
+        ..., description='The semantic models defined in the dbt project'
+    )
+
+
+# NOTE: We manually change the class, as the generated code is not correct.
+# class ManifestV11(RootModel[WritableManifest]):
+#     root: WritableManifest
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v10.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,161 +1,152 @@
 # generated by datamodel-codegen:
-#   filename:  manifest_v10.json
+#   filename:  manifest_v9.json
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra, Field, constr
+from pydantic import AwareDatetime, ConfigDict, Field, constr
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class ManifestMetadata(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     dbt_schema_version: Optional[
         str
-    ] = 'https://schemas.getdbt.com/dbt/manifest/v10.json'
-    dbt_version: Optional[str] = '1.6.0'
-    generated_at: Optional[datetime] = '2023-08-07T20:10:03.381822Z'
-    invocation_id: Optional[str] = '03dee192-ff77-43cc-bc3f-5eeaf6d36344'
+    ] = 'https://schemas.getdbt.com/dbt/manifest/v9.json'
+    dbt_version: Optional[str] = '1.5.0b5'
+    generated_at: Optional[AwareDatetime] = '2023-04-12T03:35:01.188035Z'
+    invocation_id: Optional[str] = '8aa1596d-f52f-40bc-ad4b-f5e48fc7e6c2'
     env: Optional[Dict[str, str]] = {}
-    project_name: Optional[str] = Field(None, description='Name of the root project')
     project_id: Optional[str] = Field(
-        None,
-        description='A unique identifier for the project, hashed from the project name',
+        None, description='A unique identifier for the project'
     )
     user_id: Optional[
-        constr(regex=r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}')
+        constr(pattern=r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}')
     ] = Field(None, description='A unique identifier for the user')
     send_anonymous_usage_stats: Optional[bool] = Field(
         None, description='Whether dbt is configured to send anonymous usage statistics'
     )
     adapter_type: Optional[str] = Field(
         None, description='The type name of the adapter'
     )
 
 
 class ResourceType(Enum):
     analysis = 'analysis'
 
 
 class FileHash(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     checksum: str
 
 
-class OnConfigurationChange(Enum):
-    apply = 'apply'
-    continue_ = 'continue'
-    fail = 'fail'
-
-
 class Hook(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     sql: str
     transaction: Optional[bool] = True
     index: Optional[int] = None
 
 
 class Docs(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     show: Optional[bool] = True
     node_color: Optional[str] = None
 
 
 class ContractConfig(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     enforced: Optional[bool] = False
 
 
 class Type(Enum):
     check = 'check'
     not_null = 'not_null'
     unique = 'unique'
     primary_key = 'primary_key'
     foreign_key = 'foreign_key'
     custom = 'custom'
 
 
 class ColumnLevelConstraint(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     type: Type
     name: Optional[str] = None
     expression: Optional[str] = None
     warn_unenforced: Optional[bool] = True
     warn_unsupported: Optional[bool] = True
 
 
 class RefArgs(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     package: Optional[str] = None
     version: Optional[Union[str, float]] = None
 
 
 class DependsOn(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     macros: Optional[List[str]] = []
     nodes: Optional[List[str]] = []
 
 
 class InjectedCTE(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     id: str
     sql: str
 
 
 class Contract(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     enforced: Optional[bool] = False
     checksum: Optional[str] = None
 
 
 class ResourceType1(Enum):
     test = 'test'
 
 
 class TestConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
     alias: Optional[str] = None
     schema_: Optional[str] = Field('dbt_test__audit', alias='schema')
     database: Optional[str] = None
     tags: Optional[Union[List[str], str]] = []
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     materialized: Optional[str] = 'test'
     severity: Optional[
-        constr(regex=r'^([Ww][Aa][Rr][Nn]|[Ee][Rr][Rr][Oo][Rr])$')
+        constr(pattern=r'^([Ww][Aa][Rr][Nn]|[Ee][Rr][Rr][Oo][Rr])$')
     ] = 'ERROR'
     store_failures: Optional[bool] = None
     where: Optional[str] = None
     limit: Optional[int] = None
     fail_calc: Optional[str] = 'count(*)'
     warn_if: Optional[str] = '!= 0'
     error_if: Optional[str] = '!= 0'
@@ -172,64 +163,54 @@
 class Access(Enum):
     protected = 'protected'
     private = 'private'
     public = 'public'
 
 
 class ModelLevelConstraint(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     type: Type
     name: Optional[str] = None
     expression: Optional[str] = None
     warn_unenforced: Optional[bool] = True
     warn_unsupported: Optional[bool] = True
     columns: Optional[List[str]] = []
 
 
-class DeferRelation(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[str] = None
-    schema_: str = Field(..., alias='schema')
-    alias: str
-    relation_name: Optional[str] = None
-
-
 class ResourceType4(Enum):
     rpc = 'rpc'
 
 
 class ResourceType5(Enum):
-    sql_operation = 'sql_operation'
+    sql_operation = 'sql operation'
 
 
 class ResourceType6(Enum):
     test = 'test'
 
 
 class TestMetadata(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     kwargs: Optional[Dict[str, Any]] = {}
     namespace: Optional[str] = None
 
 
 class ResourceType7(Enum):
     snapshot = 'snapshot'
 
 
 class SnapshotConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
     alias: Optional[str] = None
     schema_: Optional[str] = Field(None, alias='schema')
     database: Optional[str] = None
     tags: Optional[Union[List[str], str]] = []
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
@@ -239,38 +220,37 @@
     post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
     pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
     quoting: Optional[Dict[str, Any]] = {}
     column_types: Optional[Dict[str, Any]] = {}
     full_refresh: Optional[bool] = None
     unique_key: Optional[str] = None
     on_schema_change: Optional[str] = 'ignore'
-    on_configuration_change: Optional[OnConfigurationChange] = 'apply'
     grants: Optional[Dict[str, Any]] = {}
     packages: Optional[List[str]] = []
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     contract: Optional[ContractConfig] = Field(
-        default_factory=lambda: ContractConfig.parse_obj({'enforced': False})
+        default_factory=lambda: ContractConfig.model_validate({'enforced': False})
     )
     strategy: Optional[str] = None
     target_schema: Optional[str] = None
     target_database: Optional[str] = None
     updated_at: Optional[str] = None
     check_cols: Optional[Union[str, List[str]]] = None
 
 
 class ResourceType8(Enum):
     seed = 'seed'
 
 
 class SeedConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
     alias: Optional[str] = None
     schema_: Optional[str] = Field(None, alias='schema')
     database: Optional[str] = None
     tags: Optional[Union[List[str], str]] = []
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
@@ -280,104 +260,143 @@
     post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
     pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
     quoting: Optional[Dict[str, Any]] = {}
     column_types: Optional[Dict[str, Any]] = {}
     full_refresh: Optional[bool] = None
     unique_key: Optional[Union[str, List[str]]] = None
     on_schema_change: Optional[str] = 'ignore'
-    on_configuration_change: Optional[OnConfigurationChange] = 'apply'
     grants: Optional[Dict[str, Any]] = {}
     packages: Optional[List[str]] = []
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     contract: Optional[ContractConfig] = Field(
-        default_factory=lambda: ContractConfig.parse_obj({'enforced': False})
+        default_factory=lambda: ContractConfig.model_validate({'enforced': False})
     )
     quote_columns: Optional[bool] = None
 
 
 class MacroDependsOn(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     macros: Optional[List[str]] = []
 
 
 class ResourceType9(Enum):
     source = 'source'
 
 
 class Quoting(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[bool] = None
     schema_: Optional[bool] = Field(None, alias='schema')
     identifier: Optional[bool] = None
     column: Optional[bool] = None
 
 
-class PeriodEnum(Enum):
+class FreshnessMetadata(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: Optional[str] = 'https://schemas.getdbt.com/dbt/sources/v3.json'
+    dbt_version: Optional[str] = '1.5.0b5'
+    generated_at: Optional[AwareDatetime] = '2023-04-12T03:35:01.185979Z'
+    invocation_id: Optional[str] = '8aa1596d-f52f-40bc-ad4b-f5e48fc7e6c2'
+    env: Optional[Dict[str, str]] = {}
+
+
+class Status(Enum):
+    runtime_error = 'runtime error'
+
+
+class SourceFreshnessRuntimeError(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    unique_id: str
+    error: Optional[Union[str, int]] = None
+    status: Status
+
+
+class Status1(Enum):
+    pass_ = 'pass'
+    warn = 'warn'
+    error = 'error'
+    runtime_error = 'runtime error'
+
+
+class Period(Enum):
     minute = 'minute'
     hour = 'hour'
     day = 'day'
 
 
 class Time(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     count: Optional[int] = None
-    period: Optional[PeriodEnum] = None
+    period: Optional[Period] = None
 
 
-class ExternalPartition(BaseParserModel):
-    class Config:
-        extra = Extra.allow
+class TimingInfo(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    started_at: Optional[AwareDatetime] = None
+    completed_at: Optional[AwareDatetime] = None
 
+
+class ExternalPartition(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
     name: Optional[str] = ''
     description: Optional[str] = ''
     data_type: Optional[str] = ''
     meta: Optional[Dict[str, Any]] = {}
 
 
 class SourceConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
 
 
 class ResourceType10(Enum):
     macro = 'macro'
 
 
 class SupportedLanguage(Enum):
     python = 'python'
     sql = 'sql'
 
 
 class MacroArgument(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     type: Optional[str] = None
     description: Optional[str] = ''
 
 
 class ResourceType11(Enum):
     doc = 'doc'
 
 
 class Documentation(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     resource_type: ResourceType11
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     block_contents: str
@@ -391,247 +410,92 @@
     dashboard = 'dashboard'
     notebook = 'notebook'
     analysis = 'analysis'
     ml = 'ml'
     application = 'application'
 
 
-class MaturityEnum(Enum):
+class Maturity(Enum):
     low = 'low'
     medium = 'medium'
     high = 'high'
 
 
 class Owner(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     email: Optional[str] = None
     name: Optional[str] = None
 
 
 class ExposureConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
 
 
 class ResourceType13(Enum):
     metric = 'metric'
 
 
-class Type3(Enum):
-    simple = 'simple'
-    ratio = 'ratio'
-    cumulative = 'cumulative'
-    derived = 'derived'
-
-
-class GrainToDateEnum(Enum):
-    day = 'day'
-    week = 'week'
-    month = 'month'
-    quarter = 'quarter'
-    year = 'year'
-
-
-class WhereFilter(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    where_sql_template: str
-
-
-class OffsetToGrainEnum(Enum):
-    day = 'day'
-    week = 'week'
-    month = 'month'
-    quarter = 'quarter'
-    year = 'year'
+class MetricFilter(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    field: str
+    operator: str
+    value: str
 
 
-class Granularity(Enum):
+class Period1(Enum):
     day = 'day'
     week = 'week'
     month = 'month'
-    quarter = 'quarter'
     year = 'year'
 
 
-class MetricTimeWindow(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    count: int
-    granularity: Granularity
-
-
-class FileSlice(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    filename: str
-    content: str
-    start_line_number: int
-    end_line_number: int
+class MetricTime(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    count: Optional[int] = None
+    period: Optional[Period1] = None
 
 
 class MetricConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
     group: Optional[str] = None
 
 
 class ResourceType14(Enum):
     group = 'group'
 
 
 class Group(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     resource_type: ResourceType14
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     owner: Owner
 
 
-class ResourceType15(Enum):
-    model = 'model'
-    analysis = 'analysis'
-    test = 'test'
-    snapshot = 'snapshot'
-    operation = 'operation'
-    seed = 'seed'
-    rpc = 'rpc'
-    sql_operation = 'sql_operation'
-    doc = 'doc'
-    source = 'source'
-    macro = 'macro'
-    exposure = 'exposure'
-    metric = 'metric'
-    group = 'group'
-    semantic_model = 'semantic_model'
-
-
-class NodeRelation(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    alias: str
-    schema_name: str
-    database: Optional[str] = None
-    relation_name: Optional[str] = None
-
-
-class Defaults(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    agg_time_dimension: Optional[str] = None
-
-
-class Type4(Enum):
-    foreign = 'foreign'
-    natural = 'natural'
-    primary = 'primary'
-    unique = 'unique'
-
-
-class Entity(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    type: Type4
-    description: Optional[str] = None
-    role: Optional[str] = None
-    expr: Optional[str] = None
-
-
-class Agg(Enum):
-    sum = 'sum'
-    min = 'min'
-    max = 'max'
-    count_distinct = 'count_distinct'
-    sum_boolean = 'sum_boolean'
-    average = 'average'
-    percentile = 'percentile'
-    median = 'median'
-    count = 'count'
-
-
-class MeasureAggregationParameters(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    percentile: Optional[float] = None
-    use_discrete_percentile: Optional[bool] = False
-    use_approximate_percentile: Optional[bool] = False
-
-
-class WindowChoice(Enum):
-    sum = 'sum'
-    min = 'min'
-    max = 'max'
-    count_distinct = 'count_distinct'
-    sum_boolean = 'sum_boolean'
-    average = 'average'
-    percentile = 'percentile'
-    median = 'median'
-    count = 'count'
-
-
-class NonAdditiveDimension(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    window_choice: WindowChoice
-    window_groupings: List[str]
-
-
-class Type5(Enum):
-    categorical = 'categorical'
-    time = 'time'
-
-
-class TimeGranularity(Enum):
-    day = 'day'
-    week = 'week'
-    month = 'month'
-    quarter = 'quarter'
-    year = 'year'
-
-
-class DimensionValidityParams(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    is_start: Optional[bool] = False
-    is_end: Optional[bool] = False
-
-
-class SemanticModelConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
-    enabled: Optional[bool] = True
-
-
 class NodeConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
     alias: Optional[str] = None
     schema_: Optional[str] = Field(None, alias='schema')
     database: Optional[str] = None
     tags: Optional[Union[List[str], str]] = []
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
@@ -641,55 +505,54 @@
     post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
     pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
     quoting: Optional[Dict[str, Any]] = {}
     column_types: Optional[Dict[str, Any]] = {}
     full_refresh: Optional[bool] = None
     unique_key: Optional[Union[str, List[str]]] = None
     on_schema_change: Optional[str] = 'ignore'
-    on_configuration_change: Optional[OnConfigurationChange] = 'apply'
     grants: Optional[Dict[str, Any]] = {}
     packages: Optional[List[str]] = []
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     contract: Optional[ContractConfig] = Field(
-        default_factory=lambda: ContractConfig.parse_obj({'enforced': False})
+        default_factory=lambda: ContractConfig.model_validate({'enforced': False})
     )
 
 
 class ColumnInfo(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     name: str
     description: Optional[str] = ''
     meta: Optional[Dict[str, Any]] = {}
     data_type: Optional[str] = None
     constraints: Optional[List[ColumnLevelConstraint]] = []
     quote: Optional[bool] = None
     tags: Optional[List[str]] = []
 
 
 class SingularTestNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType1
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     alias: str
     checksum: FileHash
     config: Optional[TestConfig] = Field(
-        default_factory=lambda: TestConfig.parse_obj(
+        default_factory=lambda: TestConfig.model_validate(
             {
                 'enabled': True,
                 'alias': None,
                 'schema': 'dbt_test__audit',
                 'database': None,
                 'tags': [],
                 'meta': {},
@@ -707,60 +570,60 @@
     )
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.389955
+    created_at: Optional[float] = 1681270501.19095
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     language: Optional[str] = 'sql'
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     compiled_path: Optional[str] = None
     compiled: Optional[bool] = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
     contract: Optional[Contract] = Field(
-        default_factory=lambda: Contract.parse_obj(
+        default_factory=lambda: Contract.model_validate(
             {'enforced': False, 'checksum': None}
         )
     )
 
 
 class HookNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType2
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     alias: str
     checksum: FileHash
     config: Optional[NodeConfig] = Field(
-        default_factory=lambda: NodeConfig.parse_obj(
+        default_factory=lambda: NodeConfig.model_validate(
             {
                 'enabled': True,
                 'alias': None,
                 'schema': None,
                 'database': None,
                 'tags': [],
                 'meta': {},
@@ -769,15 +632,14 @@
                 'incremental_strategy': None,
                 'persist_docs': {},
                 'quoting': {},
                 'column_types': {},
                 'full_refresh': None,
                 'unique_key': None,
                 'on_schema_change': 'ignore',
-                'on_configuration_change': 'apply',
                 'grants': {},
                 'packages': [],
                 'docs': {'show': True, 'node_color': None},
                 'contract': {'enforced': False},
                 'post-hook': [],
                 'pre-hook': [],
             }
@@ -785,61 +647,61 @@
     )
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.3916101
+    created_at: Optional[float] = 1681270501.191555
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     language: Optional[str] = 'sql'
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     compiled_path: Optional[str] = None
     compiled: Optional[bool] = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
     contract: Optional[Contract] = Field(
-        default_factory=lambda: Contract.parse_obj(
+        default_factory=lambda: Contract.model_validate(
             {'enforced': False, 'checksum': None}
         )
     )
     index: Optional[int] = None
 
 
 class ModelNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType3
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     alias: str
     checksum: FileHash
     config: Optional[NodeConfig] = Field(
-        default_factory=lambda: NodeConfig.parse_obj(
+        default_factory=lambda: NodeConfig.model_validate(
             {
                 'enabled': True,
                 'alias': None,
                 'schema': None,
                 'database': None,
                 'tags': [],
                 'meta': {},
@@ -848,15 +710,14 @@
                 'incremental_strategy': None,
                 'persist_docs': {},
                 'quoting': {},
                 'column_types': {},
                 'full_refresh': None,
                 'unique_key': None,
                 'on_schema_change': 'ignore',
-                'on_configuration_change': 'apply',
                 'grants': {},
                 'packages': [],
                 'docs': {'show': True, 'node_color': None},
                 'contract': {'enforced': False},
                 'post-hook': [],
                 'pre-hook': [],
             }
@@ -864,66 +725,64 @@
     )
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.393298
+    created_at: Optional[float] = 1681270501.192162
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     language: Optional[str] = 'sql'
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     compiled_path: Optional[str] = None
     compiled: Optional[bool] = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
     contract: Optional[Contract] = Field(
-        default_factory=lambda: Contract.parse_obj(
+        default_factory=lambda: Contract.model_validate(
             {'enforced': False, 'checksum': None}
         )
     )
     access: Optional[Access] = 'protected'
     constraints: Optional[List[ModelLevelConstraint]] = []
     version: Optional[Union[str, float]] = None
     latest_version: Optional[Union[str, float]] = None
-    deprecation_date: Optional[datetime] = None
-    defer_relation: Optional[DeferRelation] = None
 
 
 class RPCNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType4
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     alias: str
     checksum: FileHash
     config: Optional[NodeConfig] = Field(
-        default_factory=lambda: NodeConfig.parse_obj(
+        default_factory=lambda: NodeConfig.model_validate(
             {
                 'enabled': True,
                 'alias': None,
                 'schema': None,
                 'database': None,
                 'tags': [],
                 'meta': {},
@@ -932,15 +791,14 @@
                 'incremental_strategy': None,
                 'persist_docs': {},
                 'quoting': {},
                 'column_types': {},
                 'full_refresh': None,
                 'unique_key': None,
                 'on_schema_change': 'ignore',
-                'on_configuration_change': 'apply',
                 'grants': {},
                 'packages': [],
                 'docs': {'show': True, 'node_color': None},
                 'contract': {'enforced': False},
                 'post-hook': [],
                 'pre-hook': [],
             }
@@ -948,60 +806,60 @@
     )
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.39583
+    created_at: Optional[float] = 1681270501.192949
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     language: Optional[str] = 'sql'
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     compiled_path: Optional[str] = None
     compiled: Optional[bool] = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
     contract: Optional[Contract] = Field(
-        default_factory=lambda: Contract.parse_obj(
+        default_factory=lambda: Contract.model_validate(
             {'enforced': False, 'checksum': None}
         )
     )
 
 
 class SqlNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType5
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     alias: str
     checksum: FileHash
     config: Optional[NodeConfig] = Field(
-        default_factory=lambda: NodeConfig.parse_obj(
+        default_factory=lambda: NodeConfig.model_validate(
             {
                 'enabled': True,
                 'alias': None,
                 'schema': None,
                 'database': None,
                 'tags': [],
                 'meta': {},
@@ -1010,15 +868,14 @@
                 'incremental_strategy': None,
                 'persist_docs': {},
                 'quoting': {},
                 'column_types': {},
                 'full_refresh': None,
                 'unique_key': None,
                 'on_schema_change': 'ignore',
-                'on_configuration_change': 'apply',
                 'grants': {},
                 'packages': [],
                 'docs': {'show': True, 'node_color': None},
                 'contract': {'enforced': False},
                 'post-hook': [],
                 'pre-hook': [],
             }
@@ -1026,61 +883,61 @@
     )
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.3974268
+    created_at: Optional[float] = 1681270501.1935291
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     language: Optional[str] = 'sql'
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     compiled_path: Optional[str] = None
     compiled: Optional[bool] = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
     contract: Optional[Contract] = Field(
-        default_factory=lambda: Contract.parse_obj(
+        default_factory=lambda: Contract.model_validate(
             {'enforced': False, 'checksum': None}
         )
     )
 
 
 class GenericTestNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     test_metadata: TestMetadata
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType6
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     alias: str
     checksum: FileHash
     config: Optional[TestConfig] = Field(
-        default_factory=lambda: TestConfig.parse_obj(
+        default_factory=lambda: TestConfig.model_validate(
             {
                 'enabled': True,
                 'alias': None,
                 'schema': 'dbt_test__audit',
                 'database': None,
                 'tags': [],
                 'meta': {},
@@ -1098,50 +955,50 @@
     )
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.399393
+    created_at: Optional[float] = 1681270501.19419
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     language: Optional[str] = 'sql'
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     compiled_path: Optional[str] = None
     compiled: Optional[bool] = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
     contract: Optional[Contract] = Field(
-        default_factory=lambda: Contract.parse_obj(
+        default_factory=lambda: Contract.model_validate(
             {'enforced': False, 'checksum': None}
         )
     )
     column_name: Optional[str] = None
     file_key_name: Optional[str] = None
     attached_node: Optional[str] = None
 
 
 class SnapshotNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType7
     package_name: str
     path: str
     original_file_path: str
@@ -1152,61 +1009,60 @@
     config: SnapshotConfig
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.4026701
+    created_at: Optional[float] = 1681270501.1952698
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     language: Optional[str] = 'sql'
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     compiled_path: Optional[str] = None
     compiled: Optional[bool] = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
     contract: Optional[Contract] = Field(
-        default_factory=lambda: Contract.parse_obj(
+        default_factory=lambda: Contract.model_validate(
             {'enforced': False, 'checksum': None}
         )
     )
-    defer_relation: Optional[DeferRelation] = None
 
 
 class SeedNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType8
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     alias: str
     checksum: FileHash
     config: Optional[SeedConfig] = Field(
-        default_factory=lambda: SeedConfig.parse_obj(
+        default_factory=lambda: SeedConfig.model_validate(
             {
                 'enabled': True,
                 'alias': None,
                 'schema': None,
                 'database': None,
                 'tags': [],
                 'meta': {},
@@ -1215,15 +1071,14 @@
                 'incremental_strategy': None,
                 'persist_docs': {},
                 'quoting': {},
                 'column_types': {},
                 'full_refresh': None,
                 'unique_key': None,
                 'on_schema_change': 'ignore',
-                'on_configuration_change': 'apply',
                 'grants': {},
                 'packages': [],
                 'docs': {'show': True, 'node_color': None},
                 'contract': {'enforced': False},
                 'quote_columns': None,
                 'post-hook': [],
                 'pre-hook': [],
@@ -1232,175 +1087,180 @@
     )
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.4056058
+    created_at: Optional[float] = 1681270501.1968079
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     root_path: Optional[str] = None
     depends_on: Optional[MacroDependsOn] = Field(
-        default_factory=lambda: MacroDependsOn.parse_obj({'macros': []})
+        default_factory=lambda: MacroDependsOn.model_validate({'macros': []})
     )
-    defer_relation: Optional[DeferRelation] = None
 
 
 class FreshnessThreshold(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     warn_after: Optional[Time] = {'count': None, 'period': None}
     error_after: Optional[Time] = {'count': None, 'period': None}
     filter: Optional[str] = None
 
 
-class ExternalTable(BaseParserModel):
-    class Config:
-        extra = Extra.allow
+class SourceFreshnessOutput(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    unique_id: str
+    max_loaded_at: AwareDatetime
+    snapshotted_at: AwareDatetime
+    max_loaded_at_time_ago_in_s: float
+    status: Status1
+    criteria: FreshnessThreshold
+    adapter_response: Dict[str, Any]
+    timing: List[TimingInfo]
+    thread_id: str
+    execution_time: float
 
+
+class ExternalTable(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
     location: Optional[str] = None
     file_format: Optional[str] = None
     row_format: Optional[str] = None
     tbl_properties: Optional[str] = None
     partitions: Optional[Union[List[str], List[ExternalPartition]]] = None
 
 
 class Macro(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     resource_type: ResourceType10
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     macro_sql: str
     depends_on: Optional[MacroDependsOn] = Field(
-        default_factory=lambda: MacroDependsOn.parse_obj({'macros': []})
+        default_factory=lambda: MacroDependsOn.model_validate({'macros': []})
     )
     description: Optional[str] = ''
     meta: Optional[Dict[str, Any]] = {}
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     arguments: Optional[List[MacroArgument]] = []
-    created_at: Optional[float] = 1691439003.409885
+    created_at: Optional[float] = 1681270501.198105
     supported_languages: Optional[List[SupportedLanguage]] = None
 
 
 class Exposure(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     resource_type: ResourceType12
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     type: Type2
     owner: Owner
     description: Optional[str] = ''
     label: Optional[str] = None
-    maturity: Optional[MaturityEnum] = None
+    maturity: Optional[Maturity] = None
     meta: Optional[Dict[str, Any]] = {}
     tags: Optional[List[str]] = []
     config: Optional[ExposureConfig] = Field(
-        default_factory=lambda: ExposureConfig.parse_obj({'enabled': True})
+        default_factory=lambda: ExposureConfig.model_validate({'enabled': True})
     )
     unrendered_config: Optional[Dict[str, Any]] = {}
     url: Optional[str] = None
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
-    created_at: Optional[float] = 1691439003.411563
-
+    created_at: Optional[float] = 1681270501.198782
 
-class MetricInputMeasure(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    filter: Optional[WhereFilter] = None
-    alias: Optional[str] = None
-
-
-class MetricInput(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    filter: Optional[WhereFilter] = None
-    alias: Optional[str] = None
-    offset_window: Optional[MetricTimeWindow] = None
-    offset_to_grain: Optional[OffsetToGrainEnum] = None
-
-
-class SourceFileMetadata(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    repo_file_path: str
-    file_slice: FileSlice
-
-
-class Measure(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
+class Metric(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    agg: Agg
-    description: Optional[str] = None
-    create_metric: Optional[bool] = False
-    expr: Optional[str] = None
-    agg_params: Optional[MeasureAggregationParameters] = None
-    non_additive_dimension: Optional[NonAdditiveDimension] = None
-    agg_time_dimension: Optional[str] = None
-
-
-class DimensionTypeParams(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    time_granularity: TimeGranularity
-    validity_params: Optional[DimensionValidityParams] = None
+    resource_type: ResourceType13
+    package_name: str
+    path: str
+    original_file_path: str
+    unique_id: str
+    fqn: List[str]
+    description: str
+    label: str
+    calculation_method: str
+    expression: str
+    filters: List[MetricFilter]
+    time_grains: List[str]
+    dimensions: List[str]
+    timestamp: Optional[str] = None
+    window: Optional[MetricTime] = None
+    model: Optional[str] = None
+    model_unique_id: Optional[str] = None
+    meta: Optional[Dict[str, Any]] = {}
+    tags: Optional[List[str]] = []
+    config: Optional[MetricConfig] = Field(
+        default_factory=lambda: MetricConfig.model_validate(
+            {'enabled': True, 'group': None}
+        )
+    )
+    unrendered_config: Optional[Dict[str, Any]] = {}
+    sources: Optional[List[List[str]]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
+    refs: Optional[List[RefArgs]] = []
+    metrics: Optional[List[List[str]]] = []
+    created_at: Optional[float] = 1681270501.199492
+    group: Optional[str] = None
 
 
 class AnalysisNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     alias: str
     checksum: FileHash
     config: Optional[NodeConfig] = Field(
-        default_factory=lambda: NodeConfig.parse_obj(
+        default_factory=lambda: NodeConfig.model_validate(
             {
                 'enabled': True,
                 'alias': None,
                 'schema': None,
                 'database': None,
                 'tags': [],
                 'meta': {},
@@ -1409,15 +1269,14 @@
                 'incremental_strategy': None,
                 'persist_docs': {},
                 'quoting': {},
                 'column_types': {},
                 'full_refresh': None,
                 'unique_key': None,
                 'on_schema_change': 'ignore',
-                'on_configuration_change': 'apply',
                 'grants': {},
                 'packages': [],
                 'docs': {'show': True, 'node_color': None},
                 'contract': {'enforced': False},
                 'post-hook': [],
                 'pre-hook': [],
             }
@@ -1425,176 +1284,86 @@
     )
     tags: Optional[List[str]] = []
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     group: Optional[str] = None
     docs: Optional[Docs] = Field(
-        default_factory=lambda: Docs.parse_obj({'show': True, 'node_color': None})
+        default_factory=lambda: Docs.model_validate({'show': True, 'node_color': None})
     )
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1691439003.386713
+    created_at: Optional[float] = 1681270501.189703
     config_call_dict: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
     raw_code: Optional[str] = ''
     language: Optional[str] = 'sql'
     refs: Optional[List[RefArgs]] = []
     sources: Optional[List[List[str]]] = []
     metrics: Optional[List[List[str]]] = []
     depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
     )
     compiled_path: Optional[str] = None
     compiled: Optional[bool] = False
     compiled_code: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
     contract: Optional[Contract] = Field(
-        default_factory=lambda: Contract.parse_obj(
+        default_factory=lambda: Contract.model_validate(
             {'enforced': False, 'checksum': None}
         )
     )
 
 
 class SourceDefinition(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType9
     package_name: str
     path: str
     original_file_path: str
     unique_id: str
     fqn: List[str]
     source_name: str
     source_description: str
     loader: str
     identifier: str
     quoting: Optional[Quoting] = Field(
-        default_factory=lambda: Quoting.parse_obj(
+        default_factory=lambda: Quoting.model_validate(
             {'database': None, 'schema': None, 'identifier': None, 'column': None}
         )
     )
     loaded_at_field: Optional[str] = None
     freshness: Optional[FreshnessThreshold] = None
     external: Optional[ExternalTable] = None
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     source_meta: Optional[Dict[str, Any]] = {}
     tags: Optional[List[str]] = []
     config: Optional[SourceConfig] = Field(
-        default_factory=lambda: SourceConfig.parse_obj({'enabled': True})
+        default_factory=lambda: SourceConfig.model_validate({'enabled': True})
     )
     patch_path: Optional[str] = None
     unrendered_config: Optional[Dict[str, Any]] = {}
     relation_name: Optional[str] = None
-    created_at: Optional[float] = 1691439003.408927
-
-
-class MetricTypeParams(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    measure: Optional[MetricInputMeasure] = None
-    input_measures: Optional[List[MetricInputMeasure]] = []
-    numerator: Optional[MetricInput] = None
-    denominator: Optional[MetricInput] = None
-    expr: Optional[str] = None
-    window: Optional[MetricTimeWindow] = None
-    grain_to_date: Optional[GrainToDateEnum] = None
-    metrics: Optional[List[MetricInput]] = None
-
-
-class Dimension(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    type: Type5
-    description: Optional[str] = None
-    is_partition: Optional[bool] = False
-    type_params: Optional[DimensionTypeParams] = None
-    expr: Optional[str] = None
-    metadata: Optional[SourceFileMetadata] = None
-
-
-class Metric(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    resource_type: ResourceType13
-    package_name: str
-    path: str
-    original_file_path: str
-    unique_id: str
-    fqn: List[str]
-    description: str
-    label: str
-    type: Type3
-    type_params: MetricTypeParams
-    filter: Optional[WhereFilter] = None
-    metadata: Optional[SourceFileMetadata] = None
-    meta: Optional[Dict[str, Any]] = {}
-    tags: Optional[List[str]] = []
-    config: Optional[MetricConfig] = Field(
-        default_factory=lambda: MetricConfig.parse_obj({'enabled': True, 'group': None})
-    )
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    sources: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
-    )
-    refs: Optional[List[RefArgs]] = []
-    metrics: Optional[List[List[str]]] = []
-    created_at: Optional[float] = 1691439003.41419
-    group: Optional[str] = None
+    created_at: Optional[float] = 1681270501.197819
 
 
-class SemanticModel(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    resource_type: ResourceType15
-    package_name: str
-    path: str
-    original_file_path: str
-    unique_id: str
-    fqn: List[str]
-    model: str
-    node_relation: Optional[NodeRelation] = None
-    description: Optional[str] = None
-    defaults: Optional[Defaults] = None
-    entities: Optional[List[Entity]] = []
-    measures: Optional[List[Measure]] = []
-    dimensions: Optional[List[Dimension]] = []
-    metadata: Optional[SourceFileMetadata] = None
-    depends_on: Optional[DependsOn] = Field(
-        default_factory=lambda: DependsOn.parse_obj({'macros': [], 'nodes': []})
-    )
-    refs: Optional[List[RefArgs]] = []
-    created_at: Optional[float] = 1691439003.4182558
-    config: Optional[SemanticModelConfig] = Field(
-        default_factory=lambda: SemanticModelConfig.parse_obj({'enabled': True})
+class ManifestV9(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
     )
-    primary_entity: Optional[str] = None
-
-
-class ManifestV10(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
     metadata: ManifestMetadata = Field(..., description='Metadata about the manifest')
     nodes: Dict[
         str,
         Union[
             AnalysisNode,
             SingularTestNode,
             HookNode,
@@ -1642,24 +1411,20 @@
                     SqlNode,
                     GenericTestNode,
                     SnapshotNode,
                     SeedNode,
                     SourceDefinition,
                     Exposure,
                     Metric,
-                    SemanticModel,
                 ]
             ],
         ]
     ] = Field(None, description='A mapping of the disabled nodes in the target')
     parent_map: Optional[Dict[str, List[str]]] = Field(
         None, description='A mapping from\xa0child nodes to their dependencies'
     )
     child_map: Optional[Dict[str, List[str]]] = Field(
         None, description='A mapping from parent nodes to their dependents'
     )
     group_map: Optional[Dict[str, List[str]]] = Field(
         None, description='A mapping from group names to their nodes'
     )
-    semantic_models: Dict[str, SemanticModel] = Field(
-        ..., description='The semantic models defined in the dbt project'
-    )
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/manifest/manifest_v9.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/manifest/manifest_v3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1318 +1,1564 @@
 # generated by datamodel-codegen:
-#   filename:  manifest_v9.json
+#   filename:  manifest_v3.json
+
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra, Field, constr
+from pydantic import AwareDatetime, ConfigDict, Field, constr
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class ManifestMetadata(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     dbt_schema_version: Optional[
         str
-    ] = 'https://schemas.getdbt.com/dbt/manifest/v9.json'
-    dbt_version: Optional[str] = '1.5.0b5'
-    generated_at: Optional[datetime] = '2023-04-12T03:35:01.188035Z'
-    invocation_id: Optional[Optional[str]] = '8aa1596d-f52f-40bc-ad4b-f5e48fc7e6c2'
+    ] = 'https://schemas.getdbt.com/dbt/manifest/v3.json'
+    dbt_version: Optional[str] = '0.21.0rc1'
+    generated_at: Optional[AwareDatetime] = '2021-09-24T13:29:14.317700Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
-    project_id: Optional[Optional[str]] = Field(
+    project_id: Optional[str] = Field(
         None, description='A unique identifier for the project'
     )
     user_id: Optional[
-        Optional[
-            constr(
-                regex=r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
-            )
-        ]
+        constr(pattern=r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}')
     ] = Field(None, description='A unique identifier for the user')
-    send_anonymous_usage_stats: Optional[Optional[bool]] = Field(
+    send_anonymous_usage_stats: Optional[bool] = Field(
         None, description='Whether dbt is configured to send anonymous usage statistics'
     )
-    adapter_type: Optional[Optional[str]] = Field(
+    adapter_type: Optional[str] = Field(
         None, description='The type name of the adapter'
     )
 
 
 class ResourceType(Enum):
     analysis = 'analysis'
 
 
 class FileHash(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     checksum: str
 
 
 class Hook(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     sql: str
     transaction: Optional[bool] = True
-    index: Optional[Optional[int]] = None
-
-
-class Docs(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    show: Optional[bool] = True
-    node_color: Optional[Optional[str]] = None
-
-
-class ContractConfig(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    enforced: Optional[bool] = False
-
+    index: Optional[int] = None
 
-class Type(Enum):
-    check = 'check'
-    not_null = 'not_null'
-    unique = 'unique'
-    primary_key = 'primary_key'
-    foreign_key = 'foreign_key'
-    custom = 'custom'
-
-
-class ColumnLevelConstraint(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    type: Type
-    name: Optional[Optional[str]] = None
-    expression: Optional[Optional[str]] = None
-    warn_unenforced: Optional[bool] = True
-    warn_unsupported: Optional[bool] = True
 
+class DependsOn(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    macros: Optional[List[str]] = []
+    nodes: Optional[List[str]] = []
 
-class RefArgs(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
+class ColumnInfo(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
     name: str
-    package: Optional[Optional[str]] = None
-    version: Optional[Optional[Union[str, float]]] = None
-
+    description: Optional[str] = ''
+    meta: Optional[Dict[str, Any]] = {}
+    data_type: Optional[str] = None
+    quote: Optional[bool] = None
+    tags: Optional[List[str]] = []
 
-class DependsOn(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
-    macros: Optional[List[str]] = []
-    nodes: Optional[List[str]] = []
+class Docs(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    show: Optional[bool] = True
 
 
 class InjectedCTE(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     id: str
     sql: str
 
 
-class Contract(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    enforced: Optional[bool] = False
-    checksum: Optional[Optional[str]] = None
-
-
 class ResourceType1(Enum):
     test = 'test'
 
 
 class TestConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field('dbt_test__audit', alias='schema')
-    database: Optional[Optional[str]] = None
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field('dbt_test__audit', alias='schema')
+    database: Optional[str] = None
     tags: Optional[Union[List[str], str]] = []
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
     materialized: Optional[str] = 'test'
     severity: Optional[
-        constr(regex=r'^([Ww][Aa][Rr][Nn]|[Ee][Rr][Rr][Oo][Rr])$')
+        constr(pattern=r'^([Ww][Aa][Rr][Nn]|[Ee][Rr][Rr][Oo][Rr])$')
     ] = 'ERROR'
-    store_failures: Optional[Optional[bool]] = None
-    where: Optional[Optional[str]] = None
-    limit: Optional[Optional[int]] = None
+    store_failures: Optional[bool] = None
+    where: Optional[str] = None
+    limit: Optional[int] = None
     fail_calc: Optional[str] = 'count(*)'
     warn_if: Optional[str] = '!= 0'
     error_if: Optional[str] = '!= 0'
 
 
 class ResourceType2(Enum):
-    operation = 'operation'
-
-
-class ResourceType3(Enum):
     model = 'model'
 
 
-class Access(Enum):
-    protected = 'protected'
-    private = 'private'
-    public = 'public'
-
-
-class Type1(Enum):
-    check = 'check'
-    not_null = 'not_null'
-    unique = 'unique'
-    primary_key = 'primary_key'
-    foreign_key = 'foreign_key'
-    custom = 'custom'
-
-
-class ModelLevelConstraint(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    type: Type1
-    name: Optional[Optional[str]] = None
-    expression: Optional[Optional[str]] = None
-    warn_unenforced: Optional[bool] = True
-    warn_unsupported: Optional[bool] = True
-    columns: Optional[List[str]] = []
+class ResourceType3(Enum):
+    operation = 'operation'
 
 
 class ResourceType4(Enum):
     rpc = 'rpc'
 
 
 class ResourceType5(Enum):
-    sql_operation = 'sql operation'
-
-
-class ResourceType6(Enum):
     test = 'test'
 
 
 class TestMetadata(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
     kwargs: Optional[Dict[str, Any]] = {}
-    namespace: Optional[Optional[str]] = None
-
+    namespace: Optional[str] = None
 
-class ResourceType7(Enum):
-    snapshot = 'snapshot'
 
+class ResourceType6(Enum):
+    seed = 'seed'
 
-class SnapshotConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
 
+class SeedConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field(None, alias='schema')
+    database: Optional[str] = None
     tags: Optional[Union[List[str], str]] = []
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    materialized: Optional[str] = 'snapshot'
-    incremental_strategy: Optional[Optional[str]] = None
+    materialized: Optional[str] = 'seed'
     persist_docs: Optional[Dict[str, Any]] = {}
     post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
     pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
     quoting: Optional[Dict[str, Any]] = {}
     column_types: Optional[Dict[str, Any]] = {}
-    full_refresh: Optional[Optional[bool]] = None
-    unique_key: Optional[Optional[str]] = None
-    on_schema_change: Optional[Optional[str]] = 'ignore'
-    grants: Optional[Dict[str, Any]] = {}
-    packages: Optional[List[str]] = []
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    contract: Optional[ContractConfig] = {'enforced': False}
-    strategy: Optional[Optional[str]] = None
-    target_schema: Optional[Optional[str]] = None
-    target_database: Optional[Optional[str]] = None
-    updated_at: Optional[Optional[str]] = None
-    check_cols: Optional[Optional[Union[str, List[str]]]] = None
+    full_refresh: Optional[bool] = None
+    on_schema_change: Optional[str] = 'ignore'
+    quote_columns: Optional[bool] = None
+
+
+class ResourceType7(Enum):
+    snapshot = 'snapshot'
 
 
 class ResourceType8(Enum):
+    analysis = 'analysis'
+
+
+class ResourceType9(Enum):
+    test = 'test'
+
+
+class ParsedDataTestNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    fqn: List[str]
+    unique_id: str
+    package_name: str
+    root_path: str
+    path: str
+    original_file_path: str
+    name: str
+    resource_type: ResourceType9
+    alias: str
+    checksum: FileHash
+    config: Optional[TestConfig] = Field(
+        default_factory=lambda: TestConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': 'dbt_test__audit',
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'test',
+                'severity': 'ERROR',
+                'store_failures': None,
+                'where': None,
+                'limit': None,
+                'fail_calc': 'count(*)',
+                'warn_if': '!= 0',
+                'error_if': '!= 0',
+            }
+        )
+    )
+    tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = {}
+    meta: Optional[Dict[str, Any]] = {}
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = {}
+    created_at: Optional[int] = 1632490154
+    config_call_dict: Optional[Dict[str, Any]] = {}
+
+
+class ResourceType10(Enum):
+    operation = 'operation'
+
+
+class ResourceType11(Enum):
+    model = 'model'
+
+
+class ResourceType12(Enum):
+    rpc = 'rpc'
+
+
+class ResourceType13(Enum):
+    test = 'test'
+
+
+class ParsedSchemaTestNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    test_metadata: TestMetadata
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    fqn: List[str]
+    unique_id: str
+    package_name: str
+    root_path: str
+    path: str
+    original_file_path: str
+    name: str
+    resource_type: ResourceType13
+    alias: str
+    checksum: FileHash
+    config: Optional[TestConfig] = Field(
+        default_factory=lambda: TestConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': 'dbt_test__audit',
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'test',
+                'severity': 'ERROR',
+                'store_failures': None,
+                'where': None,
+                'limit': None,
+                'fail_calc': 'count(*)',
+                'warn_if': '!= 0',
+                'error_if': '!= 0',
+            }
+        )
+    )
+    tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = {}
+    meta: Optional[Dict[str, Any]] = {}
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = {}
+    created_at: Optional[int] = 1632490154
+    config_call_dict: Optional[Dict[str, Any]] = {}
+    column_name: Optional[str] = None
+
+
+class ResourceType14(Enum):
     seed = 'seed'
 
 
-class SeedConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
+class ParsedSeedNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    fqn: List[str]
+    unique_id: str
+    package_name: str
+    root_path: str
+    path: str
+    original_file_path: str
+    name: str
+    resource_type: ResourceType14
+    alias: str
+    checksum: FileHash
+    config: Optional[SeedConfig] = Field(
+        default_factory=lambda: SeedConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'seed',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'quote_columns': None,
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
+    tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = {}
+    meta: Optional[Dict[str, Any]] = {}
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = {}
+    created_at: Optional[int] = 1632490154
+    config_call_dict: Optional[Dict[str, Any]] = {}
+
+
+class ResourceType15(Enum):
+    snapshot = 'snapshot'
+
 
+class SnapshotConfig(BaseParserModel):
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field(None, alias='schema')
+    database: Optional[str] = None
     tags: Optional[Union[List[str], str]] = []
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    materialized: Optional[str] = 'seed'
-    incremental_strategy: Optional[Optional[str]] = None
+    materialized: Optional[str] = 'snapshot'
     persist_docs: Optional[Dict[str, Any]] = {}
     post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
     pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
     quoting: Optional[Dict[str, Any]] = {}
     column_types: Optional[Dict[str, Any]] = {}
-    full_refresh: Optional[Optional[bool]] = None
-    unique_key: Optional[Optional[Union[str, List[str]]]] = None
-    on_schema_change: Optional[Optional[str]] = 'ignore'
-    grants: Optional[Dict[str, Any]] = {}
-    packages: Optional[List[str]] = []
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    contract: Optional[ContractConfig] = {'enforced': False}
-    quote_columns: Optional[Optional[bool]] = None
-
-
-class MacroDependsOn(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    macros: Optional[List[str]] = []
+    full_refresh: Optional[bool] = None
+    on_schema_change: Optional[str] = 'ignore'
+    strategy: Optional[str] = None
+    unique_key: Optional[str] = None
+    target_schema: Optional[str] = None
+    target_database: Optional[str] = None
+    updated_at: Optional[str] = None
+    check_cols: Optional[Union[str, List[str]]] = None
 
 
-class ResourceType9(Enum):
+class ResourceType16(Enum):
     source = 'source'
 
 
 class Quoting(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[Optional[bool]] = None
-    schema_: Optional[Optional[bool]] = Field(None, alias='schema')
-    identifier: Optional[Optional[bool]] = None
-    column: Optional[Optional[bool]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    database: Optional[bool] = None
+    schema_: Optional[bool] = Field(None, alias='schema')
+    identifier: Optional[bool] = None
+    column: Optional[bool] = None
 
 
 class FreshnessMetadata(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    dbt_schema_version: Optional[str] = 'https://schemas.getdbt.com/dbt/sources/v3.json'
-    dbt_version: Optional[str] = '1.5.0b5'
-    generated_at: Optional[datetime] = '2023-04-12T03:35:01.185979Z'
-    invocation_id: Optional[Optional[str]] = '8aa1596d-f52f-40bc-ad4b-f5e48fc7e6c2'
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: Optional[str] = 'https://schemas.getdbt.com/dbt/sources/v2.json'
+    dbt_version: Optional[str] = '0.21.0rc1'
+    generated_at: Optional[AwareDatetime] = '2021-09-24T13:29:14.312598Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class Status(Enum):
     runtime_error = 'runtime error'
 
 
 class SourceFreshnessRuntimeError(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    error: Optional[Optional[Union[str, int]]] = None
+    error: Optional[Union[str, int]] = None
     status: Status
 
 
 class Status1(Enum):
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
     runtime_error = 'runtime error'
 
 
-class PeriodEnum(Enum):
+class Period(Enum):
     minute = 'minute'
     hour = 'hour'
     day = 'day'
 
 
 class Time(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    count: Optional[Optional[int]] = None
-    period: Optional[Optional[PeriodEnum]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    count: int
+    period: Period
 
 
 class TimingInfo(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    started_at: Optional[Optional[datetime]] = None
-    completed_at: Optional[Optional[datetime]] = None
+    started_at: Optional[AwareDatetime] = None
+    completed_at: Optional[AwareDatetime] = None
 
 
 class ExternalPartition(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     name: Optional[str] = ''
     description: Optional[str] = ''
     data_type: Optional[str] = ''
     meta: Optional[Dict[str, Any]] = {}
 
 
 class SourceConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
 
 
-class ResourceType10(Enum):
+class ResourceType17(Enum):
     macro = 'macro'
 
 
-class SupportedLanguage(Enum):
-    python = 'python'
-    sql = 'sql'
+class MacroDependsOn(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    macros: Optional[List[str]] = []
 
 
 class MacroArgument(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    type: Optional[Optional[str]] = None
+    type: Optional[str] = None
     description: Optional[str] = ''
 
 
-class ResourceType11(Enum):
-    doc = 'doc'
-
-
-class Documentation(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    resource_type: ResourceType11
+class ParsedDocumentation(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
+    name: str
     block_contents: str
 
 
-class ResourceType12(Enum):
-    exposure = 'exposure'
-
-
-class Type2(Enum):
+class Type(Enum):
     dashboard = 'dashboard'
     notebook = 'notebook'
     analysis = 'analysis'
     ml = 'ml'
     application = 'application'
 
 
-class MaturityEnum(Enum):
+class ResourceType18(Enum):
+    model = 'model'
+    analysis = 'analysis'
+    test = 'test'
+    snapshot = 'snapshot'
+    operation = 'operation'
+    seed = 'seed'
+    rpc = 'rpc'
+    docs = 'docs'
+    source = 'source'
+    macro = 'macro'
+    exposure = 'exposure'
+
+
+class Maturity(Enum):
     low = 'low'
     medium = 'medium'
     high = 'high'
 
 
-class Owner(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
-    email: Optional[Optional[str]] = None
-    name: Optional[Optional[str]] = None
-
-
-class ExposureConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
-    enabled: Optional[bool] = True
-
-
-class ResourceType13(Enum):
-    metric = 'metric'
-
-
-class MetricFilter(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    field: str
-    operator: str
-    value: str
-
-
-class PeriodEnum1(Enum):
-    day = 'day'
-    week = 'week'
-    month = 'month'
-    year = 'year'
-
-
-class MetricTime(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    count: Optional[Optional[int]] = None
-    period: Optional[Optional[PeriodEnum1]] = None
-
-
-class MetricConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
-    enabled: Optional[bool] = True
-    group: Optional[Optional[str]] = None
-
-
-class ResourceType14(Enum):
-    group = 'group'
-
-
-class Group(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    resource_type: ResourceType14
-    package_name: str
-    path: str
-    original_file_path: str
-    unique_id: str
-    owner: Owner
+class ExposureOwner(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    email: str
+    name: Optional[str] = None
 
 
 class NodeConfig(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
     enabled: Optional[bool] = True
-    alias: Optional[Optional[str]] = None
-    schema_: Optional[Optional[str]] = Field(None, alias='schema')
-    database: Optional[Optional[str]] = None
+    alias: Optional[str] = None
+    schema_: Optional[str] = Field(None, alias='schema')
+    database: Optional[str] = None
     tags: Optional[Union[List[str], str]] = []
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
     materialized: Optional[str] = 'view'
-    incremental_strategy: Optional[Optional[str]] = None
     persist_docs: Optional[Dict[str, Any]] = {}
     post_hook: Optional[List[Hook]] = Field([], alias='post-hook')
     pre_hook: Optional[List[Hook]] = Field([], alias='pre-hook')
     quoting: Optional[Dict[str, Any]] = {}
     column_types: Optional[Dict[str, Any]] = {}
-    full_refresh: Optional[Optional[bool]] = None
-    unique_key: Optional[Optional[Union[str, List[str]]]] = None
-    on_schema_change: Optional[Optional[str]] = 'ignore'
-    grants: Optional[Dict[str, Any]] = {}
-    packages: Optional[List[str]] = []
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    contract: Optional[ContractConfig] = {'enforced': False}
+    full_refresh: Optional[bool] = None
+    on_schema_change: Optional[str] = 'ignore'
 
 
-class ColumnInfo(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
+class CompiledDataTestNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    compiled: bool
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    fqn: List[str]
+    unique_id: str
+    package_name: str
+    root_path: str
+    path: str
+    original_file_path: str
     name: str
+    resource_type: ResourceType1
+    alias: str
+    checksum: FileHash
+    config: Optional[TestConfig] = Field(
+        default_factory=lambda: TestConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': 'dbt_test__audit',
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'test',
+                'severity': 'ERROR',
+                'store_failures': None,
+                'where': None,
+                'limit': None,
+                'fail_calc': 'count(*)',
+                'warn_if': '!= 0',
+                'error_if': '!= 0',
+            }
+        )
+    )
+    tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    data_type: Optional[Optional[str]] = None
-    constraints: Optional[List[ColumnLevelConstraint]] = []
-    quote: Optional[Optional[bool]] = None
-    tags: Optional[List[str]] = []
-
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = {}
+    created_at: Optional[int] = 1632490154
+    config_call_dict: Optional[Dict[str, Any]] = {}
+    compiled_sql: Optional[str] = None
+    extra_ctes_injected: Optional[bool] = False
+    extra_ctes: Optional[List[InjectedCTE]] = []
+    relation_name: Optional[str] = None
 
-class SingularTestNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
-    database: Optional[Optional[str]] = None
+class CompiledModelNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    compiled: bool
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    name: str
-    resource_type: ResourceType1
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
+    name: str
+    resource_type: ResourceType2
     alias: str
     checksum: FileHash
-    config: Optional[TestConfig] = {
-        'enabled': True,
-        'alias': None,
-        'schema': 'dbt_test__audit',
-        'database': None,
-        'tags': [],
-        'meta': {},
-        'group': None,
-        'materialized': 'test',
-        'severity': 'ERROR',
-        'store_failures': None,
-        'where': None,
-        'limit': None,
-        'fail_calc': 'count(*)',
-        'warn_if': '!= 0',
-        'error_if': '!= 0',
-    }
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.19095
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    language: Optional[str] = 'sql'
-    refs: Optional[List[RefArgs]] = []
-    sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    compiled_path: Optional[Optional[str]] = None
-    compiled: Optional[bool] = False
-    compiled_code: Optional[Optional[str]] = None
+    compiled_sql: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
-    contract: Optional[Contract] = {'enforced': False, 'checksum': None}
-
+    relation_name: Optional[str] = None
 
-class HookNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
-    database: Optional[Optional[str]] = None
+class CompiledHookNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    compiled: bool
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    name: str
-    resource_type: ResourceType2
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
+    name: str
+    resource_type: ResourceType3
     alias: str
     checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'meta': {},
-        'group': None,
-        'materialized': 'view',
-        'incremental_strategy': None,
-        'persist_docs': {},
-        'quoting': {},
-        'column_types': {},
-        'full_refresh': None,
-        'unique_key': None,
-        'on_schema_change': 'ignore',
-        'grants': {},
-        'packages': [],
-        'docs': {'show': True, 'node_color': None},
-        'contract': {'enforced': False},
-        'post-hook': [],
-        'pre-hook': [],
-    }
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.191555
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    language: Optional[str] = 'sql'
-    refs: Optional[List[RefArgs]] = []
-    sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    compiled_path: Optional[Optional[str]] = None
-    compiled: Optional[bool] = False
-    compiled_code: Optional[Optional[str]] = None
+    compiled_sql: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
-    contract: Optional[Contract] = {'enforced': False, 'checksum': None}
-    index: Optional[Optional[int]] = None
+    relation_name: Optional[str] = None
+    index: Optional[int] = None
 
 
-class ModelNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[Optional[str]] = None
+class CompiledRPCNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    compiled: bool
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    name: str
-    resource_type: ResourceType3
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
+    name: str
+    resource_type: ResourceType4
     alias: str
     checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'meta': {},
-        'group': None,
-        'materialized': 'view',
-        'incremental_strategy': None,
-        'persist_docs': {},
-        'quoting': {},
-        'column_types': {},
-        'full_refresh': None,
-        'unique_key': None,
-        'on_schema_change': 'ignore',
-        'grants': {},
-        'packages': [],
-        'docs': {'show': True, 'node_color': None},
-        'contract': {'enforced': False},
-        'post-hook': [],
-        'pre-hook': [],
-    }
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.192162
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    language: Optional[str] = 'sql'
-    refs: Optional[List[RefArgs]] = []
-    sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    compiled_path: Optional[Optional[str]] = None
-    compiled: Optional[bool] = False
-    compiled_code: Optional[Optional[str]] = None
+    compiled_sql: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
-    contract: Optional[Contract] = {'enforced': False, 'checksum': None}
-    access: Optional[Access] = 'protected'
-    constraints: Optional[List[ModelLevelConstraint]] = []
-    version: Optional[Optional[Union[str, float]]] = None
-    latest_version: Optional[Optional[Union[str, float]]] = None
+    relation_name: Optional[str] = None
 
 
-class RPCNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[Optional[str]] = None
+class CompiledSchemaTestNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    test_metadata: TestMetadata
+    compiled: bool
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    name: str
-    resource_type: ResourceType4
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
+    name: str
+    resource_type: ResourceType5
     alias: str
     checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'meta': {},
-        'group': None,
-        'materialized': 'view',
-        'incremental_strategy': None,
-        'persist_docs': {},
-        'quoting': {},
-        'column_types': {},
-        'full_refresh': None,
-        'unique_key': None,
-        'on_schema_change': 'ignore',
-        'grants': {},
-        'packages': [],
-        'docs': {'show': True, 'node_color': None},
-        'contract': {'enforced': False},
-        'post-hook': [],
-        'pre-hook': [],
-    }
+    config: Optional[TestConfig] = Field(
+        default_factory=lambda: TestConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': 'dbt_test__audit',
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'test',
+                'severity': 'ERROR',
+                'store_failures': None,
+                'where': None,
+                'limit': None,
+                'fail_calc': 'count(*)',
+                'warn_if': '!= 0',
+                'error_if': '!= 0',
+            }
+        )
+    )
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.192949
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    language: Optional[str] = 'sql'
-    refs: Optional[List[RefArgs]] = []
-    sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    compiled_path: Optional[Optional[str]] = None
-    compiled: Optional[bool] = False
-    compiled_code: Optional[Optional[str]] = None
+    compiled_sql: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
-    contract: Optional[Contract] = {'enforced': False, 'checksum': None}
+    relation_name: Optional[str] = None
+    column_name: Optional[str] = None
 
 
-class SqlNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[Optional[str]] = None
+class CompiledSeedNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    compiled: bool
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    name: str
-    resource_type: ResourceType5
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
+    name: str
+    resource_type: ResourceType6
     alias: str
     checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'meta': {},
-        'group': None,
-        'materialized': 'view',
-        'incremental_strategy': None,
-        'persist_docs': {},
-        'quoting': {},
-        'column_types': {},
-        'full_refresh': None,
-        'unique_key': None,
-        'on_schema_change': 'ignore',
-        'grants': {},
-        'packages': [],
-        'docs': {'show': True, 'node_color': None},
-        'contract': {'enforced': False},
-        'post-hook': [],
-        'pre-hook': [],
-    }
+    config: Optional[SeedConfig] = Field(
+        default_factory=lambda: SeedConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'seed',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'quote_columns': None,
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.1935291
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    language: Optional[str] = 'sql'
-    refs: Optional[List[RefArgs]] = []
-    sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    compiled_path: Optional[Optional[str]] = None
-    compiled: Optional[bool] = False
-    compiled_code: Optional[Optional[str]] = None
+    compiled_sql: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
-    contract: Optional[Contract] = {'enforced': False, 'checksum': None}
+    relation_name: Optional[str] = None
 
 
-class GenericTestNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    test_metadata: TestMetadata
-    database: Optional[Optional[str]] = None
+class CompiledSnapshotNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    compiled: bool
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    name: str
-    resource_type: ResourceType6
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
+    name: str
+    resource_type: ResourceType7
     alias: str
     checksum: FileHash
-    config: Optional[TestConfig] = {
-        'enabled': True,
-        'alias': None,
-        'schema': 'dbt_test__audit',
-        'database': None,
-        'tags': [],
-        'meta': {},
-        'group': None,
-        'materialized': 'test',
-        'severity': 'ERROR',
-        'store_failures': None,
-        'where': None,
-        'limit': None,
-        'fail_calc': 'count(*)',
-        'warn_if': '!= 0',
-        'error_if': '!= 0',
-    }
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.19419
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    language: Optional[str] = 'sql'
-    refs: Optional[List[RefArgs]] = []
-    sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    compiled_path: Optional[Optional[str]] = None
-    compiled: Optional[bool] = False
-    compiled_code: Optional[Optional[str]] = None
+    compiled_sql: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
-    contract: Optional[Contract] = {'enforced': False, 'checksum': None}
-    column_name: Optional[Optional[str]] = None
-    file_key_name: Optional[Optional[str]] = None
-    attached_node: Optional[Optional[str]] = None
+    relation_name: Optional[str] = None
 
 
-class SnapshotNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[Optional[str]] = None
+class ParsedAnalysisNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    name: str
-    resource_type: ResourceType7
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
+    name: str
+    resource_type: ResourceType8
     alias: str
     checksum: FileHash
-    config: SnapshotConfig
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.1952698
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    language: Optional[str] = 'sql'
-    refs: Optional[List[RefArgs]] = []
-    sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    compiled_path: Optional[Optional[str]] = None
-    compiled: Optional[bool] = False
-    compiled_code: Optional[Optional[str]] = None
-    extra_ctes_injected: Optional[bool] = False
-    extra_ctes: Optional[List[InjectedCTE]] = []
-    contract: Optional[Contract] = {'enforced': False, 'checksum': None}
-
 
-class SeedNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
-    database: Optional[Optional[str]] = None
+class ParsedHookNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
+    fqn: List[str]
+    unique_id: str
+    package_name: str
+    root_path: str
+    path: str
+    original_file_path: str
     name: str
-    resource_type: ResourceType8
+    resource_type: ResourceType10
+    alias: str
+    checksum: FileHash
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
+    tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = {}
+    meta: Optional[Dict[str, Any]] = {}
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = {}
+    created_at: Optional[int] = 1632490154
+    config_call_dict: Optional[Dict[str, Any]] = {}
+    index: Optional[int] = None
+
+
+class ParsedModelNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
+    name: str
+    resource_type: ResourceType11
+    alias: str
+    checksum: FileHash
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
+    tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = {}
+    meta: Optional[Dict[str, Any]] = {}
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = {}
+    created_at: Optional[int] = 1632490154
+    config_call_dict: Optional[Dict[str, Any]] = {}
+
+
+class ParsedRPCNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    fqn: List[str]
     unique_id: str
+    package_name: str
+    root_path: str
+    path: str
+    original_file_path: str
+    name: str
+    resource_type: ResourceType12
+    alias: str
+    checksum: FileHash
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
+    tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
+    description: Optional[str] = ''
+    columns: Optional[Dict[str, ColumnInfo]] = {}
+    meta: Optional[Dict[str, Any]] = {}
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
+    deferred: Optional[bool] = False
+    unrendered_config: Optional[Dict[str, Any]] = {}
+    created_at: Optional[int] = 1632490154
+    config_call_dict: Optional[Dict[str, Any]] = {}
+
+
+class ParsedSnapshotNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
     fqn: List[str]
+    unique_id: str
+    package_name: str
+    root_path: str
+    path: str
+    original_file_path: str
+    name: str
+    resource_type: ResourceType15
     alias: str
     checksum: FileHash
-    config: Optional[SeedConfig] = {
-        'enabled': True,
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'meta': {},
-        'group': None,
-        'materialized': 'seed',
-        'incremental_strategy': None,
-        'persist_docs': {},
-        'quoting': {},
-        'column_types': {},
-        'full_refresh': None,
-        'unique_key': None,
-        'on_schema_change': 'ignore',
-        'grants': {},
-        'packages': [],
-        'docs': {'show': True, 'node_color': None},
-        'contract': {'enforced': False},
-        'quote_columns': None,
-        'post-hook': [],
-        'pre-hook': [],
-    }
+    config: SnapshotConfig
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.1968079
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    root_path: Optional[Optional[str]] = None
-    depends_on: Optional[MacroDependsOn] = {'macros': []}
 
 
 class FreshnessThreshold(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    warn_after: Optional[Optional[Time]] = {'count': None, 'period': None}
-    error_after: Optional[Optional[Time]] = {'count': None, 'period': None}
-    filter: Optional[Optional[str]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    warn_after: Optional[Time] = None
+    error_after: Optional[Time] = None
+    filter: Optional[str] = None
 
 
 class SourceFreshnessOutput(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    max_loaded_at: datetime
-    snapshotted_at: datetime
+    max_loaded_at: AwareDatetime
+    snapshotted_at: AwareDatetime
     max_loaded_at_time_ago_in_s: float
     status: Status1
     criteria: FreshnessThreshold
     adapter_response: Dict[str, Any]
     timing: List[TimingInfo]
     thread_id: str
     execution_time: float
 
 
 class ExternalTable(BaseParserModel):
-    class Config:
-        extra = Extra.allow
-
-    location: Optional[Optional[str]] = None
-    file_format: Optional[Optional[str]] = None
-    row_format: Optional[Optional[str]] = None
-    tbl_properties: Optional[Optional[str]] = None
-    partitions: Optional[Optional[Union[List[str], List[ExternalPartition]]]] = None
-
+    model_config = ConfigDict(
+        extra='allow',
+    )
+    location: Optional[str] = None
+    file_format: Optional[str] = None
+    row_format: Optional[str] = None
+    tbl_properties: Optional[str] = None
+    partitions: Optional[List[ExternalPartition]] = None
 
-class Macro(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
-    name: str
-    resource_type: ResourceType10
+class ParsedMacro(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
+    name: str
     macro_sql: str
-    depends_on: Optional[MacroDependsOn] = {'macros': []}
+    resource_type: ResourceType17
+    tags: Optional[List[str]] = []
+    depends_on: Optional[MacroDependsOn] = Field(
+        default_factory=lambda: MacroDependsOn.model_validate({'macros': []})
+    )
     description: Optional[str] = ''
     meta: Optional[Dict[str, Any]] = {}
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
     arguments: Optional[List[MacroArgument]] = []
-    created_at: Optional[float] = 1681270501.198105
-    supported_languages: Optional[Optional[List[SupportedLanguage]]] = None
-
+    created_at: Optional[int] = 1632490154
 
-class Exposure(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
-    name: str
-    resource_type: ResourceType12
+class ParsedExposure(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
-    type: Type2
-    owner: Owner
+    name: str
+    type: Type
+    owner: ExposureOwner
+    resource_type: Optional[ResourceType18] = 'exposure'
     description: Optional[str] = ''
-    label: Optional[Optional[str]] = None
-    maturity: Optional[Optional[MaturityEnum]] = None
+    maturity: Optional[Maturity] = None
     meta: Optional[Dict[str, Any]] = {}
     tags: Optional[List[str]] = []
-    config: Optional[ExposureConfig] = {'enabled': True}
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    url: Optional[Optional[str]] = None
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    refs: Optional[List[RefArgs]] = []
+    url: Optional[str] = None
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
+    refs: Optional[List[List[str]]] = []
     sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    created_at: Optional[float] = 1681270501.198782
-
+    created_at: Optional[int] = 1632490154
 
-class Metric(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
-    name: str
-    resource_type: ResourceType13
+class CompiledAnalysisNode(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    raw_sql: str
+    compiled: bool
+    database: Optional[str] = None
+    schema_: str = Field(..., alias='schema')
+    fqn: List[str]
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
-    description: str
-    label: str
-    calculation_method: str
-    expression: str
-    filters: List[MetricFilter]
-    time_grains: List[str]
-    dimensions: List[str]
-    timestamp: Optional[Optional[str]] = None
-    window: Optional[Optional[MetricTime]] = None
-    model: Optional[Optional[str]] = None
-    model_unique_id: Optional[Optional[str]] = None
-    meta: Optional[Dict[str, Any]] = {}
-    tags: Optional[List[str]] = []
-    config: Optional[MetricConfig] = {'enabled': True, 'group': None}
-    unrendered_config: Optional[Dict[str, Any]] = {}
-    sources: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    refs: Optional[List[RefArgs]] = []
-    metrics: Optional[List[List[str]]] = []
-    created_at: Optional[float] = 1681270501.199492
-    group: Optional[Optional[str]] = None
-
-
-class AnalysisNode(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[Optional[str]] = None
-    schema_: str = Field(..., alias='schema')
     name: str
     resource_type: ResourceType
-    package_name: str
-    path: str
-    original_file_path: str
-    unique_id: str
-    fqn: List[str]
     alias: str
     checksum: FileHash
-    config: Optional[NodeConfig] = {
-        'enabled': True,
-        'alias': None,
-        'schema': None,
-        'database': None,
-        'tags': [],
-        'meta': {},
-        'group': None,
-        'materialized': 'view',
-        'incremental_strategy': None,
-        'persist_docs': {},
-        'quoting': {},
-        'column_types': {},
-        'full_refresh': None,
-        'unique_key': None,
-        'on_schema_change': 'ignore',
-        'grants': {},
-        'packages': [],
-        'docs': {'show': True, 'node_color': None},
-        'contract': {'enforced': False},
-        'post-hook': [],
-        'pre-hook': [],
-    }
+    config: Optional[NodeConfig] = Field(
+        default_factory=lambda: NodeConfig.model_validate(
+            {
+                'enabled': True,
+                'alias': None,
+                'schema': None,
+                'database': None,
+                'tags': [],
+                'meta': {},
+                'materialized': 'view',
+                'persist_docs': {},
+                'quoting': {},
+                'column_types': {},
+                'full_refresh': None,
+                'on_schema_change': 'ignore',
+                'post-hook': [],
+                'pre-hook': [],
+            }
+        )
+    )
     tags: Optional[List[str]] = []
+    refs: Optional[List[List[str]]] = []
+    sources: Optional[List[List]] = []
+    depends_on: Optional[DependsOn] = Field(
+        default_factory=lambda: DependsOn.model_validate({'macros': [], 'nodes': []})
+    )
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
-    group: Optional[Optional[str]] = None
-    docs: Optional[Docs] = {'show': True, 'node_color': None}
-    patch_path: Optional[Optional[str]] = None
-    build_path: Optional[Optional[str]] = None
+    docs: Optional[Docs] = Field(
+        default_factory=lambda: Docs.model_validate({'show': True})
+    )
+    patch_path: Optional[str] = None
+    compiled_path: Optional[str] = None
+    build_path: Optional[str] = None
     deferred: Optional[bool] = False
     unrendered_config: Optional[Dict[str, Any]] = {}
-    created_at: Optional[float] = 1681270501.189703
+    created_at: Optional[int] = 1632490154
     config_call_dict: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    raw_code: Optional[str] = ''
-    language: Optional[str] = 'sql'
-    refs: Optional[List[RefArgs]] = []
-    sources: Optional[List[List[str]]] = []
-    metrics: Optional[List[List[str]]] = []
-    depends_on: Optional[DependsOn] = {'macros': [], 'nodes': []}
-    compiled_path: Optional[Optional[str]] = None
-    compiled: Optional[bool] = False
-    compiled_code: Optional[Optional[str]] = None
+    compiled_sql: Optional[str] = None
     extra_ctes_injected: Optional[bool] = False
     extra_ctes: Optional[List[InjectedCTE]] = []
-    contract: Optional[Contract] = {'enforced': False, 'checksum': None}
+    relation_name: Optional[str] = None
 
 
-class SourceDefinition(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    database: Optional[Optional[str]] = None
+class ParsedSourceDefinition(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    fqn: List[str]
+    database: Optional[str] = None
     schema_: str = Field(..., alias='schema')
-    name: str
-    resource_type: ResourceType9
+    unique_id: str
     package_name: str
+    root_path: str
     path: str
     original_file_path: str
-    unique_id: str
-    fqn: List[str]
+    name: str
     source_name: str
     source_description: str
     loader: str
     identifier: str
-    quoting: Optional[Quoting] = {
-        'database': None,
-        'schema': None,
-        'identifier': None,
-        'column': None,
-    }
-    loaded_at_field: Optional[Optional[str]] = None
-    freshness: Optional[Optional[FreshnessThreshold]] = None
-    external: Optional[Optional[ExternalTable]] = None
+    resource_type: ResourceType16
+    quoting: Optional[Quoting] = Field(
+        default_factory=lambda: Quoting.model_validate(
+            {'database': None, 'schema': None, 'identifier': None, 'column': None}
+        )
+    )
+    loaded_at_field: Optional[str] = None
+    freshness: Optional[FreshnessThreshold] = None
+    external: Optional[ExternalTable] = None
     description: Optional[str] = ''
     columns: Optional[Dict[str, ColumnInfo]] = {}
     meta: Optional[Dict[str, Any]] = {}
     source_meta: Optional[Dict[str, Any]] = {}
     tags: Optional[List[str]] = []
-    config: Optional[SourceConfig] = {'enabled': True}
-    patch_path: Optional[Optional[str]] = None
+    config: Optional[SourceConfig] = Field(
+        default_factory=lambda: SourceConfig.model_validate({'enabled': True})
+    )
+    patch_path: Optional[str] = None
     unrendered_config: Optional[Dict[str, Any]] = {}
-    relation_name: Optional[Optional[str]] = None
-    created_at: Optional[float] = 1681270501.197819
-
+    relation_name: Optional[str] = None
+    created_at: Optional[int] = 1632490154
 
-class ManifestV9(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
+class ManifestV3(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: ManifestMetadata = Field(..., description='Metadata about the manifest')
     nodes: Dict[
         str,
         Union[
-            AnalysisNode,
-            SingularTestNode,
-            HookNode,
-            ModelNode,
-            RPCNode,
-            SqlNode,
-            GenericTestNode,
-            SnapshotNode,
-            SeedNode,
+            CompiledAnalysisNode,
+            CompiledDataTestNode,
+            CompiledModelNode,
+            CompiledHookNode,
+            CompiledRPCNode,
+            CompiledSchemaTestNode,
+            CompiledSeedNode,
+            CompiledSnapshotNode,
+            ParsedAnalysisNode,
+            ParsedDataTestNode,
+            ParsedHookNode,
+            ParsedModelNode,
+            ParsedRPCNode,
+            ParsedSchemaTestNode,
+            ParsedSeedNode,
+            ParsedSnapshotNode,
         ],
     ] = Field(
         ..., description='The nodes defined in the dbt project and its dependencies'
     )
-    sources: Dict[str, SourceDefinition] = Field(
+    sources: Dict[str, ParsedSourceDefinition] = Field(
         ..., description='The sources defined in the dbt project and its dependencies'
     )
-    macros: Dict[str, Macro] = Field(
+    macros: Dict[str, ParsedMacro] = Field(
         ..., description='The macros defined in the dbt project and its dependencies'
     )
-    docs: Dict[str, Documentation] = Field(
+    docs: Dict[str, ParsedDocumentation] = Field(
         ..., description='The docs defined in the dbt project and its dependencies'
     )
-    exposures: Dict[str, Exposure] = Field(
+    exposures: Dict[str, ParsedExposure] = Field(
         ..., description='The exposures defined in the dbt project and its dependencies'
     )
-    metrics: Dict[str, Metric] = Field(
-        ..., description='The metrics defined in the dbt project and its dependencies'
-    )
-    groups: Dict[str, Group] = Field(
-        ..., description='The groups defined in the dbt project'
-    )
     selectors: Dict[str, Any] = Field(
         ..., description='The selectors defined in selectors.yml'
     )
     disabled: Optional[
-        Optional[
-            Dict[
-                str,
-                List[
-                    Union[
-                        AnalysisNode,
-                        SingularTestNode,
-                        HookNode,
-                        ModelNode,
-                        RPCNode,
-                        SqlNode,
-                        GenericTestNode,
-                        SnapshotNode,
-                        SeedNode,
-                        SourceDefinition,
-                        Exposure,
-                        Metric,
-                    ]
-                ],
+        List[
+            Union[
+                CompiledAnalysisNode,
+                CompiledDataTestNode,
+                CompiledModelNode,
+                CompiledHookNode,
+                CompiledRPCNode,
+                CompiledSchemaTestNode,
+                CompiledSeedNode,
+                CompiledSnapshotNode,
+                ParsedAnalysisNode,
+                ParsedDataTestNode,
+                ParsedHookNode,
+                ParsedModelNode,
+                ParsedRPCNode,
+                ParsedSchemaTestNode,
+                ParsedSeedNode,
+                ParsedSnapshotNode,
+                ParsedSourceDefinition,
             ]
         ]
-    ] = Field(None, description='A mapping of the disabled nodes in the target')
-    parent_map: Optional[Optional[Dict[str, List[str]]]] = Field(
+    ] = Field(None, description='A list of the disabled nodes in the target')
+    parent_map: Optional[Dict[str, List[str]]] = Field(
         None, description='A mapping from\xa0child nodes to their dependencies'
     )
-    child_map: Optional[Optional[Dict[str, List[str]]]] = Field(
+    child_map: Optional[Dict[str, List[str]]] = Field(
         None, description='A mapping from parent nodes to their dependents'
     )
-    group_map: Optional[Optional[Dict[str, List[str]]]] = Field(
-        None, description='A mapping from group names to their nodes'
-    )
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/__init__.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v5.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,84 @@
 # generated by datamodel-codegen:
-#   filename:  run-results_v1.json
-#   timestamp: 2022-03-01T06:21:36+00:00
+#   filename:  run-results_v5.json
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra
+from pydantic import ConfigDict
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class BaseArtifactMetadata(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: str
+    dbt_version: Optional[str] = '1.7.0b1'
+    generated_at: Optional[str] = None
+    invocation_id: Optional[str] = None
+    env: Optional[Dict[str, str]] = None
 
-    class Config:
-        extra = Extra.forbid
 
-    dbt_schema_version: str
-    dbt_version: Optional[str] = '0.19.0'
-    generated_at: Optional[datetime] = '2021-02-10T04:42:33.678063Z'
-    invocation_id: Optional[Optional[str]] = None
-    env: Optional[Dict[str, str]] = {}
+class TimingInfo(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    name: str
+    started_at: Optional[str] = None
+    completed_at: Optional[str] = None
 
 
 class Status(Enum):
     success = 'success'
     error = 'error'
     skipped = 'skipped'
 
 
 class Status1(Enum):
     pass_ = 'pass'
     error = 'error'
     fail = 'fail'
     warn = 'warn'
+    skipped = 'skipped'
 
 
 class Status2(Enum):
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
     runtime_error = 'runtime error'
 
 
-class TimingInfo(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    name: str
-    started_at: Optional[Optional[datetime]] = None
-    completed_at: Optional[Optional[datetime]] = None
-
-
 class RunResultOutput(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     status: Union[Status, Status1, Status2]
     timing: List[TimingInfo]
     thread_id: str
     execution_time: float
-    message: Optional[Optional[Union[str, int]]] = None
     adapter_response: Dict[str, Any]
+    message: Optional[str] = None
+    failures: Optional[int] = None
     unique_id: str
+    compiled: Optional[bool] = None
+    compiled_code: Optional[str] = None
+    relation_name: Optional[str] = None
 
 
-class RunResultsV1(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+class RunResultsV5(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: BaseArtifactMetadata
     results: List[RunResultOutput]
     elapsed_time: float
-    args: Optional[Dict[str, Any]] = {}
+    args: Optional[Dict[str, Any]] = None
+
+
+# NOTE: We manually change the class, as the generated code is not correct.
+# class RunResultsV5(RootModel[RunResultsArtifact]):
+#     root: RunResultsArtifact
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # generated by datamodel-codegen:
 #   filename:  run-results_v2.json
-#   timestamp: 2022-03-01T06:21:36+00:00
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra
+from pydantic import AwareDatetime, ConfigDict
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class BaseArtifactMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     dbt_schema_version: str
     dbt_version: Optional[str] = '0.20.0rc1'
-    generated_at: Optional[datetime] = '2021-06-07T14:49:01.097134Z'
-    invocation_id: Optional[Optional[str]] = None
+    generated_at: Optional[AwareDatetime] = '2021-06-07T14:49:01.097134Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class Status(Enum):
     success = 'success'
     error = 'error'
     skipped = 'skipped'
@@ -42,40 +39,37 @@
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
     runtime_error = 'runtime error'
 
 
 class TimingInfo(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    started_at: Optional[Optional[datetime]] = None
-    completed_at: Optional[Optional[datetime]] = None
+    started_at: Optional[AwareDatetime] = None
+    completed_at: Optional[AwareDatetime] = None
 
 
 class RunResultOutput(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     status: Union[Status, Status1, Status2]
     timing: List[TimingInfo]
     thread_id: str
     execution_time: float
     adapter_response: Dict[str, Any]
-    message: Optional[Optional[str]] = None
-    failures: Optional[Optional[int]] = None
+    message: Optional[str] = None
+    failures: Optional[int] = None
     unique_id: str
 
 
 class RunResultsV2(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: BaseArtifactMetadata
     results: List[RunResultOutput]
     elapsed_time: float
     args: Optional[Dict[str, Any]] = {}
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # generated by datamodel-codegen:
-#   filename:  run-results_v3.json
-#   timestamp: 2022-03-01T06:21:37+00:00
+#   filename:  run-results_v4.json
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra
+from pydantic import AwareDatetime, ConfigDict
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class BaseArtifactMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     dbt_schema_version: str
-    dbt_version: Optional[str] = '0.21.0rc1'
-    generated_at: Optional[datetime] = '2021-09-24T13:29:14.315088Z'
-    invocation_id: Optional[Optional[str]] = None
+    dbt_version: Optional[str] = '1.0.0b2'
+    generated_at: Optional[AwareDatetime] = '2021-11-02T20:18:06.799863Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class Status(Enum):
     success = 'success'
     error = 'error'
     skipped = 'skipped'
@@ -43,47 +40,43 @@
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
     runtime_error = 'runtime error'
 
 
 class TimingInfo(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    started_at: Optional[Optional[datetime]] = None
-    completed_at: Optional[Optional[datetime]] = None
+    started_at: Optional[AwareDatetime] = None
+    completed_at: Optional[AwareDatetime] = None
 
 
 class FreshnessMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    dbt_schema_version: Optional[
-        str] = 'https://schemas.getdbt.com/dbt/sources/v2.json'
-    dbt_version: Optional[str] = '0.21.0rc1'
-    generated_at: Optional[datetime] = '2021-09-24T13:29:14.312598Z'
-    invocation_id: Optional[Optional[str]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: Optional[str] = 'https://schemas.getdbt.com/dbt/sources/v3.json'
+    dbt_version: Optional[str] = '1.0.0b2'
+    generated_at: Optional[AwareDatetime] = '2021-11-02T20:18:06.796684Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class Status3(Enum):
     runtime_error = 'runtime error'
 
 
 class SourceFreshnessRuntimeError(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    error: Optional[Optional[Union[str, int]]] = None
+    error: Optional[Union[str, int]] = None
     status: Status3
 
 
 class Status4(Enum):
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
@@ -93,66 +86,61 @@
 class Period(Enum):
     minute = 'minute'
     hour = 'hour'
     day = 'day'
 
 
 class Time(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    count: int
-    period: Period
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    count: Optional[int] = None
+    period: Optional[Period] = None
 
 
 class RunResultOutput(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     status: Union[Status, Status1, Status2]
     timing: List[TimingInfo]
     thread_id: str
     execution_time: float
     adapter_response: Dict[str, Any]
-    message: Optional[Optional[str]] = None
-    failures: Optional[Optional[int]] = None
+    message: Optional[str] = None
+    failures: Optional[int] = None
     unique_id: str
 
 
 class FreshnessThreshold(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    warn_after: Optional[Optional[Time]] = None
-    error_after: Optional[Optional[Time]] = None
-    filter: Optional[Optional[str]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    warn_after: Optional[Time] = {'count': None, 'period': None}
+    error_after: Optional[Time] = {'count': None, 'period': None}
+    filter: Optional[str] = None
 
 
-class RunResultsV3(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+class RunResultsV4(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: BaseArtifactMetadata
     results: List[RunResultOutput]
     elapsed_time: float
     args: Optional[Dict[str, Any]] = {}
 
 
 class SourceFreshnessOutput(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    max_loaded_at: datetime
-    snapshotted_at: datetime
+    max_loaded_at: AwareDatetime
+    snapshotted_at: AwareDatetime
     max_loaded_at_time_ago_in_s: float
     status: Status4
     criteria: FreshnessThreshold
     adapter_response: Dict[str, Any]
     timing: List[TimingInfo]
     thread_id: str
     execution_time: float
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v4.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # generated by datamodel-codegen:
-#   filename:  run-results_v4.json
-#   timestamp: 2022-03-01T06:21:37+00:00
+#   filename:  run-results_v3.json
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra
+from pydantic import AwareDatetime, ConfigDict
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class BaseArtifactMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     dbt_schema_version: str
-    dbt_version: Optional[str] = '1.0.0b2'
-    generated_at: Optional[datetime] = '2021-11-02T20:18:06.799863Z'
-    invocation_id: Optional[Optional[str]] = None
+    dbt_version: Optional[str] = '0.21.0rc1'
+    generated_at: Optional[AwareDatetime] = '2021-09-24T13:29:14.315088Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class Status(Enum):
     success = 'success'
     error = 'error'
     skipped = 'skipped'
@@ -43,116 +40,107 @@
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
     runtime_error = 'runtime error'
 
 
 class TimingInfo(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    started_at: Optional[Optional[datetime]] = None
-    completed_at: Optional[Optional[datetime]] = None
+    started_at: Optional[AwareDatetime] = None
+    completed_at: Optional[AwareDatetime] = None
 
 
 class FreshnessMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    dbt_schema_version: Optional[
-        str] = 'https://schemas.getdbt.com/dbt/sources/v3.json'
-    dbt_version: Optional[str] = '1.0.0b2'
-    generated_at: Optional[datetime] = '2021-11-02T20:18:06.796684Z'
-    invocation_id: Optional[Optional[str]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: Optional[str] = 'https://schemas.getdbt.com/dbt/sources/v2.json'
+    dbt_version: Optional[str] = '0.21.0rc1'
+    generated_at: Optional[AwareDatetime] = '2021-09-24T13:29:14.312598Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class Status3(Enum):
     runtime_error = 'runtime error'
 
 
 class SourceFreshnessRuntimeError(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    error: Optional[Optional[Union[str, int]]] = None
+    error: Optional[Union[str, int]] = None
     status: Status3
 
 
 class Status4(Enum):
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
     runtime_error = 'runtime error'
 
 
-class PeriodEnum(Enum):
+class Period(Enum):
     minute = 'minute'
     hour = 'hour'
     day = 'day'
 
 
 class Time(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    count: Optional[Optional[int]] = None
-    period: Optional[Optional[PeriodEnum]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    count: int
+    period: Period
 
 
 class RunResultOutput(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     status: Union[Status, Status1, Status2]
     timing: List[TimingInfo]
     thread_id: str
     execution_time: float
     adapter_response: Dict[str, Any]
-    message: Optional[Optional[str]] = None
-    failures: Optional[Optional[int]] = None
+    message: Optional[str] = None
+    failures: Optional[int] = None
     unique_id: str
 
 
 class FreshnessThreshold(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    warn_after: Optional[Optional[Time]] = {'count': None, 'period': None}
-    error_after: Optional[Optional[Time]] = {'count': None, 'period': None}
-    filter: Optional[Optional[str]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    warn_after: Optional[Time] = None
+    error_after: Optional[Time] = None
+    filter: Optional[str] = None
 
 
-class RunResultsV4(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+class RunResultsV3(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: BaseArtifactMetadata
     results: List[RunResultOutput]
     elapsed_time: float
     args: Optional[Dict[str, Any]] = {}
 
 
 class SourceFreshnessOutput(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    max_loaded_at: datetime
-    snapshotted_at: datetime
+    max_loaded_at: AwareDatetime
+    snapshotted_at: AwareDatetime
     max_loaded_at_time_ago_in_s: float
     status: Status4
     criteria: FreshnessThreshold
     adapter_response: Dict[str, Any]
     timing: List[TimingInfo]
     thread_id: str
     execution_time: float
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v5.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v6.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 # generated by datamodel-codegen:
-#   filename:  run-results_v5.json
+#   filename:  run-results_v6.json
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra
+from pydantic import ConfigDict, Field
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
-class BaseArtifactMetadata(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+class Metadata(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     dbt_schema_version: str
-    dbt_version: Optional[str] = '1.7.0b1'
+    dbt_version: Optional[str] = '1.8.0a1'
     generated_at: Optional[str] = None
-    invocation_id: Optional[Optional[str]] = None
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = None
 
 
-class StatusEnum(Enum):
+class Status(Enum):
     success = 'success'
     error = 'error'
     skipped = 'skipped'
 
 
-class StatusEnum1(Enum):
+class Status1(Enum):
     pass_ = 'pass'
     error = 'error'
     fail = 'fail'
     warn = 'warn'
     skipped = 'skipped'
 
 
-class StatusEnum2(Enum):
+class Status2(Enum):
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
     runtime_error = 'runtime error'
 
 
-class TimingInfo(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+class TimingItem(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    started_at: Optional[Optional[str]] = None
-    completed_at: Optional[Optional[str]] = None
+    started_at: Optional[str] = None
+    completed_at: Optional[str] = None
 
 
-class RunResultOutput(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    status: Union[StatusEnum, StatusEnum1, StatusEnum2]
-    timing: List[TimingInfo]
+class Result(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    status: Union[Status, Status1, Status2]
+    timing: List[TimingItem]
     thread_id: str
     execution_time: float
     adapter_response: Dict[str, Any]
-    message: Optional[str]
-    failures: Optional[int]
+    message: Optional[str] = None
+    failures: Optional[int] = None
     unique_id: str
-    compiled: Optional[bool]
-    compiled_code: Optional[str]
-    relation_name: Optional[str]
-
-# NOTE Manually replaced the class, as datamodel-code-generator didn't work as expected.
-class RunResultsV5(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
+    compiled: Optional[bool] = None
+    compiled_code: Optional[str] = None
+    relation_name: Optional[str] = None
+
 
-    metadata: BaseArtifactMetadata
-    results: List[RunResultOutput]
+class RunResultsV6(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    metadata: Metadata = Field(..., title='BaseArtifactMetadata')
+    results: List[Result]
     elapsed_time: float
     args: Optional[Dict[str, Any]] = None
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/run_results/run_results_v6.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/run_results/run_results_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,74 @@
 # generated by datamodel-codegen:
-#   filename:  run-results_v6.json
+#   filename:  run-results_v1.json
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra, Field
+from pydantic import AwareDatetime, ConfigDict
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
-class Metadata(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+class BaseArtifactMetadata(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     dbt_schema_version: str
-    dbt_version: Optional[str] = '1.8.0a1'
-    generated_at: Optional[str] = None
-    invocation_id: Optional[Optional[str]] = None
-    env: Optional[Dict[str, str]] = None
+    dbt_version: Optional[str] = '0.19.0'
+    generated_at: Optional[AwareDatetime] = '2021-02-10T04:42:33.678063Z'
+    invocation_id: Optional[str] = None
+    env: Optional[Dict[str, str]] = {}
 
 
-class StatusEnum(Enum):
+class Status(Enum):
     success = 'success'
     error = 'error'
     skipped = 'skipped'
 
 
-class StatusEnum1(Enum):
+class Status1(Enum):
     pass_ = 'pass'
     error = 'error'
     fail = 'fail'
     warn = 'warn'
-    skipped = 'skipped'
 
 
-class StatusEnum2(Enum):
+class Status2(Enum):
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
     runtime_error = 'runtime error'
 
 
-class TimingItem(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
+class TimingInfo(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    started_at: Optional[Optional[str]] = None
-    completed_at: Optional[Optional[str]] = None
+    started_at: Optional[AwareDatetime] = None
+    completed_at: Optional[AwareDatetime] = None
 
 
-class Result(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
-
-    status: Union[StatusEnum, StatusEnum1, StatusEnum2]
-    timing: List[TimingItem]
+class RunResultOutput(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    status: Union[Status, Status1, Status2]
+    timing: List[TimingInfo]
     thread_id: str
     execution_time: float
+    message: Optional[Union[str, int]] = None
     adapter_response: Dict[str, Any]
-    message: Optional[str]
-    failures: Optional[int]
     unique_id: str
-    compiled: Optional[bool]
-    compiled_code: Optional[str]
-    relation_name: Optional[str]
-
 
-class RunResultsV6(BaseParserModel):
-    class Config:
-        extra = Extra.forbid
 
-    metadata: Metadata = Field(..., title='BaseArtifactMetadata')
-    results: List[Result]
+class RunResultsV1(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    metadata: BaseArtifactMetadata
+    results: List[RunResultOutput]
     elapsed_time: float
-    args: Optional[Dict[str, Any]] = None
+    args: Optional[Dict[str, Any]] = {}
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/__init__.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v1.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/sources/sources_v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 # generated by datamodel-codegen:
 #   filename:  sources_v1.json
-#   timestamp: 2022-03-01T06:21:38+00:00
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra
+from pydantic import AwareDatetime, ConfigDict
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class FreshnessMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    dbt_schema_version: Optional[
-        str] = 'https://schemas.getdbt.com/dbt/sources/v1.json'
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: Optional[str] = 'https://schemas.getdbt.com/dbt/sources/v1.json'
     dbt_version: Optional[str] = '0.19.0'
-    generated_at: Optional[datetime] = '2021-02-10T04:42:33.675309Z'
-    invocation_id: Optional[Optional[str]] = None
+    generated_at: Optional[AwareDatetime] = '2021-02-10T04:42:33.675309Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class Status(Enum):
     runtime_error = 'runtime error'
 
 
 class SourceFreshnessRuntimeError(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    error: Optional[Optional[Union[str, int]]] = None
+    error: Optional[Union[str, int]] = None
     status: Status
 
 
 class Status1(Enum):
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
@@ -50,47 +45,43 @@
 class Period(Enum):
     minute = 'minute'
     hour = 'hour'
     day = 'day'
 
 
 class Time(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     count: int
     period: Period
 
 
 class FreshnessThreshold(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    warn_after: Optional[Optional[Time]] = None
-    error_after: Optional[Optional[Time]] = None
-    filter: Optional[Optional[str]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    warn_after: Optional[Time] = None
+    error_after: Optional[Time] = None
+    filter: Optional[str] = None
 
 
 class SourceFreshnessOutput(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    max_loaded_at: datetime
-    snapshotted_at: datetime
+    max_loaded_at: AwareDatetime
+    snapshotted_at: AwareDatetime
     max_loaded_at_time_ago_in_s: float
     status: Status1
     criteria: FreshnessThreshold
     adapter_response: Dict[str, Any]
 
 
 class SourcesV1(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: FreshnessMetadata
     results: List[Union[SourceFreshnessRuntimeError, SourceFreshnessOutput]]
     elapsed_time: float
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/sources/sources_v2.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/sources/sources_v3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 # generated by datamodel-codegen:
-#   filename:  sources_v2.json
-#   timestamp: 2022-03-01T06:21:38+00:00
+#   filename:  sources_v3.json
 
 from __future__ import annotations
 
-from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import Extra
+from pydantic import AwareDatetime, ConfigDict
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class FreshnessMetadata(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    dbt_schema_version: Optional[
-        str] = 'https://schemas.getdbt.com/dbt/sources/v2.json'
-    dbt_version: Optional[str] = '0.21.0rc1'
-    generated_at: Optional[datetime] = '2021-09-24T13:29:14.312598Z'
-    invocation_id: Optional[Optional[str]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    dbt_schema_version: Optional[str] = 'https://schemas.getdbt.com/dbt/sources/v3.json'
+    dbt_version: Optional[str] = '1.0.0b2'
+    generated_at: Optional[AwareDatetime] = '2021-11-02T20:18:06.796684Z'
+    invocation_id: Optional[str] = None
     env: Optional[Dict[str, str]] = {}
 
 
 class Status(Enum):
     runtime_error = 'runtime error'
 
 
 class SourceFreshnessRuntimeError(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    error: Optional[Optional[Union[str, int]]] = None
+    error: Optional[Union[str, int]] = None
     status: Status
 
 
 class Status1(Enum):
     pass_ = 'pass'
     warn = 'warn'
     error = 'error'
@@ -50,60 +45,55 @@
 class Period(Enum):
     minute = 'minute'
     hour = 'hour'
     day = 'day'
 
 
 class Time(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    count: int
-    period: Period
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    count: Optional[int] = None
+    period: Optional[Period] = None
 
 
 class TimingInfo(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     name: str
-    started_at: Optional[Optional[datetime]] = None
-    completed_at: Optional[Optional[datetime]] = None
+    started_at: Optional[AwareDatetime] = None
+    completed_at: Optional[AwareDatetime] = None
 
 
 class FreshnessThreshold(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
-    warn_after: Optional[Optional[Time]] = None
-    error_after: Optional[Optional[Time]] = None
-    filter: Optional[Optional[str]] = None
+    model_config = ConfigDict(
+        extra='forbid',
+    )
+    warn_after: Optional[Time] = {'count': None, 'period': None}
+    error_after: Optional[Time] = {'count': None, 'period': None}
+    filter: Optional[str] = None
 
 
 class SourceFreshnessOutput(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     unique_id: str
-    max_loaded_at: datetime
-    snapshotted_at: datetime
+    max_loaded_at: AwareDatetime
+    snapshotted_at: AwareDatetime
     max_loaded_at_time_ago_in_s: float
     status: Status1
     criteria: FreshnessThreshold
     adapter_response: Dict[str, Any]
     timing: List[TimingInfo]
     thread_id: str
     execution_time: float
 
 
-class SourcesV2(BaseParserModel):
-
-    class Config:
-        extra = Extra.forbid
-
+class SourcesV3(BaseParserModel):
+    model_config = ConfigDict(
+        extra='forbid',
+    )
     metadata: FreshnessMetadata
     results: List[Union[SourceFreshnessRuntimeError, SourceFreshnessOutput]]
     elapsed_time: float
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/utils.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/parsers/version_map.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/parsers/version_map.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/catalog/catalog_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v10.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v10.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -9261,8 +9261,8 @@
 000242c0: 0a20 2022 2473 6368 656d 6122 3a20 2268  .  "$schema": "h
 000242d0: 7474 703a 2f2f 6a73 6f6e 2d73 6368 656d  ttp://json-schem
 000242e0: 612e 6f72 672f 6472 6166 742d 3037 2f73  a.org/draft-07/s
 000242f0: 6368 656d 6123 222c 0a20 2022 2469 6422  chema#",.  "$id"
 00024300: 3a20 2268 7474 7073 3a2f 2f73 6368 656d  : "https://schem
 00024310: 6173 2e67 6574 6462 742e 636f 6d2f 6462  as.getdbt.com/db
 00024320: 742f 6d61 6e69 6665 7374 2f76 3130 2e6a  t/manifest/v10.j
-00024330: 736f 6e22 0a7d                           son".}
+00024330: 736f 6e22 0a7d 0a                        son".}.
```

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v11.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v11.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v12.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v12.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v4.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v5.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v6.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v7.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v8.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/manifest/manifest_v9.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v4.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v5.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v5.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/run-results/run-results_v6.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/run-results/run-results_v6.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v1.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/sources/sources_v1.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v2.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/sources/sources_v2.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/resources/sources/sources_v3.json` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/resources/sources/sources_v3.json`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/dbt_artifacts_parser/utils.py` & `dbt_artifacts_parser-0.7.0/dbt_artifacts_parser/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/pyproject.toml` & `dbt_artifacts_parser-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 dynamic = ["version", "description"]
 dependencies = [
-    "pydantic >=1.6,<2.0",
+    "pydantic >=2.0,<3.0",
 ]
 
 [project.urls]
 Home = "https://github.com/yu-iskw/dbt-artifacts-parser"
 
 [project.optional-dependencies]
 test = [
@@ -63,12 +63,12 @@
 dev = [
     "flit ==3.7.1",
     "build ==0.7.0",
     "yapf >=0.29.0",
     "pyyaml >=5.3",
     "pdoc3 >=0.9.2",
     "pre-commit >=2.15.0",
-    "datamodel-code-generator >=0.12.0,<0.20.0",
+    "datamodel-code-generator >=0.20,<0.30",
 ]
 
 [tool.isort]
 profile = "black"
```

### Comparing `dbt_artifacts_parser-0.6.0/setup.py` & `dbt_artifacts_parser-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `dbt_artifacts_parser-0.6.0/PKG-INFO` & `dbt_artifacts_parser-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-artifacts-parser
-Version: 0.6.0
+Version: 0.7.0
 Summary: A dbt artifacts parser in python
 Author: yu-iskw
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -17,22 +17,22 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Dist: pydantic >=1.6,<2.0
+Requires-Dist: pydantic >=2.0,<3.0
 Requires-Dist: flit ==3.7.1 ; extra == "dev"
 Requires-Dist: build ==0.7.0 ; extra == "dev"
 Requires-Dist: yapf >=0.29.0 ; extra == "dev"
 Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev"
 Requires-Dist: pre-commit >=2.15.0 ; extra == "dev"
-Requires-Dist: datamodel-code-generator >=0.12.0,<0.20.0 ; extra == "dev"
+Requires-Dist: datamodel-code-generator >=0.20,<0.30 ; extra == "dev"
 Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
 Requires-Dist: pylint >=2.12.0 ; extra == "test"
 Requires-Dist: mypy ==0.910 ; extra == "test"
 Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "test"
 Requires-Dist: black ==21.9b0 ; extra == "test"
 Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
 Requires-Dist: yapf >=0.29.0 ; extra == "test"
@@ -44,19 +44,33 @@
 <a href="https://pypi.org/project/dbt-artifacts-parser" target="_blank">
 <img src="https://img.shields.io/pypi/v/dbt-artifacts-parser?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/dbt-artifacts-parser" target="_blank">
 <img src="https://img.shields.io/pypi/pyversions/dbt-artifacts-parser.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 
-
 # dbt-artifacts-parser
+
 This is a dbt artifacts parse in python.
 It enables us to deal with `catalog.json`, `manifest.json`, `run-results.json` and `sources.json` as python objects.
 
+## Supported Versions and Compatibility
+
+> **⚠️ Important Note:**
+>
+> - **Pydantic v1 will not be supported for dbt 1.9 or later.**
+> - **To parse dbt 1.9 or later, please migrate your code to pydantic v2.**
+> - **We will reassess version compatibility upon the release of pydantic v3.**
+
+| Version | Supported dbt Version | Supported pydantic Version |
+|---------|-----------------------|----------------------------|
+|  0.7    | dbt 1.5 to 1.8        | pydantic v2                |
+|  0.6    | dbt 1.5 to 1.8        | pydantic v1                |
+|  0.5    | dbt 1.5 to 1.7        | pydantic v1                |
+
 ## Installation
 
 ```bash
 pip install -U dbt-artifacts-parser
 ```
 
 ## Python classes
@@ -73,21 +87,23 @@
 - [ManifestV5](dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for manifest.json v5
 - [ManifestV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for manifest.json v6
 - [ManifestV7](dbt_artifacts_parser/parsers/manifest/manifest_v7.py) for manifest.json v7
 - [ManifestV8](dbt_artifacts_parser/parsers/manifest/manifest_v8.py) for manifest.json v8
 - [ManifestV9](dbt_artifacts_parser/parsers/manifest/manifest_v9.py) for manifest.json v9
 - [ManifestV10](dbt_artifacts_parser/parsers/manifest/manifest_v10.py) for manifest.json v10
 - [ManifestV11](dbt_artifacts_parser/parsers/manifest/manifest_v11.py) for manifest.json v11
+- [ManifestV12](dbt_artifacts_parser/parsers/manifest/manifest_v12.py) for manifest.json v12
 
 ### Run Results
 - [RunResultsV1](dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for run_results.json v1
 - [RunResultsV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for run_results.json v2
 - [RunResultsV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for run_results.json v3
 - [RunResultsV4](dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for run_results.json v4
 - [RunResultsV5](dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for run_results.json v5
+- [RunResultsV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for run_results.json v6
 
 ### Sources
 - [SourcesV1](dbt_artifacts_parser/parsers/sources/sources_v1.py) for sources.json v1
 - [SourcesV2](dbt_artifacts_parser/parsers/sources/sources_v2.py) for sources.json v2
 - [SourcesV3](dbt_artifacts_parser/parsers/sources/sources_v3.py) for sources.json v3
 
 ## Examples
@@ -195,14 +211,21 @@
 
 # parse manifest.json v11
 from dbt_artifacts_parser.parser import parse_manifest_v11
 
 with open("path/to/manifest.json", "r") as fp:
     manifest_dict = json.load(fp)
     manifest_obj = parse_manifest_v11(manifest=manifest_dict)
+
+# parse manifest.json v12
+from dbt_artifacts_parser.parser import parse_manifest_v12
+
+with open("path/to/manifest.json", "r") as fp:
+    manifest_dict = json.load(fp)
+    manifest_obj = parse_manifest_v12(manifest=manifest_dict)
 ```
 
 ### Parse run-results.json
 
 ```python
 import json
 
@@ -243,14 +266,21 @@
 
 # parse run-results.json v5
 from dbt_artifacts_parser.parser import parse_run_results_v5
 
 with open("path/to/run-results.json", "r") as fp:
     run_results_dict = json.load(fp)
     run_results_obj = parse_run_results_v5(run_results=run_results_dict)
+
+# parse run-results.json v6
+from dbt_artifacts_parser.parser import parse_run_results_v6
+
+with open("path/to/run-results.json", "r") as fp:
+    run_results_dict = json.load(fp)
+    run_results_obj = parse_run_results_v6(run_results=run_results_dict)
 ```
 
 ### Parse sources.json
 
 ```python
 import json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,65 +1,75 @@
-Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.6.0 Summary: A dbt
+Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.7.0 Summary: A dbt
 artifacts parser in python Author: yu-iskw Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Typing :: Typed Requires-Dist: pydantic >=1.6,<2.0 Requires-Dist: flit ==3.7.1
+Typing :: Typed Requires-Dist: pydantic >=2.0,<3.0 Requires-Dist: flit ==3.7.1
 ; extra == "dev" Requires-Dist: build ==0.7.0 ; extra == "dev" Requires-Dist:
 yapf >=0.29.0 ; extra == "dev" Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev" Requires-Dist: pre-commit
->=2.15.0 ; extra == "dev" Requires-Dist: datamodel-code-generator
->=0.12.0,<0.20.0 ; extra == "dev" Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra
-== "test" Requires-Dist: pylint >=2.12.0 ; extra == "test" Requires-Dist: mypy
-==0.910 ; extra == "test" Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra ==
-"test" Requires-Dist: black ==21.9b0 ; extra == "test" Requires-Dist: isort
+>=2.15.0 ; extra == "dev" Requires-Dist: datamodel-code-generator >=0.20,<0.30
+; extra == "dev" Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
+Requires-Dist: pylint >=2.12.0 ; extra == "test" Requires-Dist: mypy ==0.910 ;
+extra == "test" Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "test"
+Requires-Dist: black ==21.9b0 ; extra == "test" Requires-Dist: isort
 >=5.0.6,<6.0.0 ; extra == "test" Requires-Dist: yapf >=0.29.0 ; extra == "test"
 Project-URL: Home, https://github.com/yu-iskw/dbt-artifacts-parser Provides-
 Extra: dev Provides-Extra: test [![Test python](https://github.com/yu-iskw/dbt-
 artifacts-parser/actions/workflows/test.yml/badge.svg)](https://github.com/yu-
 iskw/dbt-artifacts-parser/actions/workflows/test.yml) _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]# dbt-artifacts-parser This is a dbt artifacts parse
 in python. It enables us to deal with `catalog.json`, `manifest.json`, `run-
-results.json` and `sources.json` as python objects. ## Installation ```bash pip
-install -U dbt-artifacts-parser ``` ## Python classes Those are the classes to
-parse dbt artifacts. ### Catalog - [CatalogV1](dbt_artifacts_parser/parsers/
-catalog/catalog_v1.py) for catalog.json v1 ### Manifest - [ManifestV1]
+results.json` and `sources.json` as python objects. ## Supported Versions and
+Compatibility > **â ï¸ Important Note:** > > - **Pydantic v1 will not be
+supported for dbt 1.9 or later.** > - **To parse dbt 1.9 or later, please
+migrate your code to pydantic v2.** > - **We will reassess version
+compatibility upon the release of pydantic v3.** | Version | Supported dbt
+Version | Supported pydantic Version | |---------|-----------------------|-----
+-----------------------| | 0.7 | dbt 1.5 to 1.8 | pydantic v2 | | 0.6 | dbt 1.5
+to 1.8 | pydantic v1 | | 0.5 | dbt 1.5 to 1.7 | pydantic v1 | ## Installation
+```bash pip install -U dbt-artifacts-parser ``` ## Python classes Those are the
+classes to parse dbt artifacts. ### Catalog - [CatalogV1](dbt_artifacts_parser/
+parsers/catalog/catalog_v1.py) for catalog.json v1 ### Manifest - [ManifestV1]
 (dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for manifest.json v1 -
 [ManifestV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for
 manifest.json v2 - [ManifestV3](dbt_artifacts_parser/parsers/manifest/
 manifest_v3.py) for manifest.json v3 - [ManifestV4](dbt_artifacts_parser/
 parsers/manifest/manifest_v4.py) for manifest.json v4 - [ManifestV5]
 (dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for manifest.json v5 -
 [ManifestV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for
 manifest.json v6 - [ManifestV7](dbt_artifacts_parser/parsers/manifest/
 manifest_v7.py) for manifest.json v7 - [ManifestV8](dbt_artifacts_parser/
 parsers/manifest/manifest_v8.py) for manifest.json v8 - [ManifestV9]
 (dbt_artifacts_parser/parsers/manifest/manifest_v9.py) for manifest.json v9 -
 [ManifestV10](dbt_artifacts_parser/parsers/manifest/manifest_v10.py) for
 manifest.json v10 - [ManifestV11](dbt_artifacts_parser/parsers/manifest/
-manifest_v11.py) for manifest.json v11 ### Run Results - [RunResultsV1]
-(dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for run_results.json v1
-- [RunResultsV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for
-run_results.json v2 - [RunResultsV3](dbt_artifacts_parser/parsers/manifest/
-manifest_v3.py) for run_results.json v3 - [RunResultsV4](dbt_artifacts_parser/
-parsers/manifest/manifest_v4.py) for run_results.json v4 - [RunResultsV5]
-(dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for run_results.json v5
-### Sources - [SourcesV1](dbt_artifacts_parser/parsers/sources/sources_v1.py)
-for sources.json v1 - [SourcesV2](dbt_artifacts_parser/parsers/sources/
-sources_v2.py) for sources.json v2 - [SourcesV3](dbt_artifacts_parser/parsers/
-sources/sources_v3.py) for sources.json v3 ## Examples ### Parse catalog.json
-```python import json # parse any version of catalog.json from
+manifest_v11.py) for manifest.json v11 - [ManifestV12](dbt_artifacts_parser/
+parsers/manifest/manifest_v12.py) for manifest.json v12 ### Run Results -
+[RunResultsV1](dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for
+run_results.json v1 - [RunResultsV2](dbt_artifacts_parser/parsers/manifest/
+manifest_v2.py) for run_results.json v2 - [RunResultsV3](dbt_artifacts_parser/
+parsers/manifest/manifest_v3.py) for run_results.json v3 - [RunResultsV4]
+(dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for run_results.json v4
+- [RunResultsV5](dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for
+run_results.json v5 - [RunResultsV6](dbt_artifacts_parser/parsers/manifest/
+manifest_v6.py) for run_results.json v6 ### Sources - [SourcesV1]
+(dbt_artifacts_parser/parsers/sources/sources_v1.py) for sources.json v1 -
+[SourcesV2](dbt_artifacts_parser/parsers/sources/sources_v2.py) for
+sources.json v2 - [SourcesV3](dbt_artifacts_parser/parsers/sources/
+sources_v3.py) for sources.json v3 ## Examples ### Parse catalog.json ```python
+import json # parse any version of catalog.json from
 dbt_artifacts_parser.parser import parse_catalog with open("path/to/
 catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog(catalog=catalog_dict) # parse catalog.json v1 from
 dbt_artifacts_parser.parser import parse_catalog_v1 with open("path/to/
 catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog_v1(catalog=catalog_dict) ``` ### Parse manifest.json ```python
 import json # parse any version of manifest.json from
@@ -94,15 +104,18 @@
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
 parse_manifest_v9(manifest=manifest_dict) # parse manifest.json v10 from
 dbt_artifacts_parser.parser import parse_manifest_v10 with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
 parse_manifest_v10(manifest=manifest_dict) # parse manifest.json v11 from
 dbt_artifacts_parser.parser import parse_manifest_v11 with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
-parse_manifest_v11(manifest=manifest_dict) ``` ### Parse run-results.json
+parse_manifest_v11(manifest=manifest_dict) # parse manifest.json v12 from
+dbt_artifacts_parser.parser import parse_manifest_v12 with open("path/to/
+manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
+parse_manifest_v12(manifest=manifest_dict) ``` ### Parse run-results.json
 ```python import json # parse any version of run-results.json from
 dbt_artifacts_parser.parser import parse_run_results with open("path/to/run-
 resultsjson", "r") as fp: run_results_dict = json.load(fp) run_results_obj =
 parse_run_results(run_results=run_results_dict) # parse run-results.json v1
 from dbt_artifacts_parser.parser import parse_run_results_v1 with open("path/
 to/run-results.json", "r") as fp: run_results_dict = json.load(fp)
 run_results_obj = parse_run_results_v1(run_results=run_results_dict) # parse
@@ -115,22 +128,26 @@
 parse_run_results_v3(run_results=run_results_dict) # parse run-results.json v4
 from dbt_artifacts_parser.parser import parse_run_results_v4 with open("path/
 to/run-results.json", "r") as fp: run_results_dict = json.load(fp)
 run_results_obj = parse_run_results_v4(run_results=run_results_dict) # parse
 run-results.json v5 from dbt_artifacts_parser.parser import
 parse_run_results_v5 with open("path/to/run-results.json", "r") as fp:
 run_results_dict = json.load(fp) run_results_obj = parse_run_results_v5
-(run_results=run_results_dict) ``` ### Parse sources.json ```python import json
-# parse any version of sources.json from dbt_artifacts_parser.parser import
-parse_sources with open("path/to/sources.json", "r") as fp: sources_dict =
-json.load(fp) sources_obj = parse_sources(sources=sources_dict) # parse
-sources.json v1 from dbt_artifacts_parser.parser import parse_sources_v1 with
-open("path/to/sources.json", "r") as fp: sources_dict = json.load(fp)
-sources_obj = parse_sources_v1(sources=sources_dict) # parse sources.json v2
-from dbt_artifacts_parser.parser import parse_sources_v2 with open("path/to/
+(run_results=run_results_dict) # parse run-results.json v6 from
+dbt_artifacts_parser.parser import parse_run_results_v6 with open("path/to/run-
+results.json", "r") as fp: run_results_dict = json.load(fp) run_results_obj =
+parse_run_results_v6(run_results=run_results_dict) ``` ### Parse sources.json
+```python import json # parse any version of sources.json from
+dbt_artifacts_parser.parser import parse_sources with open("path/to/
+sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
+parse_sources(sources=sources_dict) # parse sources.json v1 from
+dbt_artifacts_parser.parser import parse_sources_v1 with open("path/to/
+sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
+parse_sources_v1(sources=sources_dict) # parse sources.json v2 from
+dbt_artifacts_parser.parser import parse_sources_v2 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v2(sources=sources_dict) # parse sources.json v3 from
 dbt_artifacts_parser.parser import parse_sources_v3 with open("path/to/
 sources.json", "r") as fp: sources_dict = json.load(fp) sources_obj =
 parse_sources_v3(sources=sources_dict) ``` ## Contributors
   _[_y_u_-_i_s_k_w_]   _[_d_l_a_w_i_n_]  _[_b_b_r_e_w_i_n_g_t_o_n_]   _[_j_u_d_a_h_r_a_n_d_]   _[_n_a_b_i_l_m_]     _[_O_n_k_a_r_V_O_7_]
  _YY_uu_ _II_ss_hh_ii_kk_aa_ww_aa    _NN_uu_ll_ll   _BB_rr_ee_nn_tt_ _BB_rr_ee_ww_ii_nn_gg_tt_oo_nn _JJ_uu_dd_aa_hh_ _RR_aa_nn_dd  _MM_oo_hh_aa_mm_ee_dd_ _NN_aa_bb_ii_ll _OO_nn_kk_aa_rr_ _RR_aa_vv_gg_aa_nn
```

