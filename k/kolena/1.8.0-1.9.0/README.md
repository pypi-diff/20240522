# Comparing `tmp/kolena-1.8.0.tar.gz` & `tmp/kolena-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena-1.8.0.tar", max compression
+gzip compressed data, was "kolena-1.9.0.tar", max compression
```

## Comparing `kolena-1.8.0.tar` & `kolena-1.9.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11346 2024-03-06 02:07:53.513324 kolena-1.8.0/LICENSE
--rw-r--r--   0        0        0      556 2024-03-06 02:07:53.513324 kolena-1.8.0/LICENSE_HEADER
--rw-r--r--   0        0        0     2089 2024-03-06 02:07:53.513324 kolena-1.8.0/README.md
--rw-r--r--   0        0        0      775 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     5041 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     2451 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/event.py
--rw-r--r--   0        0        0     5960 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v2/__init__.py
--rw-r--r--   0        0        0     1954 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v2/dataset.py
--rw-r--r--   0        0        0     1437 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v2/model.py
--rw-r--r--   0        0        0      952 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_api/v2/search.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/classification/__init__.py
--rw-r--r--   0        0        0    13253 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/classification/utils.py
--rw-r--r--   0        0        0     1151 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/instance_segmentation/__init__.py
--rw-r--r--   0        0        0     1850 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/instance_segmentation/dataset.py
--rw-r--r--   0        0        0     5056 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/instance_segmentation/evaluator.py
--rw-r--r--   0        0        0     3013 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/instance_segmentation/workflow.py
--rw-r--r--   0        0        0     1581 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0    10321 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/object_detection/dataset.py
--rw-r--r--   0        0        0     6471 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/object_detection/evaluator.py
--rw-r--r--   0        0        0    18178 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/object_detection/evaluator_multiclass.py
--rw-r--r--   0        0        0    12548 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/object_detection/evaluator_single_class.py
--rw-r--r--   0        0        0    15086 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0     7016 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/object_detection/workflow.py
--rw-r--r--   0        0        0      757 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/search/__init__.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/search/_internal/__init__.py
--rw-r--r--   0        0        0     2027 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/search/_internal/datatypes.py
--rw-r--r--   0        0        0     6401 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/search/embeddings.py
--rw-r--r--   0        0        0      677 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/workflow/__init__.py
--rw-r--r--   0        0        0     4096 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_experimental/workflow/thresholded.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      785 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     5631 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5777 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      990 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2296 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/dataframes/transformers.py
--rw-r--r--   0        0        0     3337 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0    12690 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3776 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1173 2024-03-06 02:07:53.621324 kolena-1.8.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1072 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     4884 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     6412 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0      936 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/krequests_v2.py
--rw-r--r--   0        0        0     3523 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0     5845 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1142 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0    13829 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/annotation.py
--rw-r--r--   0        0        0     5439 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/asset.py
--rw-r--r--   0        0        0      908 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/dataset/__init__.py
--rw-r--r--   0        0        0     2773 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/dataset/_common.py
--rw-r--r--   0        0        0    15659 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/dataset/dataset.py
--rw-r--r--   0        0        0     9302 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/dataset/evaluation.py
--rw-r--r--   0        0        0     2661 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/errors.py
--rw-r--r--   0        0        0     6412 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/initialize.py
--rw-r--r--   0        0        0     3931 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/io.py
--rw-r--r--   0        0        0     1206 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/metrics/__init__.py
--rw-r--r--   0        0        0     5329 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/metrics/_formula.py
--rw-r--r--   0        0        0    15311 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/metrics/_geometry.py
--rw-r--r--   0        0        0     2620 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0     7047 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6893 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     4225 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     1584 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3459 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    13835 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    12169 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4418 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4331 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      778 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/io.py
--rw-r--r--   0        0        0     1256 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/metrics.py
--rw-r--r--   0        0        0    10598 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    10845 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/plot.py
--rw-r--r--   0        0        0    18746 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    26597 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    12093 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    16067 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0      841 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/visualization/__init__.py
--rw-r--r--   0        0        0     6151 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/visualization/_activation_map.py
--rw-r--r--   0        0        0     1910 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/visualization/_utils.py
--rw-r--r--   0        0        0     9419 2024-03-06 02:07:53.625324 kolena-1.8.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3035 2024-03-06 02:08:13.229351 kolena-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 kolena-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-03-13 02:16:47.010884 kolena-1.9.0/LICENSE
+-rw-r--r--   0        0        0      556 2024-03-13 02:16:47.010884 kolena-1.9.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     2089 2024-03-13 02:16:47.010884 kolena-1.9.0/README.md
+-rw-r--r--   0        0        0      775 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     5041 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     2451 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/event.py
+-rw-r--r--   0        0        0     5960 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v2/__init__.py
+-rw-r--r--   0        0        0     1954 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v2/dataset.py
+-rw-r--r--   0        0        0     1437 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v2/model.py
+-rw-r--r--   0        0        0      952 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_api/v2/search.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_experimental/classification/__init__.py
+-rw-r--r--   0        0        0    13253 2024-03-13 02:16:47.114885 kolena-1.9.0/kolena/_experimental/classification/utils.py
+-rw-r--r--   0        0        0     1151 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/instance_segmentation/__init__.py
+-rw-r--r--   0        0        0     1850 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/instance_segmentation/dataset.py
+-rw-r--r--   0        0        0     5056 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/instance_segmentation/evaluator.py
+-rw-r--r--   0        0        0     3013 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/instance_segmentation/workflow.py
+-rw-r--r--   0        0        0     1581 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0    10321 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/object_detection/dataset.py
+-rw-r--r--   0        0        0     6471 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/object_detection/evaluator.py
+-rw-r--r--   0        0        0    18178 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/object_detection/evaluator_multiclass.py
+-rw-r--r--   0        0        0    12548 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/object_detection/evaluator_single_class.py
+-rw-r--r--   0        0        0    15086 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0     7016 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/object_detection/workflow.py
+-rw-r--r--   0        0        0      757 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/search/__init__.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/search/_internal/__init__.py
+-rw-r--r--   0        0        0     2027 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/search/_internal/datatypes.py
+-rw-r--r--   0        0        0     6401 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/search/embeddings.py
+-rw-r--r--   0        0        0      677 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/workflow/__init__.py
+-rw-r--r--   0        0        0     4096 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_experimental/workflow/thresholded.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      785 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     5631 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5777 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      990 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2296 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/dataframes/transformers.py
+-rw-r--r--   0        0        0     3337 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0    12690 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3776 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1173 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1072 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     4884 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     6412 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0      936 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/krequests_v2.py
+-rw-r--r--   0        0        0     3523 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0     5845 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1142 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0    13829 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/annotation.py
+-rw-r--r--   0        0        0     5439 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/asset.py
+-rw-r--r--   0        0        0      908 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/dataset/__init__.py
+-rw-r--r--   0        0        0     2773 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/dataset/_common.py
+-rw-r--r--   0        0        0    15456 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/dataset/dataset.py
+-rw-r--r--   0        0        0     9302 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/dataset/evaluation.py
+-rw-r--r--   0        0        0     2661 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/errors.py
+-rw-r--r--   0        0        0     6355 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/initialize.py
+-rw-r--r--   0        0        0     3931 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/io.py
+-rw-r--r--   0        0        0     1206 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/metrics/__init__.py
+-rw-r--r--   0        0        0     5329 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/metrics/_formula.py
+-rw-r--r--   0        0        0    15311 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/metrics/_geometry.py
+-rw-r--r--   0        0        0     2620 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0     7047 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6893 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     4225 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     1584 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3459 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13835 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    12169 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4418 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4331 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      778 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/io.py
+-rw-r--r--   0        0        0     1256 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/metrics.py
+-rw-r--r--   0        0        0    10598 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10845 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    18746 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    26597 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    12093 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    16067 2024-03-13 02:16:47.118885 kolena-1.9.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0      841 2024-03-13 02:16:47.122885 kolena-1.9.0/kolena/workflow/visualization/__init__.py
+-rw-r--r--   0        0        0     6151 2024-03-13 02:16:47.122885 kolena-1.9.0/kolena/workflow/visualization/_activation_map.py
+-rw-r--r--   0        0        0     1910 2024-03-13 02:16:47.122885 kolena-1.9.0/kolena/workflow/visualization/_utils.py
+-rw-r--r--   0        0        0     9419 2024-03-13 02:16:47.122885 kolena-1.9.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3035 2024-03-13 02:17:04.031032 kolena-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 kolena-1.9.0/PKG-INFO
```

### Comparing `kolena-1.8.0/LICENSE` & `kolena-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/LICENSE_HEADER` & `kolena-1.9.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/README.md` & `kolena-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/__init__.py` & `kolena-1.9.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/__init__.py` & `kolena-1.9.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/__init__.py` & `kolena-1.9.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/batched_load.py` & `kolena-1.9.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/client_log.py` & `kolena-1.9.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/core.py` & `kolena-1.9.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/event.py` & `kolena-1.9.0/kolena/_api/v1/event.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/generic.py` & `kolena-1.9.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/repository.py` & `kolena-1.9.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/token.py` & `kolena-1.9.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v1/workflow.py` & `kolena-1.9.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v2/__init__.py` & `kolena-1.9.0/kolena/_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v2/dataset.py` & `kolena-1.9.0/kolena/_api/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v2/model.py` & `kolena-1.9.0/kolena/_api/v2/model.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_api/v2/search.py` & `kolena-1.9.0/kolena/_api/v2/search.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/__init__.py` & `kolena-1.9.0/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/classification/__init__.py` & `kolena-1.9.0/kolena/_experimental/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/classification/utils.py` & `kolena-1.9.0/kolena/_experimental/classification/utils.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/instance_segmentation/__init__.py` & `kolena-1.9.0/kolena/_experimental/instance_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/instance_segmentation/dataset.py` & `kolena-1.9.0/kolena/_experimental/instance_segmentation/dataset.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/instance_segmentation/evaluator.py` & `kolena-1.9.0/kolena/_experimental/instance_segmentation/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/instance_segmentation/workflow.py` & `kolena-1.9.0/kolena/_experimental/instance_segmentation/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/object_detection/__init__.py` & `kolena-1.9.0/kolena/_experimental/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/object_detection/dataset.py` & `kolena-1.9.0/kolena/_experimental/object_detection/dataset.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/object_detection/evaluator.py` & `kolena-1.9.0/kolena/_experimental/object_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/object_detection/evaluator_multiclass.py` & `kolena-1.9.0/kolena/_experimental/object_detection/evaluator_multiclass.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/object_detection/evaluator_single_class.py` & `kolena-1.9.0/kolena/_experimental/object_detection/evaluator_single_class.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/object_detection/utils.py` & `kolena-1.9.0/kolena/_experimental/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/object_detection/workflow.py` & `kolena-1.9.0/kolena/_experimental/object_detection/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/search/__init__.py` & `kolena-1.9.0/kolena/_experimental/search/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/search/_internal/__init__.py` & `kolena-1.9.0/kolena/_experimental/search/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/search/_internal/datatypes.py` & `kolena-1.9.0/kolena/_experimental/search/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/search/embeddings.py` & `kolena-1.9.0/kolena/_experimental/search/embeddings.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/workflow/__init__.py` & `kolena-1.9.0/kolena/_experimental/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_experimental/workflow/thresholded.py` & `kolena-1.9.0/kolena/_experimental/workflow/thresholded.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_extras/__init__.py` & `kolena-1.9.0/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_extras/metrics/__init__.py` & `kolena-1.9.0/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_extras/metrics/sklearn.py` & `kolena-1.9.0/kolena/_extras/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/__init__.py` & `kolena-1.9.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/batched_load.py` & `kolena-1.9.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/cli.py` & `kolena-1.9.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/consts.py` & `kolena-1.9.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/dataframes/__init__.py` & `kolena-1.9.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/dataframes/transformers.py` & `kolena-1.9.0/kolena/_utils/dataframes/transformers.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/dataframes/validators.py` & `kolena-1.9.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/datatypes.py` & `kolena-1.9.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/endpoints.py` & `kolena-1.9.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/frozen.py` & `kolena-1.9.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/geometry.py` & `kolena-1.9.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/inference_validators.py` & `kolena-1.9.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/instrumentation.py` & `kolena-1.9.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/krequests.py` & `kolena-1.9.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/krequests_v2.py` & `kolena-1.9.0/kolena/_utils/krequests_v2.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/log.py` & `kolena-1.9.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/repository.py` & `kolena-1.9.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/serde.py` & `kolena-1.9.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/state.py` & `kolena-1.9.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/_utils/validators.py` & `kolena-1.9.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/annotation.py` & `kolena-1.9.0/kolena/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/asset.py` & `kolena-1.9.0/kolena/asset.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/dataset/__init__.py` & `kolena-1.9.0/kolena/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/dataset/_common.py` & `kolena-1.9.0/kolena/dataset/_common.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/dataset/dataset.py` & `kolena-1.9.0/kolena/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 from kolena._utils.batched_load import upload_data_frame
 from kolena._utils.consts import BatchSize
 from kolena._utils.dataframes.transformers import df_apply
 from kolena._utils.dataframes.transformers import json_normalize
 from kolena._utils.datatypes import _deserialize_dataobject
 from kolena._utils.datatypes import _serialize_dataobject
 from kolena._utils.datatypes import DATA_TYPE_FIELD
