# Comparing `tmp/skfolio-0.2.0.tar.gz` & `tmp/skfolio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skfolio-0.2.0.tar", last modified: Sun May 19 21:47:56 2024, max compression
+gzip compressed data, was "skfolio-0.2.1.tar", last modified: Wed May 22 13:18:50 2024, max compression
```

## Comparing `skfolio-0.2.0.tar` & `skfolio-0.2.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.238159 skfolio-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1526 2024-05-19 21:47:51.000000 skfolio-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-19 21:47:51.000000 skfolio-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    19630 2024-05-19 21:47:56.238159 skfolio-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15392 2024-05-19 21:47:51.000000 skfolio-0.2.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     3470 2024-05-19 21:47:52.000000 skfolio-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 21:47:56.238159 skfolio-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.214159 skfolio-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.218159 skfolio-0.2.0/src/skfolio/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.218159 skfolio-0.2.0/src/skfolio/cluster/
--rw-r--r--   0 root         (0) root         (0)      251 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/cluster/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12817 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/cluster/_hierarchical.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/datasets/
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13952 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/datasets/data/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36146 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/data/factors_dataset.csv.gz
--rw-r--r--   0 root         (0) root         (0)   426065 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/data/sp500_dataset.csv.gz
--rw-r--r--   0 root         (0) root         (0)    41898 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/datasets/data/sp500_index.csv.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/distance/
--rw-r--r--   0 root         (0) root         (0)      547 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/distance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1326 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/distance/_base.py
--rw-r--r--   0 root         (0) root         (0)    18538 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/distance/_distance.py
--rw-r--r--   0 root         (0) root         (0)      662 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/measures/
--rw-r--r--   0 root         (0) root         (0)     1631 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/measures/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8934 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/measures/_enums.py
--rw-r--r--   0 root         (0) root         (0)    16829 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/measures/_measures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.222159 skfolio-0.2.0/src/skfolio/metrics/
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4306 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/metrics/_scorer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/model_selection/
--rw-r--r--   0 root         (0) root         (0)      507 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/model_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19045 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/model_selection/_combinatorial.py
--rw-r--r--   0 root         (0) root         (0)     7686 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/model_selection/_validation.py
--rw-r--r--   0 root         (0) root         (0)     7539 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/model_selection/_walk_forward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/moments/
--rw-r--r--   0 root         (0) root         (0)      746 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/moments/covariance/
--rw-r--r--   0 root         (0) root         (0)      563 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/covariance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3955 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/covariance/_base.py
--rw-r--r--   0 root         (0) root         (0)    39003 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/covariance/_covariance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/moments/expected_returns/
--rw-r--r--   0 root         (0) root         (0)      367 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/expected_returns/__init__.py
--rw-r--r--   0 root         (0) root         (0)      871 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/expected_returns/_base.py
--rw-r--r--   0 root         (0) root         (0)    13388 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/moments/expected_returns/_expected_returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/optimization/
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5748 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/optimization/cluster/
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14834 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/_nco.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.226159 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17281 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_base.py
--rw-r--r--   0 root         (0) root         (0)    17238 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_herc.py
--rw-r--r--   0 root         (0) root         (0)    16123 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_hrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/optimization/convex/
--rw-r--r--   0 root         (0) root         (0)      570 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75439 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_base.py
--rw-r--r--   0 root         (0) root         (0)    17311 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_distributionally_robust.py
--rw-r--r--   0 root         (0) root         (0)    19140 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_maximum_diversification.py
--rw-r--r--   0 root         (0) root         (0)    43134 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_mean_risk.py
--rw-r--r--   0 root         (0) root         (0)    23622 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/convex/_risk_budgeting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/optimization/ensemble/
--rw-r--r--   0 root         (0) root         (0)      158 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/ensemble/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/ensemble/_base.py
--rw-r--r--   0 root         (0) root         (0)    13148 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/ensemble/_stacking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/optimization/naive/
--rw-r--r--   0 root         (0) root         (0)      147 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/naive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5570 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/optimization/naive/_naive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/population/
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/population/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29148 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/population/_population.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.230159 skfolio-0.2.0/src/skfolio/portfolio/
--rw-r--r--   0 root         (0) root         (0)      586 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/portfolio/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38313 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/portfolio/_base.py
--rw-r--r--   0 root         (0) root         (0)    22759 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/portfolio/_multi_period_portfolio.py
--rw-r--r--   0 root         (0) root         (0)    31649 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/portfolio/_portfolio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.234159 skfolio-0.2.0/src/skfolio/pre_selection/
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/pre_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12163 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/pre_selection/_pre_selection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.234159 skfolio-0.2.0/src/skfolio/preprocessing/
--rw-r--r--   0 root         (0) root         (0)       94 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3826 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/preprocessing/_returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.234159 skfolio-0.2.0/src/skfolio/prior/
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/_base.py
--rw-r--r--   0 root         (0) root         (0)     9397 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/_black_litterman.py
--rw-r--r--   0 root         (0) root         (0)     5740 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/_empirical.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/prior/_factor_model.py
--rw-r--r--   0 root         (0) root         (0)     1378 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.234159 skfolio-0.2.0/src/skfolio/uncertainty_set/
--rw-r--r--   0 root         (0) root         (0)      617 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/uncertainty_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3301 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/uncertainty_set/_base.py
--rw-r--r--   0 root         (0) root         (0)    10301 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/uncertainty_set/_bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     8429 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/uncertainty_set/_empirical.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.238159 skfolio-0.2.0/src/skfolio/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3550 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)    11047 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/equations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.238159 skfolio-0.2.0/src/skfolio/utils/fixes/
--rw-r--r--   0 root         (0) root         (0)       95 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/fixes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13551 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/fixes/_dendrogram.py
--rw-r--r--   0 root         (0) root         (0)     3504 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/sorting.py
--rw-r--r--   0 root         (0) root         (0)    13132 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/stats.py
--rw-r--r--   0 root         (0) root         (0)    15374 2024-05-19 21:47:51.000000 skfolio-0.2.0/src/skfolio/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:47:56.238159 skfolio-0.2.0/src/skfolio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19630 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3203 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-19 21:47:56.000000 skfolio-0.2.0/src/skfolio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.617719 skfolio-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-22 13:18:46.000000 skfolio-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-22 13:18:46.000000 skfolio-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    19608 2024-05-22 13:18:50.617719 skfolio-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15370 2024-05-22 13:18:46.000000 skfolio-0.2.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     3470 2024-05-22 13:18:47.000000 skfolio-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 13:18:50.617719 skfolio-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.593718 skfolio-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.597719 skfolio-0.2.1/src/skfolio/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.601719 skfolio-0.2.1/src/skfolio/cluster/
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/cluster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12817 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/cluster/_hierarchical.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.601719 skfolio-0.2.1/src/skfolio/datasets/
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13952 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/datasets/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.601719 skfolio-0.2.1/src/skfolio/datasets/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/datasets/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36146 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/datasets/data/factors_dataset.csv.gz
+-rw-r--r--   0 root         (0) root         (0)   426065 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/datasets/data/sp500_dataset.csv.gz
+-rw-r--r--   0 root         (0) root         (0)    41898 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/datasets/data/sp500_index.csv.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.601719 skfolio-0.2.1/src/skfolio/distance/
+-rw-r--r--   0 root         (0) root         (0)      547 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/distance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1326 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/distance/_base.py
+-rw-r--r--   0 root         (0) root         (0)    18538 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/distance/_distance.py
+-rw-r--r--   0 root         (0) root         (0)      662 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.601719 skfolio-0.2.1/src/skfolio/measures/
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/measures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8934 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/measures/_enums.py
+-rw-r--r--   0 root         (0) root         (0)    16829 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/measures/_measures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.601719 skfolio-0.2.1/src/skfolio/metrics/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/metrics/_scorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.605718 skfolio-0.2.1/src/skfolio/model_selection/
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/model_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19045 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/model_selection/_combinatorial.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/model_selection/_validation.py
+-rw-r--r--   0 root         (0) root         (0)     7539 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/model_selection/_walk_forward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.605718 skfolio-0.2.1/src/skfolio/moments/
+-rw-r--r--   0 root         (0) root         (0)      746 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/moments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.605718 skfolio-0.2.1/src/skfolio/moments/covariance/
+-rw-r--r--   0 root         (0) root         (0)      563 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/moments/covariance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3955 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/moments/covariance/_base.py
+-rw-r--r--   0 root         (0) root         (0)    39003 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/moments/covariance/_covariance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.605718 skfolio-0.2.1/src/skfolio/moments/expected_returns/
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/moments/expected_returns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      871 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/moments/expected_returns/_base.py
+-rw-r--r--   0 root         (0) root         (0)    13388 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/moments/expected_returns/_expected_returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.605718 skfolio-0.2.1/src/skfolio/optimization/
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.605718 skfolio-0.2.1/src/skfolio/optimization/cluster/
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/cluster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14834 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/cluster/_nco.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.605718 skfolio-0.2.1/src/skfolio/optimization/cluster/hierarchical/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/cluster/hierarchical/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17281 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/cluster/hierarchical/_base.py
+-rw-r--r--   0 root         (0) root         (0)    17238 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/cluster/hierarchical/_herc.py
+-rw-r--r--   0 root         (0) root         (0)    16123 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/cluster/hierarchical/_hrp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.609718 skfolio-0.2.1/src/skfolio/optimization/convex/
+-rw-r--r--   0 root         (0) root         (0)      570 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/convex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75439 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/convex/_base.py
+-rw-r--r--   0 root         (0) root         (0)    17311 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/convex/_distributionally_robust.py
+-rw-r--r--   0 root         (0) root         (0)    19140 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/convex/_maximum_diversification.py
+-rw-r--r--   0 root         (0) root         (0)    43134 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/convex/_mean_risk.py
+-rw-r--r--   0 root         (0) root         (0)    23622 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/convex/_risk_budgeting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.609718 skfolio-0.2.1/src/skfolio/optimization/ensemble/
+-rw-r--r--   0 root         (0) root         (0)      158 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/ensemble/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/ensemble/_base.py
+-rw-r--r--   0 root         (0) root         (0)    13148 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/ensemble/_stacking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.609718 skfolio-0.2.1/src/skfolio/optimization/naive/
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/naive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5570 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/optimization/naive/_naive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.609718 skfolio-0.2.1/src/skfolio/population/
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/population/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29148 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/population/_population.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.609718 skfolio-0.2.1/src/skfolio/portfolio/
+-rw-r--r--   0 root         (0) root         (0)      586 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38313 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/portfolio/_base.py
+-rw-r--r--   0 root         (0) root         (0)    22759 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/portfolio/_multi_period_portfolio.py
+-rw-r--r--   0 root         (0) root         (0)    31649 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/portfolio/_portfolio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.609718 skfolio-0.2.1/src/skfolio/pre_selection/
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/pre_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12163 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/pre_selection/_pre_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.613719 skfolio-0.2.1/src/skfolio/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)       94 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/preprocessing/_returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.613719 skfolio-0.2.1/src/skfolio/prior/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/prior/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/prior/_base.py
+-rw-r--r--   0 root         (0) root         (0)     9400 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/prior/_black_litterman.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/prior/_empirical.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/prior/_factor_model.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.613719 skfolio-0.2.1/src/skfolio/uncertainty_set/
+-rw-r--r--   0 root         (0) root         (0)      617 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/uncertainty_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/uncertainty_set/_base.py
+-rw-r--r--   0 root         (0) root         (0)    10301 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/uncertainty_set/_bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     8429 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/uncertainty_set/_empirical.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.613719 skfolio-0.2.1/src/skfolio/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3550 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/utils/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)    11047 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/utils/equations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.613719 skfolio-0.2.1/src/skfolio/utils/fixes/
+-rw-r--r--   0 root         (0) root         (0)       95 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/utils/fixes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/utils/fixes/_dendrogram.py
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/utils/sorting.py
+-rw-r--r--   0 root         (0) root         (0)    13132 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/utils/stats.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2024-05-22 13:18:46.000000 skfolio-0.2.1/src/skfolio/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:18:50.617719 skfolio-0.2.1/src/skfolio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19608 2024-05-22 13:18:50.000000 skfolio-0.2.1/src/skfolio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3203 2024-05-22 13:18:50.000000 skfolio-0.2.1/src/skfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 13:18:50.000000 skfolio-0.2.1/src/skfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-22 13:18:50.000000 skfolio-0.2.1/src/skfolio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-22 13:18:50.000000 skfolio-0.2.1/src/skfolio.egg-info/top_level.txt
```

### Comparing `skfolio-0.2.0/LICENSE` & `skfolio-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/PKG-INFO` & `skfolio-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skfolio
-Version: 0.2.0
+Version: 0.2.1
 Summary: Portfolio optimization built on top of scikit-learn
 Author-email: Hugo Delatte <delatte.hugo@gmail.com>
 Maintainer-email: Hugo Delatte <delatte.hugo@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2007-2023 The skfolio developers.
         All rights reserved.
