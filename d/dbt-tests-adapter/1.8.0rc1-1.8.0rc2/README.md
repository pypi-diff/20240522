# Comparing `tmp/dbt_tests_adapter-1.8.0rc1.tar.gz` & `tmp/dbt_tests_adapter-1.8.0rc2.tar.gz`

## Comparing `dbt_tests_adapter-1.8.0rc1.tar` & `dbt_tests_adapter-1.8.0rc2.tar`

### file list

```diff
@@ -1,158 +1,160 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/__about__.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/aliases/fixtures.py
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/aliases/test_aliases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/__init__.py
--rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/expected_catalog.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/files.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_adapter_methods.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_base.py
--rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_docs_generate.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_empty.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_ephemeral.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_generic_tests.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_incremental.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_singular_tests.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_snapshot_check_cols.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_snapshot_timestamp.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_table_materialization.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_validate_connection.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/caching/test_caching.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/catalog/files.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/catalog/relation_types.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/column_types/fixtures.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/column_types/test_column_types.py
--rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/concurrency/test_concurrency.py
--rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/constraints/fixtures.py
--rw-r--r--   0        0        0    18494 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/constraints/test_constraints.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_clone/fixtures.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_clone/test_dbt_clone.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_show/fixtures.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_show/test_dbt_show.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/empty/test_empty.py
--rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/ephemeral/test_ephemeral.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/base_grants.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_incremental_grants.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_invalid_grants.py
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_model_grants.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_seed_grants.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_snapshot_grants.py
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/hooks/fixtures.py
--rw-r--r--   0        0        0    16029 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/hooks/test_model_hooks.py
--rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/hooks/test_run_hooks.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/hooks/data/seed_model.sql
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/hooks/data/seed_run.sql
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/fixtures.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/test_incremental_predicates.py
--rw-r--r--   0        0        0    17895 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/test_incremental_unique_id.py
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/materialized_view/basic.py
--rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/materialized_view/changes.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/materialized_view/files.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/persist_docs/fixtures.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/persist_docs/test_persist_docs.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/python_model/test_python_model.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/python_model/test_spark.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/query_comment/fixtures.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/query_comment/test_query_comment.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/relations/test_changing_relation_type.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/relations/test_dropping_schema_named.py
--rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_copy/fixtures.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_copy/test_simple_copy.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/fixtures.py
--rw-r--r--   0        0        0    33348 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/seed_bom.csv
--rw-r--r--   0        0        0   111485 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/seeds.py
--rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/test_seed.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/test_seed_type_override.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_snapshot/common.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_snapshot/seeds.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_snapshot/snapshots.py
--rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_snapshot/test_snapshot.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/store_test_failures_tests/_files.py
--rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/store_test_failures_tests/basic.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/store_test_failures_tests/fixtures.py
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/unit_testing/test_case_insensitivity.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/unit_testing/test_invalid_input.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/unit_testing/test_types.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/base_array_utils.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/base_utils.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_any_value.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_array_append.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_array_concat.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_array_construct.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_bool_or.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_cast.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_concat.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_date_spine.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_date_trunc.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_dateadd.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_datediff.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_equals.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_except.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_generate_series.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_get_intervals_between.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_get_powers_of_two.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_hash.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_intersect.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_last_day.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_length.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_listagg.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_null_compare.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_position.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_replace.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_right.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_safe_cast.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_split_part.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_string_literal.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_any_value.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_array_append.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_array_concat.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_array_construct.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_bool_or.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_cast.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_cast_bool_to_text.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_concat.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_current_timestamp.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_date_spine.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_date_trunc.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_dateadd.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_datediff.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_equals.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_escape_single_quotes.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_except.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_generate_series.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_get_intervals_between.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_get_powers_of_two.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_hash.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_intersect.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_last_day.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_length.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_listagg.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_null_compare.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_position.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_replace.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_right.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_safe_cast.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_split_part.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_string_literal.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_timestamps.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_validate_sql.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_boolean.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_float.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_int.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_numeric.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_string.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/.gitignore
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/README.md
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/__about__.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/aliases/fixtures.py
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/aliases/test_aliases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/__init__.py
+-rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/expected_catalog.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/files.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_adapter_methods.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_base.py
+-rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_docs_generate.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_empty.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_ephemeral.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_generic_tests.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_incremental.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_singular_tests.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_snapshot_check_cols.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_snapshot_timestamp.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_table_materialization.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_validate_connection.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/caching/test_caching.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/catalog/files.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/catalog/relation_types.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/column_types/fixtures.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/column_types/test_column_types.py
+-rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/concurrency/test_concurrency.py
+-rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/constraints/fixtures.py
+-rw-r--r--   0        0        0    18494 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/constraints/test_constraints.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_clone/fixtures.py
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_clone/test_dbt_clone.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_show/fixtures.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_show/test_dbt_show.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/empty/test_empty.py
+-rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/ephemeral/test_ephemeral.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/base_grants.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_incremental_grants.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_invalid_grants.py
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_model_grants.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_seed_grants.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_snapshot_grants.py
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/hooks/fixtures.py
+-rw-r--r--   0        0        0    16029 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/hooks/test_model_hooks.py
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/hooks/test_run_hooks.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/hooks/data/seed_model.sql
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/hooks/data/seed_run.sql
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/fixtures.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/test_incremental_predicates.py
+-rw-r--r--   0        0        0    17895 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/test_incremental_unique_id.py
+-rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/materialized_view/basic.py
+-rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/materialized_view/changes.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/materialized_view/files.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/persist_docs/fixtures.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/persist_docs/test_persist_docs.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/python_model/test_python_model.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/python_model/test_spark.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/query_comment/fixtures.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/query_comment/test_query_comment.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/relations/test_changing_relation_type.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/relations/test_dropping_schema_named.py
+-rw-r--r--   0        0        0    19870 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_copy/fixtures.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_copy/test_simple_copy.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/fixtures.py
+-rw-r--r--   0        0        0    33348 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/seed_bom.csv
+-rw-r--r--   0        0        0   111485 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/seeds.py
+-rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/test_seed.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/test_seed_type_override.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_snapshot/common.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_snapshot/seeds.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_snapshot/snapshots.py
+-rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_snapshot/test_snapshot.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/store_test_failures_tests/_files.py
+-rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/store_test_failures_tests/basic.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/store_test_failures_tests/fixtures.py
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/unit_testing/test_case_insensitivity.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/unit_testing/test_invalid_input.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/unit_testing/test_types.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/base_array_utils.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/base_utils.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_any_value.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_array_append.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_array_concat.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_array_construct.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_bool_or.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_cast.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_concat.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_date.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_date_spine.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_date_trunc.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_dateadd.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_datediff.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_equals.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_except.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_generate_series.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_get_intervals_between.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_get_powers_of_two.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_hash.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_intersect.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_last_day.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_length.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_listagg.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_null_compare.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_position.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_replace.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_right.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_safe_cast.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_split_part.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_string_literal.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_any_value.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_array_append.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_array_concat.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_array_construct.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_bool_or.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_cast.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_cast_bool_to_text.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_concat.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_current_timestamp.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_date.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_date_spine.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_date_trunc.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_dateadd.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_datediff.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_equals.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_escape_single_quotes.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_except.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_generate_series.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_get_intervals_between.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_get_powers_of_two.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_hash.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_intersect.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_last_day.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_length.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_listagg.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_null_compare.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_position.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_replace.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_right.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_safe_cast.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_split_part.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_string_literal.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_timestamps.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_validate_sql.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_boolean.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_float.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_int.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_numeric.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_string.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/.gitignore
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/README.md
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 dbt_tests_adapter-1.8.0rc2/PKG-INFO
```

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/aliases/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/aliases/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/aliases/test_aliases.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/aliases/test_aliases.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/expected_catalog.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/files.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/files.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_adapter_methods.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_adapter_methods.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_base.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_base.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_docs_generate.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_empty.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_ephemeral.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_generic_tests.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_incremental.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_singular_tests.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_singular_tests.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_snapshot_check_cols.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_snapshot_check_cols.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_snapshot_timestamp.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_snapshot_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/basic/test_table_materialization.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/basic/test_table_materialization.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/caching/test_caching.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/caching/test_caching.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/catalog/relation_types.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/catalog/relation_types.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/column_types/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/column_types/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/column_types/test_column_types.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/column_types/test_column_types.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/concurrency/test_concurrency.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/constraints/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/constraints/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/constraints/test_constraints.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_clone/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_clone/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_clone/test_dbt_clone.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_clone/test_dbt_clone.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,25 +69,22 @@
         shutil.copyfile(
             f"{project_root}/target/manifest.json", f"{project_root}/state/manifest.json"
         )
 
     def run_and_save_state(self, project_root, with_snapshot=False):
         results = run_dbt(["seed"])
         assert len(results) == 1
