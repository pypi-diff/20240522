# Comparing `tmp/imodels-1.4.3.tar.gz` & `tmp/imodels-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imodels-1.4.3.tar", last modified: Mon Mar 11 20:28:14 2024, max compression
+gzip compressed data, was "imodels-1.4.4.tar", last modified: Wed May 22 20:17:21 2024, max compression
```

## Comparing `imodels-1.4.3.tar` & `imodels-1.4.4.tar`

### file list

```diff
@@ -1,158 +1,160 @@
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.802377 imodels-1.4.3/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       37 2023-01-25 06:49:14.000000 imodels-1.4.3/MANIFEST.in
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    30007 2024-03-11 20:28:14.802377 imodels-1.4.3/PKG-INFO
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.786376 imodels-1.4.3/imodels/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3347 2023-10-05 03:06:01.000000 imodels-1.4.3/imodels/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.786376 imodels-1.4.3/imodels/algebraic/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       95 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/algebraic/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8826 2024-03-11 05:10:46.000000 imodels-1.4.3/imodels/algebraic/gam_multitask.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13183 2023-10-05 01:58:31.000000 imodels-1.4.3/imodels/algebraic/marginal_shrinkage_linear_model.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5849 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/algebraic/slim.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    15880 2023-09-24 16:14:07.000000 imodels-1.4.3/imodels/algebraic/tree_gam.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.786376 imodels-1.4.3/imodels/discretization/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      151 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/discretization/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    33999 2024-02-29 14:09:51.000000 imodels-1.4.3/imodels/discretization/discretizer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    18119 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/discretization/mdlp.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2153 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/discretization/simple.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.790377 imodels-1.4.3/imodels/experimental/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       64 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.790377 imodels-1.4.3/imodels/experimental/bartpy/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       56 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    10998 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/data.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.790377 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3631 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/diagnostics.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8255 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/features.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7294 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/motivation.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      746 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/residuals.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1094 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/sampling.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      406 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/sigma.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1132 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/diagnostics/trees.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      111 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/errors.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.790377 imodels-1.4.3/imodels/experimental/bartpy/extensions/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/extensions/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1084 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/extensions/baseestimator.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      770 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/extensions/ols.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.790377 imodels-1.4.3/imodels/experimental/bartpy/features/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/features/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4797 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/features/featureimportance.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2791 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/features/featureselection.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.790377 imodels-1.4.3/imodels/experimental/bartpy/initializers/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/initializers/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      875 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/initializers/initializer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6885 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/initializers/sklearntreeinitializer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4412 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/model.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1251 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/mutation.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4460 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/node.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      335 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/plotting.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1711 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/runner.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.794376 imodels-1.4.3/imodels/experimental/bartpy/samplers/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1825 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/leafnode.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3023 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/modelsampler.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.794376 imodels-1.4.3/imodels/experimental/bartpy/samplers/oblivioustrees/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/oblivioustrees/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6904 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/oblivioustrees/likelihoodratio.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2727 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/oblivioustrees/proposer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2230 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/oblivioustrees/treemutation.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      220 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/sampler.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1437 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/scalar.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1797 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/schedule.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      642 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/sigma.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4812 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/treemutation.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.794376 imodels-1.4.3/imodels/experimental/bartpy/samplers/unconstrainedtree/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/unconstrainedtree/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     9280 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/unconstrainedtree/likelihoodratio.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3920 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/unconstrainedtree/proposer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2318 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/samplers/unconstrainedtree/treemutation.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1238 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/sigma.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    26442 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/sklearnmodel.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1651 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/split.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3342 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/splitcondition.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1022 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/trace.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5430 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/bartpy/tree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24992 2023-09-15 14:56:03.000000 imodels-1.4.3/imodels/experimental/figs_ensembles.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8446 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/figs_shrinkage.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3336 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/stablelinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2333 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/stableskope.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7382 2023-12-08 13:01:30.000000 imodels-1.4.3/imodels/experimental/tree_gam_simple.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1485 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/experimental/util.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.794376 imodels-1.4.3/imodels/importance/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      513 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/importance/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    23294 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/importance/block_transformers.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    21216 2023-08-17 03:01:49.000000 imodels-1.4.3/imodels/importance/block_transformers_ys.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8743 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/importance/local_stumps.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    20013 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/importance/mdi_plus.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22612 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/importance/ppms.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3942 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/importance/ranking_stability.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22232 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/importance/rf_plus.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.794376 imodels-1.4.3/imodels/rule_list/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       70 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_list/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.794376 imodels-1.4.3/imodels/rule_list/bayesian_rule_list/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      166 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_list/bayesian_rule_list/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12271 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_list/bayesian_rule_list/bayesian_rule_list.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22508 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_list/bayesian_rule_list/brl_util.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11499 2023-09-15 14:56:03.000000 imodels-1.4.3/imodels/rule_list/corels_wrapper.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11982 2023-09-15 14:56:03.000000 imodels-1.4.3/imodels/rule_list/greedy_rule_list.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2133 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_list/one_r.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      255 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_list/rule_list.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.798377 imodels-1.4.3/imodels/rule_set/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       95 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_set/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3855 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/rule_set/boosted_rules.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    23303 2023-09-15 14:56:03.000000 imodels-1.4.3/imodels/rule_set/brs.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2259 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_set/fplasso.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2694 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_set/fpskope.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13771 2024-02-29 14:50:40.000000 imodels-1.4.3/imodels/rule_set/rule_fit.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1299 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_set/rule_set.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    20793 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_set/skope_rules.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      598 2023-06-29 13:15:18.000000 imodels-1.4.3/imodels/rule_set/slipper.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     9158 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/rule_set/slipper_util.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.798377 imodels-1.4.3/imodels/tree/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       70 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.798377 imodels-1.4.3/imodels/tree/c45_tree/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/c45_tree/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16579 2023-02-12 05:44:55.000000 imodels-1.4.3/imodels/tree/c45_tree/c45_tree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4412 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/c45_tree/c45_utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8855 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/cart_ccp.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4780 2023-09-15 14:56:03.000000 imodels-1.4.3/imodels/tree/cart_wrapper.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7638 2023-09-23 23:38:52.000000 imodels-1.4.3/imodels/tree/custom_greedy_tree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    28408 2024-02-29 13:44:21.000000 imodels-1.4.3/imodels/tree/figs.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.798377 imodels-1.4.3/imodels/tree/gosdt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/gosdt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11031 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/gosdt/pygosdt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17200 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/gosdt/pygosdt_helper.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6936 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/gosdt/pygosdt_shrinkage.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    18637 2023-11-16 02:41:43.000000 imodels-1.4.3/imodels/tree/hierarchical_shrinkage.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.798377 imodels-1.4.3/imodels/tree/iterative_random_forest/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      109 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/iterative_random_forest/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1104 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/iterative_random_forest/iterative_random_forest.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    18121 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/tree/tao.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5764 2023-10-24 23:50:37.000000 imodels-1.4.3/imodels/tree/viz_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.802377 imodels-1.4.3/imodels/util/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       72 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1357 2023-01-26 21:22:50.000000 imodels-1.4.3/imodels/util/arguments.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4755 2023-10-06 21:24:09.000000 imodels-1.4.3/imodels/util/automl.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2237 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/checks.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5014 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/convert.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13267 2024-03-11 20:25:08.000000 imodels-1.4.3/imodels/util/data_util.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2138 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/distillation.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2030 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/explain_errors.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8671 2024-02-29 13:55:54.000000 imodels-1.4.3/imodels/util/extract.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2077 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/metrics.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6634 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/neural_nets.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3753 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/prune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3117 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/rule.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5692 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/score.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2188 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/transforms.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6948 2023-11-02 20:03:33.000000 imodels-1.4.3/imodels/util/tree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3585 2023-01-25 06:49:14.000000 imodels-1.4.3/imodels/util/tree_interaction_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-03-11 20:28:14.786376 imodels-1.4.3/imodels.egg-info/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    30007 2024-03-11 20:28:14.000000 imodels-1.4.3/imodels.egg-info/PKG-INFO
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5071 2024-03-11 20:28:14.000000 imodels-1.4.3/imodels.egg-info/SOURCES.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-03-11 20:28:14.000000 imodels-1.4.3/imodels.egg-info/dependency_links.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      168 2024-03-11 20:28:14.000000 imodels-1.4.3/imodels.egg-info/requires.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        8 2024-03-11 20:28:14.000000 imodels-1.4.3/imodels.egg-info/top_level.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1074 2023-01-25 06:49:14.000000 imodels-1.4.3/license.md
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    29435 2024-03-10 06:44:33.000000 imodels-1.4.3/readme.md
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-03-11 20:28:14.802377 imodels-1.4.3/setup.cfg
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2137 2024-03-11 20:27:25.000000 imodels-1.4.3/setup.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.069165 imodels-1.4.4/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       37 2023-01-25 06:49:14.000000 imodels-1.4.4/MANIFEST.in
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    30007 2024-05-22 20:17:21.069165 imodels-1.4.4/PKG-INFO
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.057165 imodels-1.4.4/imodels/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3347 2023-10-05 03:06:01.000000 imodels-1.4.4/imodels/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.057165 imodels-1.4.4/imodels/algebraic/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       95 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/algebraic/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13936 2024-04-03 16:20:42.000000 imodels-1.4.4/imodels/algebraic/gam_multitask.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13183 2023-10-05 01:58:31.000000 imodels-1.4.4/imodels/algebraic/marginal_shrinkage_linear_model.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5849 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/algebraic/slim.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    15880 2023-09-24 16:14:07.000000 imodels-1.4.4/imodels/algebraic/tree_gam.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7641 2024-04-22 13:41:13.000000 imodels-1.4.4/imodels/algebraic/tree_gam_minimal.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.057165 imodels-1.4.4/imodels/discretization/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      151 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/discretization/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    33999 2024-02-29 14:09:51.000000 imodels-1.4.4/imodels/discretization/discretizer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    18119 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/discretization/mdlp.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2153 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/discretization/simple.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.057165 imodels-1.4.4/imodels/experimental/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       64 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/experimental/bartpy/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       56 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    10998 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/data.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3631 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/diagnostics.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8255 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/features.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7294 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/motivation.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      746 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/residuals.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1094 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/sampling.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      406 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/sigma.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1132 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/diagnostics/trees.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      111 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/errors.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/experimental/bartpy/extensions/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/extensions/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1084 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/extensions/baseestimator.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      770 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/extensions/ols.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/experimental/bartpy/features/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/features/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4797 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/features/featureimportance.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2791 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/features/featureselection.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/experimental/bartpy/initializers/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/initializers/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      875 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/initializers/initializer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6885 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/initializers/sklearntreeinitializer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4412 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/model.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1251 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/mutation.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4460 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/node.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      335 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/plotting.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1711 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/runner.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/experimental/bartpy/samplers/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1825 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/leafnode.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3023 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/modelsampler.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/experimental/bartpy/samplers/oblivioustrees/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/oblivioustrees/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6904 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/oblivioustrees/likelihoodratio.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2727 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/oblivioustrees/proposer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2230 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/oblivioustrees/treemutation.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      220 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/sampler.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1437 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/scalar.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1797 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/schedule.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      642 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/sigma.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4812 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/treemutation.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/experimental/bartpy/samplers/unconstrainedtree/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/unconstrainedtree/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     9280 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/unconstrainedtree/likelihoodratio.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3920 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/unconstrainedtree/proposer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2318 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/samplers/unconstrainedtree/treemutation.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1238 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/sigma.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    26442 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/sklearnmodel.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1651 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/split.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3342 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/splitcondition.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1022 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/trace.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5430 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/bartpy/tree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24992 2023-09-15 14:56:03.000000 imodels-1.4.4/imodels/experimental/figs_ensembles.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8446 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/figs_shrinkage.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3336 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/stablelinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2333 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/stableskope.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7382 2023-12-08 13:01:30.000000 imodels-1.4.4/imodels/experimental/tree_gam_simple.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1485 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/experimental/util.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.061165 imodels-1.4.4/imodels/importance/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      513 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/importance/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    23294 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/importance/block_transformers.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    21216 2023-08-17 03:01:49.000000 imodels-1.4.4/imodels/importance/block_transformers_ys.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8743 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/importance/local_stumps.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    20013 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/importance/mdi_plus.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22612 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/importance/ppms.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3942 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/importance/ranking_stability.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22232 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/importance/rf_plus.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.065165 imodels-1.4.4/imodels/rule_list/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       70 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_list/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.065165 imodels-1.4.4/imodels/rule_list/bayesian_rule_list/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      166 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_list/bayesian_rule_list/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12271 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_list/bayesian_rule_list/bayesian_rule_list.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22508 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_list/bayesian_rule_list/brl_util.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11499 2023-09-15 14:56:03.000000 imodels-1.4.4/imodels/rule_list/corels_wrapper.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11982 2023-09-15 14:56:03.000000 imodels-1.4.4/imodels/rule_list/greedy_rule_list.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2133 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_list/one_r.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      255 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_list/rule_list.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.065165 imodels-1.4.4/imodels/rule_set/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       95 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_set/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3855 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/rule_set/boosted_rules.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    23303 2023-09-15 14:56:03.000000 imodels-1.4.4/imodels/rule_set/brs.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2259 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_set/fplasso.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2694 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_set/fpskope.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13771 2024-02-29 14:50:40.000000 imodels-1.4.4/imodels/rule_set/rule_fit.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1299 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_set/rule_set.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    20793 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_set/skope_rules.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      598 2023-06-29 13:15:18.000000 imodels-1.4.4/imodels/rule_set/slipper.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     9158 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/rule_set/slipper_util.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.065165 imodels-1.4.4/imodels/tree/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       70 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.065165 imodels-1.4.4/imodels/tree/c45_tree/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/c45_tree/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16579 2023-02-12 05:44:55.000000 imodels-1.4.4/imodels/tree/c45_tree/c45_tree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4412 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/c45_tree/c45_utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8855 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/cart_ccp.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4780 2023-09-15 14:56:03.000000 imodels-1.4.4/imodels/tree/cart_wrapper.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7638 2023-09-23 23:38:52.000000 imodels-1.4.4/imodels/tree/custom_greedy_tree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    28408 2024-02-29 13:44:21.000000 imodels-1.4.4/imodels/tree/figs.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.065165 imodels-1.4.4/imodels/tree/gosdt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/gosdt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11031 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/gosdt/pygosdt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17200 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/gosdt/pygosdt_helper.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6936 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/gosdt/pygosdt_shrinkage.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    18637 2023-11-16 02:41:43.000000 imodels-1.4.4/imodels/tree/hierarchical_shrinkage.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.065165 imodels-1.4.4/imodels/tree/iterative_random_forest/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      109 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/iterative_random_forest/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1104 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/iterative_random_forest/iterative_random_forest.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    18121 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/tree/tao.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5764 2023-10-24 23:50:37.000000 imodels-1.4.4/imodels/tree/viz_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.069165 imodels-1.4.4/imodels/util/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       72 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1357 2023-01-26 21:22:50.000000 imodels-1.4.4/imodels/util/arguments.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4755 2023-10-06 21:24:09.000000 imodels-1.4.4/imodels/util/automl.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2237 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/checks.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5014 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/convert.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14256 2024-03-11 23:30:44.000000 imodels-1.4.4/imodels/util/data_util.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2138 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/distillation.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4606 2024-03-13 20:44:10.000000 imodels-1.4.4/imodels/util/ensemble.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2030 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/explain_errors.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8671 2024-02-29 13:55:54.000000 imodels-1.4.4/imodels/util/extract.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2077 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/metrics.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6634 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/neural_nets.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3753 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/prune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3117 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/rule.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5704 2024-05-22 20:14:27.000000 imodels-1.4.4/imodels/util/score.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4816 2024-03-14 18:00:47.000000 imodels-1.4.4/imodels/util/transforms.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6948 2023-11-02 20:03:33.000000 imodels-1.4.4/imodels/util/tree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3585 2023-01-25 06:49:14.000000 imodels-1.4.4/imodels/util/tree_interaction_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-22 20:17:21.057165 imodels-1.4.4/imodels.egg-info/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    30007 2024-05-22 20:17:20.000000 imodels-1.4.4/imodels.egg-info/PKG-INFO
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5134 2024-05-22 20:17:21.000000 imodels-1.4.4/imodels.egg-info/SOURCES.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-05-22 20:17:20.000000 imodels-1.4.4/imodels.egg-info/dependency_links.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      168 2024-05-22 20:17:20.000000 imodels-1.4.4/imodels.egg-info/requires.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        8 2024-05-22 20:17:20.000000 imodels-1.4.4/imodels.egg-info/top_level.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1074 2023-01-25 06:49:14.000000 imodels-1.4.4/license.md
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    29435 2024-03-10 06:44:33.000000 imodels-1.4.4/readme.md
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-05-22 20:17:21.069165 imodels-1.4.4/setup.cfg
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2137 2024-05-22 20:16:40.000000 imodels-1.4.4/setup.py
```

### Comparing `imodels-1.4.3/PKG-INFO` & `imodels-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodels
-Version: 1.4.3
+Version: 1.4.4
 Summary: Implementations of various interpretable models
 Home-page: https://github.com/csinva/imodels
 Author: Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen, Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others
 Author-email: chandan_singh@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodels Version: 1.4.3 Summary: Implementations of
