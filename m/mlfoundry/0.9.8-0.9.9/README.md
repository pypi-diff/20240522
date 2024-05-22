# Comparing `tmp/mlfoundry-0.9.8.tar.gz` & `tmp/mlfoundry-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.9.8.tar", max compression
+gzip compressed data, was "mlfoundry-0.9.9.tar", max compression
```

## Comparing `mlfoundry-0.9.8.tar` & `mlfoundry-0.9.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     3165 2023-09-17 13:41:19.060412 mlfoundry-0.9.8/README.md
--rw-r--r--   0        0        0      941 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0    32966 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1840 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      932 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2768 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/constants.py
--rw-r--r--   0        0        0     1392 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/enums.py
--rw-r--r--   0        0        0      383 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     2037 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      774 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/transformers_registry.py
--rw-r--r--   0        0        0      724 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15423 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22410 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      153 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0    12820 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     3128 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    20108 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5952 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0       50 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-09-17 13:41:19.080412 mlfoundry-0.9.8/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    50888 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    50309 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4468 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/run_utils.py
--rw-r--r--   0        0        0    10048 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4615 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-09-17 13:41:19.084412 mlfoundry-0.9.8/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3456 2023-09-17 13:41:34.948750 mlfoundry-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     4664 1970-01-01 00:00:00.000000 mlfoundry-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     3165 2023-10-04 11:42:52.677186 mlfoundry-0.9.9/README.md
+-rw-r--r--   0        0        0      941 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0    32966 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1840 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      932 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2768 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/constants.py
+-rw-r--r--   0        0        0     1392 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/enums.py
+-rw-r--r--   0        0        0      383 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     2037 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      774 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/transformers_registry.py
+-rw-r--r--   0        0        0      724 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15423 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22410 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      153 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0    12820 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3128 2023-10-04 11:42:52.693187 mlfoundry-0.9.9/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    20108 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5952 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0       50 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    50888 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    50309 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4468 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0    10048 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4615 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-10-04 11:42:52.697187 mlfoundry-0.9.9/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3464 2023-10-04 11:43:06.633331 mlfoundry-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 mlfoundry-0.9.9/PKG-INFO
```

### Comparing `mlfoundry-0.9.8/README.md` & `mlfoundry-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/__init__.py` & `mlfoundry-0.9.9/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/__main__.py` & `mlfoundry-0.9.9/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/amplitude.py` & `mlfoundry-0.9.9/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.9.9/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/background/interface.py` & `mlfoundry-0.9.9/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/background/sender.py` & `mlfoundry-0.9.9/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/background/system_metrics.py` & `mlfoundry-0.9.9/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/background/utils.py` & `mlfoundry-0.9.9/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.9.9/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/cli/commands/download.py` & `mlfoundry-0.9.9/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/cli/commands/login.py` & `mlfoundry-0.9.9/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/constants.py` & `mlfoundry-0.9.9/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/enums.py` & `mlfoundry-0.9.9/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/transformers_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/transformers_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.9.9/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/git_info.py` & `mlfoundry-0.9.9/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/integrations/lightning.py` & `mlfoundry-0.9.9/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/integrations/transformers.py` & `mlfoundry-0.9.9/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/internal_namespace.py` & `mlfoundry-0.9.9/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.9.9/mlfoundry/log_types/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.9.9/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.9.9/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.9.9/mlfoundry/log_types/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.9.9/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/image/image.py` & `mlfoundry-0.9.9/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.9.9/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/image/types.py` & `mlfoundry-0.9.9/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/plot.py` & `mlfoundry-0.9.9/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.9.9/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/log_types/utils.py` & `mlfoundry-0.9.9/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/login.py` & `mlfoundry-0.9.9/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.9.9/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.9.9/mlfoundry/mlfoundry_api.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.9.9/mlfoundry/mlfoundry_run.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/monitoring/entities.py` & `mlfoundry-0.9.9/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.9.9/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.9.9/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.9.9/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.9.9/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/run_utils.py` & `mlfoundry-0.9.9/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/session.py` & `mlfoundry-0.9.9/mlfoundry/session.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.9.9/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/tracking/entities.py` & `mlfoundry-0.9.9/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.9.9/mlfoundry/tracking/servicefoundry_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,22 @@
     def get_token_from_api_key(self, api_key: str) -> Token:
         response = http_request_safe(
             host_creds=self.host_creds,
             endpoint="/v1/oauth/api-key/token",
             method="get",
             params={"apiKey": api_key},
             timeout=3,
-            max_retries=0,
+            max_retries=2,
         )
         response = response.json()
         return Token.parse_obj(response)
 
     def get_integration_from_id(self, integration_id: str):
         integration_id = integration_id or ""
         response = http_request_safe(
             host_creds=self.host_creds,
             endpoint=f"/v1/integrations/{integration_id}",
             method="get",
             timeout=3,
-            max_retries=0,
+            max_retries=2,
         )
         return response.json()