-        assert not any(r.node.deferred for r in results)
         results = run_dbt(["run"])
         assert len(results) == 2
-        assert not any(r.node.deferred for r in results)
         results = run_dbt(["test"])
         assert len(results) == 2
 
         if with_snapshot:
             results = run_dbt(["snapshot"])
             assert len(results) == 1
-            assert not any(r.node.deferred for r in results)
 
         # copy files
         self.copy_state(project_root)
 
 
 # -- Below we define base classes for tests you import the one based on if your adapter uses dbt clone or not --
 class BaseClonePossible(BaseClone):
@@ -210,14 +207,15 @@
 class BaseCloneSameTargetAndState(BaseClone):
     def test_clone_same_target_and_state(self, project, unique_schema, other_schema):
         project.create_test_schema(other_schema)
         self.run_and_save_state(project.project_root)
 
         clone_args = [
             "clone",
+            "--defer",
             "--state",
             "target",
         ]
 
         results, output = run_dbt_and_capture(clone_args, expect_pass=False)
         assert "Warning: The state and target directories are the same: 'target'" in output
```

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_debug/test_dbt_debug.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_debug/test_dbt_debug.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_show/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_show/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/dbt_show/test_dbt_show.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/dbt_show/test_dbt_show.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/empty/test_empty.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/empty/test_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/ephemeral/test_ephemeral.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/ephemeral/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/base_grants.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/base_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_incremental_grants.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_incremental_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_invalid_grants.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_invalid_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_model_grants.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_model_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_seed_grants.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_seed_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/grants/test_snapshot_grants.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/grants/test_snapshot_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/hooks/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/hooks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/hooks/test_model_hooks.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/hooks/test_model_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/hooks/test_run_hooks.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/hooks/test_run_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/test_incremental_predicates.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/incremental/test_incremental_unique_id.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/incremental/test_incremental_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/materialized_view/basic.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/materialized_view/basic.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/materialized_view/changes.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/materialized_view/changes.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/persist_docs/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/persist_docs/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/persist_docs/test_persist_docs.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/persist_docs/test_persist_docs.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/python_model/test_python_model.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/python_model/test_python_model.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/python_model/test_spark.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/python_model/test_spark.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/query_comment/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/query_comment/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/query_comment/test_query_comment.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/query_comment/test_query_comment.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/relations/test_changing_relation_type.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/relations/test_changing_relation_type.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/relations/test_dropping_schema_named.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/relations/test_dropping_schema_named.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_copy/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_copy/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_copy/test_copy_uppercase.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_copy/test_copy_uppercase.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_copy/test_simple_copy.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_copy/test_simple_copy.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/seed_bom.csv` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/seed_bom.csv`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/seeds.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/test_seed.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/test_seed.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_seed/test_seed_type_override.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_seed/test_seed_type_override.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_snapshot/common.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_snapshot/common.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_snapshot/seeds.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_snapshot/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_snapshot/snapshots.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_snapshot/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/simple_snapshot/test_snapshot.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/simple_snapshot/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/store_test_failures_tests/_files.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/store_test_failures_tests/_files.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/store_test_failures_tests/basic.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/store_test_failures_tests/basic.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/store_test_failures_tests/fixtures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/store_test_failures_tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/unit_testing/test_case_insensitivity.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/unit_testing/test_case_insensitivity.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/unit_testing/test_invalid_input.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/unit_testing/test_invalid_input.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/unit_testing/test_types.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/unit_testing/test_types.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/base_array_utils.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/base_array_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/base_utils.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_any_value.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_array_concat.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_bool_or.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_concat.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_concat.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_date_spine.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_date_spine.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_date_trunc.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_dateadd.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_datediff.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_equals.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_equals.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_escape_single_quotes.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_except.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_except.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_generate_series.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_generate_series.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_get_intervals_between.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_get_intervals_between.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_get_powers_of_two.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_get_powers_of_two.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_hash.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_hash.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_intersect.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_last_day.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_listagg.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_null_compare.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_null_compare.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_position.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_position.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_replace.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_replace.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_right.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_right.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_split_part.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/fixture_string_literal.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/fixture_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_any_value.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_bool_or.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_cast.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_cast.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_cast_bool_to_text.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_cast_bool_to_text.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_concat.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_concat.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_current_timestamp.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_current_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_date_trunc.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_dateadd.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_datediff.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_equals.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_equals.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_escape_single_quotes.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_except.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_except.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_generate_series.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_generate_series.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_get_intervals_between.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_get_intervals_between.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_get_powers_of_two.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_get_powers_of_two.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_hash.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_intersect.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_last_day.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_length.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_length.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_listagg.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_null_compare.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_null_compare.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_position.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_position.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_replace.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_replace.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_right.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_right.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_safe_cast.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_safe_cast.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_split_part.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_string_literal.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_timestamps.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/test_validate_sql.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/test_validate_sql.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/base_data_type_macro.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/base_data_type_macro.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_bigint.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_boolean.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_boolean.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_float.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_float.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_int.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_int.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_numeric.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_numeric.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_string.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_string.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/dbt/tests/adapter/utils/data_types/test_type_timestamp.py` & `dbt_tests_adapter-1.8.0rc2/dbt/tests/adapter/utils/data_types/test_type_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/.gitignore` & `dbt_tests_adapter-1.8.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/README.md` & `dbt_tests_adapter-1.8.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_tests_adapter-1.8.0rc1/pyproject.toml` & `dbt_tests_adapter-1.8.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     # TODO: remove `dbt-core` dependency
-    "dbt-core>=1.8.0a1,<1.9.0",
+    "dbt-core>=1.8.0a1",
     # `dbt-tests-adapter` will ultimately depend on the packages below
     # `dbt-tests-adapter` temporarily uses `dbt-core` for a dbt runner
     # `dbt-core` takes the packages below as dependencies, so they are unpinned to avoid conflicts
     "dbt-adapters",
     "pyyaml",
 ]
```

### Comparing `dbt_tests_adapter-1.8.0rc1/PKG-INFO` & `dbt_tests_adapter-1.8.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-tests-adapter
-Version: 1.8.0rc1
+Version: 1.8.0rc2
 Summary: The set of reusable tests and test fixtures used to test common functionality
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-adapters
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-adapters.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-adapters/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-adapters/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Requires-Dist: dbt-adapters
-Requires-Dist: dbt-core<1.9.0,>=1.8.0a1
+Requires-Dist: dbt-core>=1.8.0a1
 Requires-Dist: pyyaml
 Provides-Extra: build
 Requires-Dist: check-wheel-contents; extra == 'build'
 Requires-Dist: twine; extra == 'build'
 Requires-Dist: wheel; extra == 'build'
 Description-Content-Type: text/markdown
```