+Metadata-Version: 2.1 Name: imodels Version: 1.4.4 Summary: Implementations of
 various interpretable models Home-page: https://github.com/csinva/imodels
 Author: Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen,
 Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others Author-email:
 chandan_singh@berkeley.edu Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9.0 Description-Content-Type: text/
 markdown Provides-Extra: dev
```

### Comparing `imodels-1.4.3/imodels/__init__.py` & `imodels-1.4.4/imodels/__init__.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/algebraic/gam_multitask.py` & `imodels-1.4.4/imodels/experimental/figs_shrinkage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,231 +1,187 @@
 from copy import deepcopy
+from typing import List
+
 import numpy as np
-import pandas as pd
+from sklearn import datasets
 from sklearn.base import BaseEstimator
-from sklearn.linear_model import ElasticNetCV, LinearRegression, RidgeCV, LassoCV
-from sklearn.tree import DecisionTreeRegressor
-from sklearn.utils.validation import check_is_fitted
-from sklearn.utils import check_array
-from sklearn.utils.multiclass import check_classification_targets
-from sklearn.utils.validation import check_X_y
-from sklearn.utils.validation import _check_sample_weight
-from sklearn.ensemble import GradientBoostingClassifier, GradientBoostingRegressor, AdaBoostClassifier, AdaBoostRegressor
+from sklearn.metrics import r2_score
+from sklearn.model_selection import cross_val_score
 from sklearn.model_selection import train_test_split
