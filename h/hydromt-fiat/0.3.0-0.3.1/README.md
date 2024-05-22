# Comparing `tmp/hydromt_fiat-0.3.0.tar.gz` & `tmp/hydromt_fiat-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromt_fiat-0.3.0.tar", last modified: Tue May 14 14:43:28 2024, max compression
+gzip compressed data, was "hydromt_fiat-0.3.1.tar", last modified: Tue May 21 15:16:36 2024, max compression
```

## Comparing `hydromt_fiat-0.3.0.tar` & `hydromt_fiat-0.3.1.tar`

### file list

```diff
@@ -1,77 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:43:28.081828 hydromt_fiat-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-14 14:43:28.081828 hydromt_fiat-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:43:28.069828 hydromt_fiat-0.3.0/hydromt_fiat/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:43:28.073828 hydromt_fiat-0.3.0/hydromt_fiat/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/dbs_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/exposure_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/hydromt_fiat_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/model_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/svi_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/api/vulnerability_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:43:28.073828 hydromt_fiat-0.3.0/hydromt_fiat/data_apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/data_apis/national_structure_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/data_apis/open_street_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    44888 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/fiat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:43:28.073828 hydromt_fiat-0.3.0/hydromt_fiat/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:43:28.073828 hydromt_fiat-0.3.0/hydromt_fiat/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/aggregation_areas.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/aggregation_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/building_footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/damage_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/equity_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)    22439 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/exposure_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)    73065 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/exposure_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/gis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/hazard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/roads.py
--rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/social_vulnerability_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26270 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/hydromt_fiat/workflows/vulnerability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:43:28.077829 hydromt_fiat-0.3.0/hydromt_fiat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-14 14:43:28.000000 hydromt_fiat-0.3.0/hydromt_fiat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-14 14:43:28.000000 hydromt_fiat-0.3.0/hydromt_fiat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:43:28.000000 hydromt_fiat-0.3.0/hydromt_fiat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 14:43:28.000000 hydromt_fiat-0.3.0/hydromt_fiat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:42:58.000000 hydromt_fiat-0.3.0/hydromt_fiat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-14 14:43:28.000000 hydromt_fiat-0.3.0/hydromt_fiat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 14:43:28.000000 hydromt_fiat-0.3.0/hydromt_fiat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:43:28.081828 hydromt_fiat-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:43:28.077829 hydromt_fiat-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_SVI_exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_aggregation_areas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_building_footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_create_step_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_equity_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_exposure_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_ground_elevation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_integrations_hazard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_raise_ground_floor_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_read_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_roads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_setup_new_composite_areas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_setup_new_composite_areas_ground_elevation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_truncate_damage_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_update_ground_floor_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_update_max_potential_damage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_update_max_potential_damage_user_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_vulnerability.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_vulnerability_exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_vulnerability_exposure_add_to_data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_vulnerability_exposure_global_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_vulnerability_expousure_with_user_dem_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-14 14:42:15.000000 hydromt_fiat-0.3.0/tests/test_vulnerability_from_csvs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.880589 hydromt_fiat-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-21 15:16:36.880589 hydromt_fiat-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.864589 hydromt_fiat-0.3.1/hydromt_fiat/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.864589 hydromt_fiat-0.3.1/hydromt_fiat/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.864589 hydromt_fiat-0.3.1/hydromt_fiat/data/attribute_linking/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/attribute_linking/NSI_attributes_to_FIAT.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.860589 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.860589 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/erosion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.864589 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/erosion/ft/
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/erosion/ft/GL000.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.864589 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/erosion/inch/
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/erosion/inch/GL000.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.864589 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/erosion/m/
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/erosion/m/GL000.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.868589 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/flooding/
+-rw-r--r--   0 runner    (1001) docker     (127)   192455 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/flooding/AllDDF_HAZUS.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)   265503 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/flooding/Hazus_IWR_curves.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   175880 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/flooding/JRC_damage_functions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   461588 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/damage_functions/flooding/JRC_damage_functions_calculation.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.868589 hydromt_fiat-0.3.1/hydromt_fiat/data/growth_scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)   473575 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/growth_scenarios/global_gdp(ppp).xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)   293976 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/growth_scenarios/global_pop.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.872589 hydromt_fiat-0.3.1/hydromt_fiat/data/max_potential_damages/
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/max_potential_damages/JRC_base_damage_values.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/max_potential_damages/damage_values_fema_hazus-inventory-technical-manual-4.2.3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/max_potential_damages/us_road_damage.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.872589 hydromt_fiat-0.3.1/hydromt_fiat/data/new_composite_areas/
+-rw-r--r--   0 runner    (1001) docker     (127)    98304 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/new_composite_areas/new_development_area_test.gpkg
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/new_composite_areas/reference_groundHeight_test.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/new_composite_areas/reference_groundHeight_test.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/new_composite_areas/reference_groundHeight_test.prj
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/new_composite_areas/reference_groundHeight_test.qix
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/new_composite_areas/reference_groundHeight_test.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/new_composite_areas/reference_groundHeight_test.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.872589 hydromt_fiat-0.3.1/hydromt_fiat/data/social_vulnerability/
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/social_vulnerability/census_vulnerability_data_codebook.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/social_vulnerability/census_vulnerability_data_codebook.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)   119203 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/social_vulnerability/us_states_counties.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.872589 hydromt_fiat-0.3.1/hydromt_fiat/data/vulnerability_linking/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/vulnerability_linking/JRC_damage_functions_linking.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/vulnerability_linking/default_hazus_iwr_curve_linking.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/data/vulnerability_linking/hazus_iwr_occupancy_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    47110 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/fiat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/hydromt_fiat/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.876589 hydromt_fiat-0.3.1/hydromt_fiat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-21 15:16:36.000000 hydromt_fiat-0.3.1/hydromt_fiat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-21 15:16:36.000000 hydromt_fiat-0.3.1/hydromt_fiat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:16:36.000000 hydromt_fiat-0.3.1/hydromt_fiat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 15:16:36.000000 hydromt_fiat-0.3.1/hydromt_fiat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:16:05.000000 hydromt_fiat-0.3.1/hydromt_fiat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-21 15:16:36.000000 hydromt_fiat-0.3.1/hydromt_fiat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 15:16:36.000000 hydromt_fiat-0.3.1/hydromt_fiat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:16:36.880589 hydromt_fiat-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:16:36.876589 hydromt_fiat-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_SVI_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_aggregation_areas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_building_footprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_create_step_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_equity_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_exposure_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_ground_elevation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_integrations_hazard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_raise_ground_floor_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_roads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_setup_new_composite_areas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_setup_new_composite_areas_ground_elevation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_truncate_damage_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_update_ground_floor_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_update_max_potential_damage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_update_max_potential_damage_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_vulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_vulnerability_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_vulnerability_exposure_add_to_data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_vulnerability_exposure_global_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_vulnerability_expousure_with_user_dem_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-21 15:15:21.000000 hydromt_fiat-0.3.1/tests/test_vulnerability_from_csvs.py
```

### Comparing `hydromt_fiat-0.3.0/LICENSE` & `hydromt_fiat-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/PKG-INFO` & `hydromt_fiat-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydromt_fiat
-Version: 0.3.0
+Version: 0.3.1
 Author-email: Dirk Eilander <dirk.eilander@deltares.nl>, Frederique de Groen <frederique.degroen@deltares.nl>, Mario Fuentes Monjaraz <mario.fuentesmonjaraz@deltares.nl>, Luis Rodriguez Galvez <luis.rodriguez@deltares.nl>, Lieke Meijer <lieke.meijer@deltares.nl>, Sarah Rautenbach <sarah.rautenbach@deltares.nl>
 Project-URL: Documentation, https://deltares.github.io/hydromt_fiat/
 Project-URL: Source, https://github.com/Deltares/hydromt_fiat
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `hydromt_fiat-0.3.0/README.rst` & `hydromt_fiat-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/hydromt_fiat/config.py` & `hydromt_fiat-0.3.1/hydromt_fiat/config.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/hydromt_fiat/fiat.py` & `hydromt_fiat-0.3.1/hydromt_fiat/fiat.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         unit: str,
         occupancy_attr: Union[str, None] = None,
         occupancy_object_type: Union[str, List[str]] = None,
         extraction_method: str = "centroid",
         damage_types: List[str] = ["structure", "content"], 
         damage_unit: str = "$", 
         country: Union[str, None] = None,
-        ground_elevation_file: Union[int, float, str, Path, None] = None,
+        ground_elevation_file: Union[int, float, str, Path, None] = None,     
     ) -> None:
         """Setup building exposure (vector) data for Delft-FIAT.
 
         Parameters
         ----------
         asset_locations : Union[str, Path]
             The path to the vector data (points or polygons) that can be used for the
@@ -335,21 +335,21 @@
         # In case the unit is passed as a pydantic value get the string
         if hasattr(unit, "value"):
             unit = unit.value
         self.exposure = ExposureVector(self.data_catalog, self.logger, self.region, unit=unit, damage_unit=damage_unit)
 
         if asset_locations == max_potential_damage:
             # The source for the asset locations, occupancy type and maximum potential
-            # damage is the same, use one source to create the exposure data.
+            # damage is the same, use one source to create the exposure data.            
             self.exposure.setup_buildings_from_single_source(
-                asset_locations,
-                ground_floor_height,
-                extraction_method,
-                ground_elevation_file=ground_elevation_file,
-            )
+                    asset_locations,
+                    ground_floor_height,
+                    extraction_method,
+                    ground_elevation_file=ground_elevation_file,
+                )
 
         else:
             # The source for the asset locations, occupancy type and maximum potential
             # damage is different, use three sources to create the exposure data.
             self.exposure.setup_buildings_from_multiple_sources(
                 asset_locations,
                 occupancy_type,
@@ -372,15 +372,15 @@
         # Link the damage functions to assets
         try:
             assert not self.vf_ids_and_linking_df.empty
         except AssertionError:
             logging.error(
                 "Please call the 'setup_vulnerability' function before "
                 "the 'setup_exposure_buildings' function. Error message: {e}"
-            )
+            )        
         self.exposure.link_exposure_vulnerability(
             self.vf_ids_and_linking_df, damage_types
         )
         self.exposure.check_required_columns()
 
         # Update the other config settings
         self.set_config("exposure.csv.file", "./exposure/exposure.csv")
@@ -843,14 +843,61 @@
         else:
             the_type = type(aggregation_area_fn)
         if the_type != gpd.GeoDataFrame:
             # This copies data from one location to the root folder for the FIAT
             # model, only use user-input data here (not the census blocks)
             self.additional_attributes_fn = aggregation_area_fn
 
+    def setup_classification(
+        self,
+        source = Union[List[str], str, Path, List[Path]],
+        attribute = Union[List[str], str],
+        type_add = Union[List[str], str],
+        old_values= Union[List[str], str],
+        new_values= Union[List[str], str],
+        damage_types = Union[List[str], str],
+        remove_object_type = bool
+        
+    ):
+        """_summary_
+
+        Parameters
+        ----------
+        source : Union[List[str], List[Path], str, Path]
+            Path(s) to the user classification file.
+        attribute : Union[List[str], str]
+            Name of the column of the user data 
+       type_add : Union[List[str], str]
+            Name of the attribute the user wants to update. Primary or Secondary
+        old_values : Union[List[str], List[Path], str, Path]
+            Name of the default (NSI) exposure classification
+        new_values : Union[List[str], str]
+            Name of the user exposure classification.
+        exposure_linking_table : Union[List[str], str]
+            Path(s) to the new exposure linking table(s).
+        damage_types : Union[List[str], str]
+            "structure"or/and "content"
+        remove_object_type: bool
+            True if Primary/Secondary Object Type from old gdf should be removed in case the object type category changed completely eg. from RES to COM.
+            E.g. Primary Object Type holds old data (RES) and Secondary was updated with new data (COM2). 
+        """
+
+        self.exposure.setup_occupancy_type(source, attribute, type_add)
+
+        # Drop Object Type that has not been updated. 
+        
+        if remove_object_type:
+            if type_add == "Primary Object Type":
+                self.exposure.exposure_db.drop("Secondary Object Type", axis =1 , inplace = True)
+            else:
+                self.exposure.exposure_db.drop("Primary Object Type", axis =1 , inplace = True) 
+        linking_table_new = self.exposure.update_user_linking_table(old_values,new_values, self.vf_ids_and_linking_df)
+        self.vf_ids_and_linking_df = linking_table_new
+        self.exposure.link_exposure_vulnerability(linking_table_new, ["structure", "content"])
+
     def setup_building_footprint(
         self,
         building_footprint_fn: Union[str, Path],
         attribute_name: str,
     ):
         """_summary_
```

