# Comparing `tmp/superlinked-4.0.1.tar.gz` & `tmp/superlinked-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superlinked-4.0.1.tar", max compression
+gzip compressed data, was "superlinked-4.1.0.tar", max compression
```

## Comparing `superlinked-4.0.1.tar` & `superlinked-4.1.0.tar`

### file list

```diff
@@ -1,228 +1,228 @@
--rw-r--r--   0        0        0    11354 2024-05-20 11:16:57.453673 superlinked-4.0.1/LICENSE
--rw-r--r--   0        0        0    28655 2024-05-20 11:16:57.453673 superlinked-4.0.1/NOTICE
--rw-r--r--   0        0        0     6840 2024-05-20 11:16:57.453673 superlinked-4.0.1/PYPI_README.md
--rw-r--r--   0        0        0     3698 2024-05-20 11:20:02.165106 superlinked-4.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/evaluation/charts/__init__.py
--rw-r--r--   0        0        0     5601 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/evaluation/charts/recency_plotter.py
--rw-r--r--   0        0        0     8077 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/evaluation/vector_sampler.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/calculation/__init__.py
--rw-r--r--   0        0        0      742 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/calculation/distance_metric.py
--rw-r--r--   0        0        0     1621 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/calculation/vector_similarity.py
--rw-r--r--   0        0        0      805 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/const.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/__init__.py
--rw-r--r--   0        0        0     3624 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/aggregation_node.py
--rw-r--r--   0        0        0     2280 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/categorical_similarity_node.py
--rw-r--r--   0        0        0     1515 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/chunking_node.py
--rw-r--r--   0        0        0     2089 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/comparison_filter_node.py
--rw-r--r--   0        0        0     2586 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/concatenation_node.py
--rw-r--r--   0        0        0     1093 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/constant_node.py
--rw-r--r--   0        0        0     4985 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/context.py
--rw-r--r--   0        0        0     1846 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/custom_node.py
--rw-r--r--   0        0        0     5923 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/dag.py
--rw-r--r--   0        0        0     1338 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/dag_effect.py
--rw-r--r--   0        0        0     3664 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/event_aggregation_node.py
--rw-r--r--   0        0        0     1004 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/exception.py
--rw-r--r--   0        0        0     2023 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/index_node.py
--rw-r--r--   0        0        0     1415 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/named_function_node.py
--rw-r--r--   0        0        0     4465 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/node.py
--rw-r--r--   0        0        0     2414 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/number_embedding_node.py
--rw-r--r--   0        0        0     2368 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/number_similarity_node.py
--rw-r--r--   0        0        0     1620 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/period_time.py
--rw-r--r--   0        0        0      897 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/persistence_params.py
--rw-r--r--   0        0        0     2449 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/recency_node.py
--rw-r--r--   0        0        0     1128 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/resolved_schema_reference.py
--rw-r--r--   0        0        0     2019 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/schema_dag.py
--rw-r--r--   0        0        0     1384 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/schema_field_node.py
--rw-r--r--   0        0        0     1378 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/schema_object_reference.py
--rw-r--r--   0        0        0     2062 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/text_embedding_node.py
--rw-r--r--   0        0        0     8036 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/data_types.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/__init__.py
--rw-r--r--   0        0        0     5281 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py
--rw-r--r--   0        0        0     5890 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/chunking_util.py
--rw-r--r--   0        0        0     1576 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/custom_embedding.py
--rw-r--r--   0        0        0     1280 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/embedding.py
--rw-r--r--   0        0        0     3138 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/number_embedding.py
--rw-r--r--   0        0        0     2383 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/number_similarity_embedding.py
--rw-r--r--   0        0        0     7995 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/recency_embedding.py
--rw-r--r--   0        0        0     2134 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py
--rw-r--r--   0        0        0     1250 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/exception.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/__init__.py
--rw-r--r--   0        0        0     5851 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/comparison_operand.py
--rw-r--r--   0        0        0      841 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/comparison_operation_type.py
--rw-r--r--   0        0        0      808 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/has_aggregation.py
--rw-r--r--   0        0        0      718 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/has_length.py
--rw-r--r--   0        0        0      836 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/has_multiplier.py
--rw-r--r--   0        0        0      940 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/weighted.py
--rw-r--r--   0        0        0     1322 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/observable.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/__init__.py
--rw-r--r--   0        0        0     5879 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/data_parser.py
--rw-r--r--   0        0        0     4806 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/dataframe_parser.py
--rw-r--r--   0        0        0      814 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/exception.py
--rw-r--r--   0        0        0     4379 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/json_parser.py
--rw-r--r--   0        0        0     1354 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/parsed_schema.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/__init__.py
--rw-r--r--   0        0        0     1072 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/event_schema.py
--rw-r--r--   0        0        0     1964 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/event_schema_object.py
--rw-r--r--   0        0        0     1014 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/exception.py
--rw-r--r--   0        0        0      627 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/general_type.py
--rw-r--r--   0        0        0     1392 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/id_schema_object.py
--rw-r--r--   0        0        0     1178 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema.py
--rw-r--r--   0        0        0     3189 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_decorator.py
--rw-r--r--   0        0        0     3209 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_factory.py
--rw-r--r--   0        0        0     5687 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_object.py
--rw-r--r--   0        0        0     3170 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_reference.py
--rw-r--r--   0        0        0      686 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_type.py
--rw-r--r--   0        0        0     3201 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_validator.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/source/__init__.py
--rw-r--r--   0        0        0      857 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/source/source.py
--rw-r--r--   0        0        0      647 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/source/types.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/space/__init__.py
--rw-r--r--   0        0        0     4398 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/space/aggregation.py
--rw-r--r--   0        0        0     2121 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/space/normalization.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/__init__.py
--rw-r--r--   0        0        0      857 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/entity.py
--rw-r--r--   0        0        0      878 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/entity_data.py
--rw-r--r--   0        0        0      696 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/entity_id.py
--rw-r--r--   0        0        0      627 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/exception.py
--rw-r--r--   0        0        0     1516 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/field.py
--rw-r--r--   0        0        0     2535 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/field_data.py
--rw-r--r--   0        0        0      733 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/field_data_type.py
--rw-r--r--   0        0        0     3213 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/field_encoder.py
--rw-r--r--   0        0        0      746 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/persistence_type.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/__init__.py
--rw-r--r--   0        0        0     1216 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
--rw-r--r--   0        0        0      671 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
--rw-r--r--   0        0        0      692 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
--rw-r--r--   0        0        0     2306 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/vdb_connector.py
--rw-r--r--   0        0        0     1075 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/vdb_knn_search_params.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/__init__.py
--rw-r--r--   0        0        0     6065 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/entity_builder.py
--rw-r--r--   0        0        0     2143 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/field_type_converter.py
--rw-r--r--   0        0        0     1059 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/knn_search_params.py
--rw-r--r--   0        0        0      769 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/node_result_params.py
--rw-r--r--   0        0        0    13379 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/storage_manager.py
--rw-r--r--   0        0        0     1462 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/storage_naming.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/__init__.py
--rw-r--r--   0        0        0      787 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/collection_util.py
--rw-r--r--   0        0        0     2074 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/dot_separated_path_util.py
--rw-r--r--   0        0        0      707 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/immutable_model.py
--rw-r--r--   0        0        0     1058 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/named_function_evaluator.py
--rw-r--r--   0        0        0      886 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/schema_util.py
--rw-r--r--   0        0        0     1642 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/string_util.py
--rw-r--r--   0        0        0      907 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/time_util.py
--rw-r--r--   0        0        0     1189 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/type_util.py
--rw-r--r--   0        0        0     4383 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/type_validator.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/compiler/__init__.py
--rw-r--r--   0        0        0     2556 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/compiler/online_schema_dag_compiler.py
--rw-r--r--   0        0        0      108 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/data_loader/__init__.py
--rw-r--r--   0        0        0      726 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/data_loader/data_loader.py
--rw-r--r--   0        0        0      221 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/__init__.py
--rw-r--r--   0        0        0      719 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/exception.py
--rw-r--r--   0        0        0     4281 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/executor.py
--rw-r--r--   0        0        0      124 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/in_memory/__init__.py
--rw-r--r--   0        0        0     7300 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
--rw-r--r--   0        0        0      119 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/query/__init__.py
--rw-r--r--   0        0        0     6478 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/query/query_executor.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/__init__.py
--rw-r--r--   0        0        0     1540 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_configuration.py
--rw-r--r--   0        0        0      818 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py
--rw-r--r--   0        0        0     4395 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_executor.py
--rw-r--r--   0        0        0     3236 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_handler.py
--rw-r--r--   0        0        0      176 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/__init__.py
--rw-r--r--   0        0        0     1904 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/effect.py
--rw-r--r--   0        0        0    10985 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/index.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/__init__.py
--rw-r--r--   0        0        0     1516 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py
--rw-r--r--   0        0        0     2448 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/aggregation_node_util.py
--rw-r--r--   0        0        0     6203 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
--rw-r--r--   0        0        0     2557 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
--rw-r--r--   0        0        0     3673 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
--rw-r--r--   0        0        0      192 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/__init__.py
--rw-r--r--   0        0        0     1183 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/param.py
--rw-r--r--   0        0        0     3798 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/param_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/__init__.py
--rw-r--r--   0        0        0      756 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/binary_op.py
--rw-r--r--   0        0        0     1521 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/binary_predicate.py
--rw-r--r--   0        0        0      924 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
--rw-r--r--   0        0        0     1128 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/query_predicate.py
--rw-r--r--   0        0        0    13173 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/query.py
--rw-r--r--   0        0        0     6223 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/query_filters.py
--rw-r--r--   0        0        0     6990 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/query_vector_factory.py
--rw-r--r--   0        0        0     3329 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/query_weighting.py
--rw-r--r--   0        0        0     2457 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/query/result.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/registry/__init__.py
--rw-r--r--   0        0        0      636 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/registry/exception.py
--rw-r--r--   0        0        0     1984 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/registry/superlinked_registry.py
--rw-r--r--   0        0        0      214 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/source/__init__.py
--rw-r--r--   0        0        0     2773 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/source/in_memory_source.py
--rw-r--r--   0        0        0     1987 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/source/rest_source.py
--rw-r--r--   0        0        0     1144 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/source/source.py
--rw-r--r--   0        0        0      183 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/__init__.py
--rw-r--r--   0        0        0     7539 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/categorical_similarity_space.py
--rw-r--r--   0        0        0     5569 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/custom_space.py
--rw-r--r--   0        0        0      856 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/exception.py
--rw-r--r--   0        0        0     8215 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/number_space.py
--rw-r--r--   0        0        0     8516 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/recency_space.py
--rw-r--r--   0        0        0     2732 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/space.py
--rw-r--r--   0        0        0     1275 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/space_field_set.py
--rw-r--r--   0        0        0     4804 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/text_similarity_space.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/evaluator/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/evaluator/dag_evaluator.py
--rw-r--r--   0        0        0     5222 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/evaluator/online_dag_evaluator.py
--rw-r--r--   0        0        0     2237 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/evaluator/query_dag_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/__init__.py
--rw-r--r--   0        0        0      787 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/exception.py
--rw-r--r--   0        0        0     6127 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/in_memory_knn_search.py
--rw-r--r--   0        0        0     6408 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/in_memory_vdb.py
--rw-r--r--   0        0        0      921 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/index_config.py
--rw-r--r--   0        0        0     1305 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/json_codec.py
--rw-r--r--   0        0        0     1562 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/object_serializer.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/__init__.py
--rw-r--r--   0        0        0      801 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/batched_chunk_input_item.py
--rw-r--r--   0        0        0     7597 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/default_online_node.py
--rw-r--r--   0        0        0     1129 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/evaluation_result.py
--rw-r--r--   0        0        0      768 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/exception.py
--rw-r--r--   0        0        0     6395 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_aggregation_node.py
--rw-r--r--   0        0        0     3288 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_categorical_similarity_node.py
--rw-r--r--   0        0        0     3540 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_chunking_node.py
--rw-r--r--   0        0        0     2330 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_comparison_filter_node.py
--rw-r--r--   0        0        0     5148 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_concatenation_node.py
--rw-r--r--   0        0        0     2115 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_constant_node.py
--rw-r--r--   0        0        0     3435 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_custom_node.py
--rw-r--r--   0        0        0     8157 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_event_aggregation_node.py
--rw-r--r--   0        0        0     4135 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_index_node.py
--rw-r--r--   0        0        0     2434 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_named_function_node.py
--rw-r--r--   0        0        0     4996 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_node.py
--rw-r--r--   0        0        0     5773 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_node_registry.py
--rw-r--r--   0        0        0     3162 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_number_embedding_node.py
--rw-r--r--   0        0        0     3272 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_number_similarity_node.py
--rw-r--r--   0        0        0     2796 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_recency_node.py
--rw-r--r--   0        0        0     3732 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_schema_dag.py
--rw-r--r--   0        0        0     3509 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_schema_field_node.py
--rw-r--r--   0        0        0     3338 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_text_embedding_node.py
--rw-r--r--   0        0        0      794 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/parent_results.py
--rw-r--r--   0        0        0     1322 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/parent_validator.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/source/__init__.py
--rw-r--r--   0        0        0     3486 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/source/in_memory_data_processor.py
--rw-r--r--   0        0        0     1539 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/source/in_memory_object_writer.py
--rw-r--r--   0        0        0     1752 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/source/in_memory_source.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/store_manager/__init__.py
--rw-r--r--   0        0        0     5707 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/store_manager/evaluation_result_store_manager.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/__init__.py
--rw-r--r--   0        0        0     2587 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/entity.py
--rw-r--r--   0        0        0     1936 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/entity_store.py
--rw-r--r--   0        0        0     4966 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/entity_store_manager.py
--rw-r--r--   0        0        0     1304 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/field.py
--rw-r--r--   0        0        0     8076 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/in_memory_entity_store.py
--rw-r--r--   0        0        0     1209 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/in_memory_object_store.py
--rw-r--r--   0        0        0     1125 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/object_store.py
--rw-r--r--   0        0        0     1570 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/object_store_manager.py
--rw-r--r--   0        0        0     3317 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/persistable_dict.py
--rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/py.typed
--rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-22 14:45:11.466898 superlinked-4.1.0/LICENSE
+-rw-r--r--   0        0        0    28655 2024-05-22 14:45:11.466898 superlinked-4.1.0/NOTICE
+-rw-r--r--   0        0        0     6840 2024-05-22 14:45:11.466898 superlinked-4.1.0/PYPI_README.md
+-rw-r--r--   0        0        0     3698 2024-05-22 14:48:01.196184 superlinked-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/evaluation/charts/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/evaluation/charts/recency_plotter.py
+-rw-r--r--   0        0        0     8077 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/evaluation/vector_sampler.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/framework/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/calculation/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/calculation/distance_metric.py
+-rw-r--r--   0        0        0     1621 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/calculation/vector_similarity.py
+-rw-r--r--   0        0        0      805 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/const.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/__init__.py
+-rw-r--r--   0        0        0     3624 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/aggregation_node.py
+-rw-r--r--   0        0        0     2280 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/categorical_similarity_node.py
+-rw-r--r--   0        0        0     1515 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/chunking_node.py
+-rw-r--r--   0        0        0     2089 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/comparison_filter_node.py
+-rw-r--r--   0        0        0     2586 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/concatenation_node.py
+-rw-r--r--   0        0        0     1093 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/constant_node.py
+-rw-r--r--   0        0        0     4985 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/context.py
+-rw-r--r--   0        0        0     1846 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/custom_node.py
+-rw-r--r--   0        0        0     5923 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/dag.py
+-rw-r--r--   0        0        0     1338 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/dag_effect.py
+-rw-r--r--   0        0        0     3664 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/event_aggregation_node.py
+-rw-r--r--   0        0        0     1004 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/exception.py
+-rw-r--r--   0        0        0     2023 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/index_node.py
+-rw-r--r--   0        0        0     1415 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/named_function_node.py
+-rw-r--r--   0        0        0     4465 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/node.py
+-rw-r--r--   0        0        0     2414 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/number_embedding_node.py
+-rw-r--r--   0        0        0     2368 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/number_similarity_node.py
+-rw-r--r--   0        0        0     1620 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/period_time.py
+-rw-r--r--   0        0        0      897 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/persistence_params.py
+-rw-r--r--   0        0        0     2449 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/recency_node.py
+-rw-r--r--   0        0        0     1128 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/resolved_schema_reference.py
+-rw-r--r--   0        0        0     2019 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/schema_dag.py
+-rw-r--r--   0        0        0     1384 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/schema_field_node.py
+-rw-r--r--   0        0        0     1378 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/schema_object_reference.py
+-rw-r--r--   0        0        0     2062 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/text_embedding_node.py
+-rw-r--r--   0        0        0     8081 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/data_types.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/__init__.py
+-rw-r--r--   0        0        0     5281 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py
+-rw-r--r--   0        0        0     5890 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/chunking_util.py
+-rw-r--r--   0        0        0     1576 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/custom_embedding.py
+-rw-r--r--   0        0        0     1280 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/embedding.py
+-rw-r--r--   0        0        0     3138 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/number_embedding.py
+-rw-r--r--   0        0        0     2424 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/number_similarity_embedding.py
+-rw-r--r--   0        0        0     8046 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/recency_embedding.py
+-rw-r--r--   0        0        0     2134 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py
+-rw-r--r--   0        0        0     1250 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/exception.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/__init__.py
+-rw-r--r--   0        0        0     5851 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/comparison_operand.py
+-rw-r--r--   0        0        0      841 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/comparison_operation_type.py
+-rw-r--r--   0        0        0      808 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/has_aggregation.py
+-rw-r--r--   0        0        0      718 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/has_length.py
+-rw-r--r--   0        0        0      836 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/has_multiplier.py
+-rw-r--r--   0        0        0      940 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/weighted.py
+-rw-r--r--   0        0        0     1322 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/observable.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/__init__.py
+-rw-r--r--   0        0        0     5879 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/data_parser.py
+-rw-r--r--   0        0        0     4806 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/dataframe_parser.py
+-rw-r--r--   0        0        0      814 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/exception.py
+-rw-r--r--   0        0        0     4379 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/json_parser.py
+-rw-r--r--   0        0        0     1354 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/parsed_schema.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/event_schema.py
+-rw-r--r--   0        0        0     1964 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/event_schema_object.py
+-rw-r--r--   0        0        0     1014 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/exception.py
+-rw-r--r--   0        0        0      627 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/general_type.py
+-rw-r--r--   0        0        0     1392 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/id_schema_object.py
+-rw-r--r--   0        0        0     1178 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema.py
+-rw-r--r--   0        0        0     3189 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_decorator.py
+-rw-r--r--   0        0        0     3209 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_factory.py
+-rw-r--r--   0        0        0     5687 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_object.py
+-rw-r--r--   0        0        0     3170 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_reference.py
+-rw-r--r--   0        0        0      686 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_type.py
+-rw-r--r--   0        0        0     3201 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_validator.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/source/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/source/source.py
+-rw-r--r--   0        0        0      647 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/source/types.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/space/__init__.py
+-rw-r--r--   0        0        0     4398 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/space/aggregation.py
+-rw-r--r--   0        0        0     2121 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/space/normalization.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/entity.py
+-rw-r--r--   0        0        0      878 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/entity_data.py
+-rw-r--r--   0        0        0      696 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/entity_id.py
+-rw-r--r--   0        0        0      627 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/exception.py
+-rw-r--r--   0        0        0     1516 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/field.py
+-rw-r--r--   0        0        0     2535 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/field_data.py
+-rw-r--r--   0        0        0      733 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/field_data_type.py
+-rw-r--r--   0        0        0     3213 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/field_encoder.py
+-rw-r--r--   0        0        0      746 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/persistence_type.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/__init__.py
+-rw-r--r--   0        0        0     1216 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
+-rw-r--r--   0        0        0      671 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
+-rw-r--r--   0        0        0      692 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
+-rw-r--r--   0        0        0     2306 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/vdb_connector.py
+-rw-r--r--   0        0        0     1075 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/vdb_knn_search_params.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/__init__.py
+-rw-r--r--   0        0        0     6065 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/entity_builder.py
+-rw-r--r--   0        0        0     2143 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/field_type_converter.py
+-rw-r--r--   0        0        0     1059 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/knn_search_params.py
+-rw-r--r--   0        0        0      769 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/node_result_params.py
+-rw-r--r--   0        0        0    13379 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/storage_manager.py
+-rw-r--r--   0        0        0     1462 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/storage_naming.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/collection_util.py
+-rw-r--r--   0        0        0     2074 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/dot_separated_path_util.py
+-rw-r--r--   0        0        0      707 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/immutable_model.py
+-rw-r--r--   0        0        0     1058 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/named_function_evaluator.py
+-rw-r--r--   0        0        0      886 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/schema_util.py
+-rw-r--r--   0        0        0     1642 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/string_util.py
+-rw-r--r--   0        0        0      907 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/time_util.py
+-rw-r--r--   0        0        0     1189 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/type_util.py
+-rw-r--r--   0        0        0     4383 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/type_validator.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/compiler/__init__.py
+-rw-r--r--   0        0        0     2556 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/compiler/online_schema_dag_compiler.py
+-rw-r--r--   0        0        0      108 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/data_loader/__init__.py
+-rw-r--r--   0        0        0      726 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/data_loader/data_loader.py
+-rw-r--r--   0        0        0      221 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/exception.py
+-rw-r--r--   0        0        0     4467 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/executor.py
+-rw-r--r--   0        0        0      124 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/in_memory/__init__.py
+-rw-r--r--   0        0        0     7228 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
+-rw-r--r--   0        0        0      119 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/query/__init__.py
+-rw-r--r--   0        0        0     6478 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/query/query_executor.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/__init__.py
+-rw-r--r--   0        0        0     1540 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_configuration.py
+-rw-r--r--   0        0        0      818 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py
+-rw-r--r--   0        0        0     4395 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_executor.py
+-rw-r--r--   0        0        0     3236 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_handler.py
+-rw-r--r--   0        0        0      176 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/effect.py
+-rw-r--r--   0        0        0    10985 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/index.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py
+-rw-r--r--   0        0        0     2448 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/aggregation_node_util.py
+-rw-r--r--   0        0        0     6203 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
+-rw-r--r--   0        0        0     2557 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
+-rw-r--r--   0        0        0     3673 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
+-rw-r--r--   0        0        0      192 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/__init__.py
+-rw-r--r--   0        0        0     1183 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/param.py
+-rw-r--r--   0        0        0     3798 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/param_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/binary_op.py
+-rw-r--r--   0        0        0     1521 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/binary_predicate.py
+-rw-r--r--   0        0        0      924 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
+-rw-r--r--   0        0        0     1128 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/query_predicate.py
+-rw-r--r--   0        0        0    13173 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/query.py
+-rw-r--r--   0        0        0     6223 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/query_filters.py
+-rw-r--r--   0        0        0     6990 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/query_vector_factory.py
+-rw-r--r--   0        0        0     3329 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/query_weighting.py
+-rw-r--r--   0        0        0     2457 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/result.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/registry/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/registry/exception.py
+-rw-r--r--   0        0        0     1984 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/registry/superlinked_registry.py
+-rw-r--r--   0        0        0      214 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/source/__init__.py
+-rw-r--r--   0        0        0     2773 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/source/in_memory_source.py
+-rw-r--r--   0        0        0     1987 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/source/rest_source.py
+-rw-r--r--   0        0        0     1144 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/source/source.py
+-rw-r--r--   0        0        0      183 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/__init__.py
+-rw-r--r--   0        0        0     7479 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/categorical_similarity_space.py
+-rw-r--r--   0        0        0     5509 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/custom_space.py
+-rw-r--r--   0        0        0      856 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/exception.py
+-rw-r--r--   0        0        0     8215 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/number_space.py
+-rw-r--r--   0        0        0     8456 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/dsl/space/recency_space.py
+-rw-r--r--   0        0        0     2743 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/dsl/space/space.py
+-rw-r--r--   0        0        0     1295 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/dsl/space/space_field_set.py
+-rw-r--r--   0        0        0     4804 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/dsl/space/text_similarity_space.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/evaluator/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/evaluator/dag_evaluator.py
+-rw-r--r--   0        0        0     5222 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/evaluator/online_dag_evaluator.py
+-rw-r--r--   0        0        0     2237 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/evaluator/query_dag_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/exception.py
+-rw-r--r--   0        0        0     6127 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/in_memory_knn_search.py
+-rw-r--r--   0        0        0     6408 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/in_memory_vdb.py
+-rw-r--r--   0        0        0      921 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/index_config.py
+-rw-r--r--   0        0        0     1305 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/json_codec.py
+-rw-r--r--   0        0        0     1562 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/object_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/batched_chunk_input_item.py
+-rw-r--r--   0        0        0     7597 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/default_online_node.py
+-rw-r--r--   0        0        0     1129 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/evaluation_result.py
+-rw-r--r--   0        0        0      768 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/exception.py
+-rw-r--r--   0        0        0     6395 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_aggregation_node.py
+-rw-r--r--   0        0        0     3288 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_categorical_similarity_node.py
+-rw-r--r--   0        0        0     3540 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_chunking_node.py
+-rw-r--r--   0        0        0     2330 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_comparison_filter_node.py
+-rw-r--r--   0        0        0     5221 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_concatenation_node.py
+-rw-r--r--   0        0        0     2115 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_constant_node.py
+-rw-r--r--   0        0        0     3435 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_custom_node.py
+-rw-r--r--   0        0        0     8157 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_event_aggregation_node.py
+-rw-r--r--   0        0        0     4135 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_index_node.py
+-rw-r--r--   0        0        0     2434 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_named_function_node.py
+-rw-r--r--   0        0        0     4996 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_node.py
+-rw-r--r--   0        0        0     5773 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_node_registry.py
+-rw-r--r--   0        0        0     3162 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_number_embedding_node.py
+-rw-r--r--   0        0        0     3272 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_number_similarity_node.py
+-rw-r--r--   0        0        0     2796 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_recency_node.py
+-rw-r--r--   0        0        0     3732 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_schema_dag.py
+-rw-r--r--   0        0        0     3509 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_schema_field_node.py
+-rw-r--r--   0        0        0     3338 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_text_embedding_node.py
+-rw-r--r--   0        0        0      794 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/parent_results.py
+-rw-r--r--   0        0        0     1322 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/parent_validator.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/source/__init__.py
+-rw-r--r--   0        0        0     3486 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/source/in_memory_data_processor.py
+-rw-r--r--   0        0        0     1539 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/source/in_memory_object_writer.py
+-rw-r--r--   0        0        0     1752 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/source/in_memory_source.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/store_manager/__init__.py
+-rw-r--r--   0        0        0     5707 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/store_manager/evaluation_result_store_manager.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/__init__.py
+-rw-r--r--   0        0        0     2587 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/entity.py
+-rw-r--r--   0        0        0     1936 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/entity_store.py
+-rw-r--r--   0        0        0     4966 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/entity_store_manager.py
+-rw-r--r--   0        0        0     1304 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/field.py
+-rw-r--r--   0        0        0     8076 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/in_memory_entity_store.py
+-rw-r--r--   0        0        0     1209 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/in_memory_object_store.py
+-rw-r--r--   0        0        0     1125 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/object_store.py
+-rw-r--r--   0        0        0     1570 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/object_store_manager.py
+-rw-r--r--   0        0        0     3317 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/persistable_dict.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/py.typed
+-rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-4.1.0/PKG-INFO
```

### Comparing `superlinked-4.0.1/LICENSE` & `superlinked-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/NOTICE` & `superlinked-4.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/PYPI_README.md` & `superlinked-4.1.0/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/pyproject.toml` & `superlinked-4.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superlinked"
-version = "4.0.1"  # The version will be dynamically updated
+version = "4.1.0"  # The version will be dynamically updated
 description = "The Superlinked vector computing library"
 authors = ["Superlinked Release <release@superlinked.com>"]
 readme = "PYPI_README.md"
 license = "Apache-2.0"
 include = ["NOTICE"]
 
 [tool.poetry.dependencies]