-from sklearn.metrics import accuracy_score, roc_auc_score
-from tqdm import tqdm
-from collections import defaultdict
-import pandas as pd
-import json
-from sklearn.preprocessing import StandardScaler
-
-import imodels
-from interpret.glassbox import ExplainableBoostingClassifier, ExplainableBoostingRegressor
-
-from sklearn.base import RegressorMixin, ClassifierMixin
-
-
-# See notes in this implementation:
-# https://github.com/interpretml/interpret/blob/develop/python/interpret-core/interpret/glassbox/_ebm/_ebm.py
-# merge ebms: https://github.com/interpretml/interpret/blob/develop/python/interpret-core/interpret/glassbox/_ebm/_merge_ebms.py#L280
-
-class MultiTaskGAM(BaseEstimator):
-    """Multi-task GAM classifier.
-    """
-
-    def __init__(
-        self,
-        ebm_kwargs={'n_jobs': 1},
-        multitask=True,
-        interactions=0.95,
-        linear_penalty='ridge',
-        onehot_prior=False,
-        renormalize_features=False,
-        random_state=42,
-    ):
-        """
-        Params
-        ------
-        Note: args override ebm_kwargs if there are duplicates
-        one_hot_prior: bool
-            If True and multitask, the linear model will be fit with a prior that the ebm
-            features predicting the target should have coef 1
-        """
-        self.ebm_kwargs = ebm_kwargs
-        self.multitask = multitask
-        self.linear_penalty = linear_penalty
-        self.random_state = random_state
-        self.interactions = interactions
-        self.onehot_prior = onehot_prior
-        self.renormalize_features = renormalize_features
-
-        # override ebm_kwargs
-        ebm_kwargs['random_state'] = random_state
-        ebm_kwargs['interactions'] = interactions
-        self.ebm_ = ExplainableBoostingRegressor(**(ebm_kwargs or {}))
-
-    def fit(self, X, y, sample_weight=None):
-        X, y = check_X_y(X, y, accept_sparse=False, multi_output=False)
-        if isinstance(self, ClassifierMixin):
-            check_classification_targets(y)
-            self.classes_, y = np.unique(y, return_inverse=True)
-        sample_weight = _check_sample_weight(sample_weight, X, dtype=None)
-
-        # just fit normal ebm
-        if not self.multitask:
-            self.ebm_.fit(X, y, sample_weight=sample_weight)
-            return self
-
-        # fit EBM to each column of X
-        self.ebms_ = []
-        num_features = X.shape[1]
-        for task_num in tqdm(range(num_features)):
-            self.ebms_.append(deepcopy(self.ebm_))
-            y_ = np.ascontiguousarray(X[:, task_num])
-            X_ = deepcopy(X)
-            X_[:, task_num] = 0
-            self.ebms_[task_num].fit(X_, y_, sample_weight=sample_weight)
-
-        # finally, fit EBM to the target
-        self.ebms_.append(deepcopy(self.ebm_))
-        self.ebms_[num_features].fit(X, y, sample_weight=sample_weight)
-
-        # extract features
-        self.term_names_list_ = [
-            ebm_.term_names_ for ebm_ in self.ebms_]
-        self.term_names_ = sum(self.term_names_list_, [])
-        feats = self._extract_ebm_features(X)
-
-        if self.renormalize_features:
-            self.scaler_ = StandardScaler()
-            feats = self.scaler_.fit_transform(feats)
-
-        # fit a linear model to the features
-        if self.linear_penalty == 'ridge':
-            self.lin_model = RidgeCV(alphas=np.logspace(-2, 3, 7))
-        elif self.linear_penalty == 'elasticnet':
-            self.lin_model = ElasticNetCV(n_alphas=7)
-        elif self.linear_penalty == 'lasso':
-            self.lin_model = LassoCV(n_alphas=7)
-
-        if self.onehot_prior:
-            coef_prior_ = np.zeros((feats.shape[1], ))
-            coef_prior_[:num_features] = 1
-            preds_prior = feats @ coef_prior_
-            residuals = y - preds_prior
-            self.lin_model.fit(feats, residuals, sample_weight=sample_weight)
-            self.lin_model.coef_ = self.lin_model.coef_ + coef_prior_
-
-        else:
-            self.lin_model.fit(feats, y, sample_weight=sample_weight)
-
-        return self
-
-    def _extract_ebm_features(self, X):
-        '''
-        Extract features by extracting all terms with EBM
-        '''
-        feats = np.empty((X.shape[0], len(self.term_names_)))
-        offset = 0
-        for ebm_num in range(len(self.ebms_)):
-            # see eval_terms function: https://interpret.ml/docs/python/api/ExplainableBoostingRegressor.html#interpret.glassbox.ExplainableBoostingRegressor.eval_terms
-            n_features_ebm_num = len(self.term_names_list_[ebm_num])
-            feats[:, offset: offset + n_features_ebm_num] = \
-                self.ebms_[ebm_num].eval_terms(X)
-            offset += n_features_ebm_num
-
-        return feats
-
-    def predict(self, X):
-        check_is_fitted(self)
-        X = check_array(X, accept_sparse=False)
-        if hasattr(self, 'ebms_'):
-            feats = self._extract_ebm_features(X)
-            if hasattr(self, 'scaler_'):
-                feats = self.scaler_.transform(feats)
-            return self.lin_model.predict(feats)
-        else:
-            return self.ebm_.predict(X)
-
-    # def predict_proba(self, X):
-    #     check_is_fitted(self)
-    #     X = check_array(X, accept_sparse=False)
-    #     return self.ebm_.predict_proba(X)
+from sklearn.tree import DecisionTreeRegressor
 