-from kolena._utils.datatypes import TypedDataObject
 from kolena._utils.endpoints import get_dataset_url
 from kolena._utils.instrumentation import with_event
 from kolena._utils.serde import from_dict
 from kolena._utils.state import API_V2
 from kolena.dataset._common import COL_DATAPOINT
 from kolena.dataset._common import COL_DATAPOINT_ID_OBJECT
 from kolena.dataset._common import DEFAULT_SOURCES
@@ -87,21 +86,16 @@
     "application/pdf": DatapointType.DOCUMENT.value,
     "text": DatapointType.DOCUMENT.value,
     "video": DatapointType.VIDEO.value,
     "audio": DatapointType.AUDIO.value,
 }
 
 
-def _dataobject_type(obj: TypedDataObject) -> str:
-    obj_type = obj._data_type()
-    return f"{obj_type._data_category()}/{obj_type.value}"
-
-
 def _get_datapoint_type(mimetype_str: str) -> Optional[str]:
-    main_type, sub_type = mimetype_str.split("/")
+    main_type, _ = mimetype_str.split("/")
     return _DATAPOINT_TYPE_MAP.get(mimetype_str, None) or _DATAPOINT_TYPE_MAP.get(main_type, None)
 
 
 def _normalize_url(x: str) -> str:
     url = urlparse(x)
     return url._replace(query="", fragment="").geturl()
