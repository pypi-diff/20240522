# Comparing `tmp/threedi_schema-0.222.dev1.tar.gz` & `tmp/threedi_schema-0.222.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi_schema-0.222.dev1.tar", last modified: Mon Apr 29 12:47:21 2024, max compression
+gzip compressed data, was "threedi_schema-0.222.dev2.tar", last modified: Mon Apr 29 13:43:40 2024, max compression
```

## Comparing `threedi_schema-0.222.dev1.tar` & `threedi_schema-0.222.dev2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.419800 threedi_schema-0.222.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-29 12:47:21.419800 threedi_schema-0.222.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:47:21.419800 threedi_schema-0.222.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.407801 threedi_schema-0.222.dev1/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.407801 threedi_schema-0.222.dev1/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.407801 threedi_schema-0.222.dev1/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    30963 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.411800 threedi_schema-0.222.dev1/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.411800 threedi_schema-0.222.dev1/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.415800 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0222_upgrade_db_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.415800 threedi_schema-0.222.dev1/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.415800 threedi_schema-0.222.dev1/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_beta_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.415800 threedi_schema-0.222.dev1/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.347011 threedi_schema-0.222.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-29 13:43:40.343011 threedi_schema-0.222.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:43:40.347011 threedi_schema-0.222.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.335011 threedi_schema-0.222.dev2/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.335011 threedi_schema-0.222.dev2/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.339011 threedi_schema-0.222.dev2/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30965 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.339011 threedi_schema-0.222.dev2/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.339011 threedi_schema-0.222.dev2/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.343011 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0222_upgrade_db_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.343011 threedi_schema-0.222.dev2/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.343011 threedi_schema-0.222.dev2/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:35.000000 threedi_schema-0.222.dev2/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-29 13:43:36.000000 threedi_schema-0.222.dev2/threedi_schema/tests/test_beta_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-29 13:43:36.000000 threedi_schema-0.222.dev2/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-29 13:43:36.000000 threedi_schema-0.222.dev2/threedi_schema/tests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-29 13:43:36.000000 threedi_schema-0.222.dev2/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-29 13:43:36.000000 threedi_schema-0.222.dev2/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-29 13:43:36.000000 threedi_schema-0.222.dev2/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:43:40.343011 threedi_schema-0.222.dev2/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-29 13:43:40.000000 threedi_schema-0.222.dev2/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-29 13:43:40.000000 threedi_schema-0.222.dev2/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:43:40.000000 threedi_schema-0.222.dev2/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 13:43:40.000000 threedi_schema-0.222.dev2/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 13:43:40.000000 threedi_schema-0.222.dev2/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 13:43:40.000000 threedi_schema-0.222.dev2/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi_schema-0.222.dev1/CHANGES.rst` & `threedi_schema-0.222.dev2/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/LICENSE` & `threedi_schema-0.222.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/PKG-INFO` & `threedi_schema-0.222.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.222.dev1
+Version: 0.222.dev2
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `threedi_schema-0.222.dev1/README.rst` & `threedi_schema-0.222.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/pyproject.toml` & `threedi_schema-0.222.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/application/schema.py` & `threedi_schema-0.222.dev2/threedi_schema/application/schema.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/application/threedi_database.py` & `threedi_schema-0.222.dev2/threedi_schema/application/threedi_database.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/beta_features.py` & `threedi_schema-0.222.dev2/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/domain/constants.py` & `threedi_schema-0.222.dev2/threedi_schema/domain/constants.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/domain/custom_types.py` & `threedi_schema-0.222.dev2/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/domain/indexes.py` & `threedi_schema-0.222.dev2/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/domain/models.py` & `threedi_schema-0.222.dev2/threedi_schema/domain/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         IntegerEnum(constants.InfiltrationSurfaceOption)
     )
     max_infiltration_volume = Column(Float)
     max_infiltration_volume_file = Column(Text)
 
     # Alias needed for API compatibility
     @property
-    def max_infiltration_volume_file(self):
+    def max_infiltration_capacity_file(self):
         return self.max_infiltration_volume_file
 
 
 class SurfaceParameter(Base):
     __tablename__ = "v2_surface_parameters"
     id = Column(Integer, primary_key=True)
     outflow_delay = Column(Float, nullable=False)
```

### Comparing `threedi_schema-0.222.dev1/threedi_schema/domain/views.py` & `threedi_schema-0.222.dev2/threedi_schema/domain/views.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/infrastructure/spatial_index.py` & `threedi_schema-0.222.dev2/threedi_schema/infrastructure/spatial_index.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/infrastructure/spatialite_versions.py` & `threedi_schema-0.222.dev2/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/infrastructure/views.py` & `threedi_schema-0.222.dev2/threedi_schema/infrastructure/views.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/env.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0200_initial.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0222_upgrade_db_settings.py` & `threedi_schema-0.222.dev2/threedi_schema/migrations/versions/0222_upgrade_db_settings.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/scripts.py` & `threedi_schema-0.222.dev2/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/tests/conftest.py` & `threedi_schema-0.222.dev2/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/tests/test_beta_features.py` & `threedi_schema-0.222.dev2/threedi_schema/tests/test_beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/tests/test_gpkg.py` & `threedi_schema-0.222.dev2/threedi_schema/tests/test_gpkg.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/tests/test_migration.py` & `threedi_schema-0.222.dev2/threedi_schema/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/tests/test_migration_213.py` & `threedi_schema-0.222.dev2/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/tests/test_schema.py` & `threedi_schema-0.222.dev2/threedi_schema/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema/tests/test_spatalite_versions.py` & `threedi_schema-0.222.dev2/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi_schema-0.222.dev1/threedi_schema.egg-info/PKG-INFO` & `threedi_schema-0.222.dev2/threedi_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.222.dev1
+Version: 0.222.dev2
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `threedi_schema-0.222.dev1/threedi_schema.egg-info/SOURCES.txt` & `threedi_schema-0.222.dev2/threedi_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