+from imodels.util import checks
 
-class MultiTaskGAMRegressor(MultiTaskGAM, RegressorMixin):
-    ...
 
+class HSFIGS:
+    def __init__(self, estimator_: BaseEstimator, reg_param: float = 1, shrinkage_scheme_: str = 'node_based'):
+        """HSTree (Tree with hierarchical shrinkage applied).
+        Hierarchical shinkage is an extremely fast post-hoc regularization method which works on any decision tree (or tree-based ensemble, such as Random Forest).
+        It does not modify the tree structure, and instead regularizes the tree by shrinking the prediction over each node towards the sample means of its ancestors (using a single regularization parameter).
+        Experiments over a wide variety of datasets show that hierarchical shrinkage substantially increases the predictive performance of individual decision trees and decision-tree ensembles.
+        https://arxiv.org/abs/2202.00858
 
-class MultiTaskGAMClassifier(MultiTaskGAM, ClassifierMixin):
-    ...
+        Params
+        ------
+        estimator_: sklearn tree or tree ensemble model (e.g. RandomForest or GradientBoosting)
 
+        reg_param: float
+            Higher is more regularization (can be arbitrarily large, should not be < 0)
 
-def test_multitask_extraction():
-    X, y, feature_names = imodels.get_clean_dataset("california_housing")
-    # X, y, feature_names = imodels.get_clean_dataset("bike_sharing")
+        shrinkage_scheme: str
+            Experimental: Used to experiment with different forms of shrinkage. options are:
+                (i) node_based shrinks based on number of samples in parent node
+                (ii) leaf_based only shrinks leaf nodes based on number of leaf samples
+                (iii) constant shrinks every node by a constant lambda
+        """
+        super().__init__()
+        self.reg_param = reg_param
+        # print('est', estimator_)
+        self.estimator_ = estimator_
+        self.shrinkage_scheme_ = shrinkage_scheme_
+        self._init_prediction_task()
+
+        if checks.check_is_fitted(self.estimator_):
+            self._shrink()
+
+    def __init__prediction_task(self):
+        self.prediction_task = 'regression'
+
+    def get_params(self, deep=True):
+        if deep:
+            return deepcopy({'reg_param': self.reg_param, 'estimator_': self.estimator_,
+                             # 'prediction_task': self.prediction_task,
+                             'shrinkage_scheme_': self.shrinkage_scheme_})
+        return {'reg_param': self.reg_param, 'estimator_': self.estimator_,
+                # 'prediction_task': self.prediction_task,
+                'shrinkage_scheme_': self.shrinkage_scheme_}
+
+    def fit(self, *args, **kwargs):
+        self.estimator_.fit(*args, **kwargs)
+        self._shrink()
+
+    def _shrink(self, reg_param):
+        for tree in self.trees_:
+            tree.shrink(reg_param)
+
+    def predict(self, *args, **kwargs):
+        return self.estimator_.predict(*args, **kwargs)
+
+    def predict_proba(self, *args, **kwargs):
+        if hasattr(self.estimator_, 'predict_proba'):
+            return self.estimator_.predict_proba(*args, **kwargs)
+        else:
+            return NotImplemented
 
-    # remove some features to speed things up
-    X = X[:10, :4]
-    y = y[:10]
-    X, X_test, y_train, y_test = train_test_split(X, y, random_state=42)
+    def score(self, *args, **kwargs):
+        if hasattr(self.estimator_, 'score'):
+            return self.estimator_.score(*args, **kwargs)
+        else:
+            return NotImplemented
 
-    # unit test
-    gam = MultiTaskGAMRegressor(multitask=False)
-    gam.fit(X, y_train)
-    gam2 = MultiTaskGAMRegressor(multitask=True)
-    gam2.fit(X, y_train)
-    preds_orig = gam.predict(X_test)
-    assert np.allclose(preds_orig, gam2.ebms_[-1].predict(X_test))
 
-    # extracted curves + intercept should sum to original predictions
-    feats_extracted = gam2._extract_ebm_features(X_test)
+class HSFIGSRegressor(HSFIGS):
+    def _init_prediction_task(self):
+        self.prediction_task = 'regression'
 
-    # get features for ebm that predicts target
-    feats_extracted_target = feats_extracted[:,
-                                             -len(gam2.term_names_list_[-1]):]
-    # assert feats_extracted_target.shape == (num_samples, num_features)
-    preds_extracted_target = np.sum(feats_extracted_target, axis=1) + \
-        gam2.ebms_[-1].intercept_
-    diff = preds_extracted_target - preds_orig
-    assert np.allclose(preds_extracted_target, preds_orig), diff
-    print('Tests pass successfully')
 
+class HSFIGSClassifier(HSFIGS):
+    def _init_prediction_task(self):
+        self.prediction_task = 'classification'
 
-if __name__ == "__main__":
-    # test_multitask_extraction()
-    # X, y, feature_names = imodels.get_clean_dataset("heart")
-    X, y, feature_names = imodels.get_clean_dataset("bike_sharing")
-    # X, y, feature_names = imodels.get_clean_dataset("diabetes")
 
