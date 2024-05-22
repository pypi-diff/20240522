# Comparing `tmp/pyedb-0.8.1.tar.gz` & `tmp/pyedb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedb-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyedb-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyedb-0.8.1.tar` & `pyedb-0.9.0.tar`

### file list

```diff
@@ -1,137 +1,138 @@
--rw-r--r--   0        0        0     1089 2024-04-25 07:42:45.492631 pyedb-0.8.1/LICENSE
--rw-r--r--   0        0        0     5476 2024-04-25 07:42:45.492631 pyedb-0.8.1/README.md
--rw-r--r--   0        0        0     4506 2024-04-25 07:42:45.556630 pyedb-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1520 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/__init__.py
--rw-r--r--   0        0        0    79042 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/application/Variables.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/application/__init__.py
--rw-r--r--   0        0        0     3406 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/clr_module.py
--rw-r--r--   0        0        0   169971 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb.py
--rw-r--r--   0        0        0       52 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/cell/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/cell/hierarchy/__init__.py
--rw-r--r--   0        0        0     3309 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/cell/hierarchy/model.py
--rw-r--r--   0        0        0   102985 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/components.py
--rw-r--r--   0        0        0    33626 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/configuration.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/__init__.py
--rw-r--r--   0        0        0     6743 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/component_def.py
--rw-r--r--   0        0        0     2029 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/component_model.py
--rw-r--r--   0        0        0     1550 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/definition_obj.py
--rw-r--r--   0        0        0     2476 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/definitions.py
--rw-r--r--   0        0        0     5967 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/package_def.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/__init__.py
--rw-r--r--   0        0        0    37653 2024-04-25 07:42:45.556630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/database.py
--rw-r--r--   0        0        0     8904 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/layout.py
--rw-r--r--   0        0        0    48320 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/primitive.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    37225 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0     4256 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/connectable.py
--rw-r--r--   0        0        0    48425 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0     2057 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0     1977 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    13190 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    48944 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    21945 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     9933 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    78754 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0     9223 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/ports.py
--rw-r--r--   0        0        0    48155 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    99967 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    42354 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    15342 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0    25287 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/terminals.py
--rw-r--r--   0        0        0     4928 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     3501 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     4726 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/general.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/__init__.py
--rw-r--r--   0        0        0     1590 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/point_data.py
--rw-r--r--   0        0        0     2990 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/polygon_data.py
--rw-r--r--   0        0        0    68343 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/hfss.py
--rw-r--r--   0        0        0    50907 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/layout.py
--rw-r--r--   0        0        0    11798 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/layout_validation.py
--rw-r--r--   0        0        0    44463 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/materials.py
--rw-r--r--   0        0        0    11857 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/net_class.py
--rw-r--r--   0        0        0    43882 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/nets.py
--rw-r--r--   0        0        0     3312 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/obj_base.py
--rw-r--r--   0        0        0    54540 2024-04-25 07:42:45.560630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/padstack.py
--rw-r--r--   0        0        0    62356 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/siwave.py
--rw-r--r--   0        0        0   115372 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/stackup.py
--rw-r--r--   0        0        0       58 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/__init__.py
--rw-r--r--   0        0        0     2220 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/heatsink.py
--rw-r--r--   0        0        0    23967 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/simulation_setup.py
--rw-r--r--   0        0        0     1931 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/dotnet/sim_setup_data/data/siw_dc_ir_settings.py
--rw-r--r--   0        0        0    14950 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/edb_logger.py
--rw-r--r--   0        0        0      111 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/__init__.py
--rw-r--r--   0        0        0    28956 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/constants.py
--rw-r--r--   0        0        0     7137 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/data_handlers.py
--rw-r--r--   0        0        0     4354 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/design_types.py
--rw-r--r--   0        0        0     3941 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/filesystem.py
--rw-r--r--   0        0        0    43608 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/general_methods.py
--rw-r--r--   0        0        0     4901 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/plot.py
--rw-r--r--   0        0        0    11206 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/process.py
--rw-r--r--   0        0        0     9220 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/generic/settings.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0     1853 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     2394 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     3329 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0     1661 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/__init__.py
--rw-r--r--   0        0        0     1883 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/color.py
--rw-r--r--   0        0        0     3187 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/content.py
--rw-r--r--   0        0        0     2052 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0     2026 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     2142 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0     1546 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0     1687 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0     1651 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/fill.py
--rw-r--r--   0        0        0     1427 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     3931 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     2405 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     2628 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0     2083 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     3023 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     2270 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     8586 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0     2042 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     2197 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     5598 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     2535 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0     2004 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     3866 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0     2014 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     5044 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     3640 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     2124 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8945 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0     2781 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     2274 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     2717 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0     1970 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    12590 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     2143 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0     1797 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     3115 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     2739 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/history_record.py
--rw-r--r--   0        0        0    22685 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/ipc2581.py
--rw-r--r--   0        0        0     2092 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/ipc2581/logistic_header.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/misc/__init__.py
--rw-r--r--   0        0        0     1759 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    12223 2024-04-25 07:42:45.564630 pyedb-0.8.1/src/pyedb/misc/downloads.py
--rw-r--r--   0        0        0     3315 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/misc.py
--rw-r--r--   0        0        0      301 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/pyedb.runtimeconfig.json
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/__init__.py
--rw-r--r--   0        0        0     1560 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/component_tags.py
--rw-r--r--   0        0        0     1184 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/net_tags.py
--rw-r--r--   0        0        0     1557 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/tag_library.py
--rw-r--r--   0        0        0     2521 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/xml_generic.py
--rw-r--r--   0        0        0     7389 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc_rule_checker_settings.py
--rw-r--r--   0        0        0      465 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/misc/utilities.py
--rw-r--r--   0        0        0    66820 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/modeler/geometry_operators.py
--rw-r--r--   0        0        0    11576 2024-04-25 07:42:45.568630 pyedb-0.8.1/src/pyedb/siwave.py
--rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 pyedb-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-26 14:42:53.632131 pyedb-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5476 2024-04-26 14:42:53.632131 pyedb-0.9.0/README.md
+-rw-r--r--   0        0        0     4532 2024-04-26 14:42:53.692130 pyedb-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1520 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/__init__.py
+-rw-r--r--   0        0        0    79042 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/application/Variables.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/application/__init__.py
+-rw-r--r--   0        0        0     3406 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/clr_module.py
+-rw-r--r--   0        0        0   171632 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb.py
+-rw-r--r--   0        0        0       52 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/cell/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/cell/hierarchy/__init__.py
+-rw-r--r--   0        0        0     3309 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/cell/hierarchy/model.py
+-rw-r--r--   0        0        0   102985 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/components.py
+-rw-r--r--   0        0        0    33626 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/configuration.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/__init__.py
+-rw-r--r--   0        0        0     6743 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/component_def.py
+-rw-r--r--   0        0        0     2029 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/component_model.py
+-rw-r--r--   0        0        0     1550 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/definition_obj.py
+-rw-r--r--   0        0        0     2476 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/definitions.py
+-rw-r--r--   0        0        0     5967 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/package_def.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    37653 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     8904 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48320 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    37225 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0     4256 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/connectable.py
+-rw-r--r--   0        0        0    48425 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0     2057 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0     1977 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    13190 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    48944 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    21945 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     9933 2024-04-26 14:42:53.692130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    78754 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0     9223 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/ports.py
+-rw-r--r--   0        0        0    48155 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    21065 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/raptor_x_simulation_setup_data.py
+-rw-r--r--   0        0        0    99967 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    42354 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    15342 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0    25287 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/terminals.py
+-rw-r--r--   0        0        0     4928 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     3501 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     4726 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/general.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/geometry/__init__.py
+-rw-r--r--   0        0        0     1590 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/geometry/point_data.py
+-rw-r--r--   0        0        0     2990 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/geometry/polygon_data.py
+-rw-r--r--   0        0        0    68343 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/hfss.py
+-rw-r--r--   0        0        0    50907 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/layout.py
+-rw-r--r--   0        0        0    11798 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/layout_validation.py
+-rw-r--r--   0        0        0    44463 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/materials.py
+-rw-r--r--   0        0        0    11857 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/net_class.py
+-rw-r--r--   0        0        0    43882 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/nets.py
+-rw-r--r--   0        0        0     3312 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/obj_base.py
+-rw-r--r--   0        0        0    56581 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/padstack.py
+-rw-r--r--   0        0        0    62356 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/siwave.py
+-rw-r--r--   0        0        0   115372 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/stackup.py
+-rw-r--r--   0        0        0       58 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/utilities/__init__.py
+-rw-r--r--   0        0        0     2220 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/utilities/heatsink.py
+-rw-r--r--   0        0        0    24639 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/edb_core/utilities/simulation_setup.py
+-rw-r--r--   0        0        0     1931 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/dotnet/sim_setup_data/data/siw_dc_ir_settings.py
+-rw-r--r--   0        0        0    14950 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/edb_logger.py
+-rw-r--r--   0        0        0      111 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/generic/__init__.py
+-rw-r--r--   0        0        0    28956 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/generic/constants.py
+-rw-r--r--   0        0        0     7137 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/generic/data_handlers.py
+-rw-r--r--   0        0        0     4354 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/generic/design_types.py
+-rw-r--r--   0        0        0     3941 2024-04-26 14:42:53.696130 pyedb-0.9.0/src/pyedb/generic/filesystem.py
+-rw-r--r--   0        0        0    43608 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/generic/general_methods.py
+-rw-r--r--   0        0        0     4901 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/generic/plot.py
+-rw-r--r--   0        0        0    11206 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/generic/process.py
+-rw-r--r--   0        0        0     9220 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/generic/settings.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0     1853 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     2394 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     3329 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0     1661 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0     1883 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/color.py
+-rw-r--r--   0        0        0     3187 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/content.py
+-rw-r--r--   0        0        0     2052 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0     2026 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     2142 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0     1546 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0     1687 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0     1651 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/fill.py
+-rw-r--r--   0        0        0     1427 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     3931 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     2405 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     2628 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0     2083 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     3023 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     2270 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     8586 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0     2042 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     2197 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     5598 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     2535 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0     2004 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     3866 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0     2014 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     5044 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     3640 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     2124 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8945 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0     2781 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     2274 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     2717 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0     1970 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    12590 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     2143 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0     1797 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     3115 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     2739 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/history_record.py
+-rw-r--r--   0        0        0    22685 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0     2092 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/__init__.py
+-rw-r--r--   0        0        0     1759 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    12223 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/downloads.py
+-rw-r--r--   0        0        0     3315 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/misc.py
+-rw-r--r--   0        0        0      301 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/pyedb.runtimeconfig.json
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/siw_feature_config/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/__init__.py
+-rw-r--r--   0        0        0     1560 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/component_tags.py
+-rw-r--r--   0        0        0     1184 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/net_tags.py
+-rw-r--r--   0        0        0     1557 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/tag_library.py
+-rw-r--r--   0        0        0     2521 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/xml_generic.py
+-rw-r--r--   0        0        0     7389 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc_rule_checker_settings.py
+-rw-r--r--   0        0        0      465 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/misc/utilities.py
+-rw-r--r--   0        0        0    66820 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/modeler/geometry_operators.py
+-rw-r--r--   0        0        0    11576 2024-04-26 14:42:53.700130 pyedb-0.9.0/src/pyedb/siwave.py
+-rw-r--r--   0        0        0     8350 1970-01-01 00:00:00.000000 pyedb-0.9.0/PKG-INFO
```

