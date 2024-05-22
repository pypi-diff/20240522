# Comparing `tmp/cimsparql-4.1.0.tar.gz` & `tmp/cimsparql-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cimsparql-4.1.0.tar", max compression
+gzip compressed data, was "cimsparql-4.1.1.tar", max compression
```

## Comparing `cimsparql-4.1.0.tar` & `cimsparql-4.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1065 2024-05-16 08:56:47.811139 cimsparql-4.1.0/LICENSE
--rw-r--r--   0        0        0     5195 2024-05-16 08:56:47.811139 cimsparql-4.1.0/README.md
--rw-r--r--   0        0        0       60 2024-05-16 08:57:06.818949 cimsparql-4.1.0/cimsparql/__init__.py
--rw-r--r--   0        0        0     4744 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/adaptions.py
--rw-r--r--   0        0        0     1642 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/constants.py
--rw-r--r--   0        0        0     9830 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/data_models.py
--rw-r--r--   0        0        0    16044 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/graphdb.py
--rw-r--r--   0        0        0    27478 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/model.py
--rw-r--r--   0        0        0     5202 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/ac_lines.sparql
--rw-r--r--   0        0        0      221 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/add_mrid.sparql
--rw-r--r--   0        0        0     1761 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/borders.sparql
--rw-r--r--   0        0        0     2073 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/branch_node_withdraw.sparql
--rw-r--r--   0        0        0     1795 2024-05-16 08:56:47.811139 cimsparql-4.1.0/cimsparql/sparql/bus.sparql
--rw-r--r--   0        0        0      984 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/connections.sparql
--rw-r--r--   0        0        0     1291 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/connectivity_nodes.sparql
--rw-r--r--   0        0        0      737 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/converter_hvdc_bidzones.sparql
--rw-r--r--   0        0        0     2614 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/converters.sparql
--rw-r--r--   0        0        0      588 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/coordinates.sparql
--rw-r--r--   0        0        0     1373 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/dc_active_power_flow.sparql
--rw-r--r--   0        0        0      242 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/disconnected.sparql
--rw-r--r--   0        0        0     3063 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/exchange.sparql
--rw-r--r--   0        0        0      792 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/full_model.sparql
--rw-r--r--   0        0        0     2813 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/loads.sparql
--rw-r--r--   0        0        0      287 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/market_dates.sparql
--rw-r--r--   0        0        0      523 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/power_flow.sparql
--rw-r--r--   0        0        0      397 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/ras_equipment.sparql
--rw-r--r--   0        0        0      573 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/regions.sparql
--rw-r--r--   0        0        0     3655 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/series_compensators.sparql
--rw-r--r--   0        0        0      426 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/station_group_code_and_names.sparql
--rw-r--r--   0        0        0      645 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/substation_voltage_level.sparql
--rw-r--r--   0        0        0     2877 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/sv_branch.sparql
--rw-r--r--   0        0        0      245 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/sv_injection.sparql
--rw-r--r--   0        0        0      781 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/switches.sparql
--rw-r--r--   0        0        0     3285 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/synchronous_machines.sparql
--rw-r--r--   0        0        0      318 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
--rw-r--r--   0        0        0     3752 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformer_branches.sparql
--rw-r--r--   0        0        0     1461 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformer_center_nodes.sparql
--rw-r--r--   0        0        0      720 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformer_winding_angle.sparql
--rw-r--r--   0        0        0      363 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformer_windings.sparql
--rw-r--r--   0        0        0     1269 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformers.sparql
--rw-r--r--   0        0        0     1844 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/transformers_connected_to_converter.sparql
--rw-r--r--   0        0        0      461 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/type_mapper.sparql
--rw-r--r--   0        0        0      814 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/wind_generating_units.sparql
--rw-r--r--   0        0        0      944 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/winding.sparql
--rw-r--r--   0        0        0     1189 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql/winding_loss.sparql
--rw-r--r--   0        0        0     2298 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/sparql_result_json.py
--rw-r--r--   0        0        0     3112 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/templates.py
--rw-r--r--   0        0        0     5650 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/type_mapper.py
--rw-r--r--   0        0        0      768 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/url.py
--rw-r--r--   0        0        0      616 2024-05-16 08:56:47.815139 cimsparql-4.1.0/cimsparql/value_mapper.py
--rw-r--r--   0        0        0      459 2024-05-16 08:56:47.823139 cimsparql-4.1.0/pkg_data/blazegraph_repo_config.xml
--rw-r--r--   0        0        0      676 2024-05-16 08:56:47.823139 cimsparql-4.1.0/pkg_data/namespaces.json
--rw-r--r--   0        0        0      805 2024-05-16 08:56:47.823139 cimsparql-4.1.0/pkg_data/native_store_config_template.ttl
--rw-r--r--   0        0        0     4333 2024-05-16 08:57:06.818949 cimsparql-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 cimsparql-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-21 11:29:20.106516 cimsparql-4.1.1/LICENSE
+-rw-r--r--   0        0        0     5195 2024-05-21 11:29:20.110516 cimsparql-4.1.1/README.md
+-rw-r--r--   0        0        0       60 2024-05-21 11:29:39.658529 cimsparql-4.1.1/cimsparql/__init__.py
+-rw-r--r--   0        0        0     4744 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/adaptions.py
+-rw-r--r--   0        0        0     1642 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/constants.py
+-rw-r--r--   0        0        0     9830 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/data_models.py
+-rw-r--r--   0        0        0    16044 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/graphdb.py
+-rw-r--r--   0        0        0    27478 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/model.py
+-rw-r--r--   0        0        0     5202 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/ac_lines.sparql
+-rw-r--r--   0        0        0      221 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/add_mrid.sparql
+-rw-r--r--   0        0        0     1761 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/borders.sparql
+-rw-r--r--   0        0        0     2073 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/branch_node_withdraw.sparql
+-rw-r--r--   0        0        0     1795 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/bus.sparql
+-rw-r--r--   0        0        0      984 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/connections.sparql
+-rw-r--r--   0        0        0     1291 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/connectivity_nodes.sparql
+-rw-r--r--   0        0        0      737 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/converter_hvdc_bidzones.sparql
+-rw-r--r--   0        0        0     2614 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/converters.sparql
+-rw-r--r--   0        0        0      588 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/coordinates.sparql
+-rw-r--r--   0        0        0     1373 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/dc_active_power_flow.sparql
+-rw-r--r--   0        0        0      242 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/disconnected.sparql
+-rw-r--r--   0        0        0     3063 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/exchange.sparql
+-rw-r--r--   0        0        0      792 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/full_model.sparql
+-rw-r--r--   0        0        0     2813 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/loads.sparql
+-rw-r--r--   0        0        0      287 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/market_dates.sparql
+-rw-r--r--   0        0        0      523 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/power_flow.sparql
+-rw-r--r--   0        0        0      397 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/ras_equipment.sparql
+-rw-r--r--   0        0        0      573 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/regions.sparql
+-rw-r--r--   0        0        0     3655 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/series_compensators.sparql
+-rw-r--r--   0        0        0      426 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/station_group_code_and_names.sparql
+-rw-r--r--   0        0        0      645 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/substation_voltage_level.sparql
+-rw-r--r--   0        0        0     2877 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/sv_branch.sparql
+-rw-r--r--   0        0        0      245 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/sv_injection.sparql
+-rw-r--r--   0        0        0      781 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/switches.sparql
+-rw-r--r--   0        0        0     3285 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/synchronous_machines.sparql
+-rw-r--r--   0        0        0      318 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
+-rw-r--r--   0        0        0     3750 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/transformer_branches.sparql
+-rw-r--r--   0        0        0     1461 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/transformer_center_nodes.sparql
+-rw-r--r--   0        0        0      720 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/transformer_winding_angle.sparql
+-rw-r--r--   0        0        0      363 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/transformer_windings.sparql
+-rw-r--r--   0        0        0     1269 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/transformers.sparql
+-rw-r--r--   0        0        0     1844 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/transformers_connected_to_converter.sparql
+-rw-r--r--   0        0        0      461 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/type_mapper.sparql
+-rw-r--r--   0        0        0      814 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/wind_generating_units.sparql
+-rw-r--r--   0        0        0      944 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/winding.sparql
+-rw-r--r--   0        0        0     1189 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql/winding_loss.sparql
+-rw-r--r--   0        0        0     2298 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/sparql_result_json.py
+-rw-r--r--   0        0        0     3112 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/templates.py
+-rw-r--r--   0        0        0     5650 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/type_mapper.py
+-rw-r--r--   0        0        0      768 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/url.py
+-rw-r--r--   0        0        0      616 2024-05-21 11:29:20.110516 cimsparql-4.1.1/cimsparql/value_mapper.py
+-rw-r--r--   0        0        0      459 2024-05-21 11:29:20.118517 cimsparql-4.1.1/pkg_data/blazegraph_repo_config.xml
+-rw-r--r--   0        0        0      676 2024-05-21 11:29:20.118517 cimsparql-4.1.1/pkg_data/namespaces.json
+-rw-r--r--   0        0        0      805 2024-05-21 11:29:20.118517 cimsparql-4.1.1/pkg_data/native_store_config_template.ttl
+-rw-r--r--   0        0        0     4333 2024-05-21 11:29:39.658529 cimsparql-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 cimsparql-4.1.1/PKG-INFO
```

### Comparing `cimsparql-4.1.0/LICENSE` & `cimsparql-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/README.md` & `cimsparql-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/adaptions.py` & `cimsparql-4.1.1/cimsparql/adaptions.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/constants.py` & `cimsparql-4.1.1/cimsparql/constants.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/data_models.py` & `cimsparql-4.1.1/cimsparql/data_models.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/graphdb.py` & `cimsparql-4.1.1/cimsparql/graphdb.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/model.py` & `cimsparql-4.1.1/cimsparql/model.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/ac_lines.sparql` & `cimsparql-4.1.1/cimsparql/sparql/ac_lines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/borders.sparql` & `cimsparql-4.1.1/cimsparql/sparql/borders.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/branch_node_withdraw.sparql` & `cimsparql-4.1.1/cimsparql/sparql/branch_node_withdraw.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/bus.sparql` & `cimsparql-4.1.1/cimsparql/sparql/bus.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/connections.sparql` & `cimsparql-4.1.1/cimsparql/sparql/connections.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/connectivity_nodes.sparql` & `cimsparql-4.1.1/cimsparql/sparql/connectivity_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/converter_hvdc_bidzones.sparql` & `cimsparql-4.1.1/cimsparql/sparql/converter_hvdc_bidzones.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/converters.sparql` & `cimsparql-4.1.1/cimsparql/sparql/converters.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/coordinates.sparql` & `cimsparql-4.1.1/cimsparql/sparql/coordinates.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/dc_active_power_flow.sparql` & `cimsparql-4.1.1/cimsparql/sparql/dc_active_power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/exchange.sparql` & `cimsparql-4.1.1/cimsparql/sparql/exchange.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/full_model.sparql` & `cimsparql-4.1.1/cimsparql/sparql/full_model.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/loads.sparql` & `cimsparql-4.1.1/cimsparql/sparql/loads.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/power_flow.sparql` & `cimsparql-4.1.1/cimsparql/sparql/power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/regions.sparql` & `cimsparql-4.1.1/cimsparql/sparql/regions.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/series_compensators.sparql` & `cimsparql-4.1.1/cimsparql/sparql/series_compensators.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/substation_voltage_level.sparql` & `cimsparql-4.1.1/cimsparql/sparql/substation_voltage_level.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/sv_branch.sparql` & `cimsparql-4.1.1/cimsparql/sparql/sv_branch.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/switches.sparql` & `cimsparql-4.1.1/cimsparql/sparql/switches.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/synchronous_machines.sparql` & `cimsparql-4.1.1/cimsparql/sparql/synchronous_machines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/transformer_branches.sparql` & `cimsparql-4.1.1/cimsparql/sparql/transformer_branches.sparql`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,22 @@
   ?terminal cim:ACDCTerminal.connected ?connected .
   optional {?winding ^cim:SvStatus.ConductingEquipment/cim:SvStatus.inService ?in_service} .
 
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
     # Use mrid of transformer as dummy node
     ?p_transformer cim:IdentifiedObject.mRID ?node_2;
-            cim:Equipment.EquipmentContainer ?Substation;
-            cim:IdentifiedObject.name ?name .
+            cim:Equipment.EquipmentContainer ?Substation .
     ?Substation cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area .
     filter(regex(?area, '${region}'))
 
     # Extract properties for the windings associated with p_transformer
     ?winding cim:TransformerEnd.Terminal ?terminal;
           cim:IdentifiedObject.mRID ?mrid;
+          cim:IdentifiedObject.name ?name;
           cim:PowerTransformerEnd.PowerTransformer ?p_transformer;
           cim:PowerTransformerEnd.ratedU ?ubase;
           cim:PowerTransformerEnd.r ?r;
           cim:PowerTransformerEnd.x ?x;
           cim:PowerTransformerEnd.b ?b;
           cim:PowerTransformerEnd.g ?g .
     optional{?winding cim:PowerTransformerEnd.phaseAngleClock ?aclock .}
```