### Comparing `hydromt_fiat-0.3.0/hydromt_fiat/validation.py` & `hydromt_fiat-0.3.1/hydromt_fiat/validation.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/hydromt_fiat.egg-info/PKG-INFO` & `hydromt_fiat-0.3.1/hydromt_fiat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydromt_fiat
-Version: 0.3.0
+Version: 0.3.1
 Author-email: Dirk Eilander <dirk.eilander@deltares.nl>, Frederique de Groen <frederique.degroen@deltares.nl>, Mario Fuentes Monjaraz <mario.fuentesmonjaraz@deltares.nl>, Luis Rodriguez Galvez <luis.rodriguez@deltares.nl>, Lieke Meijer <lieke.meijer@deltares.nl>, Sarah Rautenbach <sarah.rautenbach@deltares.nl>
 Project-URL: Documentation, https://deltares.github.io/hydromt_fiat/
 Project-URL: Source, https://github.com/Deltares/hydromt_fiat
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `hydromt_fiat-0.3.0/pyproject.toml` & `hydromt_fiat-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,20 @@
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.dynamic]
 version = { attr = "hydromt_fiat.__version__" }
 
 [tool.setuptools.packages.find]
-include = ["hydromt_fiat", "hydromt_fiat.*"]
+where = ["."]
+include = ["hydromt_fiat"]
+exclude = ["tests", "examples", "envs", "docs", "notebooks"]
+
+[tool.setuptools.package-data]
+"*" = ["*.*"]
 
 [project.optional-dependencies]
 test = [
 	"testpath",
 	"responses",
 	"pytest>=2.7.3",
 	"pytest-cov",
```

