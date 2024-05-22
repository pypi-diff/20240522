# Comparing `tmp/data_factory_testing_framework-0.2.8.tar.gz` & `tmp/data_factory_testing_framework-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_factory_testing_framework-0.2.8.tar", max compression
+gzip compressed data, was "data_factory_testing_framework-0.2.9.tar", max compression
```

## Comparing `data_factory_testing_framework-0.2.8.tar` & `data_factory_testing_framework-0.2.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1141 2024-05-01 08:28:50.110453 data_factory_testing_framework-0.2.8/LICENSE
--rw-r--r--   0        0        0     5642 2024-05-01 08:28:50.110453 data_factory_testing_framework-0.2.8/README.md
--rw-r--r--   0        0        0     2053 2024-05-01 08:30:14.394157 data_factory_testing_framework-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      260 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/__init__.py
--rw-r--r--   0        0        0      794 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/_deserializer_base.py
--rw-r--r--   0        0        0      496 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/_deserializer_data_factory.py
--rw-r--r--   0        0        0      539 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/_deserializer_fabric.py
--rw-r--r--   0        0        0        0 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/shared/__init__.py
--rw-r--r--   0        0        0     2851 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/shared/_activity_deserializer.py
--rw-r--r--   0        0        0     2077 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/shared/_data_factory_element_replacer.py
--rw-r--r--   0        0        0       13 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/__init__.py
--rw-r--r--   0        0        0       96 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/__init__.py
--rw-r--r--   0        0        0     1051 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/exceptions.py
--rw-r--r--   0        0        0     7135 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/expression_evaluator.py
--rw-r--r--   0        0        0     3387 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/expression_rule_transformer.py
--rw-r--r--   0        0        0     3204 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/expression_terminal_transformer.py
--rw-r--r--   0        0        0     2105 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/__init__.py
--rw-r--r--   0        0        0     1351 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/activity_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1898 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/branch_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1484 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/dataset_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1681 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/evaluation_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1227 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/expression_parameter_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1990 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/expression_rule_evaluator.py
--rw-r--r--   0        0        0     3226 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/function_call_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1113 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/item_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1467 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/linked_service_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1192 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/literal_evaluation_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1477 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/literal_interpolation_expression_rule_evaluator.py
--rw-r--r--   0        0        0     2896 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/logical_bool_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1685 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/pipeline_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1514 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/system_variable_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     1335 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/variable_reference_expression_rule_evaluator.py
--rw-r--r--   0        0        0     5937 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_collection_implementation.py
--rw-r--r--   0        0        0     5437 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_conversion_implementation.py
--rw-r--r--   0        0        0    10102 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_date_implementation.py
--rw-r--r--   0        0        0     1679 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_logical_implementation.py
--rw-r--r--   0        0        0     2131 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_math_implementation.py
--rw-r--r--   0        0        0     4936 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_repository.py
--rw-r--r--   0        0        0     4190 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_string_implementation.py
--rw-r--r--   0        0        0       97 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_pythonnet/__init__.py
--rw-r--r--   0        0        0     3386 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_pythonnet/csharp_datetime.py
--rw-r--r--   0        0        0        0 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/__init__.py
--rw-r--r--   0        0        0      568 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/_factories/base_repository_factory.py
--rw-r--r--   0        0        0      900 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/_factories/data_factory_repository_factory.py
--rw-r--r--   0        0        0     3164 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/_factories/fabric_repository_factory.py
--rw-r--r--   0        0        0     1368 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/data_factory_repository.py
--rw-r--r--   0        0        0     9627 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_test_framework.py
--rw-r--r--   0        0        0     1815 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/__init__.py
--rw-r--r--   0        0        0      304 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_activity_not_found_error.py
--rw-r--r--   0        0        0      471 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_activity_output_field_not_found_error.py
--rw-r--r--   0        0        0      361 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_data_factory_element_evaluation_error.py
--rw-r--r--   0        0        0      607 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_function_call_invalid_arguments_count_error.py
--rw-r--r--   0        0        0      325 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_parameter_not_found_error.py
--rw-r--r--   0        0        0      705 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_pipeline_activities_circular_dependency_error.py
--rw-r--r--   0        0        0      272 2024-05-01 08:28:50.114453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_pipeline_not_found_error.py
--rw-r--r--   0        0        0      272 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_state_iteration_item_not_set_error.py
--rw-r--r--   0        0        0      301 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_unsupported_function_error.py
--rw-r--r--   0        0        0      120 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_user_error.py
--rw-r--r--   0        0        0      349 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_variable_being_evaluated_does_not_exist_error.py
--rw-r--r--   0        0        0      293 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_variable_not_found_error.py
--rw-r--r--   0        0        0      329 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/__init__.py
--rw-r--r--   0        0        0     1490 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/_data_factory_element.py
--rw-r--r--   0        0        0      126 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/_data_factory_object_type.py
--rw-r--r--   0        0        0     3687 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/_pipeline.py
--rw-r--r--   0        0        0      895 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/__init__.py
--rw-r--r--   0        0        0     4084 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_activity.py
--rw-r--r--   0        0        0      650 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_activity_dependency.py
--rw-r--r--   0        0        0     1272 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_append_variable_activity.py
--rw-r--r--   0        0        0      784 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_control_activity.py
--rw-r--r--   0        0        0     2626 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_execute_pipeline_activity.py
--rw-r--r--   0        0        0      789 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_fail_activity.py
--rw-r--r--   0        0        0     1263 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_filter_activity.py
--rw-r--r--   0        0        0     1670 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_for_each_activity.py
--rw-r--r--   0        0        0     1980 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_if_condition_activity.py
--rw-r--r--   0        0        0     1707 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_set_variable_activity.py
--rw-r--r--   0        0        0     2395 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_switch_activity.py
--rw-r--r--   0        0        0     1917 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_until_activity.py
--rw-r--r--   0        0        0        0 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/py.typed
--rw-r--r--   0        0        0      505 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/__init__.py
--rw-r--r--   0        0        0      751 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_activity_result.py
--rw-r--r--   0        0        0      279 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_dependency_condition.py
--rw-r--r--   0        0        0     8339 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_pipeline_run_state.py
--rw-r--r--   0        0        0      544 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_pipeline_run_variable.py
--rw-r--r--   0        0        0      656 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_run_parameter.py
--rw-r--r--   0        0        0      647 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_run_parameter_type.py
--rw-r--r--   0        0        0      534 2024-05-01 08:28:50.118453 data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_run_state.py
--rw-r--r--   0        0        0     6577 1970-01-01 00:00:00.000000 data_factory_testing_framework-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1141 2024-05-22 10:00:21.782463 data_factory_testing_framework-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5642 2024-05-22 10:00:21.782463 data_factory_testing_framework-0.2.9/README.md
+-rw-r--r--   0        0        0     2053 2024-05-22 10:02:01.102338 data_factory_testing_framework-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      260 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/__init__.py
+-rw-r--r--   0        0        0      794 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/_deserializer_base.py
+-rw-r--r--   0        0        0      496 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/_deserializer_data_factory.py
+-rw-r--r--   0        0        0      539 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/_deserializer_fabric.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/shared/__init__.py
+-rw-r--r--   0        0        0     2851 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/shared/_activity_deserializer.py
+-rw-r--r--   0        0        0     2077 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/shared/_data_factory_element_replacer.py
+-rw-r--r--   0        0        0       13 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/__init__.py
+-rw-r--r--   0        0        0       96 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/__init__.py
+-rw-r--r--   0        0        0     1051 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/exceptions.py
+-rw-r--r--   0        0        0     7135 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/expression_evaluator.py
+-rw-r--r--   0        0        0     3387 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/expression_rule_transformer.py
+-rw-r--r--   0        0        0     3204 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/expression_terminal_transformer.py
+-rw-r--r--   0        0        0     2105 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/__init__.py
+-rw-r--r--   0        0        0     1351 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/activity_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1898 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/branch_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1484 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/dataset_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1681 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/evaluation_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1227 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/expression_parameter_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1990 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/expression_rule_evaluator.py
+-rw-r--r--   0        0        0     3226 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/function_call_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1113 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/item_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1467 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/linked_service_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1192 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/literal_evaluation_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1477 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/literal_interpolation_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     2896 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/logical_bool_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1685 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/pipeline_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1514 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/system_variable_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     1335 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/variable_reference_expression_rule_evaluator.py
+-rw-r--r--   0        0        0     5937 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_collection_implementation.py
+-rw-r--r--   0        0        0     5437 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_conversion_implementation.py
+-rw-r--r--   0        0        0    10102 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_date_implementation.py
+-rw-r--r--   0        0        0     1679 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_logical_implementation.py
+-rw-r--r--   0        0        0     2131 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_math_implementation.py
+-rw-r--r--   0        0        0     4936 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_repository.py
+-rw-r--r--   0        0        0     4190 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_string_implementation.py
+-rw-r--r--   0        0        0       97 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_pythonnet/__init__.py
+-rw-r--r--   0        0        0     3386 2024-05-22 10:00:21.786463 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_pythonnet/csharp_datetime.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/_factories/base_repository_factory.py
+-rw-r--r--   0        0        0      900 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/_factories/data_factory_repository_factory.py
+-rw-r--r--   0        0        0     3164 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/_factories/fabric_repository_factory.py
+-rw-r--r--   0        0        0     1368 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/data_factory_repository.py
+-rw-r--r--   0        0        0     9627 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_test_framework.py
+-rw-r--r--   0        0        0     1815 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_activity_not_found_error.py
+-rw-r--r--   0        0        0      471 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_activity_output_field_not_found_error.py
+-rw-r--r--   0        0        0      361 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_data_factory_element_evaluation_error.py
+-rw-r--r--   0        0        0      607 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_function_call_invalid_arguments_count_error.py
+-rw-r--r--   0        0        0      325 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_parameter_not_found_error.py
+-rw-r--r--   0        0        0      705 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_pipeline_activities_circular_dependency_error.py
+-rw-r--r--   0        0        0      272 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_pipeline_not_found_error.py
+-rw-r--r--   0        0        0      272 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_state_iteration_item_not_set_error.py
+-rw-r--r--   0        0        0      301 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_unsupported_function_error.py
+-rw-r--r--   0        0        0      120 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_user_error.py
+-rw-r--r--   0        0        0      349 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_variable_being_evaluated_does_not_exist_error.py
+-rw-r--r--   0        0        0      293 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_variable_not_found_error.py
+-rw-r--r--   0        0        0      329 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/__init__.py
+-rw-r--r--   0        0        0     1490 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/_data_factory_element.py
+-rw-r--r--   0        0        0      126 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/_data_factory_object_type.py
+-rw-r--r--   0        0        0     3687 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/_pipeline.py
+-rw-r--r--   0        0        0      895 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/__init__.py
+-rw-r--r--   0        0        0     4084 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_activity.py
+-rw-r--r--   0        0        0      650 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_activity_dependency.py
+-rw-r--r--   0        0        0     1272 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_append_variable_activity.py
+-rw-r--r--   0        0        0      784 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_control_activity.py
+-rw-r--r--   0        0        0     2626 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_execute_pipeline_activity.py
+-rw-r--r--   0        0        0      789 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_fail_activity.py
+-rw-r--r--   0        0        0     1263 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_filter_activity.py
+-rw-r--r--   0        0        0     1670 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_for_each_activity.py
+-rw-r--r--   0        0        0     1980 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_if_condition_activity.py
+-rw-r--r--   0        0        0     1707 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_set_variable_activity.py
+-rw-r--r--   0        0        0     2395 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_switch_activity.py
+-rw-r--r--   0        0        0     1917 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_until_activity.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/py.typed
+-rw-r--r--   0        0        0      505 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_activity_result.py
+-rw-r--r--   0        0        0      279 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_dependency_condition.py
+-rw-r--r--   0        0        0     8339 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_pipeline_run_state.py
+-rw-r--r--   0        0        0      544 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_pipeline_run_variable.py
+-rw-r--r--   0        0        0      656 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_run_parameter.py
+-rw-r--r--   0        0        0      647 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_run_parameter_type.py
+-rw-r--r--   0        0        0      534 2024-05-22 10:00:21.790464 data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_run_state.py
+-rw-r--r--   0        0        0     6577 1970-01-01 00:00:00.000000 data_factory_testing_framework-0.2.9/PKG-INFO
```

### Comparing `data_factory_testing_framework-0.2.8/LICENSE` & `data_factory_testing_framework-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/README.md` & `data_factory_testing_framework-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/pyproject.toml` & `data_factory_testing_framework-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-factory-testing-framework"
-version = "0.2.8"
+version = "0.2.9"
 description = "A stand-alone test framework that allows to write unit tests for Data Factory pipelines on Microsoft Fabric and Azure Data Factory."
 authors = ["Arjen Kroezen <arjenkroezen@microsoft.com>", "Yennifer Santos <ysantos@microsoft.com>", "Jaya Kumar <kumarjaya@microsoft.com>", "Leonard Herold <lherold@microsoft.com>"]
 readme = "README.md"
 license = "MIT"
 include = [ "README.md", "LICENSE" ]
 keywords = ["fabric", "datafactory", "unit-testing", "functional-testing", "azure"]