```

### Comparing `kolena-1.8.0/kolena/dataset/evaluation.py` & `kolena-1.9.0/kolena/dataset/evaluation.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/errors.py` & `kolena-1.9.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/initialize.py` & `kolena-1.9.0/kolena/initialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from kolena.errors import InputValidationError
 from kolena.errors import MissingTokenError
 
 
 def initialize(
     *args: Any,
     api_token: Optional[str] = None,
-    verbose: bool = False,
+    verbose: bool = True,
     proxies: Optional[Dict[str, str]] = None,
     **kwargs: Any,
 ) -> None:
     """
     Initialize a client session.
 
     !!! tip
@@ -53,15 +53,15 @@
     Retrieve an API token from the [:kolena-developer-16: Developer](https://app.kolena.com/redirect/developer) page and
     make it available through one of the following options before initializing:
 
     1. Directly through the `api_token` keyword argument
     ```python
     import kolena
 
-    kolena.initialize(api_token=your_token, verbose=True)
+    kolena.initialize(api_token=your_token)
     ```
 
     2. Populate the `KOLENA_TOKEN` environment variable and call `kolena.initialize()`:
     ```bash
     export KOLENA_TOKEN="********"
     ```
 
@@ -88,20 +88,20 @@
         Step3 -->|Yes| End
     ```
 
     !!! note
         As of version 0.29.0: the `entity` argument is no longer needed; the signature `initialize(entity, api_token)`
         has been deprecated and replaced by `initialize(api_token)`.
 
-    :param api_token: Optionally provide an API token, otherwise attempts to find a token in `$KOLENA_TOKEN`
+    :param api_token: Directly provide an API token, otherwise attempts to find a token in `$KOLENA_TOKEN`
         or your `.netrc` file. This token is a secret and should be treated with caution.
-    :param verbose: Optionally configure client to run in verbose mode, providing more information about execution. All
-        logging events are emitted as Python standard library `logging` events from the `"kolena"` logger as well as
+    :param verbose: Run the client in verbose mode, providing more information about execution. All logging
+        events are emitted as Python standard library `logging` events from the `"kolena"` logger as well as
         to stdout/stderr directly.
-    :param proxies: Optionally configure client to run with `http` or `https` proxies. The `proxies` parameter
+    :param proxies: Run the client with `http` or `https` proxies. The `proxies` parameter
         is passed through to the `requests` package and can be
         [configured accordingly](https://requests.readthedocs.io/en/latest/user/advanced/#proxies).
     :raises InvalidTokenError: The provided `api_token` is not valid.
     :raises InputValidationError: The provided combination or number of args is not valid.
     :raises MissingTokenError: An API token could not be found.
     """
     log.info("Attempting to initialize client...")