### Comparing `hydromt_fiat-0.3.0/tests/test_SVI_exposure.py` & `hydromt_fiat-0.3.1/tests/test_SVI_exposure.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_aggregation_areas.py` & `hydromt_fiat-0.3.1/tests/test_aggregation_areas.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_building_footprints.py` & `hydromt_fiat-0.3.1/tests/test_building_footprints.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_create_step_function.py` & `hydromt_fiat-0.3.1/tests/test_create_step_function.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_equity_data.py` & `hydromt_fiat-0.3.1/tests/test_equity_data.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_exposure_api.py` & `hydromt_fiat-0.3.1/tests/test_exposure_api.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_ground_elevation.py` & `hydromt_fiat-0.3.1/tests/test_ground_elevation.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_integration.py` & `hydromt_fiat-0.3.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_integrations_hazard.py` & `hydromt_fiat-0.3.1/tests/test_integrations_hazard.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_raise_ground_floor_height.py` & `hydromt_fiat-0.3.1/tests/test_raise_ground_floor_height.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_read_write.py` & `hydromt_fiat-0.3.1/tests/test_read_write.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_reader.py` & `hydromt_fiat-0.3.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_roads.py` & `hydromt_fiat-0.3.1/tests/test_roads.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_setup_new_composite_areas.py` & `hydromt_fiat-0.3.1/tests/test_setup_new_composite_areas.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_setup_new_composite_areas_ground_elevation.py` & `hydromt_fiat-0.3.1/tests/test_setup_new_composite_areas_ground_elevation.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_truncate_damage_function.py` & `hydromt_fiat-0.3.1/tests/test_truncate_damage_function.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_update_ground_floor_height.py` & `hydromt_fiat-0.3.1/tests/test_update_ground_floor_height.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_update_max_potential_damage.py` & `hydromt_fiat-0.3.1/tests/test_update_max_potential_damage.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_update_max_potential_damage_user_data.py` & `hydromt_fiat-0.3.1/tests/test_update_max_potential_damage_user_data.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_vulnerability.py` & `hydromt_fiat-0.3.1/tests/test_vulnerability.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_vulnerability_exposure.py` & `hydromt_fiat-0.3.1/tests/test_vulnerability_exposure.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_vulnerability_exposure_add_to_data_catalog.py` & `hydromt_fiat-0.3.1/tests/test_vulnerability_exposure_add_to_data_catalog.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_vulnerability_exposure_global_default.py` & `hydromt_fiat-0.3.1/tests/test_vulnerability_exposure_global_default.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_vulnerability_expousure_with_user_dem_data.py` & `hydromt_fiat-0.3.1/tests/test_vulnerability_expousure_with_user_dem_data.py`

 * *Files identical despite different names*

### Comparing `hydromt_fiat-0.3.0/tests/test_vulnerability_from_csvs.py` & `hydromt_fiat-0.3.1/tests/test_vulnerability_from_csvs.py`

 * *Files identical despite different names*