```

### Comparing `mlfoundry-0.9.8/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.9.9/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.9.9/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.8/pyproject.toml` & `mlfoundry-0.9.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.9.8" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.9" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
-homepage = "https://github.com/truefoundry/mlfoundry"
+homepage = "https://truefoundry.com"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
 ]
 
 [tool.poetry.dependencies]
 # Note: Do not use ^ or ~. They can cause unecessary confusion
 # TODO (chiragjn): Ideally no upper limit should be put on packages because that makes
 #    upgrading impossible for users, even if they only want partial compatible features
 python = ">=3.7,<4"
-GitPython = ">=3.1.26,<4.0.0"
+GitPython = ">=3.1.35,<4.0.0"
 amplitude-tracker = "0.0.7"
 click = ">=8.0.0,<9.0.0"
 coolname = ">=1.1.0,<2.0.0"
 filelock = ">=3.8.0,<4.0.0"
 numpy = ">=1.17.0,<2.0.0"
 pandas = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
@@ -32,25 +32,26 @@
 scipy = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.5.4,<2.0.0", python = "<3.10" },
     { version = ">=1.8.0,<2.0.0", python = ">=3.10" },
 ]
 tfy-mlflow-client = "0.0.40"
 tqdm = ">=4.62.3,<5.0.0"
+urllib3 = ">=1.26.17,<3"
 # Check and try to eliminate libs below this comment
 importlib-metadata = ">=4.11.3,<5.0.0"
 packaging = ">=20.0,<24.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.21.0"
 pytest = ">=7.2.0,<7.3.0"
 Pillow = ">=9.1.1,<10.0.0"
 doq = ">=0.9.1,<1.0.0"
 ipython = ">=7.10.0"
-jupyterlab = ">=3.6.2"
+ipykernel = ">=6.16.0"
 lazydocs = ">=0.4.8,<0.5.0"
 matplotlib = ">=3.0.0,<4.0.0"
 mypy = ">=0.950"
 plotly = ">=5.8.2"
 shap = ">=0.40.0"
 # TODO (chiragjn): As of 27th March, 2023 `tensorflow-io-gcs-filesystem` has upper limit 3.11
 #   Adding python version limits us to running specific tests Python < 3.12
```

### Comparing `mlfoundry-0.9.8/PKG-INFO` & `mlfoundry-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.9.8
+Version: 0.9.9
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
-Home-page: https://github.com/truefoundry/mlfoundry
+Home-page: https://truefoundry.com
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: GitPython (>=3.1.26,<4.0.0)
+Requires-Dist: GitPython (>=3.1.35,<4.0.0)
 Requires-Dist: amplitude-tracker (==0.0.7)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: coolname (>=1.1.0,<2.0.0)
 Requires-Dist: filelock (>=3.8.0,<4.0.0)
 Requires-Dist: importlib-metadata (>=4.11.3,<5.0.0)
 Requires-Dist: numpy (>=1.17.0,<2.0.0)
 Requires-Dist: packaging (>=20.0,<24.0)
@@ -25,14 +25,15 @@
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24.2,<2.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0) ; python_version < "3.10"
 Requires-Dist: scipy (>=1.8.0,<2.0.0) ; python_version >= "3.10"
 Requires-Dist: tfy-mlflow-client (==0.0.40)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
+Requires-Dist: urllib3 (>=1.26.17,<3)
 Project-URL: Repository, https://github.com/truefoundry/mlfoundry
 Description-Content-Type: text/markdown
 
 # MlFoundry
 
 ![](https://github.com/MyName/my-project/workflows/Project%20Tests/badge.svg)
```

