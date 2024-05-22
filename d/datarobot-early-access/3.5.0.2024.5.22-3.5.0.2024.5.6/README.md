# Comparing `tmp/datarobot_early_access-3.5.0.2024.5.22.tar.gz` & `tmp/datarobot_early_access-3.5.0.2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.5.0.2024.5.22.tar", last modified: Wed May 22 14:16:03 2024, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.5.0.2024.5.6.tar", last modified: Mon May  6 16:47:31 2024, max compression
```

## Comparing `datarobot_early_access-3.5.0.2024.5.22.tar` & `datarobot_early_access-3.5.0.2024.5.6.tar`

### file list

```diff
@@ -1,234 +1,233 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/
--rw-r--r--   0 root         (0) root         (0)   234174 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/CHANGES.rst
--rw-r--r--   0 root         (0) root         (0)     7555 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3761 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8911 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/README.md
--rw-r--r--   0 root         (0) root         (0)     6042 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/common_setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/
--rw-r--r--   0 root         (0) root         (0)     2527 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/__init__.py
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26398 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/chunking_service.py
--rw-r--r--   0 root         (0) root         (0)    15390 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/data_matching.py
--rw-r--r--   0 root         (0) root         (0)     5044 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/data_store.py
--rw-r--r--   0 root         (0) root         (0)     2742 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/dataset.py
--rw-r--r--   0 root         (0) root         (0)     5892 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/chat.py
--rw-r--r--   0 root         (0) root         (0)    14799 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/chat_prompt.py
--rw-r--r--   0 root         (0) root         (0)      390 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/comparison_chat.py
--rw-r--r--   0 root         (0) root         (0)     4404 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/comparison_prompt.py
--rw-r--r--   0 root         (0) root         (0)     5620 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/cost_metric_configurations.py
--rw-r--r--   0 root         (0) root         (0)      402 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/custom_model_llm_validation.py
--rw-r--r--   0 root         (0) root         (0)     9890 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py
--rw-r--r--   0 root         (0) root         (0)     7350 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py
--rw-r--r--   0 root         (0) root         (0)    12541 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/insights_configuration.py
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/llm.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/llm_blueprint.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/playground.py
--rw-r--r--   0 root         (0) root         (0)     7445 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/prompt_trace.py
--rw-r--r--   0 root         (0) root         (0)    12780 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/sidecar_model_metric.py
--rw-r--r--   0 root         (0) root         (0)     3237 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/user_limits.py
--rw-r--r--   0 root         (0) root         (0)     9278 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/vector_database.py
--rw-r--r--   0 root         (0) root         (0)     8693 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/idiomatic_project.py
--rw-r--r--   0 root         (0) root         (0)     5416 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/incremental_learning.py
--rw-r--r--   0 root         (0) root         (0)     6392 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/model.py
--rw-r--r--   0 root         (0) root         (0)    20913 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/model_lineage.py
--rw-r--r--   0 root         (0) root         (0)    31504 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/notebooks.py
--rw-r--r--   0 root         (0) root         (0)    54156 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/project_options.py
--rw-r--r--   0 root         (0) root         (0)    10044 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/recipe_operations.py
--rw-r--r--   0 root         (0) root         (0)     9052 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/recipes.py
--rw-r--r--   0 root         (0) root         (0)     7408 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/retraining.py
--rw-r--r--   0 root         (0) root         (0)      313 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/_version.py
--rw-r--r--   0 root         (0) root         (0)     5241 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/analytics.py
--rw-r--r--   0 root         (0) root         (0)    14682 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/client.py
--rw-r--r--   0 root         (0) root         (0)    12682 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/config.py
--rw-r--r--   0 root         (0) root         (0)     4664 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/context.py
--rw-r--r--   0 root         (0) root         (0)    40703 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/enums.py
--rw-r--r--   0 root         (0) root         (0)     8984 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/
--rw-r--r--   0 root         (0) root         (0)    27055 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13002 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/binary_data_utils.py
--rw-r--r--   0 root         (0) root         (0)     1156 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/eligibility_result.py
--rw-r--r--   0 root         (0) root         (0)    14350 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/feature_discovery.py
--rw-r--r--   0 root         (0) root         (0)     8744 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/image_utils.py
--rw-r--r--   0 root         (0) root         (0)   101561 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/partitioning_methods.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/
--rw-r--r--   0 root         (0) root         (0)      200 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9380 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/base.py
--rw-r--r--   0 root         (0) root         (0)     3057 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/shap_impact.py
--rw-r--r--   0 root         (0) root         (0)     1770 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/shap_matrix.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/shap_preview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1134 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/mixins/browser_mixin.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/mixins/update_attributes_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/
--rw-r--r--   0 root         (0) root         (0)     4339 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9166 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/advanced_tuning.py
--rw-r--r--   0 root         (0) root         (0)    27075 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/anomaly_assessment.py
--rw-r--r--   0 root         (0) root         (0)     2925 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/api_object.py
--rw-r--r--   0 root         (0) root         (0)     9076 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/application.py
--rw-r--r--   0 root         (0) root         (0)    15457 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/automated_documentation.py
--rw-r--r--   0 root         (0) root         (0)    20521 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/batch_job.py
--rw-r--r--   0 root         (0) root         (0)    37053 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/batch_monitoring_job.py
--rw-r--r--   0 root         (0) root         (0)    86430 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/batch_prediction_job.py
--rw-r--r--   0 root         (0) root         (0)    11451 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/blueprint.py
--rw-r--r--   0 root         (0) root         (0)    23822 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/calendar_file.py
--rw-r--r--   0 root         (0) root         (0)    13301 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/change_request.py
--rw-r--r--   0 root         (0) root         (0)     3978 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/cluster.py
--rw-r--r--   0 root         (0) root         (0)     7233 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/cluster_insight.py
--rw-r--r--   0 root         (0) root         (0)    12910 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/compliance_doc_template.py
--rw-r--r--   0 root         (0) root         (0)     4889 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/confusion_chart.py
--rw-r--r--   0 root         (0) root         (0)     7244 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/connector.py
--rw-r--r--   0 root         (0) root         (0)    20307 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/credential.py
--rw-r--r--   0 root         (0) root         (0)    33664 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_model.py
--rw-r--r--   0 root         (0) root         (0)    12041 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_model_test.py
--rw-r--r--   0 root         (0) root         (0)    63366 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_model_version.py
--rw-r--r--   0 root         (0) root         (0)    15411 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_task.py
--rw-r--r--   0 root         (0) root         (0)    22991 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_task_version.py
--rw-r--r--   0 root         (0) root         (0)     2315 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_task_version_dependency_build.py
--rw-r--r--   0 root         (0) root         (0)    17613 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/data_engine_query_generator.py
--rw-r--r--   0 root         (0) root         (0)    17068 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/data_slice.py
--rw-r--r--   0 root         (0) root         (0)    17425 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/data_source.py
--rw-r--r--   0 root         (0) root         (0)    22098 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/data_store.py
--rw-r--r--   0 root         (0) root         (0)    75540 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/dataset.py
--rw-r--r--   0 root         (0) root         (0)    30524 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/datetime_trend_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/
--rw-r--r--   0 root         (0) root         (0)      544 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16779 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/accuracy.py
--rw-r--r--   0 root         (0) root         (0)     5698 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/bias_and_fairness.py
--rw-r--r--   0 root         (0) root         (0)     7095 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/challenger.py
--rw-r--r--   0 root         (0) root         (0)     6170 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/champion_model_package.py
--rw-r--r--   0 root         (0) root         (0)    68845 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/custom_metrics.py
--rw-r--r--   0 root         (0) root         (0)    12650 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/data_drift.py
--rw-r--r--   0 root         (0) root         (0)    24249 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/data_exports.py
--rw-r--r--   0 root         (0) root         (0)   121466 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/deployment.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/mixins.py
--rw-r--r--   0 root         (0) root         (0)    10065 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/service_stats.py
--rw-r--r--   0 root         (0) root         (0)     3450 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/sharing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/documentai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/documentai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27024 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/documentai/document.py
--rw-r--r--   0 root         (0) root         (0)     8427 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/driver.py
--rw-r--r--   0 root         (0) root         (0)     9411 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/execution_environment.py
--rw-r--r--   0 root         (0) root         (0)    11344 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/execution_environment_version.py
--rw-r--r--   0 root         (0) root         (0)     5376 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_baseline_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6403 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-r--r--   0 root         (0) root         (0)     4915 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-r--r--   0 root         (0) root         (0)     4523 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-r--r--   0 root         (0) root         (0)     5208 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-r--r--   0 root         (0) root         (0)     4521 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-r--r--   0 root         (0) root         (0)     6789 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-r--r--   0 root         (0) root         (0)    53938 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_association_matrix/
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_association_matrix/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2600 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-r--r--   0 root         (0) root         (0)     7052 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-r--r--   0 root         (0) root         (0)     4753 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-r--r--   0 root         (0) root         (0)    18312 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_effect.py
--rw-r--r--   0 root         (0) root         (0)     7003 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_impact.py
--rw-r--r--   0 root         (0) root         (0)    17463 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/featurelist.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5647 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/chat.py
--rw-r--r--   0 root         (0) root         (0)    18148 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/chat_prompt.py
--rw-r--r--   0 root         (0) root         (0)     5925 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/comparison_chat.py
--rw-r--r--   0 root         (0) root         (0)    12080 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/comparison_prompt.py
--rw-r--r--   0 root         (0) root         (0)     2168 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/custom_model_llm_validation.py
--rw-r--r--   0 root         (0) root         (0)    16900 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/custom_model_validation.py
--rw-r--r--   0 root         (0) root         (0)    10350 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/llm.py
--rw-r--r--   0 root         (0) root         (0)    23244 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/llm_blueprint.py
--rw-r--r--   0 root         (0) root         (0)     7303 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/playground.py
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/user_limits.py
--rw-r--r--   0 root         (0) root         (0)    26873 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/vector_database.py
--rw-r--r--   0 root         (0) root         (0)    21315 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/job.py
--rw-r--r--   0 root         (0) root         (0)    13141 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/key_values.py
--rw-r--r--   0 root         (0) root         (0)     6516 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/lift_chart.py
--rw-r--r--   0 root         (0) root         (0)     5468 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/missing_report.py
--rw-r--r--   0 root         (0) root         (0)   303355 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/
--rw-r--r--   0 root         (0) root         (0)      204 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/__init__.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/common.py
--rw-r--r--   0 root         (0) root         (0)     3453 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/deployment.py
--rw-r--r--   0 root         (0) root         (0)    26475 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/registered_model.py
--rw-r--r--   0 root         (0) root         (0)    22985 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/registered_model_version.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/modeljob.py
--rw-r--r--   0 root         (0) root         (0)    14320 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/pairwise_statistics.py
--rw-r--r--   0 root         (0) root         (0)     5438 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/pareto_front.py
--rw-r--r--   0 root         (0) root         (0)     8726 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/payoff_matrix.py
--rw-r--r--   0 root         (0) root         (0)     7403 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/predict_job.py
--rw-r--r--   0 root         (0) root         (0)    10218 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prediction_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10918 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prediction_environment.py
--rw-r--r--   0 root         (0) root         (0)    39753 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prediction_explanations.py
--rw-r--r--   0 root         (0) root         (0)     2426 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prediction_server.py
--rw-r--r--   0 root         (0) root         (0)    15940 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/predictions.py
--rw-r--r--   0 root         (0) root         (0)     2655 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prime_file.py
--rw-r--r--   0 root         (0) root         (0)   224363 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/project.py
--rw-r--r--   0 root         (0) root         (0)    57175 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/project_options.py
--rw-r--r--   0 root         (0) root         (0)     8774 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/rating_table.py
--rw-r--r--   0 root         (0) root         (0)     4337 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/recommended_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/registry/
--rw-r--r--   0 root         (0) root         (0)      345 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/registry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18128 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/registry/job.py
--rw-r--r--   0 root         (0) root         (0)    10379 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/registry/job_run.py
--rw-r--r--   0 root         (0) root         (0)    19108 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/relationships_configuration.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/residuals.py
--rw-r--r--   0 root         (0) root         (0)     4524 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/restore_discarded_features.py
--rw-r--r--   0 root         (0) root         (0)    11692 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/roc_curve.py
--rw-r--r--   0 root         (0) root         (0)     2927 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/ruleset.py
--rw-r--r--   0 root         (0) root         (0)     5008 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/runtime_parameters.py
--rw-r--r--   0 root         (0) root         (0)    19381 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/secondary_dataset.py
--rw-r--r--   0 root         (0) root         (0)    14217 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/segmentation.py
--rw-r--r--   0 root         (0) root         (0)     4722 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/shap_impact.py
--rw-r--r--   0 root         (0) root         (0)     8216 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/shap_matrix.py
--rw-r--r--   0 root         (0) root         (0)     2676 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/shap_matrix_job.py
--rw-r--r--   0 root         (0) root         (0)     7314 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/sharing.py
--rw-r--r--   0 root         (0) root         (0)     6267 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/status_check_job.py
--rw-r--r--   0 root         (0) root         (0)     1431 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/trafarets.py
--rw-r--r--   0 root         (0) root         (0)    28260 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/training_predictions.py
--rw-r--r--   0 root         (0) root         (0)     2029 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/use_cases/
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/use_cases/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24813 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/use_cases/use_case.py
--rw-r--r--   0 root         (0) root         (0)    13496 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/use_cases/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/user_blueprints/
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/user_blueprints/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69649 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/user_blueprints/models.py
--rw-r--r--   0 root         (0) root         (0)     8758 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/user_blueprints/trafarets.py
--rw-r--r--   0 root         (0) root         (0)     2749 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/visualai/
--rw-r--r--   0 root         (0) root         (0)      226 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/visualai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18528 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/visualai/augmentation.py
--rw-r--r--   0 root         (0) root         (0)    10521 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/visualai/images.py
--rw-r--r--   0 root         (0) root         (0)    13615 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/visualai/insights.py
--rw-r--r--   0 root         (0) root         (0)     4936 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/models/word_cloud.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/py.typed
--rw-r--r--   0 root         (0) root         (0)    18404 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/
--rw-r--r--   0 root         (0) root         (0)    15618 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/deprecation.py
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/pagination.py
--rw-r--r--   0 root         (0) root         (0)     1461 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/retry.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/source.py
--rw-r--r--   0 root         (0) root         (0)     4109 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/sourcedata.py
--rw-r--r--   0 root         (0) root         (0)     4193 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/waiters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3761 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8389 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1321 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3066 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      123 2024-05-22 14:16:03.000000 datarobot_early_access-3.5.0.2024.5.22/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      965 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/setup.py
--rw-r--r--   0 root         (0) root         (0)     2498 2024-05-22 14:15:36.000000 datarobot_early_access-3.5.0.2024.5.22/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   231328 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2527 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26398 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/chunking_service.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/data_matching.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5808 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/enums.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      379 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14680 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/chat_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      390 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/comparison_chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4400 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/comparison_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5620 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/cost_metric_configurations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      402 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/custom_model_llm_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9890 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12541 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/insights_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      378 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/llm.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      388 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/llm_blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      385 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/playground.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7305 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/prompt_trace.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12780 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/sidecar_model_metric.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3237 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      386 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/user_limits.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9278 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/vector_database.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/incremental_learning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    31504 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipe_operations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipes.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/analytics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/config.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40318 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8744 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9380 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/base.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3057 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1770 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1986 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_preview.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4339 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86467 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20307 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34090 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    63934 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_slice.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      544 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/challenger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6170 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/champion_model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57732 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/custom_metrics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24249 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_exports.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   121466 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/mixins.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/sharing.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/featurelist.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      455 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5647 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18029 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5925 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12076 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2168 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_llm_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16900 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22899 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm_blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7299 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/playground.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/user_limits.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26873 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/vector_database.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13141 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/key_values.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   303355 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/common.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   224363 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57175 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/recommended_model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      345 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16789 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10379 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job_run.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5008 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/runtime_parameters.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4722 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8216 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2676 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/status_check_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24890 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8344 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/setup_weekly.py
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/CHANGES.rst` & `datarobot_early_access-3.5.0.2024.5.6/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,17 @@
 #########
 Changelog
 #########
 3.5.0b0
 =======
 