### Comparing `pyedb-0.8.1/LICENSE` & `pyedb-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/README.md` & `pyedb-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/pyproject.toml` & `pyedb-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 dependencies = [
     "cffi>=1.16.0,<1.17; platform_system=='Linux'",
     "pywin32 >= 303;platform_system=='Windows'",
     "ansys-pythonnet >= 3.1.0rc3",
     "dotnetcore2 ==3.1.23;platform_system=='Linux'",
     "pydantic>=2.6.4,<2.8",
     "toml == 0.10.2",
-]
+    "Rtree >= 1.2.0",
+    ]
 
 [project.optional-dependencies]
 tests = [
     "matplotlib>=3.5.0,<3.9",
     "numpy>=1.20.0,<2",
     "mock>=5.1.0,<5.2",
     "pandas>=1.1.0,<2.3",
```

### Comparing `pyedb-0.8.1/src/pyedb/__init__.py` & `pyedb-0.9.0/src/pyedb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 
 
 deprecation_warning()
 
 #
 
 pyedb_path = os.path.dirname(__file__)
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 version = __version__
 
 #
 
 from pyedb.generic.design_types import Edb, Siwave
```

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/application/Variables.py` & `pyedb-0.9.0/src/pyedb/dotnet/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/clr_module.py` & `pyedb-0.9.0/src/pyedb/dotnet/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,17 @@
     BundleWavePort,
     CircuitPort,
     CoaxPort,
     ExcitationSources,
     GapPort,
     WavePort,
 )
+from pyedb.dotnet.edb_core.edb_data.raptor_x_simulation_setup_data import (
+    RaptorXSimulationSetup,
+)
 from pyedb.dotnet.edb_core.edb_data.simulation_configuration import (
     SimulationConfiguration,
 )
 from pyedb.dotnet.edb_core.edb_data.siwave_simulation_setup_data import (
     SiwaveDCSimulationSetup,
     SiwaveSYZSimulationSetup,
 )
@@ -170,23 +173,24 @@
 
     >>> app = Edb("/path/to/file/myfile.gds")
 
     """
 
     def __init__(
         self,
-        edbpath=None,
-        cellname=None,
-        isreadonly=False,
-        edbversion=None,
-        isaedtowned=False,
+        edbpath: str = None,
+        cellname: str = None,
+        isreadonly: bool = False,
+        edbversion: str = None,
+        isaedtowned: bool = False,
         oproject=None,
-        student_version=False,
-        use_ppe=False,
-        technology_file=None,
+        student_version: bool = False,
+        use_ppe: bool = False,
+        technology_file: str = None,
+        remove_existing_aedt: bool = False,
     ):
         edbversion = get_string_version(edbversion)
         self._clean_variables()
         Database.__init__(self, edbversion=edbversion, student_version=student_version)
         self.standalone = True
         self.oproject = oproject
         self._main = sys.modules["__main__"]
@@ -209,25 +213,16 @@
         self.edbpath = edbpath
         self.log_name = None
         if edbpath:
             self.log_name = os.path.join(
                 os.path.dirname(edbpath),
                 "pyedb_" + os.path.splitext(os.path.split(edbpath)[-1])[0] + ".log",
             )
-            aedt_file = os.path.splitext(edbpath)[0] + ".aedt"
-            files = [aedt_file, aedt_file + ".lock"]
-            for file in files:
-                if os.path.isfile(file):
-                    try:
-                        shutil.rmtree(file)
-                        self.logger.info(f"Removing {file} to allow loading EDB file.")
-                    except:
-                        self.logger.info(
-                            f"Failed to delete {file} which is located at the same location as the EDB file."
-                        )
+            if not isreadonly:
+                self._check_remove_project_files(edbpath, remove_existing_aedt)
 
         if isaedtowned and (inside_desktop or settings.remote_rpc_session):
             self.open_edb_inside_aedt()
         elif edbpath[-3:] in ["brd", "mcm", "sip", "gds", "xml", "dxf", "tgz", "anf"]:
             self.edbpath = edbpath[:-4] + ".aedb"
             working_dir = os.path.dirname(edbpath)
             control_file = None
@@ -307,14 +302,30 @@
         if self.variable_exists(variable_name)[0]:
             self.change_design_variable_value(variable_name, val)
         else:
             self.add_design_variable(variable_name, val)
         if description:  # Add the variable description if a two-item list is passed for variable_value.
             self.__getitem__(variable_name).description = description
 
+    def _check_remove_project_files(self, edbpath: str, remove_existing_aedt: bool) -> None:
+        aedt_file = os.path.splitext(edbpath)[0] + ".aedt"
+        files = [aedt_file, aedt_file + ".lock"]
+        for file in files:
+            if os.path.isfile(file):
+                if not remove_existing_aedt:
+                    self.logger.warning(
+                        f"AEDT project-related file {file} exists and may need to be deleted before opening the EDB in HFSS 3D Layout."  # noqa: E501
+                    )
+                else:
+                    try:
+                        os.unlink(file)
+                        self.logger.info(f"Deleted AEDT project-related file {file}.")
+                    except:
+                        self.logger.info(f"Failed to delete AEDT project-related file {file}.")
+
     def _clean_variables(self):
         """Initialize internal variables and perform garbage collection."""
         self._materials = None
         self._components = None
         self._core_primitives = None
         self._stackup = None
         self._stackup2 = None
@@ -3580,14 +3591,16 @@
         for i in list(self.active_cell.SimulationSetups):
             if i.GetType() == self.edb_api.utility.utility.SimulationSetupType.kHFSS:
                 setups[i.GetName()] = HfssSimulationSetup(self, i)
             elif i.GetType() == self.edb_api.utility.utility.SimulationSetupType.kSIWave:
                 setups[i.GetName()] = SiwaveSYZSimulationSetup(self, i)
             elif i.GetType() == self.edb_api.utility.utility.SimulationSetupType.kSIWaveDCIR:
                 setups[i.GetName()] = SiwaveDCSimulationSetup(self, i)
+            elif i.GetType() == self.edb_api.utility.utility.SimulationSetupType.kRaptorX:
+                setups[i.GetName()] = RaptorXSimulationSetup(self, i)
         return setups
 
     @property
     def hfss_setups(self):
         """Active HFSS setup in EDB.
 
         Returns
@@ -3635,17 +3648,43 @@
         >>> edbapp = Edb()
         >>> setup1 = edbapp.create_hfss_setup("setup1")
         >>> setup1.hfss_port_settings.max_delta_z0 = 0.5
         """
         if name in self.setups:
             self.logger.info("setup already exists")
             return False
+        elif not name:
+            name = generate_unique_name("setup")
         setup = HfssSimulationSetup(self).create(name)
         return setup
 
+    def create_raptorx_setup(self, name=None):
+        """Create an RaptorX simulation setup from a template.
+
+        Parameters
+        ----------
+        name : str, optional
+            Setup name.
+
+        Returns
+        -------
+        :class:`legacy.edb_core.edb_data.raptor_x_simulation_setup_data.RaptorXSimulationSetup`
+
+        """
+        if name in self.setups:
+            self.logger.error("Setup name already used in the layout")
+            return False
+        version = self.edbversion.split(".")
+        if int(version[0]) >= 2024 and int(version[-1]) >= 2 or int(version[0]) > 2024:
+            setup = RaptorXSimulationSetup(self).create(name)
+            return setup
+        else:
+            self.logger.error("RaptorX simulation only supported with Ansys release 2024R2 and higher")
+            return False
+
     @pyedb_function_handler()
     def create_siwave_syz_setup(self, name=None):
         """Create a setup from a template.
 
         Parameters
         ----------
         name : str, optional
```

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/cell/hierarchy/model.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/cell/hierarchy/model.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/components.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/components.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/configuration.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/configuration.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/component_def.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/component_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/component_model.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/component_model.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/definition_obj.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/definition_obj.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/definitions.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/definitions.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/definition/package_def.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/definition/package_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/database.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/dotnet/database.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/layout.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/dotnet/layout.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/dotnet/primitive.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/dotnet/primitive.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/components_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/connectable.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/connectable.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/control_file.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/control_file.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/design_options.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/edbvalue.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/hfss_extent_info.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/layer_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/nets_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/nets_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/padstacks_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/ports.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/ports.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/primitives_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/simulation_configuration.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/sources.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/terminals.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/terminals.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/utilities.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/edb_data/variables.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/general.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/point_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/geometry/point_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/geometry/polygon_data.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/geometry/polygon_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/hfss.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/layout.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/layout_validation.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/layout_validation.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/materials.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/net_class.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/net_class.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/nets.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/obj_base.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/obj_base.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/padstack.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/padstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 """
 This module contains the `EdbPadstacks` class.
 """
 import math
 import warnings
 
+import rtree
+
 from pyedb.dotnet.clr_module import Array
 from pyedb.dotnet.edb_core.edb_data.padstacks_data import (
     EDBPadstack,
     EDBPadstackInstance,
 )
 from pyedb.dotnet.edb_core.general import convert_py_list_to_net_list
 from pyedb.generic.general_methods import generate_unique_name, pyedb_function_handler
@@ -1456,7 +1458,58 @@
             for p in references_pins
             if GeometryOperators.points_distance(positive_pin.position, p.position) <= search_radius
         ]
         if max_limit and len(pinlist) > max_limit:
             pin_dict = {GeometryOperators.points_distance(positive_pin.position, p.position): p for p in pinlist}
             pinlist = [pin[1] for pin in sorted(pin_dict.items())[:max_limit]]
         return pinlist
