# Comparing `tmp/dbt_adapters-1.1.0rc2.tar.gz` & `tmp/dbt_adapters-1.1.1.tar.gz`

## Comparing `dbt_adapters-1.1.0rc2.tar` & `dbt_adapters-1.1.1.tar`

### file list

```diff
@@ -1,154 +1,155 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/__about__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/__init__.py
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/cache.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/capability.py
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/factory.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/py.typed
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/reference_keys.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/utils.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/README.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/__init__.py
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/column.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/connections.py
--rw-r--r--   0        0        0    68352 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/impl.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/meta.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/plugin.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/query_headers.py
--rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/base/relation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/clients/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/clients/jinja.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/contracts/__init__.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/contracts/connection.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/contracts/macros.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/contracts/relation.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/__init__.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/adapter_types.proto
--rw-r--r--   0        0        0    26480 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/adapter_types_pb2.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/base_types.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/logging.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/events/types.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/alias.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/cache.py
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/compilation.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/connection.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/database.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/README.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_validation.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/sql/__init__.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/sql/connections.py
--rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/adapters/sql/impl.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/py.typed
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/dbt_project.yml
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/docs/overview.md
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/show.sql
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/validate_sql.sql
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/etc/statement.sql
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/unique.sql
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/hooks.sql
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view.sql
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/table.sql
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/view.sql
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/clone/clone.sql
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/unit.sql
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/python_model/python.sql
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create.sql
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create_backup.sql
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create_intermediate.sql
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/drop.sql
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/drop_backup.sql
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/rename.sql
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/rename_intermediate.sql
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/replace.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/schema.sql
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/replace.sql
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/create.sql
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/create.sql
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/rename.sql
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/replace.sql
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/cast.sql
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/date_spine.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/generate_series.sql
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/split_part.sql
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/LICENSE
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/README.md
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 dbt_adapters-1.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/__about__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/cache.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/capability.py
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/factory.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/py.typed
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/reference_keys.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/utils.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/README.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/__init__.py
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/column.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/connections.py
+-rw-r--r--   0        0        0    68352 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/impl.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/meta.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/plugin.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/query_headers.py
+-rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/base/relation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/clients/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/clients/jinja.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/contracts/__init__.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/contracts/connection.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/contracts/macros.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/contracts/relation.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/events/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/events/__init__.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/events/adapter_types.proto
+-rw-r--r--   0        0        0    26480 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/events/adapter_types_pb2.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/events/base_types.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/events/logging.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/events/types.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/exceptions/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/exceptions/alias.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/exceptions/cache.py
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/exceptions/compilation.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/exceptions/connection.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/exceptions/database.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/relation_configs/README.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/relation_configs/config_validation.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/sql/__init__.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/sql/connections.py
+-rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/adapters/sql/impl.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/py.typed
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/dbt_project.yml
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/docs/overview.md
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/show.sql
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/timestamps.sql
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/validate_sql.sql
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/etc/statement.sql
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/generic_test_sql/unique.sql
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/hooks.sql
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/materialized_view.sql
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/table.sql
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/view.sql
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/clone/clone.sql
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/seeds/seed.sql
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/tests/unit.sql
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/python_model/python.sql
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/create.sql
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/create_backup.sql
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/create_intermediate.sql
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/drop.sql
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/drop_backup.sql
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/rename.sql
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/rename_intermediate.sql
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/replace.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/schema.sql
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/materialized_view/replace.sql
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/table/create.sql
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/view/create.sql
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/cast.sql
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/date.sql
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/date_spine.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/generate_series.sql
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/README.md
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 dbt_adapters-1.1.1/PKG-INFO
```

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/cache.py` & `dbt_adapters-1.1.1/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/capability.py` & `dbt_adapters-1.1.1/dbt/adapters/capability.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/factory.py` & `dbt_adapters-1.1.1/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/protocol.py` & `dbt_adapters-1.1.1/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/reference_keys.py` & `dbt_adapters-1.1.1/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/utils.py` & `dbt_adapters-1.1.1/dbt/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/base/README.md` & `dbt_adapters-1.1.1/dbt/adapters/base/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/base/column.py` & `dbt_adapters-1.1.1/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/base/connections.py` & `dbt_adapters-1.1.1/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/base/impl.py` & `dbt_adapters-1.1.1/dbt/adapters/base/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/base/meta.py` & `dbt_adapters-1.1.1/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/base/plugin.py` & `dbt_adapters-1.1.1/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/base/query_headers.py` & `dbt_adapters-1.1.1/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/base/relation.py` & `dbt_adapters-1.1.1/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/clients/jinja.py` & `dbt_adapters-1.1.1/dbt/adapters/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/contracts/connection.py` & `dbt_adapters-1.1.1/dbt/adapters/contracts/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         data = cls.translate_aliases(data)
         return data
 
     @classmethod
     def translate_aliases(cls, kwargs: Dict[str, Any], recurse: bool = False) -> Dict[str, Any]:
         return translate_aliases(kwargs, cls._ALIASES, recurse)
 