```

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/_deserializer_base.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/_deserializer_base.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/_deserializer_fabric.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/_deserializer_fabric.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/shared/_activity_deserializer.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/shared/_activity_deserializer.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_deserializers/shared/_data_factory_element_replacer.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_deserializers/shared/_data_factory_element_replacer.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/exceptions.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/exceptions.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/expression_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/expression_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/expression_rule_transformer.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/expression_rule_transformer.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/expression_terminal_transformer.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/expression_terminal_transformer.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/__init__.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/activity_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/activity_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/branch_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/branch_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/dataset_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/dataset_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/evaluation_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/evaluation_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/expression_parameter_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/expression_parameter_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/function_call_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/function_call_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/item_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/item_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/linked_service_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/linked_service_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/literal_evaluation_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/literal_evaluation_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/literal_interpolation_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/literal_interpolation_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/logical_bool_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/logical_bool_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/pipeline_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/pipeline_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/system_variable_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/system_variable_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/evaluator/rules/variable_reference_expression_rule_evaluator.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/evaluator/rules/variable_reference_expression_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_collection_implementation.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_collection_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_conversion_implementation.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_conversion_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_date_implementation.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_date_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_logical_implementation.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_logical_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_math_implementation.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_math_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_repository.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_repository.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_functions/functions_string_implementation.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_functions/functions_string_implementation.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_pythonnet/csharp_datetime.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_pythonnet/csharp_datetime.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/_factories/base_repository_factory.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/_factories/base_repository_factory.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/_factories/data_factory_repository_factory.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/_factories/data_factory_repository_factory.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/_factories/fabric_repository_factory.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/_factories/fabric_repository_factory.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_repositories/data_factory_repository.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_repositories/data_factory_repository.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/_test_framework.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/_test_framework.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/__init__.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_function_call_invalid_arguments_count_error.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_function_call_invalid_arguments_count_error.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/exceptions/_pipeline_activities_circular_dependency_error.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/exceptions/_pipeline_activities_circular_dependency_error.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/_data_factory_element.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/_data_factory_element.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/_pipeline.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/_pipeline.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/__init__.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/__init__.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_activity_dependency.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_activity_dependency.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_append_variable_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_append_variable_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_control_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_control_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_execute_pipeline_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_execute_pipeline_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_fail_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_fail_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_filter_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_filter_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_for_each_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_for_each_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_if_condition_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_if_condition_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_set_variable_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_set_variable_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_switch_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_switch_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/models/activities/_until_activity.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/models/activities/_until_activity.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_activity_result.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_activity_result.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_pipeline_run_state.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_pipeline_run_state.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_pipeline_run_variable.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_pipeline_run_variable.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_run_parameter.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_run_parameter.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_run_parameter_type.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_run_parameter_type.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/src/data_factory_testing_framework/state/_run_state.py` & `data_factory_testing_framework-0.2.9/src/data_factory_testing_framework/state/_run_state.py`

 * *Files identical despite different names*

### Comparing `data_factory_testing_framework-0.2.8/PKG-INFO` & `data_factory_testing_framework-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-factory-testing-framework
-Version: 0.2.8
+Version: 0.2.9
 Summary: A stand-alone test framework that allows to write unit tests for Data Factory pipelines on Microsoft Fabric and Azure Data Factory.
 License: MIT
 Keywords: fabric,datafactory,unit-testing,functional-testing,azure
 Author: Arjen Kroezen
 Author-email: arjenkroezen@microsoft.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