```

### Comparing `kolena-1.8.0/kolena/io.py` & `kolena-1.9.0/kolena/io.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/metrics/__init__.py` & `kolena-1.9.0/kolena/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/metrics/_formula.py` & `kolena-1.9.0/kolena/metrics/_formula.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/metrics/_geometry.py` & `kolena-1.9.0/kolena/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/__init__.py` & `kolena-1.9.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/_datatypes.py` & `kolena-1.9.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/_validators.py` & `kolena-1.9.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/annotation.py` & `kolena-1.9.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/asset.py` & `kolena-1.9.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/define_workflow.py` & `kolena-1.9.0/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/evaluator.py` & `kolena-1.9.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/evaluator_function.py` & `kolena-1.9.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/ground_truth.py` & `kolena-1.9.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/inference.py` & `kolena-1.9.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/io.py` & `kolena-1.9.0/kolena/workflow/io.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/metrics.py` & `kolena-1.9.0/kolena/workflow/metrics.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/model.py` & `kolena-1.9.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/plot.py` & `kolena-1.9.0/kolena/workflow/plot.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/test_case.py` & `kolena-1.9.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/test_run.py` & `kolena-1.9.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/test_sample.py` & `kolena-1.9.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/test_suite.py` & `kolena-1.9.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/visualization/__init__.py` & `kolena-1.9.0/kolena/workflow/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/visualization/_activation_map.py` & `kolena-1.9.0/kolena/workflow/visualization/_activation_map.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/visualization/_utils.py` & `kolena-1.9.0/kolena/workflow/visualization/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/kolena/workflow/workflow.py` & `kolena-1.9.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-1.8.0/pyproject.toml` & `kolena-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena"
-version = "1.8.0"  # version is automatically set to latest git tag during release process
+version = "1.9.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning testing platform."
 authors = ["Kolena Engineering <eng@kolena.com>"]
 homepage = "https://kolena.com"
 documentation = "https://docs.kolena.com"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena-1.8.0/PKG-INFO` & `kolena-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena
-Version: 1.8.0
+Version: 1.9.0
 Summary: Client for Kolena's machine learning testing platform.
 Home-page: https://kolena.com
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.com
 Requires-Python: >=3.8,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena Version: 1.8.0 Summary: Client for Kolena's
+Metadata-Version: 2.1 Name: kolena Version: 1.9.0 Summary: Client for Kolena's
 machine learning testing platform. Home-page: https://kolena.com License:
 Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena Engineering Author-email:
 eng@kolena.com Requires-Python: >=3.8,<3.13 Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