-    def __post_serialize__(self, dct):
+    def __post_serialize__(self, dct: Dict, context: Optional[Dict] = None):
         # no super() -- do we need it?
         if self._ALIASES:
             dct.update(
                 {
                     new_name: dct[canonical_name]
                     for new_name, canonical_name in self._ALIASES.items()
                     if canonical_name in dct
```

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/contracts/relation.py` & `dbt_adapters-1.1.1/dbt/adapters/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/events/README.md` & `dbt_adapters-1.1.1/dbt/adapters/events/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/events/adapter_types.proto` & `dbt_adapters-1.1.1/dbt/adapters/events/adapter_types.proto`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/events/adapter_types_pb2.py` & `dbt_adapters-1.1.1/dbt/adapters/events/adapter_types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/events/base_types.py` & `dbt_adapters-1.1.1/dbt/adapters/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/events/logging.py` & `dbt_adapters-1.1.1/dbt/adapters/events/logging.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/events/types.py` & `dbt_adapters-1.1.1/dbt/adapters/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/__init__.py` & `dbt_adapters-1.1.1/dbt/adapters/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/alias.py` & `dbt_adapters-1.1.1/dbt/adapters/exceptions/alias.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/cache.py` & `dbt_adapters-1.1.1/dbt/adapters/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/compilation.py` & `dbt_adapters-1.1.1/dbt/adapters/exceptions/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/exceptions/database.py` & `dbt_adapters-1.1.1/dbt/adapters/exceptions/database.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/README.md` & `dbt_adapters-1.1.1/dbt/adapters/relation_configs/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_base.py` & `dbt_adapters-1.1.1/dbt/adapters/relation_configs/config_base.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_change.py` & `dbt_adapters-1.1.1/dbt/adapters/relation_configs/config_change.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/relation_configs/config_validation.py` & `dbt_adapters-1.1.1/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/sql/connections.py` & `dbt_adapters-1.1.1/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/adapters/sql/impl.py` & `dbt_adapters-1.1.1/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/docs/overview.md` & `dbt_adapters-1.1.1/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/columns.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/relation.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/schema.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/show.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/show.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/etc/datetime.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/etc/statement.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/configs.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/materialized_view.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/table.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/view.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/clone/clone.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/clone/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/materializations/tests/unit.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/materializations/tests/unit.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/python_model/python.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create_backup.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/create_backup.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/create_intermediate.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/create_intermediate.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/drop.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/rename.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/rename.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/replace.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/alter.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/materialized_view/drop.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/materialized_view/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/table/create.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/create.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/relations/view/replace.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/relations/view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/data_types.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/date_spine.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/generate_series.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/generate_series.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/listagg.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/macros/utils/split_part.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/dbt/include/global_project/tests/generic/builtin.sql` & `dbt_adapters-1.1.1/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/.gitignore` & `dbt_adapters-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/LICENSE` & `dbt_adapters-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/README.md` & `dbt_adapters-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/pyproject.toml` & `dbt_adapters-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.1.0rc2/PKG-INFO` & `dbt_adapters-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-adapters
-Version: 1.1.0rc2
+Version: 1.1.1
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-adapters
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-adapters.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-adapters/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-adapters/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
```