```

### Comparing `superlinked-4.0.1/superlinked/evaluation/charts/recency_plotter.py` & `superlinked-4.1.0/superlinked/evaluation/charts/recency_plotter.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/evaluation/vector_sampler.py` & `superlinked-4.1.0/superlinked/evaluation/vector_sampler.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/calculation/distance_metric.py` & `superlinked-4.1.0/superlinked/framework/common/calculation/distance_metric.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/calculation/vector_similarity.py` & `superlinked-4.1.0/superlinked/framework/common/calculation/vector_similarity.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/const.py` & `superlinked-4.1.0/superlinked/framework/common/const.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/aggregation_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/categorical_similarity_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/categorical_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/chunking_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/comparison_filter_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/concatenation_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/constant_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/context.py` & `superlinked-4.1.0/superlinked/framework/common/dag/context.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/custom_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/dag.py` & `superlinked-4.1.0/superlinked/framework/common/dag/dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/dag_effect.py` & `superlinked-4.1.0/superlinked/framework/common/dag/dag_effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/event_aggregation_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/exception.py` & `superlinked-4.1.0/superlinked/framework/common/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/index_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/named_function_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/number_embedding_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/number_similarity_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/number_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/period_time.py` & `superlinked-4.1.0/superlinked/framework/common/dag/period_time.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/persistence_params.py` & `superlinked-4.1.0/superlinked/framework/common/dag/persistence_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/recency_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/resolved_schema_reference.py` & `superlinked-4.1.0/superlinked/framework/common/dag/resolved_schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/schema_dag.py` & `superlinked-4.1.0/superlinked/framework/common/dag/schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/schema_field_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/schema_object_reference.py` & `superlinked-4.1.0/superlinked/framework/common/dag/schema_object_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/dag/text_embedding_node.py` & `superlinked-4.1.0/superlinked/framework/common/dag/text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/data_types.py` & `superlinked-4.1.0/superlinked/framework/common/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,26 +133,28 @@
                     if i not in other.negative_filter_indices
                     else value
                 )
                 for i, value in enumerate(other.value)
             ]
         return self.copy_with_new(values, other.negative_filter_indices)
 