-New features
-************
-- Added attribute `creation_user_name` to :class:`LLMBlueprint <datarobot.models.genai.llm_blueprint.LLMBlueprint>`.
-- Added a new class :class:`HostedCustomMetricTemplate <datarobot.models.deployment.custom_metrics.HostedCustomMetricTemplate>` for hosted custom metrics templates.
-  :meth:`HostedCustomMetricTemplate.get <datarobot.models.deployment.custom_metrics.HostedCustomMetricTemplate.get>` to retrieve a hosted custom metric template.
-  :meth:`HostedCustomMetricTemplate.list <datarobot.models.deployment.custom_metrics.HostedCustomMetricTemplate.list>` to list hosted custom metric templates.
-- Added :meth:`Job.create_from_custom_metric_gallery_template <datarobot.models.registry.job.Job.create_from_custom_metric_gallery_template>` to create a job from a custom metric gallery template.
-- Added a new class :class:`HostedCustomMetricTemplate <datarobot.models.deployment.custom_metrics.HostedCustomMetric>` for hosted custom metrics.
-    :meth:`HostedCustomMetric.list <datarobot.models.deployment.custom_metrics.HostedCustomMetric.list>` to list hosted custom metrics.
-
 Documentation changes
 *********************
-- Added usage of `external_llm_context_size` in `llm_settings` in `genai_example.rst`.
-- Updated doc string for `llm_settings` to include attribute `external_llm_context_size` for external LLMs.
 - Updated `genai_example.rst` to link to DataRobot doc pages for external vector database and external LLM deployment creation.
 
-API changes
-***********
-- Remove an unsupported `NETWORK_EGRESS_POLICY.DR_API_ACCESS` value for custom models. This value
-  was used by a feature that was never released as a GA and is not supported in the current API.
-- Implemented support for `dr-connector-v1` to `DataStore <datarobot.models.DataStore>` and `DataSource <datarobot.models.DataStore>`.
-- Added a new parameter `name` to :meth:`DataStore.list <datarobot.DataStore.list>` for searching data stores by name.
-
-Experimental changes
-*********************
-- Added experimental api support for Data Wrangling. See :class:`Recipe <datarobot._experimental.models.recipes.Recipe>`.
-  :meth:`Recipe.from_data_store <datarobot._experimental.models.recipes.Recipe.from_data_store>` to create a Recipe from data store.
-  :meth:`Recipe.retrieve_preview <datarobot._experimental.models.recipes.Recipe.retrieve_preview>` to get a sample of the data after recipe is applied.
-  :meth:`Recipe.set_inputs <datarobot._experimental.models.recipes.Recipe.set_inputs>` to set inputs to the recipe.
-  :meth:`Recipe.set_operations <datarobot._experimental.models.recipes.Recipe.set_operations>` to set operations to the recipe.
-- Added new experimental :class:`DataStore <datarobot._experimental.models.data_store.DataStore>` that adds 
-  `get_spark_session` for Databricks `databricks-v1` data stores to get a Spark session.
-
 3.4.0b0
 =======
 
 New features
 ************
 - Added a new class :class: `EvaluationDatasetConfiguration <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration>` for configuration of evaluation datasets.
   :meth:`EvaluationDatasetConfiguration.get <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration.get>` to get an evaluation dataset configuration.
@@ -71,30 +42,27 @@
 
 
 Enhancements
 ************
 
 Bugfixes
 ********
-- Updated the validation logic of `RelationshipsConfiguration` to work with native database connections
 
 API changes
 ***********
 - Remove `ImportedModel` object since it was API for SSE (standalone scoring engine) which is not part of DataRobot anymore.
 
 Deprecation summary
 *******************
 
 Configuration changes
 *********************
 
 Documentation changes
 *********************
