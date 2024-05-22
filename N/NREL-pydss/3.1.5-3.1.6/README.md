# Comparing `tmp/nrel_pydss-3.1.5.tar.gz` & `tmp/nrel_pydss-3.1.6.tar.gz`

## Comparing `nrel_pydss-3.1.5.tar` & `nrel_pydss-3.1.6.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0    21149 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/ResultData.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/SolveMode.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/__init__.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/common.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/config_data.py
--rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/controllers.py
--rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/dataset_buffer.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/dssBus.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/dssCircuit.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/dssElement.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/dssElementFactory.py
--rw-r--r--   0        0        0    24890 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/dssInstance.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/dssObjectBase.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/dssTransformer.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/element_fields.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/element_options.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/exceptions.py
--rw-r--r--   0        0        0    16434 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/export_list_reader.py
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/get_snapshot_timepoints.py
--rw-r--r--   0        0        0    16131 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/helics_interface.py
--rw-r--r--   0        0        0    44535 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/metrics.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/naerm.py
--rw-r--r--   0        0        0    20437 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/node_voltage_metrics.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyContrReader.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyDSS.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyResults.py
--rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pydss_fs_interface.py
--rw-r--r--   0        0        0    28424 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pydss_project.py
--rw-r--r--   0        0        0    38303 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pydss_results.py
--rw-r--r--   0        0        0     9438 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/registry.py
--rw-r--r--   0        0        0    38847 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/simulation_input_models.py
--rw-r--r--   0        0        0     8528 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/storage_filters.py
--rw-r--r--   0        0        0    15736 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/thermal_metrics.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/unitDefinations.py
--rw-r--r--   0        0        0    19454 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/value_storage.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/Extensions/MonteCarlo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/Extensions/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/ProfileManager/ProfileInterface.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/ProfileManager/__init__.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/ProfileManager/base_definitions.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/ProfileManager/common.py
--rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/ProfileManager/hooks/MongoDB.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/ProfileManager/hooks/__init__.py
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/ProfileManager/hooks/h5.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/__init__.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/endpoints.yaml
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/logging.yaml
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/server.py
--rw-r--r--   0        0        0    31947 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/schema/PyDSS.v1.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/schema/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/RunServer.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/config.yaml
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/app/DataWriter.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/app/HDF5.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/app/JSON_writer.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/app/Tester.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/app/__init__.py
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/app/pydss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/web/__init__.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/web/create_schema.py
--rw-r--r--   0        0        0    22395 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/web/handler.py
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/api/src/web/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/apps/__init__.py
--rw-r--r--   0        0        0    16311 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/apps/data_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/add_post_process.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/add_scenario.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/controllers.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/convert.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/create_project.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/edit_scenario.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/export.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/extract.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/pydss.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/reports.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/run.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/cli/run_server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/plots.toml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/ExportLists/ExportMode-byClass.toml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/ExportLists/ExportMode-byElement.toml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/ExportLists/Exports.toml
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/ExportLists/Subscriptions.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/ExportLists/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/Monte_Carlo/MonteCarloSettings.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/Monte_Carlo/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/FaultController.toml
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/GenController.toml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/MotorStall.toml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/MotorStallSimple.toml
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/PvController.toml
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/PvDynamic.toml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/PvFrequencyRideThru.toml
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/PvVoltageRideThru.toml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/SocketController.toml
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/StorageController.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/ThermostaticLoad.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/xfmrController.toml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/FrequencySweep.toml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/Histogram.toml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/NetworkGraph.toml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/Table.toml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/ThreeDim.toml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/TimeSeries.toml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/Topology.toml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/VoltageDistance.toml
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/XY.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/defaults/pyPlotList/__init__.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/modes/Dynamic.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/modes/QSTS.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/modes/Snapshot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/modes/__init__.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/modes/solver_base.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/__init__.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/enumerations.py
--rw-r--r--   0        0        0    16226 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/models.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/pyController.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/pyControllerAbstract.py
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/FaultController.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/GenController.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/MotorStall.py
--rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/MotorStallBackup.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/MotorStallSimple.py
--rw-r--r--   0        0        0    12715 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/PvController.py
--rw-r--r--   0        0        0    13552 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/PvDynamic.py
--rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/PvFrequencyRideThru.py
--rw-r--r--   0        0        0    20345 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/PvVoltageRideThru.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/SocketController.py
--rw-r--r--   0        0        0    22893 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/StorageController.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/ThermostaticLoad.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/__init__.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/xfmrController.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/Settings/PvControllers.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/Settings/__init__.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyControllers/Settings/PvControllers.toml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyPostprocessor/__init__.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyPostprocessor/pyPostprocess.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyPostprocessor/pyPostprocessAbstract.py
--rw-r--r--   0        0        0    19150 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py
--rw-r--r--   0        0        0    23379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyPostprocessor/PostprocessScripts/EdLiFoControl.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyPostprocessor/PostprocessScripts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/__init__.py
--rw-r--r--   0        0        0    20117 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/reports/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/reports/capacitor_change_count.py
--rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/reports/feeder_losses.py
--rw-r--r--   0        0        0    14649 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/reports/pv_reports.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/reports/reg_control_tap_number_change_count.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/reports/reports.py
--rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/reports/thermal_metrics.py
--rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/reports/voltage_metrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/utils/__init__.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/utils/dataframe_utils.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/utils/dss_utils.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/utils/pydss_utils.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/utils/simulation_utils.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/utils/timing_utils.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/src/pydss/utils/utils.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/.gitignore
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/LICENSE
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 nrel_pydss-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0    21149 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/ResultData.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/SolveMode.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/__init__.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/common.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/config_data.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/controllers.py
+-rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/dataset_buffer.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/dssBus.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/dssCircuit.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/dssElement.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/dssElementFactory.py
+-rw-r--r--   0        0        0    24890 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/dssInstance.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/dssObjectBase.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/dssTransformer.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/element_fields.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/element_options.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/exceptions.py
+-rw-r--r--   0        0        0    16434 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/export_list_reader.py
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/get_snapshot_timepoints.py
+-rw-r--r--   0        0        0    16131 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/helics_interface.py
+-rw-r--r--   0        0        0    44535 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/metrics.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/naerm.py
+-rw-r--r--   0        0        0    20437 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/node_voltage_metrics.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyContrReader.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyDSS.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyResults.py
+-rw-r--r--   0        0        0    11068 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pydss_fs_interface.py
+-rw-r--r--   0        0        0    28424 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pydss_project.py
+-rw-r--r--   0        0        0    38303 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pydss_results.py
+-rw-r--r--   0        0        0     9438 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/registry.py
+-rw-r--r--   0        0        0    38847 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/simulation_input_models.py
+-rw-r--r--   0        0        0     8528 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/storage_filters.py
+-rw-r--r--   0        0        0    15736 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/thermal_metrics.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/unitDefinations.py
+-rw-r--r--   0        0        0    19454 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/value_storage.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/Extensions/MonteCarlo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/Extensions/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/ProfileManager/ProfileInterface.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/ProfileManager/__init__.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/ProfileManager/base_definitions.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/ProfileManager/common.py
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/ProfileManager/hooks/MongoDB.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/ProfileManager/hooks/__init__.py
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/ProfileManager/hooks/h5.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/__init__.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/endpoints.yaml
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/logging.yaml
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/server.py
+-rw-r--r--   0        0        0    31947 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/schema/PyDSS.v1.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/schema/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/RunServer.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/config.yaml
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/app/DataWriter.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/app/HDF5.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/app/JSON_writer.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/app/Tester.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/app/__init__.py
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/app/pydss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/web/__init__.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/web/create_schema.py
+-rw-r--r--   0        0        0    22395 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/web/handler.py
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/api/src/web/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/apps/__init__.py
+-rw-r--r--   0        0        0    16311 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/apps/data_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/add_post_process.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/add_scenario.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/controllers.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/convert.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/create_project.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/edit_scenario.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/export.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/extract.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/pydss.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/reports.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/run.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/cli/run_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/plots.toml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/ExportLists/ExportMode-byClass.toml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/ExportLists/ExportMode-byElement.toml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/ExportLists/Exports.toml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/ExportLists/Subscriptions.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/ExportLists/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/Monte_Carlo/MonteCarloSettings.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/Monte_Carlo/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/FaultController.toml
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/GenController.toml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/MotorStall.toml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/MotorStallSimple.toml
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/PvController.toml
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/PvDynamic.toml
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/PvFrequencyRideThru.toml
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/PvVoltageRideThru.toml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/SocketController.toml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/StorageController.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/ThermostaticLoad.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/xfmrController.toml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/FrequencySweep.toml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/Histogram.toml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/NetworkGraph.toml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/Table.toml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/ThreeDim.toml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/TimeSeries.toml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/Topology.toml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/VoltageDistance.toml
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/XY.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/defaults/pyPlotList/__init__.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/modes/Dynamic.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/modes/QSTS.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/modes/Snapshot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/modes/__init__.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/modes/solver_base.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/__init__.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/enumerations.py
+-rw-r--r--   0        0        0    16226 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/models.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/pyController.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/pyControllerAbstract.py
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/FaultController.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/GenController.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/MotorStall.py
+-rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/MotorStallBackup.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/MotorStallSimple.py
+-rw-r--r--   0        0        0    12715 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/PvController.py
+-rw-r--r--   0        0        0    13552 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/PvDynamic.py
+-rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/PvFrequencyRideThru.py
+-rw-r--r--   0        0        0    20327 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/PvVoltageRideThru.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/SocketController.py
+-rw-r--r--   0        0        0    22893 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/StorageController.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/ThermostaticLoad.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/__init__.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/xfmrController.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/Settings/PvControllers.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/Settings/__init__.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyControllers/Settings/PvControllers.toml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyPostprocessor/__init__.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyPostprocessor/pyPostprocess.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyPostprocessor/pyPostprocessAbstract.py
+-rw-r--r--   0        0        0    19150 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py
+-rw-r--r--   0        0        0    23379 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyPostprocessor/PostprocessScripts/EdLiFoControl.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyPostprocessor/PostprocessScripts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/__init__.py
+-rw-r--r--   0        0        0    20117 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/reports/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/reports/capacitor_change_count.py
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/reports/feeder_losses.py
+-rw-r--r--   0        0        0    14649 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/reports/pv_reports.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/reports/reg_control_tap_number_change_count.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/reports/reports.py
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/reports/thermal_metrics.py
+-rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/reports/voltage_metrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/utils/__init__.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/utils/dataframe_utils.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/utils/dss_utils.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/utils/pydss_utils.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/utils/simulation_utils.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/utils/timing_utils.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/src/pydss/utils/utils.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/.gitignore
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/LICENSE
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 nrel_pydss-3.1.6/PKG-INFO
```

### Comparing `nrel_pydss-3.1.5/src/pydss/ResultData.py` & `nrel_pydss-3.1.6/src/pydss/ResultData.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/SolveMode.py` & `nrel_pydss-3.1.6/src/pydss/SolveMode.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/common.py` & `nrel_pydss-3.1.6/src/pydss/common.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/config_data.py` & `nrel_pydss-3.1.6/src/pydss/config_data.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/controllers.py` & `nrel_pydss-3.1.6/src/pydss/controllers.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/dataset_buffer.py` & `nrel_pydss-3.1.6/src/pydss/dataset_buffer.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/dssBus.py` & `nrel_pydss-3.1.6/src/pydss/dssBus.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/dssCircuit.py` & `nrel_pydss-3.1.6/src/pydss/dssCircuit.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/dssElement.py` & `nrel_pydss-3.1.6/src/pydss/dssElement.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/dssInstance.py` & `nrel_pydss-3.1.6/src/pydss/dssInstance.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/dssObjectBase.py` & `nrel_pydss-3.1.6/src/pydss/dssObjectBase.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/dssTransformer.py` & `nrel_pydss-3.1.6/src/pydss/dssTransformer.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/element_fields.py` & `nrel_pydss-3.1.6/src/pydss/element_fields.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/element_options.py` & `nrel_pydss-3.1.6/src/pydss/element_options.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/exceptions.py` & `nrel_pydss-3.1.6/src/pydss/exceptions.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/export_list_reader.py` & `nrel_pydss-3.1.6/src/pydss/export_list_reader.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/get_snapshot_timepoints.py` & `nrel_pydss-3.1.6/src/pydss/get_snapshot_timepoints.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/helics_interface.py` & `nrel_pydss-3.1.6/src/pydss/helics_interface.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/metrics.py` & `nrel_pydss-3.1.6/src/pydss/metrics.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/naerm.py` & `nrel_pydss-3.1.6/src/pydss/naerm.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/node_voltage_metrics.py` & `nrel_pydss-3.1.6/src/pydss/node_voltage_metrics.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyContrReader.py` & `nrel_pydss-3.1.6/src/pydss/pyContrReader.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyDSS.py` & `nrel_pydss-3.1.6/src/pydss/pyDSS.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyResults.py` & `nrel_pydss-3.1.6/src/pydss/pyResults.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pydss_fs_interface.py` & `nrel_pydss-3.1.6/src/pydss/pydss_fs_interface.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pydss_project.py` & `nrel_pydss-3.1.6/src/pydss/pydss_project.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pydss_results.py` & `nrel_pydss-3.1.6/src/pydss/pydss_results.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/registry.py` & `nrel_pydss-3.1.6/src/pydss/registry.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/simulation_input_models.py` & `nrel_pydss-3.1.6/src/pydss/simulation_input_models.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/storage_filters.py` & `nrel_pydss-3.1.6/src/pydss/storage_filters.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/thermal_metrics.py` & `nrel_pydss-3.1.6/src/pydss/thermal_metrics.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/unitDefinations.py` & `nrel_pydss-3.1.6/src/pydss/unitDefinations.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/value_storage.py` & `nrel_pydss-3.1.6/src/pydss/value_storage.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/Extensions/MonteCarlo.py` & `nrel_pydss-3.1.6/src/pydss/Extensions/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/ProfileManager/ProfileInterface.py` & `nrel_pydss-3.1.6/src/pydss/ProfileManager/ProfileInterface.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/ProfileManager/base_definitions.py` & `nrel_pydss-3.1.6/src/pydss/ProfileManager/base_definitions.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/ProfileManager/hooks/MongoDB.py` & `nrel_pydss-3.1.6/src/pydss/ProfileManager/hooks/MongoDB.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         self.client = MongoClient("mongodb://user:password@bmather-131003:27017/?authSource=admin&readPreference=primary&appname=MongoDB%20Compass&ssl=false&connect=false")
         self.db_name = usersettings["database"]
         self.db = self.client[usersettings["database"]]
         self.collections = self.db.collection_names()
         self.mapping = usersettings["mapping"]
         #self.one_Time_fix(usersettings['collection'])
         self.setup_profiles()