-    def __add__(self, other: Any) -> Vector:
+    def concatenate(self, other: Any) -> Vector:
         if not isinstance(other, Vector):
             return NotImplemented
         if self.is_empty:
             return other.__copy()
         if other.is_empty:
             return self.__copy()
         negative_filter_indices = self.negative_filter_indices.union(
             {i + self.dimension for i in other.negative_filter_indices}
         )
         vector_before_normalization = (
-            self.vector_before_normalization + other.vector_before_normalization
+            self.vector_before_normalization.concatenate(
+                other.vector_before_normalization
+            )
             if self.vector_before_normalization and other.vector_before_normalization
             else None
         )
         return self.copy_with_new(
             np.concatenate((self.value, np.array(other.value, dtype=float))),
             negative_filter_indices,
             vector_before_normalization,
```

### Comparing `superlinked-4.0.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py` & `superlinked-4.1.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/embedding/chunking_util.py` & `superlinked-4.1.0/superlinked/framework/common/embedding/chunking_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/embedding/custom_embedding.py` & `superlinked-4.1.0/superlinked/framework/common/embedding/custom_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/embedding/embedding.py` & `superlinked-4.1.0/superlinked/framework/common/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/embedding/number_embedding.py` & `superlinked-4.1.0/superlinked/framework/common/embedding/number_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/embedding/number_similarity_embedding.py` & `superlinked-4.1.0/superlinked/framework/common/embedding/number_similarity_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,13 +52,15 @@
         vector_input = np.array(
             [
                 math.sin(angle_in_radians),
                 math.cos(angle_in_radians),
             ]
         )
         vector = Vector(vector_input).normalize(self._normalization.norm(vector_input))
-        vector += Vector([1.0 if context.is_query_context() else 0.0])
+        vector = vector.concatenate(
+            Vector([1.0 if context.is_query_context() else 0.0])
+        )
         return vector
 
     @property
     def length(self) -> int:
         return self.__length
```

### Comparing `superlinked-4.0.1/superlinked/framework/common/embedding/recency_embedding.py` & `superlinked-4.1.0/superlinked/framework/common/embedding/recency_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 from datetime import datetime, timedelta
+from functools import reduce
 
 import numpy as np
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.period_time import PeriodTime
 from superlinked.framework.common.data_types import Vector
@@ -120,24 +121,24 @@
             y_value / self.max_period_time.weight, x_value / self.max_period_time.weight
         ) / (2 * math.pi)
         time_elapsed = abs(time_modulo) * full_circle_period_time
         created_at = time_period_start + period_time_in_secs - time_elapsed
         return int(created_at)
 
     def calc_recency_vector(self, created_at: int, context: ExecutionContext) -> Vector:
-        return sum(
+        return reduce(
+            lambda a, b: a.concatenate(b),
             (
                 self.calc_recency_vector_for_period_time(
                     created_at,
                     period_time_param,
                     context,
                 )
                 for period_time_param in self.__period_time_list
             ),
-            Vector([]),
         )
 
     def calc_recency_vector_for_period_time(
         self,
         created_at: int,
         period_time: PeriodTime,
         context: ExecutionContext,
```

### Comparing `superlinked-4.0.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py` & `superlinked-4.1.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/exception.py` & `superlinked-4.1.0/superlinked/framework/common/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/interface/comparison_operand.py` & `superlinked-4.1.0/superlinked/framework/common/interface/comparison_operand.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/interface/comparison_operation_type.py` & `superlinked-4.1.0/superlinked/framework/common/interface/comparison_operation_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/interface/has_aggregation.py` & `superlinked-4.1.0/superlinked/framework/common/interface/has_aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/interface/has_length.py` & `superlinked-4.1.0/superlinked/framework/common/interface/has_length.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/interface/has_multiplier.py` & `superlinked-4.1.0/superlinked/framework/common/interface/has_multiplier.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/interface/weighted.py` & `superlinked-4.1.0/superlinked/framework/common/interface/weighted.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/observable.py` & `superlinked-4.1.0/superlinked/framework/common/observable.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/parser/data_parser.py` & `superlinked-4.1.0/superlinked/framework/common/parser/data_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/parser/dataframe_parser.py` & `superlinked-4.1.0/superlinked/framework/common/parser/dataframe_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/parser/exception.py` & `superlinked-4.1.0/superlinked/framework/common/parser/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/parser/json_parser.py` & `superlinked-4.1.0/superlinked/framework/common/parser/json_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/parser/parsed_schema.py` & `superlinked-4.1.0/superlinked/framework/common/parser/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/event_schema.py` & `superlinked-4.1.0/superlinked/framework/common/schema/event_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/event_schema_object.py` & `superlinked-4.1.0/superlinked/framework/common/schema/event_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/exception.py` & `superlinked-4.1.0/superlinked/framework/common/schema/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/general_type.py` & `superlinked-4.1.0/superlinked/framework/common/schema/general_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/id_schema_object.py` & `superlinked-4.1.0/superlinked/framework/common/schema/id_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/schema.py` & `superlinked-4.1.0/superlinked/framework/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/schema_decorator.py` & `superlinked-4.1.0/superlinked/framework/common/schema/schema_decorator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/schema_factory.py` & `superlinked-4.1.0/superlinked/framework/common/schema/schema_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/schema_object.py` & `superlinked-4.1.0/superlinked/framework/common/schema/schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/schema_reference.py` & `superlinked-4.1.0/superlinked/framework/common/schema/schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/schema_type.py` & `superlinked-4.1.0/superlinked/framework/common/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/schema/schema_validator.py` & `superlinked-4.1.0/superlinked/framework/common/schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/source/source.py` & `superlinked-4.1.0/superlinked/framework/common/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/source/types.py` & `superlinked-4.1.0/superlinked/framework/common/source/types.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/space/aggregation.py` & `superlinked-4.1.0/superlinked/framework/common/space/aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/space/normalization.py` & `superlinked-4.1.0/superlinked/framework/common/space/normalization.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/entity.py` & `superlinked-4.1.0/superlinked/framework/common/storage/entity.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/entity_data.py` & `superlinked-4.1.0/superlinked/framework/common/storage/entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/entity_id.py` & `superlinked-4.1.0/superlinked/framework/common/storage/entity_id.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/exception.py` & `superlinked-4.1.0/superlinked/framework/common/storage/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/field.py` & `superlinked-4.1.0/superlinked/framework/common/storage/field.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/field_data.py` & `superlinked-4.1.0/superlinked/framework/common/storage/field_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/field_data_type.py` & `superlinked-4.1.0/superlinked/framework/common/storage/field_data_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/field_encoder.py` & `superlinked-4.1.0/superlinked/framework/common/storage/field_encoder.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/persistence_type.py` & `superlinked-4.1.0/superlinked/framework/common/storage/persistence_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py` & `superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py` & `superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py` & `superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/vdb_connector.py` & `superlinked-4.1.0/superlinked/framework/common/storage/vdb_connector.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage/vdb_knn_search_params.py` & `superlinked-4.1.0/superlinked/framework/common/storage/vdb_knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage_manager/entity_builder.py` & `superlinked-4.1.0/superlinked/framework/common/storage_manager/entity_builder.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage_manager/field_type_converter.py` & `superlinked-4.1.0/superlinked/framework/common/storage_manager/field_type_converter.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage_manager/knn_search_params.py` & `superlinked-4.1.0/superlinked/framework/common/storage_manager/knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage_manager/node_result_params.py` & `superlinked-4.1.0/superlinked/framework/common/storage_manager/node_result_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage_manager/storage_manager.py` & `superlinked-4.1.0/superlinked/framework/common/storage_manager/storage_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/storage_manager/storage_naming.py` & `superlinked-4.1.0/superlinked/framework/common/storage_manager/storage_naming.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/collection_util.py` & `superlinked-4.1.0/superlinked/framework/common/util/collection_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/dot_separated_path_util.py` & `superlinked-4.1.0/superlinked/framework/common/util/dot_separated_path_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/immutable_model.py` & `superlinked-4.1.0/superlinked/framework/common/util/immutable_model.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/named_function_evaluator.py` & `superlinked-4.1.0/superlinked/framework/common/util/named_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/schema_util.py` & `superlinked-4.1.0/superlinked/framework/common/util/schema_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/string_util.py` & `superlinked-4.1.0/superlinked/framework/common/util/string_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/time_util.py` & `superlinked-4.1.0/superlinked/framework/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/type_util.py` & `superlinked-4.1.0/superlinked/framework/common/util/type_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/common/util/type_validator.py` & `superlinked-4.1.0/superlinked/framework/common/util/type_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/compiler/online_schema_dag_compiler.py` & `superlinked-4.1.0/superlinked/framework/compiler/online_schema_dag_compiler.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/data_loader/data_loader.py` & `superlinked-4.1.0/superlinked/framework/dsl/data_loader/data_loader.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/executor/exception.py` & `superlinked-4.1.0/superlinked/framework/dsl/executor/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/executor/executor.py` & `superlinked-4.1.0/superlinked/framework/dsl/executor/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Annotated, Generic, TypeVar
+from typing import Annotated, Any, Generic, TypeVar
 
 from beartype.typing import Sequence
 from typing_extensions import Self
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.util.time_util import now
 from superlinked.framework.common.util.type_util import get_single_generic_type
@@ -28,23 +28,28 @@
 from superlinked.framework.dsl.source.source import SourceT
 from superlinked.framework.storage.entity_store import EntityStore
 from superlinked.framework.storage.entity_store_manager import EntityStoreManager
 from superlinked.framework.storage.object_store import ObjectStore
 from superlinked.framework.storage.object_store_manager import ObjectStoreManager
 
 ExecutorT = TypeVar("ExecutorT", bound="Executor")
+EntityStoreT = TypeVar("EntityStoreT", bound=EntityStore)
+ObjectStoreT = TypeVar("ObjectStoreT", bound=ObjectStore)
 
 
-class App(ABC, Generic[ExecutorT]):
+class App(ABC, Generic[ExecutorT, EntityStoreT, ObjectStoreT]):
     """
     Abstract base class for an App, a running executor that can for example do queries or ingest data.
     """
 
     def __init__(
-        self, executor: ExecutorT, entity_store: EntityStore, object_store: ObjectStore
+        self,
+        executor: ExecutorT,
+        entity_store: EntityStoreT,
+        object_store: ObjectStoreT,
     ) -> None:
         """
         Initialize the App.
 
         Args:
             executor (TExecutor): The executor instance.
             entity_store (EntityStore): The entity store instance.
@@ -122,14 +127,14 @@
 
         Returns:
             Mapping[str, Mapping[str, Any]]: The context mapping.
         """
         return self._context
 
     @abstractmethod
-    def run(self) -> App[Self]:
+    def run(self) -> App[Self, Any, Any]:
         """
         Abstract method to run the executor.
 
         Returns:
             App[Self]: An instance of App.
         """
```

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py` & `superlinked-4.1.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import Any, Mapping, cast
+from typing import Any, Mapping
 
 from beartype.typing import Sequence
 
 from superlinked.framework.common.dag.context import (
     ContextValue,
     ExecutionContext,
     ExecutionEnvironment,
@@ -84,15 +84,15 @@
         Returns:
             InMemoryApp: An instance of InMemoryApp.
         """
         return InMemoryApp(self)
 
 
 @TypeValidator.wrap
-class InMemoryApp(App[InMemoryExecutor]):
+class InMemoryApp(App[InMemoryExecutor, InMemoryEntityStore, InMemoryObjectStore]):
     """
     In-memory implementation of the App class.
 
     Attributes:
         executor (InMemoryExecutor): An instance of InMemoryExecutor.
     """
 
@@ -132,22 +132,22 @@
         ):
             for source in self.__filter_index_sources(index, self._executor._sources):
                 source._source.register(data_processor)
 
     def restore(self, reader: ObjectReader) -> None:
         node_ids = [index._node_id for index in self.executor._indices]
         app_identifier = "_".join(node_ids)
-        cast(InMemoryObjectStore, self._object_store).restore(reader, app_identifier)
-        cast(InMemoryEntityStore, self._entity_store).restore(reader, app_identifier)
+        self._object_store.restore(reader, app_identifier)
+        self._entity_store.restore(reader, app_identifier)
 
     def persist(self, writer: ObjectWriter) -> None:
         node_ids = [index._node_id for index in self.executor._indices]
         app_identifier = "_".join(node_ids)
-        cast(InMemoryObjectStore, self._object_store).persist(writer, app_identifier)
-        cast(InMemoryEntityStore, self._entity_store).persist(writer, app_identifier)
+        self._object_store.persist(writer, app_identifier)
+        self._entity_store.persist(writer, app_identifier)
 
     def query(self, query_obj: QueryObj, **params: Any) -> Result:
         """
         Execute a query. Example:
         ```
         query = (
             Query(relevance_index, weights=[{"relevance_space": Param("relevance_weight")}])
```

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/executor/query/query_executor.py` & `superlinked-4.1.0/superlinked/framework/dsl/executor/query/query_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_configuration.py` & `superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_configuration.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py` & `superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_executor.py` & `superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_handler.py` & `superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_handler.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/index/effect.py` & `superlinked-4.1.0/superlinked/framework/dsl/index/effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/index/index.py` & `superlinked-4.1.0/superlinked/framework/dsl/index/index.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py` & `superlinked-4.1.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/index/util/aggregation_node_util.py` & `superlinked-4.1.0/superlinked/framework/dsl/index/util/aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py` & `superlinked-4.1.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py` & `superlinked-4.1.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py` & `superlinked-4.1.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/param.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/param.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/param_evaluator.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/param_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/predicate/binary_op.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/predicate/binary_op.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/predicate/binary_predicate.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/predicate/binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/predicate/query_predicate.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/predicate/query_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/query.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/query.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/query_filters.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/query_filters.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/query_vector_factory.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/query_vector_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/query_weighting.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/query_weighting.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/query/result.py` & `superlinked-4.1.0/superlinked/framework/dsl/query/result.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/registry/exception.py` & `superlinked-4.1.0/superlinked/framework/dsl/registry/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/registry/superlinked_registry.py` & `superlinked-4.1.0/superlinked/framework/dsl/registry/superlinked_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/source/in_memory_source.py` & `superlinked-4.1.0/superlinked/framework/dsl/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/source/rest_source.py` & `superlinked-4.1.0/superlinked/framework/dsl/source/rest_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/source/source.py` & `superlinked-4.1.0/superlinked/framework/dsl/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/space/categorical_similarity_space.py` & `superlinked-4.1.0/superlinked/framework/dsl/space/categorical_similarity_space.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import Mapping, cast
+from typing import Mapping
 
 from superlinked.framework.common.dag.categorical_similarity_node import (
     CategoricalSimilarityNode,
 )
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.embedding.categorical_similarity_embedding import (
     CategoricalSimilarityParams,
 )
-from superlinked.framework.common.schema.schema_object import (
-    SchemaField,
-    SchemaObject,
-    String,
-)
+from superlinked.framework.common.schema.schema_object import SchemaObject, String
 from superlinked.framework.dsl.space.space import Space
 from superlinked.framework.dsl.space.space_field_set import SpaceFieldSet
 
 
 class CategoricalSimilaritySpace(Space):
     """
     Represents a space for encoding categorical similarity.
@@ -111,15 +107,15 @@
             CategoricalSimilarityParams(
                 categories=categories,
                 uncategorized_as_category=uncategorized_as_category,
                 category_separator=category_separator,
                 negative_filter=negative_filter,
             )
         )
-        self.__category = SpaceFieldSet(self, cast(set[SchemaField], self._field_set))
+        self.__category = SpaceFieldSet(self, self._field_set)
         unchecked_category_node_map = {
             single_category: CategoricalSimilarityNode(
                 parent=SchemaFieldNode(single_category),
                 categorical_similarity_param=self.categorical_similarity_param,
             )
             for single_category in self._field_set
         }
```

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/space/custom_space.py` & `superlinked-4.1.0/superlinked/framework/dsl/space/custom_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from enum import Enum
-from typing import Mapping, cast
+from typing import Mapping
 
 from superlinked.framework.common.dag.custom_node import CustomVectorEmbeddingNode
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.schema.schema_object import (
-    Array,
-    SchemaField,
-    SchemaObject,
-)
+from superlinked.framework.common.schema.schema_object import Array, SchemaObject
 from superlinked.framework.common.space.aggregation import (
     Aggregation,
     VectorAggregation,
     VectorAvg,
 )
 from superlinked.framework.common.space.normalization import L2Norm, NoNorm
 from superlinked.framework.dsl.space.exception import (
@@ -104,15 +100,15 @@
             vector: CustomVectorEmbeddingNode(
                 parent=SchemaFieldNode(vector),
                 length=length,
                 aggregation=aggregation_strategy,
             )
             for vector in self._field_set
         }
-        self.vector = SpaceFieldSet(self, cast(set[SchemaField], self._field_set))
+        self.vector = SpaceFieldSet(self, self._field_set)
         self.__schema_node_map: dict[SchemaObject, CustomVectorEmbeddingNode] = {
             schema_field.schema_obj: node
             for schema_field, node in unchecked_custom_node_map.items()
         }
 
     @property
     def _node_by_schema(self) -> Mapping[SchemaObject, Node[Vector]]:
```

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/space/exception.py` & `superlinked-4.1.0/superlinked/framework/dsl/space/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/space/number_space.py` & `superlinked-4.1.0/superlinked/framework/dsl/space/number_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/space/recency_space.py` & `superlinked-4.1.0/superlinked/framework/dsl/space/recency_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from datetime import timedelta
-from typing import Mapping, cast
+from typing import Mapping
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.named_function_node import NamedFunctionNode
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.period_time import PeriodTime
 from superlinked.framework.common.dag.recency_node import RecencyNode
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.schema.schema_object import (
-    SchemaField,
-    SchemaObject,
-    Timestamp,
-)
+from superlinked.framework.common.schema.schema_object import SchemaObject, Timestamp
 from superlinked.framework.common.space.aggregation import InputAggregationMode
 from superlinked.framework.common.util.named_function_evaluator import NamedFunction
 from superlinked.framework.dsl.space.space import Space
 from superlinked.framework.dsl.space.space_field_set import SpaceFieldSet
 
 logger = logging.getLogger()
 
@@ -90,15 +86,15 @@
                 Weights default to 1. Period time to 14 days.
             aggregation_mode (InputAggregationMode): The  aggregation mode of the number embedding.
                 Possible values are: maximum, minimum and average. Defaults to InputAggregationMode.INPUT_AVERAGE.
             negative_filter (float): The recency score of items that are older than the oldest period time.
                 Defaults to 0.0.
         """
         super().__init__(timestamp, Timestamp)
-        self.timestamp = SpaceFieldSet(self, cast(set[SchemaField], self._field_set))
+        self.timestamp = SpaceFieldSet(self, self._field_set)
         self.period_time_list: list[PeriodTime] = (
             period_time_list
             if isinstance(period_time_list, list)
             else (
                 [period_time_list]
                 if period_time_list is not None
                 else [DEFAULT_PERIOD_TIME]
```

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/space/space.py` & `superlinked-4.1.0/superlinked/framework/dsl/space/space.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Abstract base class for a space.
 
     This class defines the interface for a space in the context of the application.
     """
 
     def __init__(self, fields: SIT | list[SIT], type_: type) -> None:
         super().__init__()
-        field_list = fields if isinstance(fields, list) else [fields]
+        field_list: list[SIT] = fields if isinstance(fields, list) else [fields]
         TypeValidator.validate_list_item_type(field_list, type_, "field_list")
         self.__validate_fields(field_list)
         self._field_set = set(field_list)
 
     def __validate_fields(self, field_list: list[SIT]) -> None:
         schema_list = [field.schema_obj for field in field_list]
         if duplicates := [
```

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/space/space_field_set.py` & `superlinked-4.1.0/superlinked/framework/dsl/space/space_field_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
-from typing import Any
+from typing import Any, Generic
 
 from superlinked.framework.common.schema.id_schema_object import SchemaField
-from superlinked.framework.dsl.space.space import Space
+from superlinked.framework.dsl.space.space import SIT, Space
 
 
 @dataclass
-class SpaceFieldSet:
+class SpaceFieldSet(Generic[SIT]):
     """
     A class representing a set of fields in a space.
     Attributes:
         space (Space): The space.
         fields (set[SchemaField]): The set of fields.
     """
 
     space: Space
-    fields: set[SchemaField]
+    fields: set[SIT]
 
     def __post_init__(self) -> None:
         self.__schema_field_map = {field.schema_obj: field for field in self.fields}
 
     def get_field_for_schema(self, schema_: Any) -> SchemaField | None:
         return self.__schema_field_map.get(schema_)
```

### Comparing `superlinked-4.0.1/superlinked/framework/dsl/space/text_similarity_space.py` & `superlinked-4.1.0/superlinked/framework/dsl/space/text_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/evaluator/dag_evaluator.py` & `superlinked-4.1.0/superlinked/framework/evaluator/dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/evaluator/online_dag_evaluator.py` & `superlinked-4.1.0/superlinked/framework/evaluator/online_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/evaluator/query_dag_evaluator.py` & `superlinked-4.1.0/superlinked/framework/evaluator/query_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/new_storage/in_memory/exception.py` & `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/new_storage/in_memory/in_memory_knn_search.py` & `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/in_memory_knn_search.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/new_storage/in_memory/in_memory_vdb.py` & `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/in_memory_vdb.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/new_storage/in_memory/index_config.py` & `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/index_config.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/new_storage/in_memory/json_codec.py` & `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/json_codec.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/new_storage/in_memory/object_serializer.py` & `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/object_serializer.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/batched_chunk_input_item.py` & `superlinked-4.1.0/superlinked/framework/online/dag/batched_chunk_input_item.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/default_online_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/default_online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/evaluation_result.py` & `superlinked-4.1.0/superlinked/framework/online/dag/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/exception.py` & `superlinked-4.1.0/superlinked/framework/online/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_aggregation_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_categorical_similarity_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_categorical_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_chunking_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_comparison_filter_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_concatenation_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_concatenation_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from functools import reduce
 from math import sqrt
 from typing import cast
 
 from beartype.typing import Sequence
 from typing_extensions import override
 
 from superlinked.framework.common.dag.concatenation_node import ConcatenationNode
@@ -59,20 +60,20 @@
     def _evaluate_singles(
         self,
         parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
         context: ExecutionContext,
     ) -> Sequence[Vector | None]:
         self.__check_evaluation_inputs(parent_results)
         vectors = [
-            sum(
-                [
+            reduce(
+                lambda a, b: a.concatenate(b),
+                (
                     self.__apply_vector_weight(result.value, parent.node_id, context)
                     for parent, result in parent_result.items()
-                ],
-                Vector([]),
+                ),
             )
             for parent_result in parent_results
         ]
         weight_sum = self._get_weight_abs_sum(context)
         return [
             (
                 vector
@@ -84,20 +85,20 @@
 
     def re_weight_vector(
         self,
         vector: Vector,
         context: ExecutionContext,
     ) -> Vector:
         parts = self._split_vector(vector)
-        vector = sum(
-            [
+        vector = reduce(
+            lambda a, b: a.concatenate(b),
+            (
                 self.__apply_vector_weight(part, parent.node_id, context)
                 for part, parent in zip(parts, self.parents)
-            ],
-            Vector([]),
+            ),
         )
         weight_sum = self._get_weight_abs_sum(context)
         return vector.normalize(sqrt(weight_sum))
 
     def _get_weight_abs_sum(
         self,
         context: ExecutionContext,
```

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_constant_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_custom_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_event_aggregation_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_index_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_named_function_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_node_registry.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_node_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_number_embedding_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_number_similarity_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_number_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_recency_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_schema_dag.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_schema_field_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/online_text_embedding_node.py` & `superlinked-4.1.0/superlinked/framework/online/dag/online_text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/parent_results.py` & `superlinked-4.1.0/superlinked/framework/online/dag/parent_results.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/dag/parent_validator.py` & `superlinked-4.1.0/superlinked/framework/online/dag/parent_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/source/in_memory_data_processor.py` & `superlinked-4.1.0/superlinked/framework/online/source/in_memory_data_processor.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/source/in_memory_object_writer.py` & `superlinked-4.1.0/superlinked/framework/online/source/in_memory_object_writer.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/source/in_memory_source.py` & `superlinked-4.1.0/superlinked/framework/online/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/online/store_manager/evaluation_result_store_manager.py` & `superlinked-4.1.0/superlinked/framework/online/store_manager/evaluation_result_store_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/entity.py` & `superlinked-4.1.0/superlinked/framework/storage/entity.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/entity_store.py` & `superlinked-4.1.0/superlinked/framework/storage/entity_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/entity_store_manager.py` & `superlinked-4.1.0/superlinked/framework/storage/entity_store_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/field.py` & `superlinked-4.1.0/superlinked/framework/storage/field.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/in_memory_entity_store.py` & `superlinked-4.1.0/superlinked/framework/storage/in_memory_entity_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/in_memory_object_store.py` & `superlinked-4.1.0/superlinked/framework/storage/in_memory_object_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/object_store.py` & `superlinked-4.1.0/superlinked/framework/storage/object_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/object_store_manager.py` & `superlinked-4.1.0/superlinked/framework/storage/object_store_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/superlinked/framework/storage/persistable_dict.py` & `superlinked-4.1.0/superlinked/framework/storage/persistable_dict.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.0.1/PKG-INFO` & `superlinked-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlinked
-Version: 4.0.1
+Version: 4.1.0
 Summary: The Superlinked vector computing library
 License: Apache-2.0
 Author: Superlinked Release
 Author-email: release@superlinked.com
 Requires-Python: >=3.10,<=3.12.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