-    # remove some features to speed things up
-    X = X[:, :2]
-    X, X_test, y_train, y_test = train_test_split(X, y, random_state=42)
+class HSFIGSClassifierCV(HSFIGSClassifier):
+    def __init__(self, estimator_: BaseEstimator,
+                 reg_param_list: List[float] = [0.1, 1, 10, 50, 100, 500], shrinkage_scheme_: str = 'node_based',
+                 cv: int = 3, scoring=None, *args, **kwargs):
+        """Note: args, kwargs are not used but left so that imodels-experiments can still pass redundant args.
+        Cross-validation is used to select the best regularization parameter for hierarchical shrinkage.
+        """
+        super().__init__(estimator_, reg_param=None)
+        self.reg_param_list = np.array(reg_param_list)
+        self.cv = cv
+        self.scoring = scoring
+        self.shrinkage_scheme_ = shrinkage_scheme_
+        # print('estimator', self.estimator_,
+        #       'checks.check_is_fitted(estimator)', checks.check_is_fitted(self.estimator_))
+        # if checks.check_is_fitted(self.estimator_):
+        #     raise Warning('Passed an already fitted estimator,'
+        #                   'but shrinking not applied until fit method is called.')
+
+    def fit(self, X, y, *args, **kwargs):
+        self.scores_ = []
+        for reg_param in self.reg_param_list:
+            est = HSFIGSClassifier(deepcopy(self.estimator_), reg_param)
+            cv_scores = cross_val_score(est, X, y, cv=self.cv, scoring=self.scoring)
+            self.scores_.append(np.mean(cv_scores))
+        self.reg_param = self.reg_param_list[np.argmax(self.scores_)]
+        super().fit(X=X, y=y)
+
+
+class HSFIGSRegressorCV(HSFIGSRegressor):
+    def __init__(self, estimator_: BaseEstimator,
+                 reg_param_list: List[float] = [0.1, 1, 10, 50, 100, 500],
+                 shrinkage_scheme_: str = 'node_based',
+                 cv: int = 3, scoring=None, *args, **kwargs):
+        """Note: args, kwargs are not used but left so that imodels-experiments can still pass redundant args.
+        Cross-validation is used to select the best regularization parameter for hierarchical shrinkage.
+        """
+        super().__init__(estimator_, reg_param=None)
+        self.reg_param_list = np.array(reg_param_list)
+        self.cv = cv
+        self.scoring = scoring
+        self.shrinkage_scheme_ = shrinkage_scheme_
+        # print('estimator', self.estimator_,
+        #       'checks.check_is_fitted(estimator)', checks.check_is_fitted(self.estimator_))
+        # if checks.check_is_fitted(self.estimator_):
+        #     raise Warning('Passed an already fitted estimator,'
+        #                   'but shrinking not applied until fit method is called.')
+
+    def fit(self, X, y):
+        self.scores_ = []
+        for reg_param in self.reg_param_list:
+            est = HSFIGSRegressor(deepcopy(self.estimator_), reg_param)
+            cv_scores = cross_val_score(est, X, y, cv=self.cv, scoring=self.scoring)
+            self.scores_.append(np.mean(cv_scores))
+        self.reg_param = self.reg_param_list[np.argmax(self.scores_)]
+        super().fit(X=X, y=y)
+
+
+if __name__ == '__main__':
+    np.random.seed(15)
+    # X, y = datasets.fetch_california_housing(return_X_y=True)  # regression
+    # X, y = datasets.load_breast_cancer(return_X_y=True)  # binary classification
+    X, y = datasets.load_diabetes(return_X_y=True)  # regression
+    # X = np.random.randn(500, 10)
+    # y = (X[:, 0] > 0).astype(float) + (X[:, 1] > 1).astype(float)
 