@@ -560,15 +560,15 @@
         )
     )
 
 Black & Litterman Factor Model
 ------------------------------
 .. code-block:: python
 
-    factor_views = ["MTUM - QUAL == 0.03 ", "SIZE - TLT == 0.04", "VLUE == 0.06"]
+    factor_views = ["MTUM - QUAL == 0.03 ", "VLUE == 0.06"]
     model = MeanRisk(
         objective_function=ObjectiveFunction.MAXIMIZE_RATIO,
         prior_estimator=FactorModel(
             factor_prior_estimator=BlackLitterman(views=factor_views),
         ),
     )
```

### Comparing `skfolio-0.2.0/README.rst` & `skfolio-0.2.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -475,15 +475,15 @@
         )
     )
 
 Black & Litterman Factor Model
 ------------------------------
 .. code-block:: python
 
-    factor_views = ["MTUM - QUAL == 0.03 ", "SIZE - TLT == 0.04", "VLUE == 0.06"]
+    factor_views = ["MTUM - QUAL == 0.03 ", "VLUE == 0.06"]
     model = MeanRisk(
         objective_function=ObjectiveFunction.MAXIMIZE_RATIO,
         prior_estimator=FactorModel(
             factor_prior_estimator=BlackLitterman(views=factor_views),
         ),
     )
