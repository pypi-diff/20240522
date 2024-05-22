# Comparing `tmp/gemmapy-1.0.1.tar.gz` & `tmp/gemmapy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemmapy-1.0.1.tar", last modified: Fri May 17 06:30:06 2024, max compression
+gzip compressed data, was "gemmapy-1.0.2.tar", last modified: Wed May 22 00:24:19 2024, max compression
```

## Comparing `gemmapy-1.0.1.tar` & `gemmapy-1.0.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-17 06:30:06.541129 gemmapy-1.0.1/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    11357 2024-05-04 04:09:08.000000 gemmapy-1.0.1/LICENSE.md
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-17 06:30:06.541129 gemmapy-1.0.1/PKG-INFO
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     1306 2024-05-07 21:06:20.000000 gemmapy-1.0.1/README.rst
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-17 06:30:06.513129 gemmapy-1.0.1/gemmapy/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)       61 2024-05-04 04:09:08.000000 gemmapy-1.0.1/gemmapy/__init__.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    21504 2024-05-08 23:46:56.000000 gemmapy-1.0.1/gemmapy/_processors.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6768 2024-05-07 20:41:44.000000 gemmapy-1.0.1/gemmapy/_subprocessors.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)      936 2024-05-07 20:41:44.000000 gemmapy-1.0.1/gemmapy/_validators.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    89515 2024-05-17 06:20:47.000000 gemmapy-1.0.1/gemmapy/gemmapy_api.py
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-17 06:30:06.517129 gemmapy-1.0.1/gemmapy/sdk/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    13741 2024-05-17 06:26:34.000000 gemmapy-1.0.1/gemmapy/sdk/__init__.py
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-17 06:30:06.517129 gemmapy-1.0.1/gemmapy/sdk/api/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)      138 2024-05-17 06:26:34.000000 gemmapy-1.0.1/gemmapy/sdk/api/__init__.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)   249425 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/api/default_api.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    25975 2024-05-17 06:26:34.000000 gemmapy-1.0.1/gemmapy/sdk/api_client.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9213 2024-05-17 06:26:34.000000 gemmapy-1.0.1/gemmapy/sdk/configuration.py
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-17 06:30:06.537129 gemmapy-1.0.1/gemmapy/sdk/models/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    13544 2024-05-17 06:26:34.000000 gemmapy-1.0.1/gemmapy/sdk/models/__init__.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6156 2024-05-17 06:26:31.000000 gemmapy-1.0.1/gemmapy/sdk/models/annotation_search_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8608 2024-05-17 06:26:31.000000 gemmapy-1.0.1/gemmapy/sdk/models/annotation_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9891 2024-05-17 06:26:31.000000 gemmapy-1.0.1/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5987 2024-05-17 06:26:31.000000 gemmapy-1.0.1/gemmapy/sdk/models/api_info_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    24020 2024-05-17 06:26:31.000000 gemmapy-1.0.1/gemmapy/sdk/models/array_design_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    24987 2024-05-17 06:26:31.000000 gemmapy-1.0.1/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8819 2024-05-17 06:26:31.000000 gemmapy-1.0.1/gemmapy/sdk/models/audit_event_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7478 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    16799 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/bibliographic_reference_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    14982 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/bio_assay_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9742 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/bio_material_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10036 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/bio_sequence_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5992 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/category_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7293 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/characteristic_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6624 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/citation_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/composite_sequence_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6014 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/composite_sequence_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8528 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/contrast_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/database_entry_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5384 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/database_entry_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset1.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset10.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset2.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset3.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset4.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset5.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset6.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset7.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset8.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset9.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3064 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/dataset_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    15728 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9056 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9659 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    14048 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/differential_expression_analysis_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5109 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/experiment_expression_levels_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9358 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/experimental_factor_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    15105 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/expression_experiment_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    28654 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    31623 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9207 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/external_database_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10910 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/factor_value_basic_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    16266 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/factor_value_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filter_arg_array_design.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3168 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3140 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filter_arg_expression_experiment.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10951 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_inferred_and_paginated_response_data_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9152 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9362 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10132 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9467 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8907 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    25633 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/geeq_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene1.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene2.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene3.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene4.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene5.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5754 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene_element_expressions_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7870 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene_ontology_term_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6956 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9642 2024-05-17 06:26:32.000000 gemmapy-1.0.1/gemmapy/sdk/models/gene_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7056 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/measurement_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3208 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5194 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/ontology_term_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8221 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8314 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7818 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9986 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/paginated_results_response_data_object_differential_expression_analysis_result_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8127 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/physical_location_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/platform.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/platform1.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/platform2.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/platform3.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/platform4.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/platform5.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3068 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/platform_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/probe.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/quantitation_type.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3100 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/quantitation_type_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    17466 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/quantitation_type_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10454 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_annotation_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10489 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_array_design_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10384 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_category_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    12908 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9082 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_response_data_object_taxon_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10652 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/query_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3884 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_api_info_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4099 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3978 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3945 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4187 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4143 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3901 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_gene_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3912 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3727 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_long.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3959 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4025 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3906 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4521 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/response_error_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/search_result_type.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7682 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7127 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/search_result_value_object_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4833 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/search_results_response_data_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6838 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/search_settings_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5411 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/simple_svd_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3096 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/sort_arg_array_design.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3160 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3132 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/sort_arg_expression_experiment.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4439 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/sort_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10286 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/statement_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxa.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon1.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon2.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon3.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon4.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon5.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon6.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon7.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon8.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon9.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6759 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8441 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5162 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/vector_element_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5078 2024-05-17 06:26:33.000000 gemmapy-1.0.1/gemmapy/sdk/models/well_composed_error_body.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    13649 2024-05-17 06:26:34.000000 gemmapy-1.0.1/gemmapy/sdk/rest.py
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-17 06:30:06.541129 gemmapy-1.0.1/gemmapy.egg-info/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-17 06:30:06.000000 gemmapy-1.0.1/gemmapy.egg-info/PKG-INFO
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7909 2024-05-17 06:30:06.000000 gemmapy-1.0.1/gemmapy.egg-info/SOURCES.txt
--rw-r--r--   0 omancarci (30067) pavlab   (30005)        1 2024-05-17 06:30:06.000000 gemmapy-1.0.1/gemmapy.egg-info/dependency_links.txt
--rw-r--r--   0 omancarci (30067) pavlab   (30005)      114 2024-05-17 06:30:06.000000 gemmapy-1.0.1/gemmapy.egg-info/requires.txt
--rw-r--r--   0 omancarci (30067) pavlab   (30005)        8 2024-05-17 06:30:06.000000 gemmapy-1.0.1/gemmapy.egg-info/top_level.txt
--rw-r--r--   0 omancarci (30067) pavlab   (30005)       81 2024-05-04 04:09:08.000000 gemmapy-1.0.1/pyproject.toml
--rw-r--r--   0 omancarci (30067) pavlab   (30005)      404 2024-05-17 06:30:06.541129 gemmapy-1.0.1/setup.cfg
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-17 06:30:06.537129 gemmapy-1.0.1/tests/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3766 2024-05-08 05:16:40.000000 gemmapy-1.0.1/tests/test_basic.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:19.016328 gemmapy-1.0.2/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    11357 2024-05-04 04:09:08.000000 gemmapy-1.0.2/LICENSE.md
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-22 00:24:19.016328 gemmapy-1.0.2/PKG-INFO
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1306 2024-05-07 21:06:20.000000 gemmapy-1.0.2/README.rst
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:18.984327 gemmapy-1.0.2/gemmapy/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)       61 2024-05-04 04:09:08.000000 gemmapy-1.0.2/gemmapy/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    21984 2024-05-22 00:14:58.000000 gemmapy-1.0.2/gemmapy/_processors.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6768 2024-05-07 20:41:44.000000 gemmapy-1.0.2/gemmapy/_subprocessors.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      936 2024-05-07 20:41:44.000000 gemmapy-1.0.2/gemmapy/_validators.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    89515 2024-05-17 06:20:47.000000 gemmapy-1.0.2/gemmapy/gemmapy_api.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:18.988327 gemmapy-1.0.2/gemmapy/sdk/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    13741 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/__init__.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:18.988327 gemmapy-1.0.2/gemmapy/sdk/api/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      138 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/api/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)   268620 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/api/default_api.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    25975 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/api_client.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9213 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/configuration.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:19.016328 gemmapy-1.0.2/gemmapy/sdk/models/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    13544 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6156 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/annotation_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8608 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/annotation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9891 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5987 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/api_info_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    24020 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    24987 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8819 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/audit_event_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7478 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    16799 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bibliographic_reference_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    14982 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bio_assay_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9742 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bio_material_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10036 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bio_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5992 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/category_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7293 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/characteristic_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6624 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/citation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/composite_sequence_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6014 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8528 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/contrast_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/database_entry_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5384 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/database_entry_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset10.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset6.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset7.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset8.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset9.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3064 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    15728 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9659 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    14048 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5109 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/experiment_expression_levels_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9358 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/experimental_factor_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    15105 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    28654 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    31623 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9207 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/external_database_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10910 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/factor_value_basic_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    16266 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/factor_value_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_array_design.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3168 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3140 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_expression_experiment.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10951 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_inferred_and_paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9152 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9362 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10132 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9467 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8907 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    25633 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/geeq_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5754 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_element_expressions_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7870 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6956 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9642 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7056 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/measurement_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3208 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5194 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8221 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8314 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7818 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9986 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/paginated_results_response_data_object_differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8127 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/physical_location_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3068 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/probe.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3100 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    17466 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10454 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_annotation_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10489 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_array_design_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10384 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_category_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    12908 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9082 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_response_data_object_taxon_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10652 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/query_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3884 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_api_info_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4099 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3978 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3945 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4187 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4143 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3901 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3912 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3727 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_long.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3959 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4025 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3906 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4521 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_error_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_result_type.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7682 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7127 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_result_value_object_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4833 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_results_response_data_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6838 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_settings_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5411 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/simple_svd_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3096 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_array_design.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3160 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3132 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_expression_experiment.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4439 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/sort_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10286 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/statement_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxa.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon6.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon7.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon8.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon9.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6759 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8441 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5162 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/vector_element_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5078 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/well_composed_error_body.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    13649 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/rest.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:19.016328 gemmapy-1.0.2/gemmapy.egg-info/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/PKG-INFO
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7909 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/SOURCES.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)        1 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/dependency_links.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      114 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/requires.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)        8 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/top_level.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)       81 2024-05-04 04:09:08.000000 gemmapy-1.0.2/pyproject.toml
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      404 2024-05-22 00:24:19.016328 gemmapy-1.0.2/setup.cfg
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:19.016328 gemmapy-1.0.2/tests/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3861 2024-05-17 23:46:21.000000 gemmapy-1.0.2/tests/test_basic.py
```

### Comparing `gemmapy-1.0.1/LICENSE.md` & `gemmapy-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/PKG-INFO` & `gemmapy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemmapy
-Version: 1.0.1
+Version: 1.0.2
 Summary: a Python Wrapper for the Gemma API
 Keywords: gemma,bioinformatics
 Requires-Python: >3.10
 License-File: LICENSE.md
 Requires-Dist: certifi>=14.05.14
 Requires-Dist: six>=1.10
 Requires-Dist: python_dateutil>=2.5.3