-- Removed incorrect can_share parameters in Use Case sharing example
-
 
 Experimental changes
 ********************
 
 3.4.0
 =====
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/LICENSE.txt` & `datarobot_early_access-3.5.0.2024.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/PKG-INFO` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,83 @@
 Metadata-Version: 2.1
-Name: datarobot_early_access
-Version: 3.5.0.2024.5.22
+Name: datarobot-early-access
+Version: 3.5.0.2024.5.6
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
 Project-URL: Documentation, https://datarobot-public-api-client.readthedocs-hosted.com/en/early-access/
 Project-URL: Changelog, https://datarobot-public-api-client.readthedocs-hosted.com/en/early-access/CHANGES.html
+Description: 
+        About datarobot_early_access
+        ============================
+        .. image:: https://img.shields.io/pypi/v/datarobot_early_access.svg
+           :target: https://pypi.python.org/pypi/datarobot-early-access/
+        .. image:: https://img.shields.io/pypi/pyversions/datarobot_early_access.svg
+        .. image:: https://img.shields.io/pypi/status/datarobot_early_access.svg
+        
+        DataRobot is a client library for working with the `DataRobot`_ platform API. This package is the "early access" version of the client. **Do NOT use this package in production--you will expose yourself to risk of breaking changes and bugs.** For the most stable version, see the quarterly release on PyPI at https://pypi.org/project/datarobot/.
+        
+        This package is released under the terms of the DataRobot Tool and Utility Agreement, which
+        can be found on our `Legal`_ page, along with our privacy policy and more.
+        
+        Installation
+        =========================
+        Python >= 3.7 are supported.
+        You must have a datarobot account.
+        
+        ::
+        
+           $ pip install datarobot_early_access
+        
+        Usage
+        =========================
+        The library will look for a config file `~/.config/datarobot/drconfig.yaml` by default.
+        This is an example of what that config file should look like.
+        
+        ::
+        
+           token: your_token
+           endpoint: https://app.datarobot.com/api/v2
+        
+        Alternatively a global client can be set in the code.
+        
+        ::
+        
+           import datarobot as dr
+           dr.Client(token='your_token', endpoint='https://app.datarobot.com/api/v2')
+        
+        Alternatively environment variables can be used.
+        
+        ::
+        
+           export DATAROBOT_API_TOKEN='your_token'
+           export DATAROBOT_ENDPOINT='https://app.datarobot.com/api/v2'
+        
+        See `documentation`_ for example usage after configuring.
+        
+        Helpful links
+        =========================
+        - `API quickstart guide <https://docs.datarobot.com/en/docs/api/api-quickstart/index.html>`_
+        - `Code examples <https://docs.datarobot.com/en/docs/api/guide/python/index.html>`_
+        - `Common use cases <https://docs.datarobot.com/en/docs/api/guide/common-case/index.html>`_
+        
+        Bug Reporting and Q&A
+        =========================
+        Create an account on `DataRobot Community <https://community.datarobot.com/>`_ and post your questions and bug reports
+        `here <https://community.datarobot.com/t5/forums/postpage/board-id/datarobot-api>`_.
+        
+        .. _datarobot: https://datarobot.com
+        .. _documentation: https://datarobot-public-api-client.readthedocs-hosted.com/en/early-access/
+        .. _legal: https://www.datarobot.com/legal/
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -25,72 +89,7 @@
 Requires-Python: >=3.7
 Provides-Extra: dev
 Provides-Extra: examples
 Provides-Extra: release
 Provides-Extra: lint
 Provides-Extra: images
 Provides-Extra: test
-Provides-Extra: databricks
-License-File: LICENSE.txt
-
-
-About datarobot_early_access
-============================
-.. image:: https://img.shields.io/pypi/v/datarobot_early_access.svg
-   :target: https://pypi.python.org/pypi/datarobot-early-access/
-.. image:: https://img.shields.io/pypi/pyversions/datarobot_early_access.svg
-.. image:: https://img.shields.io/pypi/status/datarobot_early_access.svg
-
-DataRobot is a client library for working with the `DataRobot`_ platform API. This package is the "early access" version of the client. **Do NOT use this package in production--you will expose yourself to risk of breaking changes and bugs.** For the most stable version, see the quarterly release on PyPI at https://pypi.org/project/datarobot/.
-
-This package is released under the terms of the DataRobot Tool and Utility Agreement, which
-can be found on our `Legal`_ page, along with our privacy policy and more.
-
-Installation
-=========================
-Python >= 3.7 are supported.
-You must have a datarobot account.
-
-::
-
-   $ pip install datarobot_early_access
-
-Usage
-=========================
-The library will look for a config file `~/.config/datarobot/drconfig.yaml` by default.
-This is an example of what that config file should look like.
-
-::
-
-   token: your_token
-   endpoint: https://app.datarobot.com/api/v2
-
-Alternatively a global client can be set in the code.
-
-::
-
-   import datarobot as dr
-   dr.Client(token='your_token', endpoint='https://app.datarobot.com/api/v2')
-
-Alternatively environment variables can be used.
-
-::
-
-   export DATAROBOT_API_TOKEN='your_token'
-   export DATAROBOT_ENDPOINT='https://app.datarobot.com/api/v2'
-
-See `documentation`_ for example usage after configuring.
-
-Helpful links
-=========================
-- `API quickstart guide <https://docs.datarobot.com/en/docs/api/api-quickstart/index.html>`_
-- `Code examples <https://docs.datarobot.com/en/docs/api/guide/python/index.html>`_
-- `Common use cases <https://docs.datarobot.com/en/docs/api/guide/common-case/index.html>`_
-
-Bug Reporting and Q&A
-=========================
-Create an account on `DataRobot Community <https://community.datarobot.com/>`_ and post your questions and bug reports
-`here <https://community.datarobot.com/t5/forums/postpage/board-id/datarobot-api>`_.
-
-.. _datarobot: https://datarobot.com
-.. _documentation: https://datarobot-public-api-client.readthedocs-hosted.com/en/early-access/
-.. _legal: https://www.datarobot.com/legal/
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/README.md` & `datarobot_early_access-3.5.0.2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/common_setup.py` & `datarobot_early_access-3.5.0.2024.5.6/common_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,43 +108,34 @@
     "types-pytz==2022.2.1.0",
     "types-requests==2.28.11",
     "types-urllib3==1.26.25",
 ]
 
 images_require = ["Pillow==9.2.0"]
 
-databricks_require = [
-    "databricks-connect>=13.0",
-]
-
 lint_require = (
     [
         "black==22.8.0",
         "black[jupyter]==22.8.0",
         "isort==5.10.1",
         "flake8==5.0.4",
         "pylint==2.15.0",
     ]
     + _mypy_require
     + images_require
-    + databricks_require
 )
 
-tests_require = (
-    [
-        "mock==3.0.5",
-        "pytest==7.1.2",
-        "pytest-cov",
-        "responses==0.21",
-        "pytest-asyncio==0.21.1",
-        "pyarrow",
-    ]
-    + images_require
-    + databricks_require
-)
+tests_require = [
+    "mock==3.0.5",
+    "pytest==7.1.2",
+    "pytest-cov",
+    "responses==0.21",
+    "pytest-asyncio==0.21.1",
+    "pyarrow",
+] + images_require
 
 dev_require = (
     tests_require
     + lint_require
     + images_require
     + [
         "sphinx_rtd_theme==1.0.0",
@@ -205,10 +196,9 @@
     extras_require={
         "dev": dev_require,
         "examples": example_require,
         "release": release_require,
         "lint": lint_require,
         "images": images_require,
         "test": tests_require,
-        "databricks": databricks_require,
     },
 )
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_compat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/chunking_service.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/chunking_service.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/enums.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,14 @@
     AVG = "avg"
     STDDEV = "stddev"
     MEDIAN = "median"
 
 
 class DataWranglingDialect(StrEnum):
     SNOWFLAKE = "snowflake"
-    POSTGRES = "postgres"
 
 
 class RecipeInputType(StrEnum):
     DATASOURCE = "datasource"
 
 
 class DatetimeSamplingStrategy(StrEnum):
@@ -127,15 +126,14 @@
 
     COMPUTE_NEW = "compute-new"
     DROP_COLUMNS = "drop-columns"
     RENAME_COLUMNS = "rename-columns"
     FILTER = "filter"
 
     LAGS = "lags"
-    WINDOW_CATEGORICAL_STATS = "window-categorical-stats"
     WINDOW_NUMERIC_STATS = "window-numeric-stats"
     TIME_SERIES = "time-series"
 
 
 class SamplingOperations(StrEnum):
     """Supported data wrangling sampling operations."""
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/chat_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/chat_prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -293,25 +293,24 @@
     llm_blueprint_id : str
         ID of the LLM blueprint associated with the chat prompt.
     llm_id : str
         ID of the LLM type. This must be one of the IDs returned by `LLMDefinition.list`
         for this user.
     llm_settings : dict or None
         The LLM settings for the LLM blueprint. The specific keys allowed and the
-        constraints on the values are defined in the response from `LLMDefinition.list`,
-        but this typically has dict fields. Either:
-        - system_prompt - The system prompt that influences the LLM responses.
-        - max_completion_length - The maximum number of tokens in the completion.
-        - temperature - Controls the variability in the LLM response.
-        - top_p - Sets whether the model considers next tokens with top_p probability mass.
+        constraints on the values are defined in the response from `LLMDefinition.list`
+        but this typically has dict fields:
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - max_completion_length - The maximum number of token in the completion.
+        - temperature - controls the variability in the LLM response.
+        - top_p - the model considers next tokens with top_p probability mass
         or
-        - system_prompt - The system prompt that influences the LLM responses.
-        - validation_id - The ID of the external model LLM validation.
-        - external_llm_context_size - The external LLM's context size, in tokens,
-        for external model-based LLM blueprints.
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - validation_id - The ID of the custom model LLM validation
+        for custom model LLM blueprints.
     creation_date : str
         The date the chat prompt was created.
     creation_user_id : str
         ID of the creating user.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
     vector_database_settings : VectorDatabaseSettings or None
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/comparison_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/comparison_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     id : str
         Comparison prompt ID.
     text : str
         The prompt text.
     results : list[ComparisonPromptResult]
         The list of results for individual LLM blueprints that are part of the comparison prompt.
     creation_date : str
-        The date when the playground was created.
+        Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
     comparison_chat_id : str
         The ID of the comparison chat this comparison prompt is associated with.
     """
 
     def update(
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/cost_metric_configurations.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/cost_metric_configurations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/insights_configuration.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/insights_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/prompt_trace.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/prompt_trace.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,27 +77,25 @@
         The ID of the LLM blueprint that the prompt was submitted to.
     llm_name : str
         The name of the LLM in the LLM blueprint.
     llm_vendor : str
         The vendor name of the LLM.
     llm_license : str
         What type of license the LLM has.
-    llm_settings : dict or None
+    llm_settings : dict
         The LLM settings for the LLM blueprint. The specific keys allowed and the
-        constraints on the values are defined in the response from `LLMDefinition.list`,
-        but this typically has dict fields. Either:
-        - system_prompt - The system prompt that influences the LLM responses.
-        - max_completion_length - The maximum number of tokens in the completion.
+        constraints on the values are defined in the response from LLMDefinition.list
+        but this typically has dict fields:
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - max_completion_length - The maximum number of token in the completion.
         - temperature - Controls the variability in the LLM response.
-        - top_p - Sets whether the model considers next tokens with top_p probability mass.
-        or
-        - system_prompt - The system prompt that influences the LLM responses.
-        - validation_id - The ID of the external model LLM validation.
-        - external_llm_context_size - The external LLM's context size, in tokens,
-        for external model-based LLM blueprints.
+        - top_p - The model considers next tokens with top_p probability mass
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - validation_id - The ID of the custom model LLM validation
+        for custom model LLM blueprints.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
     vector_database_settings : VectorDatabaseSettings or None
         The settings for the vector database associated with the LLM blueprint, if any.
     result_metadata : ResultMetadata or None
         Metadata for the result of the prompt submission.
     result_text: str or None
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/sidecar_model_metric.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/sidecar_model_metric.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/genai/vector_database.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/vector_database.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/incremental_learning.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/incremental_learning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/notebooks.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/recipe_operations.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipe_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,18 +81,14 @@
 
 class Lags(BaseTimeAwareTask):
     def __init__(self, orders: List[int]):
         super().__init__("lags", {"orders": orders})
 
 
 class LagsOperation(WranglingOperation):
-    """
-    Generate lags in a window.
-    """
-
     def __init__(
         self,
         column: str,
         orders: List[int],
         datetime_partition_column: str,
         multiseries_id_column: Optional[str] = None,
     ):
@@ -103,62 +99,35 @@
                 "orders": orders,
                 "datetime_partition_column": datetime_partition_column,
                 "multiseries_id_column": multiseries_id_column,
             },
         )
 
 
-class WindowCategoricalStatsOperation(WranglingOperation):
-    """
-    Generate rolling statistics in a window for categorical features.
-    """
-
-    def __init__(
-        self,
-        column: str,
-        window_size: int,
-        methods: List[CategoricalStatsMethods],
-        datetime_partition_column: str,
-        multiseries_id_column: Optional[str] = None,
-        rolling_most_frequent_udf: Optional[str] = None,
-    ):
-        super().__init__(
-            directive=WranglingOperations.WINDOW_CATEGORICAL_STATS,
-            arguments={
-                "column": column,
-                "window_size": window_size,
-                "methods": methods,
-                "datetime_partition_column": datetime_partition_column,
-                "multiseries_id_column": multiseries_id_column,
-                "rolling_most_frequent_user_defined_function": rolling_most_frequent_udf,
-            },
-        )
-
-
 class WindowNumericStatsOperation(WranglingOperation):
     """Generate various rolling numeric statistics in a window. Output could be a several columns."""
 
     def __init__(
         self,
         column: str,
         window_size: int,
         methods: List[NumericStatsMethods],
         datetime_partition_column: str,
         multiseries_id_column: Optional[str] = None,
-        rolling_median_udf: Optional[str] = None,
+        rolling_median_snowflake_udf: Optional[str] = None,
     ):
         super().__init__(
             directive=WranglingOperations.WINDOW_NUMERIC_STATS,
             arguments={
                 "column": column,
                 "window_size": window_size,
                 "methods": methods,
                 "datetime_partition_column": datetime_partition_column,
                 "multiseries_id_column": multiseries_id_column,
-                "rolling_median_user_defined_function": rolling_median_udf,
+                "rolling_median_snowflake_user_defined_function": rolling_median_snowflake_udf,
             },
         )
 
 
 class TimeSeriesOperation(WranglingOperation):
     """Operation to generate a dataset ready for time series modeling: with forecast point, forecast distances,
     known in advance columns, etc.
@@ -169,16 +138,16 @@
         target_column: str,
         datetime_partition_column: str,
         forecast_distances: List[int],
         task_plan: Dict[str, List[BaseTimeAwareTask]],
         baseline_periods: Optional[List[int]] = None,
         known_in_advance_columns: Optional[List[str]] = None,
         multiseries_id_column: Optional[str] = None,
-        rolling_median_udf: Optional[str] = None,
-        rolling_most_frequent_udf: Optional[str] = None,
+        rolling_median_snowflake_udf: Optional[str] = None,
+        rolling_most_frequent_snowflake_udf: Optional[str] = None,
         forecast_point: Optional[datetime] = None,
     ):
         """
 
         Parameters
         ----------
         target_column
@@ -187,17 +156,17 @@
         task_plan:
             contains a task list for each column
         baseline_periods:
             generates naive features from the target. For example: baseline period = 1 corresponds to the naive
             latest baseline.
         known_in_advance_columns
         multiseries_id_column
-        rolling_median_udf:
+        rolling_median_snowflake_udf:
             Fully qualified path to rolling median user defined function. Used to optimize sql execution with snowflake.
-        rolling_most_frequent_udf:
+        rolling_most_frequent_snowflake_udf:
             Fully qualified path to rolling most frequent user defined function.
         forecast_point:
              To use at prediction time.
         """
         arguments = {
             "target_column": target_column,
             "datetime_partition_column": datetime_partition_column,
@@ -205,16 +174,16 @@
             "task_plan": [
                 {"column": column, "task_list": task_list}
                 for column, task_list in task_plan.items()
             ],
             "multiseries_id_column": multiseries_id_column,
             "known_in_advance_columns": known_in_advance_columns,
             "baseline_periods": baseline_periods,
-            "rolling_median_user_defined_function": rolling_median_udf,
-            "rolling_most_frequent_user_defined_function": rolling_most_frequent_udf,
+            "rolling_median_snowflake_user_defined_function": rolling_median_snowflake_udf,
+            "rolling_most_frequent_snowflake_user_defined_function": rolling_most_frequent_snowflake_udf,
             "forecast_point": forecast_point,
         }
         super().__init__(directive=WranglingOperations.TIME_SERIES, arguments=arguments)
 
 
 class ComputeNewOperation(WranglingOperation):
     def __init__(self, expression: str, new_feature_name: str):
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/recipes.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipes.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,23 +174,21 @@
         )
         r_data = self._client.get(finished_url).json()
         # TODO: create an ApiObject for Preview
         return r_data  # type: ignore[no-any-return]
 
     @classmethod
     def set_inputs(cls, recipe_id: str, inputs: List[JDBCTableDataSourceInput]) -> Recipe:
-        """Set inputs for the recipe."""
         path = f"{cls._path}{recipe_id}/inputs/"
         payload = {"inputs": [to_api(input_) for input_ in inputs]}
         response = cls._client.put(path, json=payload)
         return Recipe.from_server_data(response.json())
 
     @classmethod
     def set_operations(cls, recipe_id: str, operations: List[WranglingOperation]) -> Recipe:
-        """Set operations for the recipe."""
         path = f"{cls._path}{recipe_id}/operations/"
         payload = {"operations": [to_api(operation) for operation in operations]}
         response = cls._client.put(path, json=payload)
         return Recipe.from_server_data(response.json())
 
     @classmethod
     def get(cls, recipe_id: str) -> Recipe:
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/analytics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/client.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/config.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/config.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/context.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/enums.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -570,17 +570,18 @@
     ALL = _SHARED_TARGET_TYPE.ALL + [TRANSFORM]
 
 
 class NETWORK_EGRESS_POLICY:
     """Enum of valid network egress policy"""
 
     NONE = "NONE"
+    DR_API_ACCESS = "DR_API_ACCESS"
     PUBLIC = "PUBLIC"
 
-    ALL = [NONE, PUBLIC]
+    ALL = [NONE, DR_API_ACCESS, PUBLIC]
 
 
 @use_all
 class SOURCE_TYPE(StrEnum):
     """Enum of backtest source types"""
 
     TRAINING = "training"
@@ -1478,21 +1479,7 @@
 
 
 class PromptType(StrEnum):
     """Supported LLM Blueprint prompting types."""
 
     ONE_TIME_PROMPT = "ONE_TIME_PROMPT"
     CHAT_HISTORY_AWARE = "CHAT_HISTORY_AWARE"
-
-
-class ListHostedCustomMetricTemplatesSortQueryParams(StrEnum):
-    NAME_ASCENDING = "name"
-    NAME_DESCENDING = "-name"
-    TEMPLATE_METRIC_TYPE_ASCENDING = "template_metric_type"
-    TEMPLATE_METRIC_TYPE_DESCENDING = "-template_metric_type"
-
-
-class HostedCustomMetricsTemplateMetricTypeQueryParams(StrEnum):
-    LLM = "LLM"
-    LLM_WITH_SIDECAR = "LLMWithSidecar"
-    CLASSIFICATION = "classification"
-    REGRESSION = "regression"
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/errors.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/base.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/base.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/shap_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/shap_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/insights/shap_preview.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_preview.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/api_object.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/application.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/batch_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_prediction_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         return cast(str, JOB_TYPE.BATCH_PREDICTIONS)
 
     @classmethod
     def _jobs_path(cls) -> str:
         return "batchPredictions/"
 
     @classmethod