```

### Comparing `skfolio-0.2.0/pyproject.toml` & `skfolio-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skfolio"
-version = "0.2.0"
+version = "0.2.1"
 maintainers = [
     { name = "Hugo Delatte", email = "delatte.hugo@gmail.com" },
 ]
 authors = [
     { name = "Hugo Delatte", email = "delatte.hugo@gmail.com" },
 ]
 description = "Portfolio optimization built on top of scikit-learn"
```

### Comparing `skfolio-0.2.0/src/skfolio/__init__.py` & `skfolio-0.2.1/src/skfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/cluster/_hierarchical.py` & `skfolio-0.2.1/src/skfolio/cluster/_hierarchical.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/datasets/_base.py` & `skfolio-0.2.1/src/skfolio/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/datasets/data/factors_dataset.csv.gz` & `skfolio-0.2.1/src/skfolio/datasets/data/factors_dataset.csv.gz`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/datasets/data/sp500_dataset.csv.gz` & `skfolio-0.2.1/src/skfolio/datasets/data/sp500_dataset.csv.gz`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/datasets/data/sp500_index.csv.gz` & `skfolio-0.2.1/src/skfolio/datasets/data/sp500_index.csv.gz`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/distance/__init__.py` & `skfolio-0.2.1/src/skfolio/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/distance/_base.py` & `skfolio-0.2.1/src/skfolio/distance/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/distance/_distance.py` & `skfolio-0.2.1/src/skfolio/distance/_distance.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/exceptions.py` & `skfolio-0.2.1/src/skfolio/exceptions.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/measures/__init__.py` & `skfolio-0.2.1/src/skfolio/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/measures/_enums.py` & `skfolio-0.2.1/src/skfolio/measures/_enums.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/measures/_measures.py` & `skfolio-0.2.1/src/skfolio/measures/_measures.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/metrics/_scorer.py` & `skfolio-0.2.1/src/skfolio/metrics/_scorer.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/model_selection/_combinatorial.py` & `skfolio-0.2.1/src/skfolio/model_selection/_combinatorial.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/model_selection/_validation.py` & `skfolio-0.2.1/src/skfolio/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/model_selection/_walk_forward.py` & `skfolio-0.2.1/src/skfolio/model_selection/_walk_forward.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/moments/__init__.py` & `skfolio-0.2.1/src/skfolio/moments/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/moments/covariance/__init__.py` & `skfolio-0.2.1/src/skfolio/moments/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/moments/covariance/_base.py` & `skfolio-0.2.1/src/skfolio/moments/covariance/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/moments/covariance/_covariance.py` & `skfolio-0.2.1/src/skfolio/moments/covariance/_covariance.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/moments/expected_returns/_base.py` & `skfolio-0.2.1/src/skfolio/moments/expected_returns/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/moments/expected_returns/_expected_returns.py` & `skfolio-0.2.1/src/skfolio/moments/expected_returns/_expected_returns.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/__init__.py` & `skfolio-0.2.1/src/skfolio/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/_base.py` & `skfolio-0.2.1/src/skfolio/optimization/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/cluster/_nco.py` & `skfolio-0.2.1/src/skfolio/optimization/cluster/_nco.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_base.py` & `skfolio-0.2.1/src/skfolio/optimization/cluster/hierarchical/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_herc.py` & `skfolio-0.2.1/src/skfolio/optimization/cluster/hierarchical/_herc.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/cluster/hierarchical/_hrp.py` & `skfolio-0.2.1/src/skfolio/optimization/cluster/hierarchical/_hrp.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/convex/__init__.py` & `skfolio-0.2.1/src/skfolio/optimization/convex/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/convex/_base.py` & `skfolio-0.2.1/src/skfolio/optimization/convex/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/convex/_distributionally_robust.py` & `skfolio-0.2.1/src/skfolio/optimization/convex/_distributionally_robust.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/convex/_maximum_diversification.py` & `skfolio-0.2.1/src/skfolio/optimization/convex/_maximum_diversification.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/convex/_mean_risk.py` & `skfolio-0.2.1/src/skfolio/optimization/convex/_mean_risk.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/convex/_risk_budgeting.py` & `skfolio-0.2.1/src/skfolio/optimization/convex/_risk_budgeting.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/ensemble/_base.py` & `skfolio-0.2.1/src/skfolio/optimization/ensemble/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/ensemble/_stacking.py` & `skfolio-0.2.1/src/skfolio/optimization/ensemble/_stacking.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/optimization/naive/_naive.py` & `skfolio-0.2.1/src/skfolio/optimization/naive/_naive.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/population/_population.py` & `skfolio-0.2.1/src/skfolio/population/_population.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/portfolio/__init__.py` & `skfolio-0.2.1/src/skfolio/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/portfolio/_base.py` & `skfolio-0.2.1/src/skfolio/portfolio/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/portfolio/_multi_period_portfolio.py` & `skfolio-0.2.1/src/skfolio/portfolio/_multi_period_portfolio.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/portfolio/_portfolio.py` & `skfolio-0.2.1/src/skfolio/portfolio/_portfolio.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/pre_selection/_pre_selection.py` & `skfolio-0.2.1/src/skfolio/pre_selection/_pre_selection.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/preprocessing/_returns.py` & `skfolio-0.2.1/src/skfolio/preprocessing/_returns.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/prior/_base.py` & `skfolio-0.2.1/src/skfolio/prior/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/prior/_black_litterman.py` & `skfolio-0.2.1/src/skfolio/prior/_black_litterman.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         """
         self.prior_estimator_ = check_estimator(
             self.prior_estimator,
             default=EmpiricalPrior(mu_estimator=EquilibriumMu()),
             check_type=BasePrior,
         )
         # fitting prior estimator
-        self.prior_estimator_.fit(X)
+        self.prior_estimator_.fit(X, y)
 
         prior_mu = self.prior_estimator_.prior_model_.mu
         prior_covariance = self.prior_estimator_.prior_model_.covariance
         prior_returns = self.prior_estimator_.prior_model_.returns
 
         # we validate after all models have been fitted to keep features names
         # information.
```