### Comparing `cimsparql-4.1.0/cimsparql/sparql/transformer_center_nodes.sparql` & `cimsparql-4.1.1/cimsparql/sparql/transformer_center_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/transformer_winding_angle.sparql` & `cimsparql-4.1.1/cimsparql/sparql/transformer_winding_angle.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/transformers.sparql` & `cimsparql-4.1.1/cimsparql/sparql/transformers.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/transformers_connected_to_converter.sparql` & `cimsparql-4.1.1/cimsparql/sparql/transformers_connected_to_converter.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/wind_generating_units.sparql` & `cimsparql-4.1.1/cimsparql/sparql/wind_generating_units.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/winding.sparql` & `cimsparql-4.1.1/cimsparql/sparql/winding.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql/winding_loss.sparql` & `cimsparql-4.1.1/cimsparql/sparql/winding_loss.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/sparql_result_json.py` & `cimsparql-4.1.1/cimsparql/sparql_result_json.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/templates.py` & `cimsparql-4.1.1/cimsparql/templates.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/type_mapper.py` & `cimsparql-4.1.1/cimsparql/type_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/url.py` & `cimsparql-4.1.1/cimsparql/url.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/cimsparql/value_mapper.py` & `cimsparql-4.1.1/cimsparql/value_mapper.py`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/pkg_data/namespaces.json` & `cimsparql-4.1.1/pkg_data/namespaces.json`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/pkg_data/native_store_config_template.ttl` & `cimsparql-4.1.1/pkg_data/native_store_config_template.ttl`

 * *Files identical despite different names*

### Comparing `cimsparql-4.1.0/pyproject.toml` & `cimsparql-4.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cimsparql"
-version = "4.1.0"
+version = "4.1.1"
 description = "CIM query utilities"
 readme = "README.md"
 authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>"]
 repository = "https://github.com/statnett/cimsparql.git"
 include = ["pkg_data/*"]
 exclude = ["tests/*"]
```

### Comparing `cimsparql-4.1.0/PKG-INFO` & `cimsparql-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cimsparql
-Version: 4.1.0
+Version: 4.1.1
 Summary: CIM query utilities
 Home-page: https://github.com/statnett/cimsparql.git
 Author: Statnett Datascience
 Author-email: Datascience.Drift@Statnett.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