-    def _job_path(
+    def _job_path(  # pylint: disable=arguments-renamed
         cls,
         project_id: str,
         job_id: str,
     ) -> str:
         return f"batchPredictions/{job_id}/"
 
     @classmethod
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/blueprint.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/calendar_file.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/change_request.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/cluster.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/connector.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/credential.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         self.created_at = created_at
 
     @classmethod
     def _check_model_type(cls, data: Dict[str, Any]) -> bool:
         return cast(bool, data["customModelType"] == cls._model_type)  # type: ignore[attr-defined]
 
     @classmethod
-    def list(
+    def list(  # pylint: disable=missing-function-docstring
         cls: Type[T_CustomModelBase],
         is_deployed: Optional[bool] = None,
         order_by: Optional[str] = None,
         search_for: Optional[str] = None,
     ) -> List[T_CustomModelBase]:
         """List instances of _CustomModelBase.
 
@@ -430,15 +430,18 @@
         The username of a user who created the custom model.
     updated_at: str
         ISO-8601 formatted timestamp of when the custom model was updated
     created_at: str
         ISO-8601 formatted timestamp of when the custom model was created
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+        is only supported by the SaaS (cloud) environment.
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s.
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster
     is_training_data_for_versions_permanently_enabled: bool, optional
         Whether training data assignment on the version level is permanently enabled for the model.
@@ -645,15 +648,18 @@
             Custom inference model class labels for multiclass classification.
             Cannot be used with class_labels_file.
         class_labels_file: str, optional
             Path to file containing newline separated class labels for multiclass classification.
             Cannot be used with class_labels.
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`]
+            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`]
+            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+            is only supported by the SaaS (cloud) environment.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s.
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster.
         is_training_data_for_versions_permanently_enabled: bool, optional
             Permanently enable training data assignment on the version level for the current model,
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         id of a dataset version used for testing
     completed_at: str, optional
         ISO-8601 formatted timestamp of when the test has completed
     created_at: str, optional
         ISO-8601 formatted timestamp of when the version was created
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value is only supported by the SaaS (cloud) environment.
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster
     """
 
@@ -163,15 +165,18 @@
             The id of the testing dataset for non-unstructured custom models.
             Ignored and not required for unstructured models.
         max_wait: int, optional
             max time to wait for a test completion.
             If set to None - method will return without waiting.
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+            is only supported by the SaaS (cloud) environment.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster
 
         Returns
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -524,15 +524,17 @@
     created_at: str, optional
         ISO-8601 formatted timestamp of when the version was created.
     dependencies: List[CustomDependency]
         The parsed dependencies of the custom model version if the
         version has a valid requirements.txt file.
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value is only supported by the SaaS (cloud) environment.
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s.
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster.
     required_metadata_values: List[RequiredMetadataValue]
         Additional parameters required by the execution environment. The required keys are
@@ -705,15 +707,18 @@
             [("/home/user/Documents/myModel/file1.txt", "file1.txt"),
             ("/home/user/Documents/myModel/folder/file2.txt", "folder/file2.txt")]
             or
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+            is only supported by the SaaS (cloud) environment.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s.
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster.
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
@@ -889,15 +894,18 @@
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         files_to_delete: list, optional
             The list of a file items ids to be deleted.
             Example: ["5ea95f7a4024030aba48e4f9", "5ea6b5da402403181895cc51"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+            is only supported by the SaaS (cloud) environment.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_task.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/data_slice.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_slice.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/data_source.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,98 +34,90 @@
         data_store_id: Optional[str]
         catalog: Optional[str]
         table: Optional[str]
         schema: Optional[str]
         partition_column: Optional[str]
         query: Optional[str]
         fetch_size: Optional[int]
-        path: Optional[str]
 
 
 TDataSource = TypeVar("TDataSource", bound="DataSource")
 TDataSourceParameters = TypeVar("TDataSourceParameters", bound="DataSourceParameters")
 
 _data_source_params_converter = t.Dict(
     {
         t.Key("data_store_id"): t.Or(String(), t.Null),
         t.Key("catalog", optional=True): t.Or(String(), t.Null),
         t.Key("table", optional=True): t.Or(String(), t.Null),
         t.Key("schema", optional=True): t.Or(String(), t.Null),
         t.Key("partition_column", optional=True): t.Or(String(), t.Null),
         t.Key("query", optional=True): t.Or(String(), t.Null),
         t.Key("fetch_size", optional=True): t.Or(Int(), t.Null),
-        t.Key("path", optional=True): t.Or(String(), t.Null),
     }
 ).ignore_extra("*")
 
 
 class DataSourceParameters:
     """Data request configuration
 
     Attributes
     ----------
     data_store_id : str
         the id of the DataStore.
     table : str
-        Optional. The name of specified database table.
+        optional, the name of specified database table.
     schema : str
-        Optional. The name of the schema associated with the table.
+        optional, the name of the schema associated with the table.
     partition_column : str
-        Optional. The name of the partition column.
+        optional, the name of the partition column.
     query : str
-        Optional. The user specified SQL query.
+        optional, the user specified SQL query.
     fetch_size : int
-        Optional. A user specified fetch size in the range [1, 20000].
+        optional, a user specified fetch size in the range [1, 20000].
         By default a fetchSize will be assigned to balance throughput and memory usage
-    path: str
-        Optional. The user-specified path for BLOB storage
     """
 
     def __init__(
         self,
         data_store_id: Optional[str] = None,
         catalog: Optional[str] = None,
         table: Optional[str] = None,
         schema: Optional[str] = None,
         partition_column: Optional[str] = None,
         query: Optional[str] = None,
         fetch_size: Optional[int] = None,
-        path: Optional[str] = None,
     ) -> None:
         _data_source_params_converter.check(
             {
                 "data_store_id": data_store_id,
                 "catalog": catalog,
                 "table": table,
                 "schema": schema,
                 "partition_column": partition_column,
                 "query": query,
                 "fetch_size": fetch_size,
-                "path": path,
             }
         )
         self.data_store_id = data_store_id
         self.catalog = catalog
         self.table = table
         self.schema = schema
         self.partition_column = partition_column
         self.query = query
         self.fetch_size = fetch_size
-        self.path = path
 
     def collect_payload(self) -> DataSourceParametersPayload:
         return {
             "data_store_id": self.data_store_id,
             "catalog": self.catalog,
             "table": self.table,
             "schema": self.schema,
             "partition_column": self.partition_column,
             "query": self.query,
             "fetch_size": self.fetch_size,
-            "path": self.path,
         }
 
     @classmethod
     def from_server_data(cls, data: ServerDataType) -> DataSourceParameters:
         converted_data = _data_source_params_converter.check(from_api(data))
         return cls(**converted_data)
 
@@ -196,16 +188,15 @@
     def list(cls, typ: Optional[DataStoreListTypes] = None) -> List[DataSource]:
         """
         Returns list of available data sources.
 
         Parameters
         ----------
         typ : DataStoreListTypes
-            If specified, filters by specified datasource type. If not specified it will
-            default to DataStoreListTypes.DATABASES
+            If specified, filters by specified datasource type.
 
         Returns
         -------
         data_sources : list of DataSource instances
             contains a list of available data sources.
 
         Examples
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/data_store.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 from datarobot.utils.pagination import unpaginate
 
 field_converter = t.Dict(
     {t.Key("id"): String(), t.Key("name"): String(), t.Key("value"): String()}
 ).ignore_extra("*")
 _data_store_params_converter = t.Dict(
     {
-        t.Key("driver_id", optional=True): t.Or(String(), t.Null()),
-        t.Key("connector_id", optional=True): t.Or(String(), t.Null()),
+        t.Key("driver_id"): String(),
         t.Key("jdbc_url", optional=True): t.Or(String(), t.Null()),
         t.Key("fields", optional=True): t.Or(t.List(field_converter), t.Null()),
     }
 ).ignore_extra("*")
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
@@ -60,51 +59,33 @@
 
 class DataStoreParameters:
     """A data store's parameters'
 
     Attributes
     ----------
     driver_id : str
-        Optional. The identifier of the data driver if the type is one of DataStoreTypes.DR_DATABASE_V1
-        or DataStoreTypes.JDBC.
+            The identifier of the data driver.
     jdbc_url : str
         Optional. The full JDBC URL (for example: `jdbc:postgresql://my.dbaddress.org:5432/my_db`).
     fields: list
         Optional. If the type is `dr-database-v1`, then the fields specify the configuration.
-    connector_id: str
-        Optional. The connector identifier if the type is DataStoreTypes.DR_CONNECTOR_V1.
     """
 
     def __init__(
-        self,
-        driver_id: Optional[str],
-        jdbc_url: Optional[str],
-        fields: Optional[List[Dict[str, str]]] = None,
-        connector_id: Optional[str] = None,
+        self, driver_id: str, jdbc_url: Optional[str], fields: Optional[List[Dict[str, str]]] = None
     ):
         _data_store_params_converter.check(
-            {
-                "driver_id": driver_id,
-                "jdbc_url": jdbc_url,
-                "fields": fields,
-                "connector_id": connector_id,
-            }
+            {"driver_id": driver_id, "jdbc_url": jdbc_url, "fields": fields}
         )
         self.driver_id = driver_id
-        self.connector_id = connector_id
         self.jdbc_url = jdbc_url
         self.fields = fields
 
     def collect_payload(self) -> Dict[str, Any]:
-        """Build a dict of the parameters to send to the server"""
-        dat: Dict[str, Any] = {}
-        if self.driver_id:
-            dat["driver_id"] = self.driver_id
-        if self.connector_id:
-            dat["connector_id"] = self.connector_id
+        dat: Dict[str, Any] = {"driver_id": self.driver_id}
         if self.jdbc_url:
             dat["jdbc_url"] = self.jdbc_url
         if self.fields:
             dat["fields"] = self.fields
         return dat
 
 
@@ -157,28 +138,22 @@
         self.canonical_name = canonical_name
         self._creator = creator
         self._updated = updated
         self.params = params
         self.role = role
 
     @classmethod
-    def list(
-        cls, typ: Optional[Union[str, DataStoreListTypes]] = None, name: Optional[str] = None
-    ) -> List[DataStore]:
+    def list(cls, typ: Optional[Union[str, DataStoreListTypes]] = None) -> List[DataStore]:
         """
         Returns list of available data stores.
 
         Parameters
         ----------
         typ : str
-            If specified, filters by specified data store type. If not specified, the default
-            is DataStoreListTypes.JDBC.
-        name: str
-            If specified, filters by data store names that match or contain this name.
-            The search is case-insensitive.
+            If specified, filters by specified data store type.
 
         Returns
         -------
         data_stores : list of DataStore instances
             contains a list of available data stores.
 
         Examples
@@ -186,22 +161,16 @@
         .. code-block:: python
 
             >>> import datarobot as dr
             >>> data_stores = dr.DataStore.list()
             >>> data_stores
             [DataStore('Demo'), DataStore('Airlines')]
         """
-        params = {}
-        if typ:
-            params["type"] = typ
-        if name:
-            params["name"] = name
-
-        if params:
-            r_data = cls._client.get(cls._path, params=params).json()
+        if typ is not None:
+            r_data = cls._client.get(cls._path, params={"type": str(typ)}).json()
         else:
             r_data = cls._client.get(cls._path).json()
         return [cls.from_server_data(item) for item in r_data["data"]]
 
     @classmethod
     def get(cls, data_store_id: str) -> DataStore:
         """
@@ -229,37 +198,34 @@
         return cls.from_location(f"{cls._path}{data_store_id}/")
 
     @classmethod
     def create(
         cls,
         data_store_type: Union[str, DataStoreTypes],
         canonical_name: str,
-        driver_id: Optional[str] = None,
+        driver_id: str,
         jdbc_url: Optional[str] = None,
         fields: Optional[List[Dict[str, str]]] = None,
-        connector_id: Optional[str] = None,
     ) -> DataStore:
         """
         Creates the data store.
 
         Parameters
         ----------
         data_store_type : str or DataStoreTypes
             the type of data store.
         canonical_name : str
             the user-friendly name of the data store.
         driver_id : str
-            Optional. The identifier of the DataDriver if data_store_type is DataStoreListTypes.JDBC or
-            DataStoreListTypes.DR_DATABASE_V1.
+            the identifier of the DataDriver.
         jdbc_url : str
             Optional. The full JDBC URL (for example: `jdbc:postgresql://my.dbaddress.org:5432/my_db`).
         fields: list
             Optional. If the type is `dr-database-v1`, then the fields specify the configuration.
-        connector_id: str
-            Optional. The identifier of the Connector if data_store_type is DataStoreListTypes.DR_CONNECTOR_V1
+
         Returns
         -------
         data_store : DataStore
             the created data store.
 
         Examples
         --------
@@ -275,39 +241,35 @@
             >>> data_store
             DataStore('Demo DB')
         """
         payload = {
             "type": str(data_store_type),
             "canonicalName": canonical_name,
             "params": DataStoreParameters(
-                driver_id=driver_id, jdbc_url=jdbc_url, fields=fields, connector_id=connector_id
+                driver_id=driver_id, jdbc_url=jdbc_url, fields=fields
             ).collect_payload(),
         }
         return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
 
     def update(
         self,
         canonical_name: Optional[str] = None,
         driver_id: Optional[str] = None,
-        connector_id: Optional[str] = None,
         jdbc_url: Optional[str] = None,
         fields: Optional[List[Dict[str, str]]] = None,
     ) -> None:
         """
         Updates the data store.
 
         Parameters
         ----------
         canonical_name : str
             optional, the user-friendly name of the data store.
         driver_id : str
-            Optional. The identifier of the DataDriver. if the type is one of DataStoreTypes.DR_DATABASE_V1
-            or DataStoreTypes.JDBC.
-        connector_id : str
-            Optional. The identifier of the Connector. if the type is DataStoreTypes.DR_CONNECTOR_V1.
+            optional, the identifier of the DataDriver.
         jdbc_url : str
             Optional. The full JDBC URL (for example: `jdbc:postgresql://my.dbaddress.org:5432/my_db`).
         fields: list
             Optional. If the type is `dr-database-v1`, then the fields specify the configuration.
 
         Examples
         --------
@@ -319,34 +281,30 @@
             DataStore('Demo DB')
             >>> data_store.update(canonical_name='Demo DB updated')
             >>> data_store
             DataStore('Demo DB updated')
         """
         params = DataStoreParameters(
             driver_id=driver_id or self.params.driver_id,  # type: ignore[union-attr]
-            connector_id=connector_id or self.params.connector_id,  # type: ignore[union-attr]
             jdbc_url=jdbc_url or self.params.jdbc_url,  # type: ignore[union-attr]
             fields=fields or self.params.fields,  # type: ignore[union-attr]
         ).collect_payload()
-        # if we are updating fields, then we cannot include driver_id or connector_id
+        # if we are updating dr-database-v1 fields, then we cannot include driver_id
         if params.get("fields"):
-            params.pop("driver_id", None)
-            params.pop("connector_id", None)
-
+            del params["driver_id"]
         payload = {
             "canonicalName": canonical_name or self.canonical_name,
             "params": params,
         }
         r_data = self._client.patch(f"{self._path}{self.id}/", data=payload).json()
         self.canonical_name = r_data["canonicalName"]
         self.params = DataStoreParameters(
-            r_data["params"].get("driverId"),
+            r_data["params"]["driverId"],
             r_data["params"].get("jdbcUrl"),
             r_data["params"].get("fields"),
-            r_data["params"].get("connectorId"),
         )
 
     def delete(self) -> None:
         """Removes the DataStore"""
         self._client.delete(f"{self._path}{self.id}/")
 
     def test(
@@ -469,18 +427,15 @@
     @classmethod
     def from_server_data(  # type: ignore[override]
         cls, data: ServerDataType, keep_attrs: Optional[List[str]] = None
     ) -> DataStore:
         converted_data = cls._converter.check(from_api(data))
         params = converted_data.pop("params")
         converted_data["params"] = DataStoreParameters(
-            params.get("driver_id"),
-            params.get("jdbc_url"),
-            params.get("fields"),
-            params.get("connector_id"),
+            params["driver_id"], params.get("jdbc_url"), params.get("fields")
         )
         return cls(**converted_data)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}('{self.canonical_name or self.id}')"
 
     @property
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/challenger.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/challenger.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/champion_model_package.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/champion_model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/custom_metrics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/custom_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,21 +20,17 @@
 
 from datarobot.enums import (
     BUCKET_SIZE,
     CustomMetricAggregationType,
     CustomMetricBucketTimeStep,
     CustomMetricDirectionality,
     DEFAULT_MAX_WAIT,
-    HostedCustomMetricsTemplateMetricTypeQueryParams,
-    ListHostedCustomMetricTemplatesSortQueryParams,
 )
 from datarobot.models.api_object import APIObject
 from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
-from datarobot.models.runtime_parameters import RuntimeParameterValue
-from datarobot.models.types import Schedule
 from datarobot.utils import from_api, to_api, underscorize
 from datarobot.utils.waiters import wait_for_async_resolution
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class BaselineValues(TypedDict, total=False):
@@ -1589,335 +1585,7 @@
             segment_value=segment_value,
         )
         data = cls._client.get(path, params=params).json()
         case_converted = from_api(data, keep_null_keys=True)
         custom_metric_summary = cls.from_data(case_converted)
         custom_metric_summary.deployment_id = deployment_id
         return custom_metric_summary
-
-
-class HostedCustomMetricTemplate(APIObject):
-    """
-    Template for hosted custom metric.
-    """
-
-    _path = "customMetricsTemplates/"
-
-    _converter = t.Dict(
-        {
-            t.Key("id"): t.String(),
-            t.Key("name"): t.String(),
-            t.Key("description"): t.String(),
-            t.Key("custom_metric_metadata"): t.Dict().allow_extra("*"),
-            t.Key("default_environment"): t.Dict().allow_extra("*"),
-            t.Key("items"): t.List(t.Dict().allow_extra("*")),
-            t.Key("template_metric_type"): t.String(),
-        }
-    )
-
-    def __init__(
-        self,
-        id: str,
-        name: str,
-        description: str,
-        custom_metric_metadata: Dict[str, Any],
-        default_environment: Dict[str, Any],
-        items: List[Dict[str, Any]],
-        template_metric_type: str,
-    ):
-        self.id = id
-        self.name = name
-        self.description = description
-        self.custom_metric_metadata = custom_metric_metadata
-        self.default_environment = default_environment
-        self.items = items
-        self.template_metric_type = template_metric_type
-
-    @classmethod
-    def list(
-        cls,
-        search: Optional[str] = None,
-        order_by: Optional[ListHostedCustomMetricTemplatesSortQueryParams] = None,
-        metric_type: Optional[HostedCustomMetricsTemplateMetricTypeQueryParams] = None,
-        offset: Optional[int] = None,
-        limit: Optional[int] = None,
-    ) -> List[HostedCustomMetricTemplate]:
-        """List all hosted custom metric templates.
-
-        Parameters
-        ----------
-        search: Optional[str]
-            Search string.
-        order_by: Optional[ListHostedCustomMetricTemplatesSortQueryParams]
-            Ordering field.
-        metric_type: Optional[HostedCustomMetricsTemplateMetricTypeQueryParams]
-            Type of the metric.
-        offset: Optional[int]
-            Offset for pagination.
-        limit: Optional[int]
-            Limit for pagination.
-
-        Returns
-        -------
-        templates: List[HostedCustomMetricTemplate]
-        """
-        params: Dict[str, Any] = {}
-        if search:
-            params["search"] = search
-        if order_by:
-            params["orderBy"] = order_by
-        if metric_type:
-            params["templateMetricType"] = metric_type
-        if offset:
-            params["offset"] = offset
-        if limit:
-            params["limit"] = limit
-        response = cls._client.get(cls._path, params=params if params else None)
-        return [cls.from_server_data(d) for d in response.json()["data"]]
-
-    @classmethod
-    def get(cls, template_id: str) -> HostedCustomMetricTemplate:
-        """Get a hosted custom metric template by ID.
-
-        Parameters
-        ----------
-        template_id: str
-            ID of the template.
-
-        Returns
-        -------
-        template : HostedCustomMetricTemplate
-        """
-        response = cls._client.get(f"{cls._path}{template_id}/")
-        return cls.from_server_data(response.json())
-
-
-class MetricTimestampSpoofing:
-    """
-    Custom metric timestamp spoofing. Occurs when reading values from a file, like a dataset.
-    By default, replicates pd.to_datetime formatting behavior.
-    """
-
-    def __init__(self, column_name: str, time_format: Optional[str] = None, **kwargs):  # type: ignore[no-untyped-def]
-        self.column_name = column_name
-        self.time_format = time_format
-
-
-class BatchField:
-    """
-    A custom metric batch ID source for when reading values from a columnar dataset like a file.
-    """
-
-    def __init__(self, column_name: str, **kwargs):  # type: ignore[no-untyped-def]
-        self.column_name = column_name
-
-
-class ValueField:
-    """
-    A custom metric value source for when reading values from a columnar dataset like a file.
-    """
-
-    def __init__(self, column_name: str, **kwargs):  # type: ignore[no-untyped-def]
-        self.column_name = column_name
-
-
-class SampleCountField:
-    """
-    A weight column used with columnar datasets if pre-aggregated metric values are provided.
-    """
-
-    def __init__(self, column_name: str, **kwargs):  # type: ignore[no-untyped-def]
-        self.column_name = column_name
-
-
-class MetricBaselineValue:
-    """
-    The baseline values for a custom metric.
-    """
-
-    def __init__(self, value: float, **kwargs):  # type: ignore[no-untyped-def]
-        self.value = value
-
-
-class DeploymentDetails:
-    """
-    Information about a hosted custom metric deployment.
-    """
-
-    def __init__(  # type: ignore[no-untyped-def]
-        self,
-        id: str,
-        name: str,
-        creator_first_name: Optional[str] = None,
-        creator_last_name: Optional[str] = None,
-        creator_username: Optional[str] = None,
-        creator_gravatar_hash: Optional[str] = None,
-        created_at: Optional[str] = None,
-        **kwargs,
-    ):
-        self.id = id
-        self.name = name
-        self.creator_first_name = creator_first_name
-        self.creator_last_name = creator_last_name
-        self.creator_username = creator_username
-        self.creator_gravatar_hash = creator_gravatar_hash
-        self.created_at = created_at
-
-
-class HostedCustomMetric(APIObject):
-    """
-    Hosted custom metric.
-    """
-
-    _converter = t.Dict(
-        {
-            t.Key("id"): t.String(),
-            t.Key("deployment"): t.Dict().allow_extra("*"),
-            t.Key("schedule", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null()),
-            t.Key("units"): t.String(),
-            t.Key("type"): t.String(),
-            t.Key("is_model_specific"): t.Bool(),
-            t.Key("directionality"): t.String(),
-            t.Key("time_step"): t.String(),
-            t.Key("created_at"): t.String(),
-            t.Key("created_by"): t.Dict().allow_extra("*"),
-            t.Key("name"): t.String(),
-            t.Key(
-                "description",
-                optional=True,
-            ): t.Or(t.String(allow_blank=True), t.Null()),
-            t.Key("baseline_values", optional=True): t.Or(
-                t.List(t.Dict().allow_extra("*")), t.Null()
-            ),
-            t.Key("timestamp", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null()),
-            t.Key("value", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null()),
-            t.Key("sample_count", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null()),
-            t.Key("batch", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null()),
-            t.Key("parameter_overrides", optional=True): t.Or(
-                t.List(t.Dict().allow_extra("*")), t.Null()
-            ),
-        }
-    ).allow_extra("*")
-
-    def __init__(
-        self,
-        id: str,
-        deployment: Dict[str, Any],
-        units: str,
-        type: str,
-        is_model_specific: bool,
-        directionality: str,
-        time_step: str,
-        created_at: str,
-        created_by: Dict[str, Any],
-        name: str,
-        description: Optional[str] = None,
-        schedule: Optional[Schedule] = None,
-        baseline_values: Optional[List[Dict[str, Any]]] = None,
-        timestamp: Optional[Dict[str, Any]] = None,
-        value: Optional[Dict[str, Any]] = None,
-        sample_count: Optional[Dict[str, Any]] = None,
-        batch: Optional[Dict[str, Any]] = None,
-        parameter_overrides: Optional[List[Dict[str, Any]]] = None,
-    ):
-        """
-
-        Parameters
-        ----------
-        id: str
-            ID of the hosted custom metric.
-        deployment: Dict[str, Any]
-            Deployment details.
-        units: str
-            Units of the metric.
-        type: str
-            Type of the metric.
-        is_model_specific: bool
-            Whether the metric is model specific.
-        directionality: str
-            Directionality of the metric.
-        time_step: str
-            Time step of the metric.
-        created_at: str
-            Creation time of the metric.
-        created_by: Dict[str, Any]
-            Creator details.
-        name: str
-            Name of the metric.
-        description: Optional[str]
-            Description of the metric.
-        schedule: Optional[Dict[str, Any]]
-            Schedule details.
-        baseline_values: Optional[List[Dict[str, Any]]
-            Baseline values.
-        timestamp: Optional[Dict[str, Any]]
-            Timestamp details.
-        value: Optional[Dict[str, Any]]
-            Value details.
-        sample_count: Optional[Dict[str, Any]]
-            Sample count details.
-        batch: Optional[Dict[str, Any]]
-            Batch details.
-        parameter_overrides: Optional[List[Dict[str, Any]]
-            Parameter overrides.
-        """
-        self.id = id
-        self.deployment = DeploymentDetails(**deployment)
-        self.schedule = Schedule(**schedule) if schedule else None  # type: ignore[misc]
-        self.units = units
-        self.type = type
-        self.is_model_specific = is_model_specific
-        self.directionality = directionality
-        self.time_step = time_step
-        self.created_at = created_at
-        self.created_by = created_by
-        self.name = name
-        self.description = description
-        self.baseline_values = (
-            [MetricBaselineValue(**value) for value in baseline_values] if baseline_values else None
-        )
-        self.timestamp = MetricTimestampSpoofing(**timestamp) if timestamp else None
-        self.value = ValueField(**value) if value else None
-        self.sample_count = SampleCountField(**sample_count) if batch else None  # type: ignore[arg-type]
-        self.batch = BatchField(**batch) if batch else None
-        parameter_overrides = self._impute_null_runtime_parameter_values(parameter_overrides)
-        self.parameter_overrides = (
-            [RuntimeParameterValue(**param) for param in parameter_overrides]
-            if parameter_overrides
-            else None
-        )
-
-    def _impute_null_runtime_parameter_values(
-        self, values: Optional[List[Dict[str, Any]]]
-    ) -> Optional[List[Dict[str, Any]]]:
-        if not values:
-            return values
-        for param in values:
-            if "value" not in values:
-                param["value"] = None
-        return values
-
-    @classmethod
-    def list(
-        cls,
-        job_id: str,
-        skip: Optional[int] = None,
-        limit: Optional[int] = None,
-    ) -> List[HostedCustomMetric]:
-        """List all hosted custom metrics for a job.
-
-        Parameters
-        ----------
-        job_id: str
-            ID of the job.
-
-        Returns
-        -------
-        metrics: List[HostedCustomMetric]
-        """
-        params: Dict[str, Any] = {}
-        if skip:
-            params["skip"] = skip
-        if limit:
-            params["limit"] = limit
-        response = cls._client.get(f"customJobs/{job_id}/customMetrics/", params=params)
-        return [cls.from_server_data(d) for d in response.json()["data"]]
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/data_exports.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_exports.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/documentai/document.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/driver.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/execution_environment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_effect.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/feature_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/featurelist.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/chat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/chat_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,25 +231,24 @@
     llm_blueprint_id : str
         ID of the LLM blueprint associated with the chat prompt.
     llm_id : str
         ID of the LLM type. This must be one of the IDs returned by `LLMDefinition.list`
         for this user.
     llm_settings : dict or None
         The LLM settings for the LLM blueprint. The specific keys allowed and the
-        constraints on the values are defined in the response from `LLMDefinition.list`,
-        but this typically has dict fields. Either:
-        - system_prompt - The system prompt that influences the LLM responses.
-        - max_completion_length - The maximum number of tokens in the completion.
-        - temperature - Controls the variability in the LLM response.
-        - top_p - Sets whether the model considers next tokens with top_p probability mass.
+        constraints on the values are defined in the response from `LLMDefinition.list`
+        but this typically has dict fields:
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - max_completion_length - The maximum number of token in the completion.
+        - temperature - controls the variability in the LLM response.
+        - top_p - the model considers next tokens with top_p probability mass
         or
-        - system_prompt - The system prompt that influences the LLM responses.
-        - validation_id - The ID of the external model LLM validation.
-        - external_llm_context_size - The external LLM's context size, in tokens,
-        for external model-based LLM blueprints.
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - validation_id - The ID of the custom model LLM validation
+        for custom model LLM blueprints.
     creation_date : str
         The date the chat prompt was created.
     creation_user_id : str
         ID of the creating user.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
     vector_database_settings : VectorDatabaseSettings or None
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/comparison_chat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_chat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/comparison_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     id : str
         Comparison prompt ID.
     text : str
         The prompt text.
     results : list[ComparisonPromptResult]
         The list of results for individual LLM blueprints that are part of the comparison prompt.
     creation_date : str
-        The date when the playground was created.
+        Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
     comparison_chat_id : str
         The ID of the comparison chat this comparison prompt is associated with.
     """
 
     _path = "api/v2/genai/comparisonPrompts"
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/custom_model_llm_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_llm_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/custom_model_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/llm.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/llm_blueprint.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm_blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         t.Key("is_starred"): t.Bool,
         t.Key("playground_id"): t.String,
         t.Key("llm_id", optional=True): t.Or(t.String, t.Null),
         t.Key("llm_settings", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null),
         t.Key("llm_name", optional=True): t.Or(t.String, t.Null),
         t.Key("creation_date"): t.String,
         t.Key("creation_user_id"): t.String,
-        t.Key("creation_user_name"): t.String(allow_blank=True),
         t.Key("last_update_date"): t.String,
         t.Key("last_update_user_id"): t.String,
         t.Key("prompt_type"): t.Enum(*enum_to_list(PromptType)),
         t.Key("vector_database_id", optional=True): t.Or(t.String, t.Null),
         t.Key("vector_database_settings", optional=True): t.Or(
             vector_database_settings_trafaret, t.Null
         ),
@@ -164,25 +163,22 @@
         but this typically has dict fields:
         - system_prompt - The system prompt that tells the LLM how to behave.
         - max_completion_length - The maximum number of token in the completion.
         - temperature - controls the variability in the LLM response.
         - top_p - the model considers next tokens with top_p probability mass
         or
         - system_prompt - The system prompt that tells the LLM how to behave.
-        - validation_id - The ID of the external model LLM validation
-        - external_llm_context_size - The external LLM's context size in tokens
-        for external model LLM blueprints.
+        - validation_id - The ID of the custom model LLM validation
+        for custom model LLM blueprints.
     creation_date : str
-        The date when the playground was created.
+        Date when the playground was created.
     creation_user_id : str
-        The ID of the user creating the playground.
-    creation_user_name : str
-        The name of the user creating the playground.
+        ID of the creating user.
     last_update_date : str
-        The date when the playground was most recently updated.
+        Date when the playground was most recently updated.
     last_update_user_id : str
         ID of the user who most recently updated the playground.
     prompt_type : PromptType
         The prompting strategy for the LLM Blueprint.
         Currently supported options are listed in PromptType.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
@@ -214,15 +210,14 @@
         name: str,
         description: str,
         is_saved: bool,
         is_starred: bool,
         playground_id: str,
         creation_date: str,
         creation_user_id: str,
-        creation_user_name: str,
         last_update_date: str,
         last_update_user_id: str,
         prompt_type: PromptType,
         llm_id: Optional[str] = None,
         llm_name: Optional[str] = None,
         llm_settings: Optional[LLMSettingsCommonDict | LLMSettingsCustomModelDict] = None,
         vector_database_id: Optional[str] = None,
@@ -242,15 +237,14 @@
         self.is_starred = is_starred
         self.playground_id = playground_id
         self.llm_id = llm_id
         self.llm_name = llm_name
         self.llm_settings = llm_settings
         self.creation_date = creation_date
         self.creation_user_id = creation_user_id
-        self.creation_user_name = creation_user_name
         self.last_update_date = last_update_date
         self.last_update_user_id = last_update_user_id
         self.prompt_type = prompt_type
         self.vector_database_id = vector_database_id
         self.vector_database_settings = (
             VectorDatabaseSettings.from_server_data(vector_database_settings)
             if vector_database_settings
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/playground.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/playground.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     name : str
         Playground name.
     description : str
         Description of the playground.
     use_case_id : str
         Linked use case ID.
     creation_date : str
-        The date when the playground was created.
+        Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
     last_update_date : str
         Date when the playground was most recently updated.
     last_update_user_id : str
         ID of the user who most recently updated the playground.
     saved_llm_blueprints_count : int
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/user_limits.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/user_limits.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/genai/vector_database.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/vector_database.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/key_values.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/key_values.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/missing_report.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/deployment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/registered_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/model_registry/registered_model_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/modeljob.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/pareto_front.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/predict_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prediction_environment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prediction_server.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/predictions.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/prime_file.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/project.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/project_options.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/rating_table.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/recommended_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/registry/job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,48 +475,7 @@
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
         """
 
         new_object = self.get(self.id)
         self._update_values(new_object)
-
-    @classmethod
-    def create_from_custom_metric_gallery_template(
-        cls,
-        template_id: str,
-        name: str,
-        description: Optional[str] = None,
-        sidecar_deployment_id: Optional[str] = None,
-    ) -> Job:
-        """Create a job from a custom metric gallery template.
-
-        Parameters
-        ----------
-        template_id: str
-            ID of the template.
-        name: str
-            Name of the job.
-        description: Optional[str]
-            Description of the job.
-        sidecar_deployment_id: Optional[str]
-            ID of the sidecar deployment. Only relevant for templates that use sidecar deployments.
-
-        Returns
-        -------
-        Job
-            retrieved job
-
-        Raises
-        ------
-        datarobot.errors.ClientError
-            if the server responded with 4xx status.
-        datarobot.errors.ServerError
-            if the server responded with 5xx status.
-        """
-        payload = {"name": name, "templateId": template_id}
-        if description:
-            payload["description"] = description
-        if sidecar_deployment_id:
-            payload["sidecarDeploymentId"] = sidecar_deployment_id
-        response = cls._client.post(f"{cls._path}fromCustomMetricGalleryTemplate/", data=payload)
-        return cls.from_server_data(response.json())
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/registry/job_run.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job_run.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/relationships_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,16 +175,16 @@
     """
 
     _path = "relationshipsConfigurations/"
     data_source_trafaret = t.Dict(
         {
             t.Key("data_store_name"): String,
             t.Key("data_store_id"): String,
-            t.Key("url", optional=True): t.Or(String, t.Null),
-            t.Key("dbtable", optional=True): t.Or(String, t.Null),
+            t.Key("url"): String,
+            t.Key("dbtable"): t.Or(String, t.Null),
             t.Key("schema", optional=True): t.Or(String(allow_blank=True), t.Null),
             t.Key("catalog", optional=True): t.Or(String(allow_blank=True), t.Null),
             t.Key("data_source_id", optional=True): t.Or(String, t.Null),
         }
     ).ignore_extra("*")
     feature_list_info = t.Dict(
         {
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/residuals.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/roc_curve.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/ruleset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/runtime_parameters.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/segmentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/shap_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/sharing.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/status_check_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/status_check_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/trafarets.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/training_predictions.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/types.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/use_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,14 +575,15 @@
             >>> user_ids = ["60912e09fd1f04e832a575c1", "639ce542862e9b1b1bfa8f1b", "63e185e7cd3a5f8e190c6393"]
             >>> sharing_roles = []
             >>> for user_id in user_ids:
             ...     new_sharing_role = SharingRole(
             ...         role=SHARING_ROLE.CONSUMER,
             ...         share_recipient_type=SHARING_RECIPIENT_TYPE.USER,
             ...         id=user_id,
+            ...         can_share=True,
             ...     )
             ...     sharing_roles.append(new_sharing_role)
             >>> use_case = UseCase.get(use_case_id="5f33f1fd9071ae13568237b2")
             >>> use_case.share(roles=sharing_roles)
 
         Similarly, a :class:`SharingRole <datarobot.models.sharing.SharingRole>` instance can be used to
         remove a user's access if the ``role`` is set to ``SHARING_ROLE.NO_ROLE``, like in this example:
@@ -594,14 +595,15 @@
             >>> from datarobot.enums import SHARING_ROLE, SHARING_RECIPIENT_TYPE
             >>>
             >>> user_to_remove = "foo.bar@datarobot.com"
             ... remove_sharing_role = SharingRole(
             ...     role=SHARING_ROLE.NO_ROLE,
             ...     share_recipient_type=SHARING_RECIPIENT_TYPE.USER,
             ...     username=user_to_remove,
+            ...     can_share=False,
             ... )
             >>> use_case = UseCase.get(use_case_id="5f33f1fd9071ae13568237b2")
             >>> use_case.share(roles=[remove_sharing_role])
         """
         if any(
             role.role
             not in [
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/use_cases/utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/validators.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/visualai/images.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/models/word_cloud.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/rest.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/deprecation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/pagination.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/retry.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/source.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot/utils/waiters.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.5.0.2024.5.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,83 @@
 Metadata-Version: 2.1
-Name: datarobot-early-access
-Version: 3.5.0.2024.5.22
+Name: datarobot_early_access
+Version: 3.5.0.2024.5.6
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
 Project-URL: Documentation, https://datarobot-public-api-client.readthedocs-hosted.com/en/early-access/
 Project-URL: Changelog, https://datarobot-public-api-client.readthedocs-hosted.com/en/early-access/CHANGES.html
+Description: 
+        About datarobot_early_access
+        ============================
+        .. image:: https://img.shields.io/pypi/v/datarobot_early_access.svg
+           :target: https://pypi.python.org/pypi/datarobot-early-access/
+        .. image:: https://img.shields.io/pypi/pyversions/datarobot_early_access.svg
+        .. image:: https://img.shields.io/pypi/status/datarobot_early_access.svg
+        
+        DataRobot is a client library for working with the `DataRobot`_ platform API. This package is the "early access" version of the client. **Do NOT use this package in production--you will expose yourself to risk of breaking changes and bugs.** For the most stable version, see the quarterly release on PyPI at https://pypi.org/project/datarobot/.
+        
+        This package is released under the terms of the DataRobot Tool and Utility Agreement, which
+        can be found on our `Legal`_ page, along with our privacy policy and more.
+        
+        Installation
+        =========================
+        Python >= 3.7 are supported.
+        You must have a datarobot account.
+        
+        ::
+        
+           $ pip install datarobot_early_access
+        
+        Usage
+        =========================
+        The library will look for a config file `~/.config/datarobot/drconfig.yaml` by default.
+        This is an example of what that config file should look like.
+        
+        ::
+        
+           token: your_token
+           endpoint: https://app.datarobot.com/api/v2
+        
+        Alternatively a global client can be set in the code.
+        
+        ::
+        
+           import datarobot as dr
+           dr.Client(token='your_token', endpoint='https://app.datarobot.com/api/v2')
+        
+        Alternatively environment variables can be used.
+        
+        ::
+        
+           export DATAROBOT_API_TOKEN='your_token'
+           export DATAROBOT_ENDPOINT='https://app.datarobot.com/api/v2'
+        
+        See `documentation`_ for example usage after configuring.
+        
+        Helpful links
+        =========================
+        - `API quickstart guide <https://docs.datarobot.com/en/docs/api/api-quickstart/index.html>`_
+        - `Code examples <https://docs.datarobot.com/en/docs/api/guide/python/index.html>`_
+        - `Common use cases <https://docs.datarobot.com/en/docs/api/guide/common-case/index.html>`_
+        
+        Bug Reporting and Q&A
+        =========================
+        Create an account on `DataRobot Community <https://community.datarobot.com/>`_ and post your questions and bug reports
+        `here <https://community.datarobot.com/t5/forums/postpage/board-id/datarobot-api>`_.
+        
+        .. _datarobot: https://datarobot.com
+        .. _documentation: https://datarobot-public-api-client.readthedocs-hosted.com/en/early-access/
+        .. _legal: https://www.datarobot.com/legal/
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -25,72 +89,7 @@
 Requires-Python: >=3.7
 Provides-Extra: dev
 Provides-Extra: examples
 Provides-Extra: release
 Provides-Extra: lint
 Provides-Extra: images
 Provides-Extra: test
-Provides-Extra: databricks
-License-File: LICENSE.txt
-
-
-About datarobot_early_access
-============================
-.. image:: https://img.shields.io/pypi/v/datarobot_early_access.svg
-   :target: https://pypi.python.org/pypi/datarobot-early-access/
-.. image:: https://img.shields.io/pypi/pyversions/datarobot_early_access.svg
-.. image:: https://img.shields.io/pypi/status/datarobot_early_access.svg
-
-DataRobot is a client library for working with the `DataRobot`_ platform API. This package is the "early access" version of the client. **Do NOT use this package in production--you will expose yourself to risk of breaking changes and bugs.** For the most stable version, see the quarterly release on PyPI at https://pypi.org/project/datarobot/.
-
-This package is released under the terms of the DataRobot Tool and Utility Agreement, which
-can be found on our `Legal`_ page, along with our privacy policy and more.
-
-Installation
-=========================
-Python >= 3.7 are supported.
-You must have a datarobot account.
-
-::
-
-   $ pip install datarobot_early_access
-
-Usage
-=========================
-The library will look for a config file `~/.config/datarobot/drconfig.yaml` by default.
-This is an example of what that config file should look like.
-
-::
-
-   token: your_token
-   endpoint: https://app.datarobot.com/api/v2
-
-Alternatively a global client can be set in the code.
-
-::
-
-   import datarobot as dr
-   dr.Client(token='your_token', endpoint='https://app.datarobot.com/api/v2')
-
-Alternatively environment variables can be used.
-
-::
-
-   export DATAROBOT_API_TOKEN='your_token'
-   export DATAROBOT_ENDPOINT='https://app.datarobot.com/api/v2'
-
-See `documentation`_ for example usage after configuring.
-
-Helpful links
-=========================
-- `API quickstart guide <https://docs.datarobot.com/en/docs/api/api-quickstart/index.html>`_
-- `Code examples <https://docs.datarobot.com/en/docs/api/guide/python/index.html>`_
-- `Common use cases <https://docs.datarobot.com/en/docs/api/guide/common-case/index.html>`_
-
-Bug Reporting and Q&A
-=========================
-Create an account on `DataRobot Community <https://community.datarobot.com/>`_ and post your questions and bug reports
-`here <https://community.datarobot.com/t5/forums/postpage/board-id/datarobot-api>`_.
-
-.. _datarobot: https://datarobot.com
-.. _documentation: https://datarobot-public-api-client.readthedocs-hosted.com/en/early-access/
-.. _legal: https://www.datarobot.com/legal/
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 datarobot/errors.py
 datarobot/py.typed
 datarobot/rest.py
 datarobot/_experimental/__init__.py
 datarobot/_experimental/models/__init__.py
 datarobot/_experimental/models/chunking_service.py
 datarobot/_experimental/models/data_matching.py
-datarobot/_experimental/models/data_store.py
 datarobot/_experimental/models/dataset.py
 datarobot/_experimental/models/enums.py
 datarobot/_experimental/models/idiomatic_project.py
 datarobot/_experimental/models/incremental_learning.py
 datarobot/_experimental/models/model.py
 datarobot/_experimental/models/model_lineage.py
 datarobot/_experimental/models/notebooks.py
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,37 +5,35 @@
 requests_toolbelt>=0.6
 trafaret!=1.1.0,<2.2,>=0.7
 urllib3<2.0.0,>=1.23
 typing-extensions<5,>=4.3.0
 mypy-extensions<2,>=0.4.0
 strenum>=0.4.15
 
-[databricks]
-databricks-connect>=13.0
-
 [dev]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
 pytest-asyncio==0.21.1
 pyarrow
 Pillow==9.2.0
-databricks-connect>=13.0
 black==22.8.0
 black[jupyter]==22.8.0
 isort==5.10.1
 flake8==5.0.4
 pylint==2.15.0
 mypy==1.0.0
 types-PyYAML==6.0.12
 types-python-dateutil==2.8.19
 types-pytz==2022.2.1.0
 types-requests==2.28.11
 types-urllib3==1.26.25
+Pillow==9.2.0
+Pillow==9.2.0
 sphinx_rtd_theme==1.0.0
 nbsphinx==0.8.9
 numpydoc==1.4.0
 jupyter_contrib_nbextensions
 sphinx-autodoc-typehints==1.17.1
 sphinxcontrib-spelling==8.0.0
 pyenchant==3.2.2
@@ -61,21 +59,19 @@
 mypy==1.0.0
 types-PyYAML==6.0.12
 types-python-dateutil==2.8.19
 types-pytz==2022.2.1.0
 types-requests==2.28.11
 types-urllib3==1.26.25
 Pillow==9.2.0
-databricks-connect>=13.0
 
 [release]
 zest.releaser[recommended]==6.22.0
 
 [test]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
 pytest-asyncio==0.21.1
 pyarrow
 Pillow==9.2.0
-databricks-connect>=13.0
```

### Comparing `datarobot_early_access-3.5.0.2024.5.22/pyproject.toml` & `datarobot_early_access-3.5.0.2024.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/setup.py` & `datarobot_early_access-3.5.0.2024.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.22/setup_weekly.py` & `datarobot_early_access-3.5.0.2024.5.6/setup_weekly.py`

 * *Files identical despite different names*