### Comparing `skfolio-0.2.0/src/skfolio/prior/_empirical.py` & `skfolio-0.2.1/src/skfolio/prior/_empirical.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,36 +116,37 @@
         if not self.is_log_normal:
             if self.investment_horizon is not None:
                 raise ValueError(
                     "`investment_horizon` must be `None` when "
                     "`is_log_normal` is `False`"
                 )
             # Expected returns
-            self.mu_estimator_.fit(X)
+            self.mu_estimator_.fit(X, y)
             mu = self.mu_estimator_.mu_
 
             # Covariance
-            self.covariance_estimator_.fit(X)
+            self.covariance_estimator_.fit(X, y)
             covariance = self.covariance_estimator_.covariance_
         else:
             if self.investment_horizon is None:
                 raise ValueError(
                     "`investment_horizon` must be provided when "
                     "`is_log_normal` is `True`"
                 )
             # Convert linear returns to log returns
             X_log = np.log(1 + X)
+            y_log = np.log(1 + y) if y is not None else None
 
             # Estimates the moments on the log returns
             # Expected returns
-            self.mu_estimator_.fit(X_log)
+            self.mu_estimator_.fit(X_log, y_log)
             mu = self.mu_estimator_.mu_
 
             # Covariance
-            self.covariance_estimator_.fit(X_log)
+            self.covariance_estimator_.fit(X_log, y_log)
             covariance = self.covariance_estimator_.covariance_
 
             # Using the property of aggregation across time we scale this distribution
             # to the investment horizon by the “square-root rule”.
             mu *= self.investment_horizon
             covariance *= self.investment_horizon