-        #quit()
         pass
 
     def one_Time_fix(self, collection_name):
         self.logger.info("Creating aggregated load profiles")
         C = self.db[collection_name]
         cursor = C.find({"name": "customer_metadata"})
         customer_metadata = cursor.next()
```

### Comparing `nrel_pydss-3.1.5/src/pydss/ProfileManager/hooks/h5.py` & `nrel_pydss-3.1.6/src/pydss/ProfileManager/hooks/h5.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/endpoints.yaml` & `nrel_pydss-3.1.6/src/pydss/api/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/logging.yaml` & `nrel_pydss-3.1.6/src/pydss/api/logging.yaml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/server.py` & `nrel_pydss-3.1.6/src/pydss/api/server.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/schema/PyDSS.v1.json` & `nrel_pydss-3.1.6/src/pydss/api/schema/PyDSS.v1.json`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/src/app/DataWriter.py` & `nrel_pydss-3.1.6/src/pydss/api/src/app/DataWriter.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/src/app/HDF5.py` & `nrel_pydss-3.1.6/src/pydss/api/src/app/HDF5.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/src/app/JSON_writer.py` & `nrel_pydss-3.1.6/src/pydss/api/src/app/JSON_writer.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/src/app/Tester.py` & `nrel_pydss-3.1.6/src/pydss/api/src/app/Tester.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/src/app/pydss.py` & `nrel_pydss-3.1.6/src/pydss/api/src/app/pydss.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/src/web/handler.py` & `nrel_pydss-3.1.6/src/pydss/api/src/web/handler.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/api/src/web/parser.py` & `nrel_pydss-3.1.6/src/pydss/api/src/web/parser.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/apps/data_viewer.py` & `nrel_pydss-3.1.6/src/pydss/apps/data_viewer.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/add_post_process.py` & `nrel_pydss-3.1.6/src/pydss/cli/add_post_process.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/add_scenario.py` & `nrel_pydss-3.1.6/src/pydss/cli/add_scenario.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/controllers.py` & `nrel_pydss-3.1.6/src/pydss/cli/controllers.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/convert.py` & `nrel_pydss-3.1.6/src/pydss/cli/convert.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/create_project.py` & `nrel_pydss-3.1.6/src/pydss/cli/create_project.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/edit_scenario.py` & `nrel_pydss-3.1.6/src/pydss/cli/edit_scenario.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/export.py` & `nrel_pydss-3.1.6/src/pydss/cli/export.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/extract.py` & `nrel_pydss-3.1.6/src/pydss/cli/extract.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/pydss.py` & `nrel_pydss-3.1.6/src/pydss/cli/pydss.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/reports.py` & `nrel_pydss-3.1.6/src/pydss/cli/reports.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/run.py` & `nrel_pydss-3.1.6/src/pydss/cli/run.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/cli/run_server.py` & `nrel_pydss-3.1.6/src/pydss/cli/run_server.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/defaults/ExportLists/ExportMode-byClass.toml` & `nrel_pydss-3.1.6/src/pydss/defaults/ExportLists/ExportMode-byClass.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/defaults/ExportLists/Exports.toml` & `nrel_pydss-3.1.6/src/pydss/defaults/ExportLists/Exports.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/PvController.toml` & `nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/PvController.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/PvDynamic.toml` & `nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/PvDynamic.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/PvFrequencyRideThru.toml` & `nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/PvFrequencyRideThru.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/PvVoltageRideThru.toml` & `nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/PvVoltageRideThru.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/defaults/pyControllerList/StorageController.toml` & `nrel_pydss-3.1.6/src/pydss/defaults/pyControllerList/StorageController.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/modes/Dynamic.py` & `nrel_pydss-3.1.6/src/pydss/modes/Dynamic.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/modes/QSTS.py` & `nrel_pydss-3.1.6/src/pydss/modes/QSTS.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/modes/Snapshot.py` & `nrel_pydss-3.1.6/src/pydss/modes/Snapshot.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/modes/solver_base.py` & `nrel_pydss-3.1.6/src/pydss/modes/solver_base.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/enumerations.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/enumerations.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/models.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/models.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/pyController.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/pyController.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/FaultController.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/FaultController.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/GenController.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/GenController.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/MotorStall.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/MotorStall.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/MotorStallBackup.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/MotorStallBackup.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/MotorStallSimple.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/MotorStallSimple.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/PvController.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/PvController.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/PvDynamic.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/PvDynamic.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/PvFrequencyRideThru.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/PvFrequencyRideThru.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/PvVoltageRideThru.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/PvVoltageRideThru.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,23 +398,23 @@
     def _trip(self, Deadtime, time2Pmax, forceTrip, permissive_to_trip=False):
         
         u_in = self._controlled_element.GetVariable('VoltagesMagAng')[::2]
         u_base = self._controlled_element.sBus[0].GetVariable('kVBase') * 1000
         u_in = max(u_in) / u_base if self._voltage_calc_mode == VoltageCalcModes.MAX else sum(u_in) / (u_base * len(u_in))
 
         if self._is_connected or forceTrip:
-            self._controlled_element.SetParameter('enabled', False)
+            self._controlled_element.SetParameter('kw', 0)
 
             self._is_connected = False
             self._tripped_start_time = self.__dss_solver.GetDateTime()
             self._tripped_p_max_delay = time2Pmax
             self._tripped_dead_time = Deadtime
             
         elif permissive_to_trip:
-            self._controlled_element.SetParameter('enabled', False)
+            self._controlled_element.SetParameter('kw', 0)
 
             self._is_connected = False
             self._tripped_start_time = self.__dss_solver.GetDateTime()
             self._tripped_p_max_delay = time2Pmax
             self._tripped_dead_time = Deadtime
         return
```

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/SocketController.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/SocketController.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/StorageController.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/StorageController.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/ThermostaticLoad.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/ThermostaticLoad.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/xfmrController.py` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/xfmrController.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Controllers/Settings/PvControllers.toml` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Controllers/Settings/PvControllers.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyControllers/Settings/PvControllers.toml` & `nrel_pydss-3.1.6/src/pydss/pyControllers/Settings/PvControllers.toml`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyPostprocessor/pyPostprocess.py` & `nrel_pydss-3.1.6/src/pydss/pyPostprocessor/pyPostprocess.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyPostprocessor/pyPostprocessAbstract.py` & `nrel_pydss-3.1.6/src/pydss/pyPostprocessor/pyPostprocessAbstract.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py` & `nrel_pydss-3.1.6/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyPostprocessor/PostprocessScripts/EdLiFoControl.py` & `nrel_pydss-3.1.6/src/pydss/pyPostprocessor/PostprocessScripts/EdLiFoControl.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py` & `nrel_pydss-3.1.6/src/pydss/pyPostprocessor/PostprocessScripts/DERMSOptimizer_helper_modules/opt_funcs.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/reports/capacitor_change_count.py` & `nrel_pydss-3.1.6/src/pydss/reports/capacitor_change_count.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/reports/feeder_losses.py` & `nrel_pydss-3.1.6/src/pydss/reports/feeder_losses.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/reports/pv_reports.py` & `nrel_pydss-3.1.6/src/pydss/reports/pv_reports.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/reports/reg_control_tap_number_change_count.py` & `nrel_pydss-3.1.6/src/pydss/reports/reg_control_tap_number_change_count.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/reports/reports.py` & `nrel_pydss-3.1.6/src/pydss/reports/reports.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/reports/thermal_metrics.py` & `nrel_pydss-3.1.6/src/pydss/reports/thermal_metrics.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/reports/voltage_metrics.py` & `nrel_pydss-3.1.6/src/pydss/reports/voltage_metrics.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/utils/dataframe_utils.py` & `nrel_pydss-3.1.6/src/pydss/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/utils/dss_utils.py` & `nrel_pydss-3.1.6/src/pydss/utils/dss_utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/utils/pydss_utils.py` & `nrel_pydss-3.1.6/src/pydss/utils/pydss_utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/utils/simulation_utils.py` & `nrel_pydss-3.1.6/src/pydss/utils/simulation_utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/utils/timing_utils.py` & `nrel_pydss-3.1.6/src/pydss/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/src/pydss/utils/utils.py` & `nrel_pydss-3.1.6/src/pydss/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/.gitignore` & `nrel_pydss-3.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/LICENSE` & `nrel_pydss-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nrel_pydss-3.1.5/pyproject.toml` & `nrel_pydss-3.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "NREL-pydss"
-version = "3.1.5"
+version = "3.1.6"
 description = "A high-level python interface for OpenDSS"
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">=3.9"
 authors = [
     { name = "Aadil Latif", email = "Aadil.Latif@nrel.gov" },
 ]
```

### Comparing `nrel_pydss-3.1.5/PKG-INFO` & `nrel_pydss-3.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NREL-pydss
-Version: 3.1.5
+Version: 3.1.6
 Summary: A high-level python interface for OpenDSS
 Project-URL: Homepage, http://www.github.com/nrel/pydss
 Author-email: Aadil Latif <Aadil.Latif@nrel.gov>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