+
+    @pyedb_function_handler()
+    def get_padstack_instances_rtree_index(self, nets=None):
+        """Returns padstack instances Rtree index.
+
+        Parameters
+        ----------
+        nets : str or list, optional
+            net name of list of nets name applying filtering on padstack instances selection. If ``None`` is provided
+            all instances are included in the index. Default value is ``None``.
+
+        Returns
+        -------
+        Rtree index object.
+
+        """
+        if isinstance(nets, str):
+            nets = [nets]
+        padstack_instances_index = rtree.index.Index()
+        if nets:
+            instances = [inst for inst in list(self.instances.values()) if inst.net_name in nets]
+        else:
+            instances = list(self.instances.values())
+        for inst in instances:
+            padstack_instances_index.insert(inst.id, inst.position)
+        return padstack_instances_index
+
+    @pyedb_function_handler()
+    def get_padstack_instances_intersecting_bounding_box(self, bounding_box, nets=None):
+        """Returns the list of padstack instances ID intersecting a given bounding box and nets.
+
+        Parameters
+        ----------
+        bounding_box : tuple or list.
+            bounding box, [x1, y1, x2, y2]
+        nets : str or list, optional
+            net name of list of nets name applying filtering on padstack instances selection. If ``None`` is provided
+            all instances are included in the index. Default value is ``None``.
+
+        Returns
+        -------
+        List of padstack instances ID intersecting the bounding box.
+        """
+        if not bounding_box:
+            raise Exception("No bounding box was provided")
+        index = self.get_padstack_instances_rtree_index(nets=nets)
+        if not len(bounding_box) == 4:
+            raise Exception("The bounding box length must be equal to 4")
+        if isinstance(bounding_box, list):
+            bounding_box = tuple(bounding_box)
+        return list(index.intersection(bounding_box))
```

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/siwave.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/stackup.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/stackup.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/heatsink.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/utilities/heatsink.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/edb_core/utilities/simulation_setup.py` & `pyedb-0.9.0/src/pyedb/dotnet/edb_core/utilities/simulation_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             "kAnalysisOption": None,
             "kSIwaveDCIR": self._pedb.simsetupdata.SIwave.SIWDCIRSimulationSettings,
             "kSIwaveEMI": None,
             "kHFSSPI": None,
             "kDDRwizard": None,
             "kQ3D": None,
             "kNumSetupTypes": None,
+            "kRaptorX": self._pedb.simsetupdata.RaptorX.RaptorXSimulationSettings,
         }
         if self._edb_object:
             self._name = self._edb_object.GetName()
 
         self._sweep_list = {}
 
     @pyedb_function_handler
@@ -68,14 +69,16 @@
         if not name:
             name = generate_unique_name(self.setup_type)
             self._name = name
 
         setup_type = self._setup_type_mapping[self._setup_type]
         edb_setup_info = self._pedb.simsetupdata.SimSetupInfo[setup_type]()
         edb_setup_info.Name = name
+        if edb_setup_info.get_SimSetupType().ToString() == "kRaptorX":
+            self._edb_setup_info = edb_setup_info
         self._edb_object = self._set_edb_setup_info(edb_setup_info)
         self._update_setup()
 
     @pyedb_function_handler
     def _set_edb_setup_info(self, edb_setup_info):
         """Create a setup object from a setup information object."""
         utility = self._pedb._edb.Utility
@@ -92,14 +95,17 @@
             "kSIwaveDCIR": utility.SIWaveDCIRSimulationSetup,
             "kSIwaveEMI": None,
             "kHFSSPI": None,
             "kDDRwizard": None,
             "kQ3D": None,
             "kNumSetupTypes": None,
         }
+        version = self._pedb.edbversion.split(".")
+        if int(version[0]) == 2024 and int(version[1]) == 2 or int(version[0]) > 2024:
+            setup_type_mapping["kRaptorX"] = utility.RaptorXSimulationSetup
         setup_utility = setup_type_mapping[self._setup_type]
         return setup_utility(edb_setup_info)
 
     @pyedb_function_handler()
     def _update_setup(self):
         """Update setup in EDB."""
         if self._setup_type == "kHFSS":
@@ -118,17 +124,16 @@
     @property
     def enabled(self):
         """Flag indicating if the setup is enabled."""
         return self.get_sim_setup_info.SimulationSettings.Enabled
 
     @enabled.setter
     def enabled(self, value):
-        edb_setup_info = self.get_sim_setup_info
-        edb_setup_info.SimulationSettings.Enabled = value
-        self._edb_object = self._set_edb_setup_info(edb_setup_info)
+        self.get_sim_setup_info.SimulationSettings.Enabled = value
+        self._edb_object = self._set_edb_setup_info(self.get_sim_setup_info)
         self._update_setup()
 
     @property
     def name(self):
         """Name of the setup."""
         return self._edb_object.GetName()
 
@@ -171,17 +176,20 @@
         """Add a frequency sweep.
 
         Parameters
         ----------
         sweep_data: EdbFrequencySweep
         """
         self._sweep_list[sweep_data.name] = sweep_data
-        edb_setup_info = self.get_sim_setup_info
+        if self.setup_type == "kRaptorX":
+            edb_setup_info = self._edb_setup_info
+        else:
+            edb_setup_info = self.get_sim_setup_info
 
-        if self._setup_type in ["kSIwave", "kHFSS"]:
+        if self._setup_type in ["kSIwave", "kHFSS", "kRaptorX"]:
             for _, v in self._sweep_list.items():
                 edb_setup_info.SweepDataList.Add(v._edb_object)
 
         self._edb_object = self._set_edb_setup_info(edb_setup_info)
         self._update_setup()
 
     @pyedb_function_handler
@@ -193,22 +201,21 @@
             sweep_data : EdbFrequencySweep.
         """
         name = sweep_data.name
         if name in self._sweep_list:
             self._sweep_list.pop(name)
 
         fsweep = []
-        for k, val in self.frequency_sweeps.items():
-            if not k == name:
-                fsweep.append(val)
-        self.get_sim_setup_info.SweepDataList.Clear()
-        for i in fsweep:
-            self.get_sim_setup_info.SweepDataList.Add(i._edb_object)
-        self._update_setup()
-        return True if name in self.frequency_sweeps else False
+        if self.frequency_sweeps:
+            fsweep = [val for key, val in self.frequency_sweeps.items() if not key == name]
+            self.get_sim_setup_info.SweepDataList.Clear()
+            for i in fsweep:
+                self.get_sim_setup_info.SweepDataList.Add(i._edb_object)
+            self._update_setup()
+            return True if name in self.frequency_sweeps else False
 
     @pyedb_function_handler()
     def add_frequency_sweep(self, name=None, frequency_sweep=None):
         """Add frequency sweep.
 
         Parameters
         ----------
@@ -718,14 +725,16 @@
         if not frequency_list:
             frequency_list = [
                 ["linear count", "0", "1kHz", 1],
                 ["log scale", "1kHz", "0.1GHz", 10],
                 ["linear scale", "0.1GHz", "10GHz", "0.1GHz"],
             ]
         temp = []
+        if isinstance(frequency_list, list) and not isinstance(frequency_list[0], list):
+            frequency_list = [frequency_list]
         for i in frequency_list:
             if i[0] == "linear count":
                 temp.extend(list(self._edb_sweep_data.SetFrequencies(i[1], i[2], i[3])))
             elif i[0] == "linear scale":
                 temp.extend(list(self._edb_sweep_data.SetFrequencies(i[1], i[2], i[3])))
             elif i[0] == "log scale":
                 temp.extend(list(self._edb_sweep_data.SetLogFrequencies(i[1], i[2], i[3])))
```

