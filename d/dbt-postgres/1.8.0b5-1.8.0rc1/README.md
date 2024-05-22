# Comparing `tmp/dbt_postgres-1.8.0b5.tar.gz` & `tmp/dbt_postgres-1.8.0rc1.tar.gz`

## Comparing `dbt_postgres-1.8.0b5.tar` & `dbt_postgres-1.8.0rc1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/__version__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/column.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/connections.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/impl.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/constants.py
--rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/index.py
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/materialized_view.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/dbt_project.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/profile_template.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/sample_profiles.yml
--rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/adapters.sql
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/catalog.sql
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations.sql
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/timestamps.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/describe.sql
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/view/rename.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/view/replace.sql
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/any_value.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/dateadd.sql
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/datediff.sql
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/last_day.sql
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/listagg.sql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/split_part.sql
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/LICENSE
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/README.md
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/pyproject.toml
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b5/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/__version__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/column.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/connections.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/impl.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/relation.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/relation_configs/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/relation_configs/constants.py
+-rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/relation_configs/index.py
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/adapters/postgres/relation_configs/materialized_view.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/dbt_project.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/profile_template.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/sample_profiles.yml
+-rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/adapters.sql
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/catalog.sql
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations.sql
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/timestamps.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/materialized_view/describe.sql
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/any_value.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/LICENSE
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/README.md
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0rc1/PKG-INFO
```

### Comparing `dbt_postgres-1.8.0b5/dbt/adapters/postgres/connections.py` & `dbt_postgres-1.8.0rc1/dbt/adapters/postgres/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/adapters/postgres/impl.py` & `dbt_postgres-1.8.0rc1/dbt/adapters/postgres/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation.py` & `dbt_postgres-1.8.0rc1/dbt/adapters/postgres/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/index.py` & `dbt_postgres-1.8.0rc1/dbt/adapters/postgres/relation_configs/index.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/adapters/postgres/relation_configs/materialized_view.py` & `dbt_postgres-1.8.0rc1/dbt/adapters/postgres/relation_configs/materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/adapters.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/catalog.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/timestamps.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/materializations/snapshot_merge.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/materialized_view/alter.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/relations/table/replace.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/relations/table/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/datediff.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/dbt/include/postgres/macros/utils/listagg.sql` & `dbt_postgres-1.8.0rc1/dbt/include/postgres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/.gitignore` & `dbt_postgres-1.8.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/LICENSE` & `dbt_postgres-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/README.md` & `dbt_postgres-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/pyproject.toml` & `dbt_postgres-1.8.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b5/PKG-INFO` & `dbt_postgres-1.8.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-postgres
-Version: 1.8.0b5
+Version: 1.8.0rc1
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-postgres
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-postgres.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-postgres/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-postgres/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: dbt-postgres Version: 1.8.0b5 Summary: The set of
+Metadata-Version: 2.3 Name: dbt-postgres Version: 1.8.0rc1 Summary: The set of
 adapter protocols and base functionality that supports integration with dbt-
 core Project-URL: Homepage, https://github.com/dbt-labs/dbt-postgres Project-
 URL: Documentation, https://docs.getdbt.com Project-URL: Repository, https://
 github.com/dbt-labs/dbt-postgres.git Project-URL: Issues, https://github.com/
 dbt-labs/dbt-postgres/issues Project-URL: Changelog, https://github.com/dbt-
 labs/dbt-postgres/blob/main/CHANGELOG.md Author-email: dbt Labs
 dbtlabs.com> Maintainer-email: dbt Labs
```