```

### Comparing `skfolio-0.2.0/src/skfolio/prior/_factor_model.py` & `skfolio-0.2.1/src/skfolio/prior/_factor_model.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/typing.py` & `skfolio-0.2.1/src/skfolio/typing.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/uncertainty_set/__init__.py` & `skfolio-0.2.1/src/skfolio/uncertainty_set/__init__.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/uncertainty_set/_base.py` & `skfolio-0.2.1/src/skfolio/uncertainty_set/_base.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/uncertainty_set/_bootstrap.py` & `skfolio-0.2.1/src/skfolio/uncertainty_set/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/uncertainty_set/_empirical.py` & `skfolio-0.2.1/src/skfolio/uncertainty_set/_empirical.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/utils/bootstrap.py` & `skfolio-0.2.1/src/skfolio/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/utils/equations.py` & `skfolio-0.2.1/src/skfolio/utils/equations.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/utils/fixes/_dendrogram.py` & `skfolio-0.2.1/src/skfolio/utils/fixes/_dendrogram.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/utils/sorting.py` & `skfolio-0.2.1/src/skfolio/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/utils/stats.py` & `skfolio-0.2.1/src/skfolio/utils/stats.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio/utils/tools.py` & `skfolio-0.2.1/src/skfolio/utils/tools.py`

 * *Files identical despite different names*

### Comparing `skfolio-0.2.0/src/skfolio.egg-info/PKG-INFO` & `skfolio-0.2.1/src/skfolio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skfolio
-Version: 0.2.0
+Version: 0.2.1
 Summary: Portfolio optimization built on top of scikit-learn
 Author-email: Hugo Delatte <delatte.hugo@gmail.com>
 Maintainer-email: Hugo Delatte <delatte.hugo@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2007-2023 The skfolio developers.
         All rights reserved.
@@ -560,15 +560,15 @@
         )
     )
 
 Black & Litterman Factor Model
 ------------------------------
 .. code-block:: python
 
-    factor_views = ["MTUM - QUAL == 0.03 ", "SIZE - TLT == 0.04", "VLUE == 0.06"]
+    factor_views = ["MTUM - QUAL == 0.03 ", "VLUE == 0.06"]
     model = MeanRisk(
         objective_function=ObjectiveFunction.MAXIMIZE_RATIO,
         prior_estimator=FactorModel(
             factor_prior_estimator=BlackLitterman(views=factor_views),
         ),
     )
```

### Comparing `skfolio-0.2.0/src/skfolio.egg-info/SOURCES.txt` & `skfolio-0.2.1/src/skfolio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