### Comparing `pyedb-0.8.1/src/pyedb/dotnet/sim_setup_data/data/siw_dc_ir_settings.py` & `pyedb-0.9.0/src/pyedb/dotnet/sim_setup_data/data/siw_dc_ir_settings.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/edb_logger.py` & `pyedb-0.9.0/src/pyedb/edb_logger.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/generic/constants.py` & `pyedb-0.9.0/src/pyedb/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/generic/data_handlers.py` & `pyedb-0.9.0/src/pyedb/generic/data_handlers.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/generic/design_types.py` & `pyedb-0.9.0/src/pyedb/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/generic/filesystem.py` & `pyedb-0.9.0/src/pyedb/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/generic/general_methods.py` & `pyedb-0.9.0/src/pyedb/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/generic/plot.py` & `pyedb-0.9.0/src/pyedb/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/generic/process.py` & `pyedb-0.9.0/src/pyedb/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/generic/settings.py` & `pyedb-0.9.0/src/pyedb/generic/settings.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/bom/bom.py` & `pyedb-0.9.0/src/pyedb/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/bom/bom_item.py` & `pyedb-0.9.0/src/pyedb/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/bom/characteristics.py` & `pyedb-0.9.0/src/pyedb/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/bom/refdes.py` & `pyedb-0.9.0/src/pyedb/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/color.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/content.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_color.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_fill.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/dictionary_line.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/entry_color.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/entry_color.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/entry_line.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/fill.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/layer_ref.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/layer_ref.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/content/standard_geometries_dictionary.py` & `pyedb-0.9.0/src/pyedb/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/cad_data.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/component.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/drill.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/feature.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/layer.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/layer_feature.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/logical_net.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/outline.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/package.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_def.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_instance.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/path.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/phy_net.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/pin.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/polygon.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/profile.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup_group.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/stackup_layer.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_data/step.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/cad_header.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/ecad.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ecad/spec.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/history_record.py` & `pyedb-0.9.0/src/pyedb/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/ipc2581.py` & `pyedb-0.9.0/src/pyedb/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/ipc2581/logistic_header.py` & `pyedb-0.9.0/src/pyedb/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/misc/aedtlib_personalib_install.py` & `pyedb-0.9.0/src/pyedb/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/misc/downloads.py` & `pyedb-0.9.0/src/pyedb/misc/downloads.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/misc/misc.py` & `pyedb-0.9.0/src/pyedb/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/component_tags.py` & `pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/component_tags.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/net_tags.py` & `pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/net_tags.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/tag_library.py` & `pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/tag_library.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc/xml_generic.py` & `pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc/xml_generic.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/misc/siw_feature_config/emc_rule_checker_settings.py` & `pyedb-0.9.0/src/pyedb/misc/siw_feature_config/emc_rule_checker_settings.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/modeler/geometry_operators.py` & `pyedb-0.9.0/src/pyedb/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/src/pyedb/siwave.py` & `pyedb-0.9.0/src/pyedb/siwave.py`

 * *Files identical despite different names*