-    kwargs = dict(
-        random_state=42,
+    X_train, X_test, y_train, y_test = train_test_split(
+        X, y, test_size=0.33, random_state=10
     )
-    results = defaultdict(list)
-    for gam in tqdm([
-            # AdaBoostRegressor(estimator=MultiTaskGAMRegressor(
-        # multitask=True), n_estimators=2),
-        # MultiTaskGAMRegressor(multitask=True, onehot_prior=True),
-        # MultiTaskGAMRegressor(multitask=True, onehot_prior=False),
-        MultiTaskGAMRegressor(multitask=True, renormalize_features=True),
-        MultiTaskGAMRegressor(multitask=True, renormalize_features=False),
-        # ExplainableBoostingRegressor(n_jobs=1, interactions=0)
-    ]):
-        np.random.seed(42)
-        results["model_name"].append(gam)
-        print('Fitting', results['model_name'][-1])
-        gam.fit(X, y_train)
-        results['test_corr'].append(np.corrcoef(
-            y_test, gam.predict(X_test))[0, 1].round(3))
-        results['test_r2'].append(gam.score(X_test, y_test).round(3))
-        if hasattr(gam, 'lin_model'):
-            print('lin model coef', gam.lin_model.coef_)
-
-    # don't round strings
-    with pd.option_context(
-        "display.max_rows", None, "display.max_columns", None, "display.width", 1000
-    ):
-        print(pd.DataFrame(results).round(3))
+    print('X.shape', X.shape)
+    print('ys', np.unique(y_train))
+
+    # m = HSTree(estimator_=DecisionTreeClassifier(), reg_param=0.1)
+    # m = DecisionTreeClassifier(max_leaf_nodes = 20,random_state=1, max_features=None)
+    m = DecisionTreeRegressor(random_state=42, max_leaf_nodes=20)
+    # print('best alpha', m.reg_param)
+    m.fit(X_train, y_train)
+    # m.predict_proba(X_train)  # just run this
+    print('score', r2_score(y_test, m.predict(X_test)))
+    print('running again....')
+
+    # x = DecisionTreeRegressor(random_state = 42, ccp_alpha = 0.3)
+    # x.fit(X_train,y_train)
+
+    # m = HSTree(estimator_=DecisionTreeRegressor(random_state=42, max_features=None), reg_param=10)
+    # m = HSTree(estimator_=DecisionTreeClassifier(random_state=42, max_features=None), reg_param=0)
+    m = HSFIGSClassifierCV(estimator_=DecisionTreeRegressor(max_leaf_nodes=10, random_state=1),
+                           shrinkage_scheme_='node_based',
+                           reg_param_list=[0.1, 1, 2, 5, 10, 25, 50, 100, 500])
+    # m = ShrunkTreeCV(estimator_=DecisionTreeClassifier())
+
+    # m = HSTreeClassifier(estimator_ = GradientBoostingClassifier(random_state = 10),reg_param = 5)
+    m.fit(X_train, y_train)
+    print('best alpha', m.reg_param)
+    # m.predict_proba(X_train)  # just run this
+    # print('score', m.score(X_test, y_test))
+    print('score', r2_score(y_test, m.predict(X_test)))
```

### Comparing `imodels-1.4.3/imodels/algebraic/marginal_shrinkage_linear_model.py` & `imodels-1.4.4/imodels/algebraic/marginal_shrinkage_linear_model.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/algebraic/slim.py` & `imodels-1.4.4/imodels/algebraic/slim.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/algebraic/tree_gam.py` & `imodels-1.4.4/imodels/algebraic/tree_gam.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/discretization/discretizer.py` & `imodels-1.4.4/imodels/discretization/discretizer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/discretization/mdlp.py` & `imodels-1.4.4/imodels/discretization/mdlp.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/discretization/simple.py` & `imodels-1.4.4/imodels/discretization/simple.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/data.py` & `imodels-1.4.4/imodels/experimental/bartpy/data.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/diagnostics/diagnostics.py` & `imodels-1.4.4/imodels/experimental/bartpy/diagnostics/diagnostics.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/diagnostics/features.py` & `imodels-1.4.4/imodels/experimental/bartpy/diagnostics/features.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/diagnostics/motivation.py` & `imodels-1.4.4/imodels/experimental/bartpy/diagnostics/motivation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/diagnostics/residuals.py` & `imodels-1.4.4/imodels/experimental/bartpy/diagnostics/residuals.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/diagnostics/sampling.py` & `imodels-1.4.4/imodels/experimental/bartpy/diagnostics/sampling.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/diagnostics/trees.py` & `imodels-1.4.4/imodels/experimental/bartpy/diagnostics/trees.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/extensions/baseestimator.py` & `imodels-1.4.4/imodels/experimental/bartpy/extensions/baseestimator.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/extensions/ols.py` & `imodels-1.4.4/imodels/experimental/bartpy/extensions/ols.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/features/featureimportance.py` & `imodels-1.4.4/imodels/experimental/bartpy/features/featureimportance.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/features/featureselection.py` & `imodels-1.4.4/imodels/experimental/bartpy/features/featureselection.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/initializers/initializer.py` & `imodels-1.4.4/imodels/experimental/bartpy/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/initializers/sklearntreeinitializer.py` & `imodels-1.4.4/imodels/experimental/bartpy/initializers/sklearntreeinitializer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/model.py` & `imodels-1.4.4/imodels/experimental/bartpy/model.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/mutation.py` & `imodels-1.4.4/imodels/experimental/bartpy/mutation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/node.py` & `imodels-1.4.4/imodels/experimental/bartpy/node.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/runner.py` & `imodels-1.4.4/imodels/experimental/bartpy/runner.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/leafnode.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/leafnode.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/modelsampler.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/modelsampler.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/oblivioustrees/likelihoodratio.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/oblivioustrees/likelihoodratio.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/oblivioustrees/proposer.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/oblivioustrees/proposer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/oblivioustrees/treemutation.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/oblivioustrees/treemutation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/scalar.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/scalar.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/schedule.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/schedule.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/sigma.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/sigma.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/treemutation.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/treemutation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/unconstrainedtree/likelihoodratio.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/unconstrainedtree/likelihoodratio.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/unconstrainedtree/proposer.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/unconstrainedtree/proposer.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/samplers/unconstrainedtree/treemutation.py` & `imodels-1.4.4/imodels/experimental/bartpy/samplers/unconstrainedtree/treemutation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/sigma.py` & `imodels-1.4.4/imodels/experimental/bartpy/sigma.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/sklearnmodel.py` & `imodels-1.4.4/imodels/experimental/bartpy/sklearnmodel.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/split.py` & `imodels-1.4.4/imodels/experimental/bartpy/split.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/splitcondition.py` & `imodels-1.4.4/imodels/experimental/bartpy/splitcondition.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/trace.py` & `imodels-1.4.4/imodels/experimental/bartpy/trace.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/bartpy/tree.py` & `imodels-1.4.4/imodels/experimental/bartpy/tree.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/figs_ensembles.py` & `imodels-1.4.4/imodels/experimental/figs_ensembles.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/stablelinear.py` & `imodels-1.4.4/imodels/experimental/stablelinear.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/stableskope.py` & `imodels-1.4.4/imodels/experimental/stableskope.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/tree_gam_simple.py` & `imodels-1.4.4/imodels/experimental/tree_gam_simple.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/experimental/util.py` & `imodels-1.4.4/imodels/experimental/util.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/importance/__init__.py` & `imodels-1.4.4/imodels/importance/__init__.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/importance/block_transformers.py` & `imodels-1.4.4/imodels/importance/block_transformers.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/importance/block_transformers_ys.py` & `imodels-1.4.4/imodels/importance/block_transformers_ys.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/importance/local_stumps.py` & `imodels-1.4.4/imodels/importance/local_stumps.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/importance/mdi_plus.py` & `imodels-1.4.4/imodels/importance/mdi_plus.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/importance/ppms.py` & `imodels-1.4.4/imodels/importance/ppms.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/importance/ranking_stability.py` & `imodels-1.4.4/imodels/importance/ranking_stability.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/importance/rf_plus.py` & `imodels-1.4.4/imodels/importance/rf_plus.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_list/bayesian_rule_list/bayesian_rule_list.py` & `imodels-1.4.4/imodels/rule_list/bayesian_rule_list/bayesian_rule_list.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_list/bayesian_rule_list/brl_util.py` & `imodels-1.4.4/imodels/rule_list/bayesian_rule_list/brl_util.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_list/corels_wrapper.py` & `imodels-1.4.4/imodels/rule_list/corels_wrapper.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_list/greedy_rule_list.py` & `imodels-1.4.4/imodels/rule_list/greedy_rule_list.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_list/one_r.py` & `imodels-1.4.4/imodels/rule_list/one_r.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/boosted_rules.py` & `imodels-1.4.4/imodels/rule_set/boosted_rules.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/brs.py` & `imodels-1.4.4/imodels/rule_set/brs.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/fplasso.py` & `imodels-1.4.4/imodels/rule_set/fplasso.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/fpskope.py` & `imodels-1.4.4/imodels/rule_set/fpskope.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/rule_fit.py` & `imodels-1.4.4/imodels/rule_set/rule_fit.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/rule_set.py` & `imodels-1.4.4/imodels/rule_set/rule_set.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/skope_rules.py` & `imodels-1.4.4/imodels/rule_set/skope_rules.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/slipper.py` & `imodels-1.4.4/imodels/rule_set/slipper.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/rule_set/slipper_util.py` & `imodels-1.4.4/imodels/rule_set/slipper_util.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/c45_tree/c45_tree.py` & `imodels-1.4.4/imodels/tree/c45_tree/c45_tree.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/c45_tree/c45_utils.py` & `imodels-1.4.4/imodels/tree/c45_tree/c45_utils.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/cart_ccp.py` & `imodels-1.4.4/imodels/tree/cart_ccp.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/cart_wrapper.py` & `imodels-1.4.4/imodels/tree/cart_wrapper.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/custom_greedy_tree.py` & `imodels-1.4.4/imodels/tree/custom_greedy_tree.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/figs.py` & `imodels-1.4.4/imodels/tree/figs.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/gosdt/pygosdt.py` & `imodels-1.4.4/imodels/tree/gosdt/pygosdt.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/gosdt/pygosdt_helper.py` & `imodels-1.4.4/imodels/tree/gosdt/pygosdt_helper.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/gosdt/pygosdt_shrinkage.py` & `imodels-1.4.4/imodels/tree/gosdt/pygosdt_shrinkage.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/hierarchical_shrinkage.py` & `imodels-1.4.4/imodels/tree/hierarchical_shrinkage.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/iterative_random_forest/iterative_random_forest.py` & `imodels-1.4.4/imodels/tree/iterative_random_forest/iterative_random_forest.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/tao.py` & `imodels-1.4.4/imodels/tree/tao.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/tree/viz_utils.py` & `imodels-1.4.4/imodels/tree/viz_utils.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/arguments.py` & `imodels-1.4.4/imodels/util/arguments.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/automl.py` & `imodels-1.4.4/imodels/util/automl.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/checks.py` & `imodels-1.4.4/imodels/util/checks.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/convert.py` & `imodels-1.4.4/imodels/util/convert.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/data_util.py` & `imodels-1.4.4/imodels/util/data_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from scipy.sparse import issparse
 from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import OneHotEncoder
 
 from imodels.util.tree_interaction_utils import make_rj, make_vp
 
+
 DSET_CLASSIFICATION_KWARGS = {
     # classification
+    'iris': {'dataset_name': 61, 'data_source': 'openml'},
     "pima_diabetes": {"dataset_name": 40715, "data_source": "openml"},
     "sonar": {"dataset_name": "sonar", "data_source": "pmlb"},
     "heart": {"dataset_name": "heart", "data_source": "imodels"},
     "diabetes": {"dataset_name": "diabetes", "data_source": "pmlb"},
     "breast_cancer_recurrence": {
         "dataset_name": "breast_cancer",
         "data_source": "imodels",
@@ -55,38 +57,41 @@
     "satellite_image": {"dataset_name": "294_satellite_image", "data_source": "pmlb"},
     "california_housing": {
         "dataset_name": "california_housing",
         "data_source": "sklearn",
     },
     # 'breast_tumor': {'dataset_name': '1201_BNG_breastTumor', 'data_source': 'pmlb' # v big
 }
-DSET_MULTITASK_NAMES = ['3s-bbc1000', '3s-guardian1000', '3s-inter3000', '3s-reuters1000',
-                        'birds', 'cal500', 'chd_49', 'corel16k001', 'corel16k002',
-                        'corel16k003', 'corel16k004', 'corel16k005', 'corel16k006',
-                        'corel16k007', 'corel16k008', 'corel16k009', 'corel16k010',
-                        'corel5k', 'emotions', 'flags', 'foodtruck', 'genbase', 'image',
-                        'mediamill', 'scene', 'stackex_chemistry', 'stackex_chess',
-                        'stackex_cooking', 'stackex_cs', 'water-quality', 'yeast', 'yelp']
-DSET_MULTITASK_KWARGS = {
+DSET_CLASSIFICATION_MULTITASK_NAMES = [
+    '3s-bbc1000', '3s-guardian1000', '3s-inter3000', '3s-reuters1000',
+    'birds', 'cal500', 'chd_49', 'corel16k001', 'corel16k002',
+    'corel16k003', 'corel16k004', 'corel16k005', 'corel16k006',
+    'corel16k007', 'corel16k008', 'corel16k009', 'corel16k010',
+    'corel5k', 'emotions', 'flags', 'foodtruck', 'genbase', 'image',
+    'mediamill', 'scene', 'stackex_chemistry', 'stackex_chess',
+    'stackex_cooking', 'stackex_cs', 'water-quality', 'yeast', 'yelp']
+DSET_CLASSIFICATION_MULTITASK_KWARGS = {
     name + '_multitask': {"dataset_name": name, "data_source": "imodels-multitask"}
-    for name in DSET_MULTITASK_NAMES
+    for name in DSET_CLASSIFICATION_MULTITASK_NAMES
 }
 DSET_KWARGS = {
     **DSET_CLASSIFICATION_KWARGS, **DSET_REGRESSION_KWARGS,
-    **DSET_MULTITASK_KWARGS}
+    **DSET_CLASSIFICATION_MULTITASK_KWARGS}
 
 
 def get_clean_dataset(
     dataset_name: str,
     data_source: str = "imodels",
     data_path=os.path.expanduser("~/cache_imodels_data"),
     convertna: bool = True,
     test_size: float = None,
     random_state: int = 42,
     verbose=True,
+    return_target_col_names: bool = False,
+    override_cache: bool = False,
 ) -> Tuple[np.ndarray, np.ndarray, list]:
     """Fetch clean data (as numpy arrays) from various sources including imodels, pmlb, openml, and sklearn.
     If data is not downloaded, will download and cache. Otherwise will load locally.
     Cleans features so that they are type float and features names don't start with a digit.
 
     Parameters
     ----------
@@ -98,23 +103,29 @@
     data_path: str
         path to load/save data (default: 'data')
     test_size: float, optional
         if not None, will split data into train and test sets (with fraction test_size in test set)
         & change the return signature to `X_train, X_test, y_train, y_test, feature_names`
     random_state: int, optional
         if test_size is not None, will use this random state to split data
+    return_target_col_names: bool, optional
+        if True, will return target columns for multitask datasets as final return value
+    override_cache: bool, False
+        if True, will override the downloaded cache for a dataset
 
 
     Returns
     -------
     X: np.ndarray
         features
     y: np.ndarray
         outcome
     feature_names: list
+    (if passing test_size, will return more outputs)
+    (if multitask dataset, will return target_col_names as well)
 
     Example
     -------
     ```
     # download compas dataset from imodels
     X, y, feature_names = imodels.get_clean_dataset('compas_two_year_clean', data_source='imodels')
     # download ionosphere dataset from pmlb
@@ -145,34 +156,37 @@
 
         def _split(X, y, feature_names):
             return X, y, feature_names
 
     if data_source == "imodels":
         if not dataset_name.endswith("csv"):
             dataset_name = dataset_name + ".csv"
-        if not os.path.isfile(dataset_name):
+        if not os.path.isfile(dataset_name) or override_cache:
             _download_imodels_dataset(dataset_name, data_path)
         df = pd.read_csv(oj(data_path, "imodels_data", dataset_name))
         X, y = df.iloc[:, :-1].values, df.iloc[:, -1].values
         feature_names = df.columns.values[:-1]
         if convertna:
             X = np.nan_to_num(X.astype("float32"))
         return _split(X, y, _clean_feat_names(feature_names))
     elif data_source == 'imodels-multitask':
         if not dataset_name.endswith("csv"):
             dataset_name = dataset_name + ".csv"
-        if not os.path.isfile(dataset_name):
+        if not os.path.isfile(dataset_name) or override_cache:
             _download_imodels_multitask_dataset(dataset_name, data_path)
         df = pd.read_csv(oj(data_path, "imodels_multitask_data", dataset_name))
         target_cols = [col for col in df.columns if col.endswith('__target')]
         feature_names = [col for col in df.columns if col not in target_cols]
         X, y = df[feature_names].values, df[target_cols].values
         if convertna:
             X = np.nan_to_num(X.astype("float32"))
-        return _split(X, y, _clean_feat_names(feature_names))
+        if return_target_col_names:
+            return *(_split(X, y, _clean_feat_names(feature_names))), _clean_feat_names(target_cols)
+        else:
+            return _split(X, y, _clean_feat_names(feature_names))
 
     elif data_source == "pmlb":
         from pmlb import fetch_data
 
         feature_names = list(
             fetch_data(
                 dataset_name,
@@ -239,15 +253,19 @@
     if data_id == "1182":  # adult, positive is ">50K"
         y = (y == ">50K").astype(int)
     return y
 
 
 def _clean_feat_names(feature_names):
     # shouldn't start with a digit
-    return ["X_" + x if x[0].isdigit() else x for x in feature_names]
+    feature_names = ["X_" + x if x[0].isdigit() else x for x in feature_names]
+    # shouldn't end with __target
+    feature_names = [x if not x.endswith(
+        "__target") else x[:-8] for x in feature_names]
+    return feature_names
 
 
 def _clean_features(X):
     if issparse(X):
         X = X.toarray()
     try:
         return X.astype(float)
@@ -276,19 +294,22 @@
         f.write(r.text)
 
 
 def _download_imodels_multitask_dataset(dataset_fname, data_path: str):
     dataset_fname = dataset_fname.split(
         "/")[-1]  # remove anything about the path
     download_path = f"https://huggingface.co/datasets/imodels/multitask-tabular-datasets/raw/main/{dataset_fname}"
+    download_path_large = f'https://huggingface.co/datasets/imodels/multitask-tabular-datasets/resolve/main/{dataset_fname}'
     r = requests.get(download_path)
     if r.status_code == 404:
         raise Exception(
             f"404 Error for dataset {dataset_fname} (see valid files at https://huggingface.co/datasets/imodels/multitask-tabular-datasets)"
         )
+    elif 'git-lfs' in r.text:
+        r = requests.get(download_path_large)
 
     os.makedirs(oj(data_path, "imodels_multitask_data"), exist_ok=True)
     with open(oj(data_path, "imodels_multitask_data", dataset_fname), "w") as f:
         f.write(r.text)
 
 
 def encode_categories(X, features, encoder=None):
```

### Comparing `imodels-1.4.3/imodels/util/distillation.py` & `imodels-1.4.4/imodels/util/distillation.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/explain_errors.py` & `imodels-1.4.4/imodels/util/explain_errors.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/extract.py` & `imodels-1.4.4/imodels/util/extract.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/metrics.py` & `imodels-1.4.4/imodels/util/metrics.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/neural_nets.py` & `imodels-1.4.4/imodels/util/neural_nets.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/prune.py` & `imodels-1.4.4/imodels/util/prune.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/rule.py` & `imodels-1.4.4/imodels/util/rule.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/score.py` & `imodels-1.4.4/imodels/util/score.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Tuple
 from warnings import warn
 
 import pandas as pd
 import numpy as np
-from sklearn.utils import indices_to_mask
+from sklearn.utils._mask import indices_to_mask
 from sklearn.linear_model import Lasso, LogisticRegression
 from sklearn.linear_model._coordinate_descent import _alpha_grid
 from sklearn.model_selection import cross_val_score
 
 from imodels.util.rule import Rule
 
 
@@ -88,15 +88,16 @@
                                                      max_rules=max_rules,
                                                      cv=cv,
                                                      random_state=random_state)
     else:
         raise ValueError("Invalid alpha and max_rules passed")
 
     if prediction_task == 'regression':
-        lin_model = Lasso(alpha=final_alpha, random_state=random_state, max_iter=2000)
+        lin_model = Lasso(alpha=final_alpha,
+                          random_state=random_state, max_iter=2000)
     else:
         lin_model = LogisticRegression(
             penalty=penalty, C=(1 / final_alpha), solver='liblinear',
             random_state=random_state, max_iter=200)
 
     lin_model.fit(X, y)
 
@@ -106,15 +107,15 @@
 
     nonzero_rules = []
     coef_zero_threshold = 1e-6 / np.mean(np.abs(y))
     for r, w, s in zip(rules, coef_[-len(rules):], support):
         if abs(w) > coef_zero_threshold:
             nonzero_rules.append(Rule(r, args=[w], support=s))
             coefs.append(w)
-    
+
     return nonzero_rules, coefs, lin_model.intercept_
 
 
 def get_best_alpha_under_max_rules(X, y, rules: List[str],
                                    penalty='l1',
                                    prediction_task='regression',
                                    max_rules=30,
@@ -135,15 +136,15 @@
         if prediction_task == 'regression':
             m = Lasso(alpha=alpha, random_state=random_state, max_iter=2000)
             cv_scoring = 'neg_mean_squared_error'
         else:
             m = LogisticRegression(
                 penalty=penalty, C=(1 / alpha), solver='liblinear', random_state=random_state)
             cv_scoring = 'accuracy'
-        
+
         m.fit(X, y)
         rule_coefs = m.coef_.flatten()
         rule_count = np.sum(np.abs(rule_coefs) > coef_zero_threshold)
 
         if rule_count > max_rules:
             break
 
@@ -152,9 +153,9 @@
             alpha_scores.append(np.mean(fold_scores))
 
     if cv and np.all(alpha_scores != alpha_scores[0]):
         # check for rare case in which diff alphas lead to identical scores
         final_alpha = alphas[np.argmax(alpha_scores)]
     else:
         final_alpha = alphas[i - 1]
-        
+
     return final_alpha
```

### Comparing `imodels-1.4.3/imodels/util/tree.py` & `imodels-1.4.4/imodels/util/tree.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels/util/tree_interaction_utils.py` & `imodels-1.4.4/imodels/util/tree_interaction_utils.py`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/imodels.egg-info/PKG-INFO` & `imodels-1.4.4/imodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodels
-Version: 1.4.3
+Version: 1.4.4
 Summary: Implementations of various interpretable models
 Home-page: https://github.com/csinva/imodels
 Author: Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen, Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others
 Author-email: chandan_singh@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodels Version: 1.4.3 Summary: Implementations of
+Metadata-Version: 2.1 Name: imodels Version: 1.4.4 Summary: Implementations of
 various interpretable models Home-page: https://github.com/csinva/imodels
 Author: Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen,
 Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others Author-email:
 chandan_singh@berkeley.edu Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9.0 Description-Content-Type: text/
 markdown Provides-Extra: dev
```

### Comparing `imodels-1.4.3/imodels.egg-info/SOURCES.txt` & `imodels-1.4.4/imodels.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 imodels.egg-info/requires.txt
 imodels.egg-info/top_level.txt
 imodels/algebraic/__init__.py
 imodels/algebraic/gam_multitask.py
 imodels/algebraic/marginal_shrinkage_linear_model.py
 imodels/algebraic/slim.py
 imodels/algebraic/tree_gam.py
+imodels/algebraic/tree_gam_minimal.py
 imodels/discretization/__init__.py
 imodels/discretization/discretizer.py
 imodels/discretization/mdlp.py
 imodels/discretization/simple.py
 imodels/experimental/__init__.py
 imodels/experimental/figs_ensembles.py
 imodels/experimental/figs_shrinkage.py
@@ -117,14 +118,15 @@
 imodels/util/__init__.py
 imodels/util/arguments.py
 imodels/util/automl.py
 imodels/util/checks.py
 imodels/util/convert.py
 imodels/util/data_util.py
 imodels/util/distillation.py
+imodels/util/ensemble.py
 imodels/util/explain_errors.py
 imodels/util/extract.py
 imodels/util/metrics.py
 imodels/util/neural_nets.py
 imodels/util/prune.py
 imodels/util/rule.py
 imodels/util/score.py
```

### Comparing `imodels-1.4.3/license.md` & `imodels-1.4.4/license.md`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/readme.md` & `imodels-1.4.4/readme.md`

 * *Files identical despite different names*

### Comparing `imodels-1.4.3/setup.py` & `imodels-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'corels',  # optionally requires corels for optimalrulelistclassifier
     'gosdt-deprecated',  # optionally requires gosdt for optimaltreeclassifier
     'irf',  # optionally require irf for iterativeRandomForestClassifier
 ]
 
 setuptools.setup(
     name="imodels",
-    version="1.4.3",
+    version="1.4.4",
     author="Chandan Singh, Keyan Nasseri, Matthew Epland, Yan Shuo Tan, Omer Ronen, Tiffany Tang, Abhineet Agarwal, Theo Saarinen, Bin Yu, and others",
     author_email="chandan_singh@berkeley.edu",
     description="Implementations of various interpretable models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/csinva/imodels",
     packages=setuptools.find_packages(
```