```

### Comparing `gemmapy-1.0.1/README.rst` & `gemmapy-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/_processors.py` & `gemmapy-1.0.2/gemmapy/_processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,26 +319,36 @@
                 nrows = out.shape[0]
                 out.insert(0,"NCBIid",sub.rep(y.gene_ncbi_id,nrows))
                 out.insert(0,"GeneSymbol",sub.rep(y.gene_official_symbol,nrows))
                 out.insert(0,"Probe",sub.field_in_list(y.vectors,'design_element_name'))
                 return out
             dataset_exp = pd.concat([compile_exp_frame(y) for y in x.gene_expression_levels],ignore_index = True)
         
-        samples = self.get_dataset_samples(dataset)
-        
-        dataset_exp = \
-            dataset_exp.\
-                reindex(
-                    columns = \
-                        list(dataset_exp.columns[~np.array(
-                            sub.list_in_list(dataset_exp.columns,
-                                             samples.sample_name))]) + \
-                            list(samples.sample_name))
         
-        out.update({dataset:dataset_exp })
+        samples = self.get_dataset_samples(dataset)
+
+        if dataset_exp.shape == (0,0):
+            gene_data = pd.DataFrame({
+                'Probe': pd.Series(dtype = 'str'),
+                'GeneSymbol': pd.Series(dtype = 'str'),
+                'NCBIid': pd.Series(dtype = 'int')
+                })
+            expression = pd.DataFrame(columns = samples.sample_name,dtype = 'float64')
+            
+            out.update({dataset: pd.concat([gene_data,expression],axis = 1)})
+        else:
+            dataset_exp = \
+                dataset_exp.\
+                    reindex(
+                        columns = \
+                            list(dataset_exp.columns[~np.array(
+                                sub.list_in_list(dataset_exp.columns,
+                                                 samples.sample_name))]) + \
+                                list(samples.sample_name))     
+            out.update({dataset:dataset_exp })
 
 
     return out
 
 def process_platforms(d:list):
     
     df = pd.DataFrame({
```

### Comparing `gemmapy-1.0.1/gemmapy/_subprocessors.py` & `gemmapy-1.0.2/gemmapy/_subprocessors.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/_validators.py` & `gemmapy-1.0.2/gemmapy/_validators.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/gemmapy_api.py` & `gemmapy-1.0.2/gemmapy/gemmapy_api.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/__init__.py` & `gemmapy-1.0.2/gemmapy/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/api/default_api.py` & `gemmapy-1.0.2/gemmapy/sdk/api/default_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
+import time
+from gemmapy.sdk.rest import ApiException
+
 
 # python 2 and python 3 compatibility library
 import six
 
 from gemmapy.sdk.api_client import ApiClient
 
 
@@ -43,19 +46,31 @@
 
         :param async_req bool
         :return: ResponseDataObjectApiInfoValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_api_info_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_api_info_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_api_info_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_api_info_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_api_info_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve an object with basic API information  # noqa: E501
 
         The payload contains a list of featured external databases that Gemma uses under the `externalDatabases` field. Those are mainly genomic references and sources of gene annotations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -138,19 +153,31 @@
         :param async_req bool
         :param Dataset dataset: (required)
         :return: ResponseDataObjectSetAnnotationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_annotations_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_annotations_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_annotations_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_annotations_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_annotations_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the annotations of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_annotations_with_http_info(dataset, async_req=True)
@@ -239,19 +266,31 @@
         :param async_req bool
         :param Dataset1 dataset: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_design_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_design_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_design_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_design_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_design_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the design of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_design_with_http_info(dataset, async_req=True)
@@ -345,19 +384,31 @@
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_differential_expression_with_http_info(datasets, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_differential_expression_with_http_info(datasets, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_differential_expression_with_http_info(datasets, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_differential_expression_with_http_info(datasets, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_differential_expression_with_http_info(self, datasets, **kwargs):  # noqa: E501
         """Retrieve the expression levels of a set of datasets subject to a threshold on their differential expressions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_differential_expression_with_http_info(datasets, async_req=True)
@@ -464,19 +515,31 @@
         :param int offset:
         :param int limit:
         :return: ResponseDataObjectListDifferentialExpressionAnalysisValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_differential_expression_analyses_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_differential_expression_analyses_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_differential_expression_analyses_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_differential_expression_analyses_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_differential_expression_analyses_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve annotations and surface level stats for a dataset's differential analyses  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_differential_expression_analyses_with_http_info(dataset, async_req=True)
@@ -571,19 +634,31 @@
         :param async_req bool
         :param Dataset3 dataset: (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_differential_expression_analyses_result_sets_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_differential_expression_analyses_result_sets_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_differential_expression_analyses_result_sets_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_differential_expression_analyses_result_sets_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_differential_expression_analyses_result_sets_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the result sets of all differential analyses of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_differential_expression_analyses_result_sets_with_http_info(dataset, async_req=True)
@@ -674,19 +749,31 @@
         :param Dataset4 dataset: (required)
         :param bool filter:
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_expression_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_expression_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_expression_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_expression_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_expression_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve processed expression data of a dataset  # noqa: E501
 
         This endpoint is deprecated and getDatasetProcessedExpression() should be used instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -782,19 +869,31 @@
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_expression_for_genes_with_http_info(datasets, genes, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_expression_for_genes_with_http_info(datasets, genes, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_expression_for_genes_with_http_info(datasets, genes, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_expression_for_genes_with_http_info(datasets, genes, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_expression_for_genes_with_http_info(self, datasets, genes, **kwargs):  # noqa: E501
         """Retrieve the expression data matrix of a set of datasets and genes  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_expression_for_genes_with_http_info(datasets, genes, async_req=True)
@@ -902,19 +1001,31 @@
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_expression_for_genes_in_taxa_with_http_info(datasets, taxa, genes, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_expression_for_genes_in_taxa_with_http_info(datasets, taxa, genes, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_expression_for_genes_in_taxa_with_http_info(datasets, taxa, genes, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_expression_for_genes_in_taxa_with_http_info(datasets, taxa, genes, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_expression_for_genes_in_taxa_with_http_info(self, datasets, taxa, genes, **kwargs):  # noqa: E501
         """Retrieve the expression data matrix of a set of datasets and genes  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_expression_for_genes_in_taxa_with_http_info(datasets, taxa, genes, async_req=True)
@@ -1029,19 +1140,31 @@
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_expression_pca_with_http_info(datasets, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_expression_pca_with_http_info(datasets, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_expression_pca_with_http_info(datasets, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_expression_pca_with_http_info(datasets, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_expression_pca_with_http_info(self, datasets, **kwargs):  # noqa: E501
         """Retrieve the principal components (PCA) of a set of datasets  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_expression_pca_with_http_info(datasets, async_req=True)
@@ -1143,19 +1266,31 @@
         :param async_req bool
         :param Dataset5 dataset: (required)
         :return: ResponseDataObjectListArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_platforms_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_platforms_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_platforms_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_platforms_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_platforms_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the platforms of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_platforms_with_http_info(dataset, async_req=True)
@@ -1244,19 +1379,31 @@
         :param async_req bool
         :param Dataset6 dataset: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_processed_expression_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_processed_expression_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_processed_expression_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_processed_expression_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_processed_expression_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve processed expression data of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_processed_expression_with_http_info(dataset, async_req=True)
@@ -1345,19 +1492,31 @@
         :param async_req bool
         :param Dataset7 dataset: (required)
         :return: ResponseDataObjectSetQuantitationTypeValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_quantitation_types_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_quantitation_types_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_quantitation_types_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_quantitation_types_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_quantitation_types_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve quantitation types of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_quantitation_types_with_http_info(dataset, async_req=True)
@@ -1447,19 +1606,31 @@
         :param Dataset8 dataset: (required)
         :param QuantitationType quantitation_type:
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_raw_expression_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_raw_expression_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_raw_expression_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_raw_expression_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_raw_expression_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve raw expression data of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_raw_expression_with_http_info(dataset, async_req=True)
@@ -1551,19 +1722,31 @@
         :param async_req bool
         :param Dataset9 dataset: (required)
         :return: ResponseDataObjectListBioAssayValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_samples_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_samples_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_samples_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_samples_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_samples_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the samples of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_samples_with_http_info(dataset, async_req=True)
@@ -1652,19 +1835,31 @@
         :param async_req bool
         :param Dataset10 dataset: (required)
         :return: ResponseDataObjectSimpleSVDValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_dataset_svd_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_dataset_svd_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_dataset_svd_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_dataset_svd_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_dataset_svd_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the singular value decomposition (SVD) of a dataset expression data  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_svd_with_http_info(dataset, async_req=True)
@@ -1757,19 +1952,31 @@
         :param int limit:
         :param SortArgExpressionExperiment sort:
         :return: QueriedAndFilteredAndInferredAndPaginatedResponseDataObjectExpressionExperimentWithSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_datasets_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_datasets_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_datasets_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_datasets_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_datasets_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all datasets  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_datasets_with_http_info(async_req=True)
@@ -1872,19 +2079,31 @@
         :param int min_frequency: Minimum number of associated datasets to report an annotation. If used, the limit will default to 5000.
         :param str category: A category URI to restrict reported annotations. If unspecified, annotations from all categories are reported. If empty, uncategorized terms are reported.
         :return: QueriedAndFilteredAndInferredAndLimitedResponseDataObjectAnnotationWithUsageStatisticsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_datasets_annotations_usage_statistics_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_datasets_annotations_usage_statistics_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_datasets_annotations_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_datasets_annotations_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_datasets_annotations_usage_statistics_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve usage statistics of annotations among datasets matching the provided query and filter  # noqa: E501
 
         Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -1990,19 +2209,31 @@
         :param int limit:
         :param SortArgExpressionExperiment sort:
         :return: FilteredAndInferredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_datasets_by_ids_with_http_info(dataset, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_datasets_by_ids_with_http_info(dataset, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_datasets_by_ids_with_http_info(dataset, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_datasets_by_ids_with_http_info(dataset, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_datasets_by_ids_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve datasets by their identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_datasets_by_ids_with_http_info(dataset, async_req=True)
@@ -2107,19 +2338,31 @@
         :param FilterArgExpressionExperiment filter:
         :param int limit:
         :return: QueriedAndFilteredAndInferredAndLimitedResponseDataObjectCategoryWithUsageStatisticsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_datasets_categories_usage_statistics_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_datasets_categories_usage_statistics_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_datasets_categories_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_datasets_categories_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_datasets_categories_usage_statistics_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve usage statistics of categories among datasets matching the provided query and filter  # noqa: E501
 
         Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -2214,19 +2457,31 @@
         :param FilterArgExpressionExperiment filter:
         :param int limit:
         :return: QueriedAndFilteredAndInferredAndLimitedResponseDataObjectArrayDesignWithUsageStatisticsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_datasets_platforms_usage_statistics_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_datasets_platforms_usage_statistics_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_datasets_platforms_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_datasets_platforms_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_datasets_platforms_usage_statistics_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve usage statistics of platforms among datasets matching the provided query and filter  # noqa: E501
 
         Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -2319,19 +2574,31 @@
         :param QueryArg query:
         :param FilterArgExpressionExperiment filter:
         :return: QueriedAndFilteredAndInferredResponseDataObjectTaxonWithUsageStatisticsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_datasets_taxa_usage_statistics_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_datasets_taxa_usage_statistics_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_datasets_taxa_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_datasets_taxa_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_datasets_taxa_usage_statistics_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve taxa usage statistics for datasets matching the provided query and filter  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_datasets_taxa_usage_statistics_with_http_info(async_req=True)
@@ -2419,19 +2686,31 @@
         :param async_req bool
         :param Gene gene: (required)
         :return: ResponseDataObjectListGeneOntologyTermValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_gene_go_terms_with_http_info(gene, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_gene_go_terms_with_http_info(gene, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_gene_go_terms_with_http_info(gene, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_gene_go_terms_with_http_info(gene, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_gene_go_terms_with_http_info(self, gene, **kwargs):  # noqa: E501
         """Retrieve the GO terms associated to a gene  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_gene_go_terms_with_http_info(gene, async_req=True)
@@ -2520,19 +2799,31 @@
         :param async_req bool
         :param Gene1 gene: (required)
         :return: ResponseDataObjectListPhysicalLocationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_gene_locations_with_http_info(gene, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_gene_locations_with_http_info(gene, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_gene_locations_with_http_info(gene, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_gene_locations_with_http_info(gene, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_gene_locations_with_http_info(self, gene, **kwargs):  # noqa: E501
         """Retrieve the physical locations of a given gene  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_gene_locations_with_http_info(gene, async_req=True)
@@ -2623,19 +2914,31 @@
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_gene_probes_with_http_info(gene, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_gene_probes_with_http_info(gene, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_gene_probes_with_http_info(gene, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_gene_probes_with_http_info(gene, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_gene_probes_with_http_info(self, gene, **kwargs):  # noqa: E501
         """Retrieve the probes associated to a genes across all platforms  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_gene_probes_with_http_info(gene, async_req=True)
@@ -2730,19 +3033,31 @@
         :param async_req bool
         :param list[object] genes: (required)
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_genes_with_http_info(genes, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_genes_with_http_info(genes, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_genes_with_http_info(genes, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_genes_with_http_info(genes, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_genes_with_http_info(self, genes, **kwargs):  # noqa: E501
         """Retrieve genes matching gene identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_genes_with_http_info(genes, async_req=True)
@@ -2833,19 +3148,31 @@
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_genes1_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_genes1_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_genes1_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_genes1_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_genes1_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all genes  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_genes1_with_http_info(async_req=True)
@@ -2934,19 +3261,31 @@
         :param QueryArg query:
         :param FilterArgExpressionExperiment filter:
         :return: ResponseDataObjectLong
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_number_of_datasets_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_number_of_datasets_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_number_of_datasets_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_number_of_datasets_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_number_of_datasets_with_http_info(self, **kwargs):  # noqa: E501
         """Count datasets matching the provided query and filter  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_number_of_datasets_with_http_info(async_req=True)
@@ -3034,19 +3373,31 @@
         :param async_req bool
         :param FilterArgArrayDesign filter:
         :return: ResponseDataObjectLong
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_number_of_platforms_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_number_of_platforms_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_number_of_platforms_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_number_of_platforms_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_number_of_platforms_with_http_info(self, **kwargs):  # noqa: E501
         """Count platforms matching the provided filter  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_number_of_platforms_with_http_info(async_req=True)
@@ -3131,19 +3482,31 @@
         :param async_req bool
         :param FilterArgExpressionAnalysisResultSet filter:
         :return: ResponseDataObjectLong
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_number_of_result_sets_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_number_of_result_sets_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_number_of_result_sets_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_number_of_result_sets_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_number_of_result_sets_with_http_info(self, **kwargs):  # noqa: E501
         """Count result sets matching the provided filter  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_number_of_result_sets_with_http_info(async_req=True)
@@ -3228,19 +3591,31 @@
         :param async_req bool
         :param Platform platform: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_platform_annotations_with_http_info(platform, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_platform_annotations_with_http_info(platform, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_platform_annotations_with_http_info(platform, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_platform_annotations_with_http_info(platform, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_platform_annotations_with_http_info(self, platform, **kwargs):  # noqa: E501
         """Retrieve the annotations of a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_platform_annotations_with_http_info(platform, async_req=True)
@@ -3331,19 +3706,31 @@
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_platform_datasets_with_http_info(platform, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_platform_datasets_with_http_info(platform, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_platform_datasets_with_http_info(platform, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_platform_datasets_with_http_info(platform, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_platform_datasets_with_http_info(self, platform, **kwargs):  # noqa: E501
         """Retrieve all experiments using a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_platform_datasets_with_http_info(platform, async_req=True)
@@ -3441,19 +3828,31 @@
         :param int offset:
         :param int limit:
         :return: FilteredAndPaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_platform_element_with_http_info(platform, probes, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_platform_element_with_http_info(platform, probes, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_platform_element_with_http_info(platform, probes, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_platform_element_with_http_info(platform, probes, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_platform_element_with_http_info(self, platform, probes, **kwargs):  # noqa: E501
         """Retrieve the selected probes for a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_platform_element_with_http_info(platform, probes, async_req=True)
@@ -3559,19 +3958,31 @@
         :param int offset:
         :param int limit:
         :return: FilteredAndPaginatedResponseDataObjectGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_platform_element_genes_with_http_info(platform, probe, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_platform_element_genes_with_http_info(platform, probe, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_platform_element_genes_with_http_info(platform, probe, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_platform_element_genes_with_http_info(platform, probe, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_platform_element_genes_with_http_info(self, platform, probe, **kwargs):  # noqa: E501
         """Retrieve the genes associated to a probe in a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_platform_element_genes_with_http_info(platform, probe, async_req=True)
@@ -3675,19 +4086,31 @@
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_platform_elements_with_http_info(platform, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_platform_elements_with_http_info(platform, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_platform_elements_with_http_info(platform, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_platform_elements_with_http_info(platform, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_platform_elements_with_http_info(self, platform, **kwargs):  # noqa: E501
         """Retrieve the probes for a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_platform_elements_with_http_info(platform, async_req=True)
@@ -3785,19 +4208,31 @@
         :param int limit:
         :param SortArgArrayDesign sort:
         :return: FilteredAndPaginatedResponseDataObjectArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_platforms_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_platforms_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_platforms_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_platforms_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_platforms_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all platforms  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_platforms_with_http_info(async_req=True)
@@ -3895,19 +4330,31 @@
         :param int limit:
         :param SortArgArrayDesign sort:
         :return: FilteredAndPaginatedResponseDataObjectArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_platforms_by_ids_with_http_info(platform, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_platforms_by_ids_with_http_info(platform, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_platforms_by_ids_with_http_info(platform, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_platforms_by_ids_with_http_info(platform, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_platforms_by_ids_with_http_info(self, platform, **kwargs):  # noqa: E501
         """Retrieve all platforms matching a set of platform identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_platforms_by_ids_with_http_info(platform, async_req=True)
@@ -4013,19 +4460,31 @@
         :param int offset:
         :param int limit:
         :return: PaginatedResultsResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_result_set_with_http_info(result_set, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_result_set_with_http_info(result_set, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_result_set_with_http_info(result_set, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_result_set_with_http_info(result_set, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_result_set_with_http_info(self, result_set, **kwargs):  # noqa: E501
         """Retrieve a single analysis result set by its identifier  # noqa: E501
 
         A slice or results can be retrieved by specifying the `offset` and `limit` parameters. This is only applicable to the JSON representation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -4129,19 +4588,31 @@
         :param int limit:
         :param SortArgExpressionAnalysisResultSet sort:
         :return: FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_result_sets_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_result_sets_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_result_sets_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_result_sets_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_result_sets_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all result sets matching the provided criteria  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_result_sets_with_http_info(async_req=True)
@@ -4242,19 +4713,31 @@
 
         :param async_req bool
         :return: ResponseDataObjectListTaxonValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxa_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxa_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxa_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxa_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxa_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all available taxa  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxa_with_http_info(async_req=True)
@@ -4336,19 +4819,31 @@
         :param async_req bool
         :param list[object] taxa: (required)
         :return: ResponseDataObjectListTaxonValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxa_by_ids_with_http_info(taxa, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxa_by_ids_with_http_info(taxa, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxa_by_ids_with_http_info(taxa, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxa_by_ids_with_http_info(taxa, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxa_by_ids_with_http_info(self, taxa, **kwargs):  # noqa: E501
         """Retrieve taxa by their identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxa_by_ids_with_http_info(taxa, async_req=True)
@@ -4442,19 +4937,31 @@
         :param int limit:
         :param SortArgExpressionExperiment sort:
         :return: FilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxon_datasets_with_http_info(self, taxon, **kwargs):  # noqa: E501
         """Retrieve the datasets for a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxon_datasets_with_http_info(taxon, async_req=True)
@@ -4556,19 +5063,31 @@
         :param Taxon4 taxon: (required)
         :param Gene3 gene: (required)
         :return: ResponseDataObjectListGeneOntologyTermValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxon_gene_go_terms_with_http_info(taxon, gene, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxon_gene_go_terms_with_http_info(taxon, gene, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxon_gene_go_terms_with_http_info(taxon, gene, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxon_gene_go_terms_with_http_info(taxon, gene, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxon_gene_go_terms_with_http_info(self, taxon, gene, **kwargs):  # noqa: E501
         """Retrieve the GO terms associated to a gene in a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxon_gene_go_terms_with_http_info(taxon, gene, async_req=True)
@@ -4665,19 +5184,31 @@
         :param Taxon5 taxon: (required)
         :param Gene4 gene: (required)
         :return: ResponseDataObjectListPhysicalLocationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxon_gene_locations_with_http_info(taxon, gene, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxon_gene_locations_with_http_info(taxon, gene, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxon_gene_locations_with_http_info(taxon, gene, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxon_gene_locations_with_http_info(taxon, gene, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxon_gene_locations_with_http_info(self, taxon, gene, **kwargs):  # noqa: E501
         """Retrieve physical locations for a given gene and taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxon_gene_locations_with_http_info(taxon, gene, async_req=True)
@@ -4776,19 +5307,31 @@
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxon_gene_probes_with_http_info(taxon, gene, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxon_gene_probes_with_http_info(taxon, gene, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxon_gene_probes_with_http_info(taxon, gene, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxon_gene_probes_with_http_info(taxon, gene, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxon_gene_probes_with_http_info(self, taxon, gene, **kwargs):  # noqa: E501
         """Retrieve the probes associated to a genes across all platforms in a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxon_gene_probes_with_http_info(taxon, gene, async_req=True)
@@ -4892,19 +5435,31 @@
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxon_genes_with_http_info(taxon, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxon_genes_with_http_info(taxon, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxon_genes_with_http_info(taxon, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxon_genes_with_http_info(taxon, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxon_genes_with_http_info(self, taxon, **kwargs):  # noqa: E501
         """Retrieve all genes in a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxon_genes_with_http_info(taxon, async_req=True)
@@ -5000,19 +5555,31 @@
         :param Taxon8 taxon: (required)
         :param list[object] gene: (required)
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxon_genes_by_ids_with_http_info(taxon, gene, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxon_genes_by_ids_with_http_info(taxon, gene, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxon_genes_by_ids_with_http_info(taxon, gene, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxon_genes_by_ids_with_http_info(taxon, gene, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxon_genes_by_ids_with_http_info(self, taxon, gene, **kwargs):  # noqa: E501
         """Retrieve genes matching gene identifiers in a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxon_genes_by_ids_with_http_info(taxon, gene, async_req=True)
@@ -5113,19 +5680,31 @@
         :param int size: (required)
         :param str strand:
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, start, size, **kwargs)  # noqa: E501
-        else:
-            (data) = self.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, start, size, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, start, size, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, start, size, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def get_taxon_genes_overlapping_chromosome_with_http_info(self, taxon, chromosome, start, size, **kwargs):  # noqa: E501
         """Retrieve genes overlapping a given region in a taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, start, size, async_req=True)
@@ -5243,19 +5822,31 @@
         :param int limit: Maximum number of search results to return; capped at 2000 unless `resultObject` is excluded.
         :param list[str] exclude: List of fields to exclude from the payload. Only `resultObject` is supported.
         :return: SearchResultsResponseDataObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.search_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.search_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.search_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.search_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def search_with_http_info(self, **kwargs):  # noqa: E501
         """Search everything in Gemma  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.search_with_http_info(async_req=True)
@@ -5357,19 +5948,31 @@
         :param async_req bool
         :param list[str] query: A comma-delimited list of keywords to find annotations.
         :return: ResponseDataObjectListAnnotationSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.search_annotations_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.search_annotations_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.search_annotations_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.search_annotations_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def search_annotations_with_http_info(self, **kwargs):  # noqa: E501
         """Search for annotation tags  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.search_annotations_with_http_info(async_req=True)
@@ -5456,19 +6059,31 @@
         :param async_req bool
         :param list[str] query: A comma-delimited list of keywords to find annotations. (required)
         :return: ResponseDataObjectListAnnotationSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.search_annotations_by_path_query_with_http_info(query, **kwargs)  # noqa: E501
-        else:
-            (data) = self.search_annotations_by_path_query_with_http_info(query, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.search_annotations_by_path_query_with_http_info(query, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.search_annotations_by_path_query_with_http_info(query, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def search_annotations_by_path_query_with_http_info(self, query, **kwargs):  # noqa: E501
         """Search for annotation tags  # noqa: E501
 
         This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -5564,19 +6179,31 @@
         :param int limit:
         :param SortArgExpressionExperiment sort:
         :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.search_datasets_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.search_datasets_with_http_info(**kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.search_datasets_with_http_info(**kwargs)  # noqa: E501
+                else:
+                    (data) = self.search_datasets_with_http_info(**kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def search_datasets_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve datasets associated to an annotation tags search  # noqa: E501
 
         This is deprecated in favour of the [/datasets](#/default/getDatasets) endpoint. Use the `AND` operator to intersect the results of multiple queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -5680,19 +6307,31 @@
         :param int limit:
         :param SortArgExpressionExperiment sort:
         :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.search_datasets_by_query_in_path_with_http_info(query, **kwargs)  # noqa: E501
-        else:
-            (data) = self.search_datasets_by_query_in_path_with_http_info(query, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.search_datasets_by_query_in_path_with_http_info(query, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.search_datasets_by_query_in_path_with_http_info(query, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def search_datasets_by_query_in_path_with_http_info(self, query, **kwargs):  # noqa: E501
         """Retrieve datasets associated to an annotation tags search  # noqa: E501
 
         This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -5801,19 +6440,31 @@
         :param int limit:
         :param SortArgExpressionExperiment sort:
         :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.search_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
-        else:
-            (data) = self.search_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.search_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.search_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def search_taxon_datasets_with_http_info(self, taxon, **kwargs):  # noqa: E501
         """Retrieve datasets within a given taxa associated to an annotation tags search  # noqa: E501
 
         This is deprecated in favour of the [/datasets](#/default/getDatasets) endpoint with a `query` parameter and a `filter` parameter with `taxon.id = {taxon} or taxon.commonName = {taxon} or taxon.scientificName = {taxon}` to restrict the taxon instead.  Use the `AND` operator to intersect the results of multiple queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -5925,19 +6576,31 @@
         :param int limit:
         :param SortArgExpressionExperiment sort:
         :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.search_taxon_datasets_by_query_in_path_with_http_info(taxon, query, **kwargs)  # noqa: E501
-        else:
-            (data) = self.search_taxon_datasets_by_query_in_path_with_http_info(taxon, query, **kwargs)  # noqa: E501
-            return data
+        
+         
+        attempts = 0
+        
+        while True:
+            try:
+                if kwargs.get('async_req'):
+                    return self.search_taxon_datasets_by_query_in_path_with_http_info(taxon, query, **kwargs)  # noqa: E501
+                else:
+                    (data) = self.search_taxon_datasets_by_query_in_path_with_http_info(taxon, query, **kwargs)  # noqa: E501
+                    return data
+            except ApiException as err:
+                if err.status in [429,500] and attempts < 2:
+                    attempts += 1
+                    time.sleep(3)
+                else: 
+                    raise err
 
     def search_taxon_datasets_by_query_in_path_with_http_info(self, taxon, query, **kwargs):  # noqa: E501
         """Retrieve datasets within a given taxa associated to an annotation tags search  # noqa: E501
 
         This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
```

### Comparing `gemmapy-1.0.1/gemmapy/sdk/api_client.py` & `gemmapy-1.0.2/gemmapy/sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'gemmapy/1.0.1'
+        self.user_agent = 'gemmapy/1.0.2'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `gemmapy-1.0.1/gemmapy/sdk/configuration.py` & `gemmapy-1.0.2/gemmapy/sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/__init__.py` & `gemmapy-1.0.2/gemmapy/sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/annotation_search_result_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/annotation_search_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/annotation_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/annotation_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/api_info_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/api_info_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/array_design_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/array_design_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/audit_event_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/audit_event_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/bibliographic_reference_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/bibliographic_reference_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/bio_assay_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/bio_assay_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/bio_material_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/bio_material_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/bio_sequence_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/bio_sequence_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/category_with_usage_statistics_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/category_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/characteristic_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/characteristic_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/citation_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/citation_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/composite_sequence_arg.py` & `gemmapy-1.0.2/gemmapy/sdk/models/composite_sequence_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/composite_sequence_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/composite_sequence_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/contrast_result_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/contrast_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/database_entry_arg.py` & `gemmapy-1.0.2/gemmapy/sdk/models/database_entry_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/database_entry_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/database_entry_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset1.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset1.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset10.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset10.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset2.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset2.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset3.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset3.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset4.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset4.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset5.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset5.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset6.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset6.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset7.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset7.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset8.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset8.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset9.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset9.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/dataset_arg.py` & `gemmapy-1.0.2/gemmapy/sdk/models/dataset_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/differential_expression_analysis_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/experiment_expression_levels_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/experiment_expression_levels_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/experimental_factor_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/experimental_factor_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/expression_experiment_set_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/expression_experiment_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/external_database_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/external_database_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/factor_value_basic_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/factor_value_basic_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/factor_value_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/factor_value_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filter_arg_array_design.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_array_design.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filter_arg_expression_experiment.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_expression_experiment.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_inferred_and_paginated_response_data_object_expression_experiment_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_inferred_and_paginated_response_data_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/geeq_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/geeq_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene1.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene1.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene2.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene2.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene3.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene3.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene4.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene4.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene5.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene5.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene_arg.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene_element_expressions_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene_element_expressions_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene_ontology_term_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene_ontology_term_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene_set_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/gene_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/gene_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/measurement_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/measurement_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/ontology_term_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/ontology_term_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/paginated_results_response_data_object_differential_expression_analysis_result_set_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/paginated_results_response_data_object_differential_expression_analysis_result_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/physical_location_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/physical_location_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/platform.py` & `gemmapy-1.0.2/gemmapy/sdk/models/platform.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/platform1.py` & `gemmapy-1.0.2/gemmapy/sdk/models/platform1.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/platform2.py` & `gemmapy-1.0.2/gemmapy/sdk/models/platform2.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/platform3.py` & `gemmapy-1.0.2/gemmapy/sdk/models/platform3.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/platform4.py` & `gemmapy-1.0.2/gemmapy/sdk/models/platform4.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/platform5.py` & `gemmapy-1.0.2/gemmapy/sdk/models/platform5.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/platform_arg.py` & `gemmapy-1.0.2/gemmapy/sdk/models/platform_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/probe.py` & `gemmapy-1.0.2/gemmapy/sdk/models/probe.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/quantitation_type.py` & `gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/quantitation_type_arg.py` & `gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/quantitation_type_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_annotation_with_usage_statistics_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_annotation_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_array_design_with_usage_statistics_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_array_design_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_category_with_usage_statistics_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_category_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_inferred_response_data_object_taxon_with_usage_statistics_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_response_data_object_taxon_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/query_arg.py` & `gemmapy-1.0.2/gemmapy/sdk/models/query_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_api_info_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_api_info_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_gene_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_gene_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_long.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_long.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/response_error_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/response_error_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/search_result_type.py` & `gemmapy-1.0.2/gemmapy/sdk/models/search_result_type.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/search_result_value_object_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/search_result_value_object_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/search_results_response_data_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/search_results_response_data_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/search_settings_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/search_settings_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/simple_svd_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/simple_svd_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/sort_arg_array_design.py` & `gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_array_design.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py` & `gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/sort_arg_expression_experiment.py` & `gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_expression_experiment.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/sort_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/sort_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/statement_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/statement_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxa.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxa.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon1.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon1.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon2.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon2.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon3.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon3.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon4.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon4.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon5.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon5.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon6.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon6.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon7.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon7.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon8.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon8.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon9.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon9.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon_arg.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/vector_element_value_object.py` & `gemmapy-1.0.2/gemmapy/sdk/models/vector_element_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/models/well_composed_error_body.py` & `gemmapy-1.0.2/gemmapy/sdk/models/well_composed_error_body.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy/sdk/rest.py` & `gemmapy-1.0.2/gemmapy/sdk/rest.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/gemmapy.egg-info/PKG-INFO` & `gemmapy-1.0.2/gemmapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemmapy
-Version: 1.0.1
+Version: 1.0.2
 Summary: a Python Wrapper for the Gemma API
 Keywords: gemma,bioinformatics
 Requires-Python: >3.10
 License-File: LICENSE.md
 Requires-Dist: certifi>=14.05.14
 Requires-Dist: six>=1.10
 Requires-Dist: python_dateutil>=2.5.3
```

### Comparing `gemmapy-1.0.1/gemmapy.egg-info/SOURCES.txt` & `gemmapy-1.0.2/gemmapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.1/tests/test_basic.py` & `gemmapy-1.0.2/tests/test_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,25 @@
 @author: omancarci
 """
 import pytest
 import gemmapy
 import pandas as pd
 from gemmapy import _subprocessors as sub
 import anndata as ad
+import time
 
 
 api = gemmapy.GemmaPy()
 
+@pytest.fixture(autouse=True)
+def slow_down_tests():
+    yield
+    time.sleep(1)
+
+
 def test_get_result_sets():
     res = api.get_result_sets([200])
     
     assert type(res) is pd.core.frame.DataFrame
     
     res2 = api.get_result_sets(result_sets = [res.result_ID[0]])
     assert type(res2) is pd.core.frame.DataFrame
```