### Comparing `pyedb-0.8.1/PKG-INFO` & `pyedb-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyedb
-Version: 0.8.1
+Version: 0.9.0
 Summary: Higher-Level Pythonic Ansys Electronics Data Base
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyEDB developers <simon.vandenbrouck@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cffi>=1.16.0,<1.17; platform_system=='Linux'
 Requires-Dist: pywin32 >= 303;platform_system=='Windows'
 Requires-Dist: ansys-pythonnet >= 3.1.0rc3
 Requires-Dist: dotnetcore2 ==3.1.23;platform_system=='Linux'
 Requires-Dist: pydantic>=2.6.4,<2.8
 Requires-Dist: toml == 0.10.2
+Requires-Dist: Rtree >= 1.2.0
 Requires-Dist: ansys-sphinx-theme>=0.10.0,<0.16 ; extra == "doc"
 Requires-Dist: imageio>=2.30.0,<2.35 ; extra == "doc"
 Requires-Dist: ipython>=8.13.0,<8.24 ; extra == "doc"
 Requires-Dist: jupyterlab>=4.0.0,<4.3 ; extra == "doc"
 Requires-Dist: matplotlib>=3.5.0,<3.9 ; extra == "doc"
 Requires-Dist: nbsphinx>=0.9.0,<0.10 ; extra == "doc"
 Requires-Dist: numpydoc>=1.5.0,<1.8 ; extra == "doc"
```

