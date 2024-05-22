# Comparing `tmp/tactics2d-0.1.6.tar.gz` & `tmp/tactics2d-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tactics2d-0.1.6.tar", last modified: Sun Mar 31 17:41:48 2024, max compression
+gzip compressed data, was "tactics2d-0.1.7.tar", last modified: Wed May 22 12:00:34 2024, max compression
```

## Comparing `tactics2d-0.1.6.tar` & `tactics2d-0.1.7.tar`

### file list

```diff
@@ -1,152 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:48.009847 tactics2d-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-31 17:41:39.000000 tactics2d-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-31 17:41:39.000000 tactics2d-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    50707 2024-03-31 17:41:48.005847 tactics2d-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-03-31 17:41:39.000000 tactics2d-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-31 17:41:39.000000 tactics2d-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-31 17:41:39.000000 tactics2d-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 17:41:48.009847 tactics2d-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 17:41:39.000000 tactics2d-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.985847 tactics2d-0.1.6/tactics2d/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.985847 tactics2d-0.1.6/tactics2d/dataset_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18486 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/map.config
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/parse_argoverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/parse_dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/parse_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/parse_levelx.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/parse_ngsim.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/parse_nuplan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/parse_womd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.985847 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.989847 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14253 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/compressed_lidar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    69858 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20066 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/keypoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    28040 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    51233 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/map_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24102 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/scenario_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/vector_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.989847 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/compressed_lidar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/keypoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/map_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/scenario_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/vector_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.989847 tactics2d-0.1.6/tactics2d/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17544 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/envs/parking.py
--rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/envs/racing.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/envs/urban.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.989847 tactics2d-0.1.6/tactics2d/map/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.993847 tactics2d-0.1.6/tactics2d/map/converter/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/converter/gpkg2osm.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/converter/xodr2osm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.993847 tactics2d-0.1.6/tactics2d/map/element/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/element/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/element/junction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/element/lane.py
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/element/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/element/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/element/regulatory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/element/roadline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.993847 tactics2d-0.1.6/tactics2d/map/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17467 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/generator/generate_parking_lot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/generator/generate_racing_track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.993847 tactics2d-0.1.6/tactics2d/map/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/parser/fix_osm.py
--rw-r--r--   0 runner    (1001) docker     (127)    21644 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/parser/parse_osm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19920 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/map/parser/parse_xodr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.993847 tactics2d-0.1.6/tactics2d/math/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.993847 tactics2d-0.1.6/tactics2d/math/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/geometry/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/geometry/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.997847 tactics2d-0.1.6/tactics2d/math/interpolate/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/interpolate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/interpolate/b_spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/interpolate/bezier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/interpolate/cubic_spline.py
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/interpolate/dubins.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/interpolate/reeds_shepp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/math/interpolate/spiral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.997847 tactics2d-0.1.6/tactics2d/participant/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.997847 tactics2d-0.1.6/tactics2d/participant/element/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/element/cyclist.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/element/other.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/element/participant_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/element/participant_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/element/pedestrian.py
--rw-r--r--   0 runner    (1001) docker     (127)    15969 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/element/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/guess_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:47.997847 tactics2d-0.1.6/tactics2d/participant/trajectory/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/trajectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/trajectory/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/trajectory/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)    42987 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/participant/trajectory_classifier.m
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:48.001847 tactics2d-0.1.6/tactics2d/physics/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/physics/physics_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/physics/point_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/physics/single_track_drift.py
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/physics/single_track_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11893 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/physics/single_track_kinematics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:48.001847 tactics2d-0.1.6/tactics2d/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/sensor/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/sensor/lidar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/sensor/render_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/sensor/render_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/sensor/sensor_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:48.001847 tactics2d-0.1.6/tactics2d/traffic/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:48.001847 tactics2d-0.1.6/tactics2d/traffic/event_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/arrival.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/event_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/no_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/off_lane.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/off_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/out_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/event_detection/time_exceed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/scenario_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tactics2d/traffic/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:48.005847 tactics2d-0.1.6/tactics2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50707 2024-03-31 17:41:47.000000 tactics2d-0.1.6/tactics2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-03-31 17:41:47.000000 tactics2d-0.1.6/tactics2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 17:41:47.000000 tactics2d-0.1.6/tactics2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-31 17:41:47.000000 tactics2d-0.1.6/tactics2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-31 17:41:47.000000 tactics2d-0.1.6/tactics2d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:48.005847 tactics2d-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_dataset_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_map_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_map_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_math_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)    19275 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:39.000000 tactics2d-0.1.6/test/test_traffic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:48.005847 tactics2d-0.1.6/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tutorial/action_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tutorial/rs_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tutorial/train_parking_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-03-31 17:41:39.000000 tactics2d-0.1.6/tutorial/train_racing_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.635365 tactics2d-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 12:00:26.000000 tactics2d-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 12:00:26.000000 tactics2d-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    50707 2024-05-22 12:00:34.635365 tactics2d-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-05-22 12:00:26.000000 tactics2d-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.611365 tactics2d-0.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.615365 tactics2d-0.1.7/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-22 12:00:26.000000 tactics2d-0.1.7/docs/tutorial/train_racing_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 12:00:26.000000 tactics2d-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 12:00:26.000000 tactics2d-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:00:34.635365 tactics2d-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:00:26.000000 tactics2d-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.615365 tactics2d-0.1.7/tactics2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.615365 tactics2d-0.1.7/tactics2d/dataset_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18486 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/map.config
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/parse_argoverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/parse_dlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/parse_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/parse_levelx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/parse_ngsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/parse_nuplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/parse_womd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.615365 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.619365 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14253 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/compressed_lidar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69858 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20066 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/keypoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28040 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51233 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/map_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24102 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/scenario_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/vector_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.619365 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/compressed_lidar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/keypoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/map_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/scenario_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/vector_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.619365 tactics2d-0.1.7/tactics2d/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18914 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/envs/parking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/envs/racing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/envs/urban.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.619365 tactics2d-0.1.7/tactics2d/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.619365 tactics2d-0.1.7/tactics2d/map/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/converter/gpkg2osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/converter/xodr2osm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.623365 tactics2d-0.1.7/tactics2d/map/element/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/element/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/element/junction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/element/lane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/element/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/element/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/element/regulatory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/element/roadline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.623365 tactics2d-0.1.7/tactics2d/map/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19008 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/generator/generate_parking_lot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/generator/generate_racing_track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.623365 tactics2d-0.1.7/tactics2d/map/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/parser/fix_osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21622 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/parser/parse_osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22457 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/map/parser/parse_xodr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.623365 tactics2d-0.1.7/tactics2d/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.623365 tactics2d-0.1.7/tactics2d/math/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/geometry/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/geometry/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.623365 tactics2d-0.1.7/tactics2d/math/interpolate/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/interpolate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/interpolate/b_spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/interpolate/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/interpolate/cubic_spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/interpolate/dubins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/interpolate/reeds_shepp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/math/interpolate/spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.627365 tactics2d-0.1.7/tactics2d/participant/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.627365 tactics2d-0.1.7/tactics2d/participant/element/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/element/cyclist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/element/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/element/participant_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/element/participant_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/element/pedestrian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15969 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/element/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/guess_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.627365 tactics2d-0.1.7/tactics2d/participant/trajectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/trajectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/trajectory/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/trajectory/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42987 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/participant/trajectory_classifier.m
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.627365 tactics2d-0.1.7/tactics2d/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/physics/physics_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/physics/point_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/physics/single_track_drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/physics/single_track_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/physics/single_track_kinematics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.631365 tactics2d-0.1.7/tactics2d/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/sensor/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12091 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/sensor/lidar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/sensor/render_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/sensor/render_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/sensor/sensor_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.631365 tactics2d-0.1.7/tactics2d/traffic/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.631365 tactics2d-0.1.7/tactics2d/traffic/event_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/arrival.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/event_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/no_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/off_lane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/off_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/out_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/event_detection/time_exceed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/scenario_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 12:00:26.000000 tactics2d-0.1.7/tactics2d/traffic/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.635365 tactics2d-0.1.7/tactics2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50707 2024-05-22 12:00:34.000000 tactics2d-0.1.7/tactics2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-22 12:00:34.000000 tactics2d-0.1.7/tactics2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:00:34.000000 tactics2d-0.1.7/tactics2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 12:00:34.000000 tactics2d-0.1.7/tactics2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 12:00:34.000000 tactics2d-0.1.7/tactics2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:34.635365 tactics2d-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_dataset_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_map_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_map_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_math_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19220 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:00:26.000000 tactics2d-0.1.7/test/test_traffic.py
```

### Comparing `tactics2d-0.1.6/LICENSE` & `tactics2d-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/PKG-INFO` & `tactics2d-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tactics2d
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tactics2D: A Reinforcement Learning Environment Library with Generative Scenarios for Driving Decision-making
 Author-email: Yueyuan Li <rowena.academic@gmail.com>
 Maintainer-email: Yueyuan Li <rowena.academic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `tactics2d-0.1.6/README.md` & `tactics2d-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/pyproject.toml` & `tactics2d-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tactics2d"
-version = "0.1.6"
+version = "0.1.7"
 description = "Tactics2D: A Reinforcement Learning Environment Library with Generative Scenarios for Driving Decision-making"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { file = "LICENSE" }
 requires-python = ">= 3.8"
 keywords = ["reinforcement-learning", "environment", "simulator", "decision-making", "traffic-behavior"]
 authors = [
     { name = "Yueyuan Li", email = "rowena.academic@gmail.com" }
```

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/__init__.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/map.config` & `tactics2d-0.1.7/tactics2d/dataset_parser/map.config`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/parse_argoverse.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/parse_argoverse.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/parse_dlp.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/parse_dlp.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/parse_interaction.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/parse_interaction.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/parse_levelx.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/parse_levelx.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/parse_nuplan.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/parse_nuplan.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/parse_womd.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/parse_womd.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/compressed_lidar_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/compressed_lidar_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/dataset_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/keypoint_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/keypoint_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/label_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/label_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/map_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/map_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/scenario_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/scenario_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb2/vector_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb2/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/compressed_lidar_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/compressed_lidar_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/dataset_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/keypoint_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/keypoint_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/label_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/label_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/map_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/map_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/scenario_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/scenario_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/dataset_parser/womd_proto/pb3/vector_pb2.py` & `tactics2d-0.1.7/tactics2d/dataset_parser/womd_proto/pb3/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/envs/parking.py` & `tactics2d-0.1.7/tactics2d/envs/parking.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Arrival,
     NoAction,
     OutBound,
     StaticCollision,
     TimeExceed,
 )
 
-MAX_STEER = 0.75
+MAX_STEER = 0.524  # 0.75
 MAX_ACCEL = 2.0
 
 
 def truncate_angle(angle: float):
     """Truncate angle to [-pi, pi]"""
     while angle > np.pi:
         angle -= 2 * np.pi
@@ -137,14 +137,15 @@
                 np.array([self._max_steer, self._max_accel]),
                 dtype=np.float32,
             )
         else:
             self.action_space = spaces.Discrete(5)
 
         self._max_iou = -np.inf
+        self._min_dist_to_target = np.inf
 
         self.scenario_manager = self._ParkingScenarioManager(
             type_proportion, self.max_step, 100, self.render_fps, self.render_mode != "human"
         )
 
     def _get_reward(
         self, scenario_status: ScenarioStatus, traffic_status: TrafficStatus, iou: float
@@ -157,23 +158,41 @@
         ):
             reward = -1
         elif scenario_status == ScenarioStatus.OUT_BOUND:
             reward = -5
         elif scenario_status == ScenarioStatus.COMPLETED:
             reward = 5
         else:
-            time_penalty = -np.tanh(self.scenario_manager.cnt_step / self.max_step) * 0.1
+            time_penalty = -np.tanh(self.scenario_manager.cnt_step / self.max_step) * 0.001
             if self._max_iou == -np.inf:
                 iou_reward = iou if not iou is None else 0
             else:
                 iou_reward = iou - self._max_iou if not iou is None else 0
 
             reward = time_penalty + iou_reward
             self._max_iou = max(self._max_iou, iou) if not iou is None else self._max_iou
 
+            curr_dist_to_target = np.linalg.norm(
+                np.array(
+                    [
+                        self.scenario_manager.agent.current_state.x,
+                        self.scenario_manager.agent.current_state.y,
+                    ]
+                )
+                - np.array(
+                    [
+                        self.scenario_manager.target_area.geometry.centroid.x,
+                        self.scenario_manager.target_area.geometry.centroid.y,
+                    ]
+                )
+            )
+            if curr_dist_to_target < self._min_dist_to_target:
+                reward += (self._min_dist_to_target - curr_dist_to_target) * 0.1
+                self._min_dist_to_target = curr_dist_to_target
+
         return reward
 
     def _get_relative_pose(self, state):
         target_pose = np.array(
             [
                 self.scenario_manager.target_area.geometry.centroid.x,
                 self.scenario_manager.target_area.geometry.centroid.y,
@@ -190,19 +209,17 @@
         state_infos = dict()
         state_infos["lidar"] = observations[1]
         state_infos["state"] = state
         state_infos["target_area"] = self.scenario_manager.target_area
         state_infos["target_heading"] = self.scenario_manager.target_heading
         state_infos["traffic_status"] = traffic_status
         state_infos["scenario_status"] = scenario_status
-        (
-            state_infos["diff_position"],
-            state_infos["diff_angle"],
-            state_infos["diff_heading"],
-        ) = self._get_relative_pose(state)
+        (state_infos["diff_position"], state_infos["diff_angle"], state_infos["diff_heading"]) = (
+            self._get_relative_pose(state)
+        )
         return state_infos
 
     def step(self, action: Union[np.ndarray, int]):
         """This function takes a step in the environment.
 
         Args:
             action (Union[Tuple[float], int]): The action command for the agent vehicle.
@@ -231,18 +248,15 @@
             terminated = True
         elif (scenario_status != ScenarioStatus.NORMAL) or (traffic_status != TrafficStatus.NORMAL):
             truncated = True
 
         reward = self._get_reward(scenario_status, traffic_status, iou)
 
         infos = self._get_infos(
-            self.scenario_manager.agent.current_state,
-            observations,
-            scenario_status,
-            traffic_status,
+            self.scenario_manager.agent.current_state, observations, scenario_status, traffic_status
         )
 
         return observations[0], reward, terminated, truncated, infos
 
     def render(self):
         if self.render_mode == "human":
             self.scenario_manager.render()
@@ -264,22 +278,36 @@
         observations = self.scenario_manager.get_observation()
         infos = self._get_infos(
             self.scenario_manager.agent.current_state,
             observations,
             ScenarioStatus.NORMAL,
             TrafficStatus.NORMAL,
         )
+        self._min_dist_to_target = np.linalg.norm(
+            np.array(
+                [
+                    self.scenario_manager.agent.current_state.x,
+                    self.scenario_manager.agent.current_state.y,
+                ]
+            )
+            - np.array(
+                [
+                    self.scenario_manager.target_area.geometry.centroid.x,
+                    self.scenario_manager.target_area.geometry.centroid.y,
+                ]
+            )
+        )
 
         return observations[0], infos
 
     class _ParkingScenarioManager(ScenarioManager):
         _max_steer = MAX_STEER
         _max_accel = MAX_ACCEL
         _lidar_range = 20
-        _lidar_line = 120
+        _lidar_line = 360
         _window_size = (500, 500)
         _state_size = (200, 200)
 
         def __init__(
             self,
             type_proportion: float = 0.5,
             max_step: int = None,
@@ -291,15 +319,15 @@
 
             self.agent = Vehicle(id_=0)
             self.agent.load_from_template("medium_car")
             self.agent.physics_model = SingleTrackKinematics(
                 lf=self.agent.length / 2 - self.agent.front_overhang,
                 lr=self.agent.length / 2 - self.agent.rear_overhang,
                 steer_range=(-self._max_steer, self._max_steer),
-                speed_range=self.agent.speed_range,
+                speed_range=(-0.5, 0.5),
                 accel_range=(-self._max_accel, self._max_accel),
                 interval=self.step_size,
             )
             self.participants = {self.agent.id_: self.agent}
 
             self.map_ = Map(name="ParkingLot", scenario_type="parking")
             self.map_generator = ParkingLotGenerator(
@@ -338,15 +366,15 @@
             agent_pose = Polygon(self.agent.get_pose())
 
             is_time_exceed = self.status_checklist["time_exceed"].update()
             if is_time_exceed:
                 scenario_status = ScenarioStatus.TIME_EXCEEDED
                 return scenario_status, traffic_status, None
 
-            is_no_action = self.status_checklist["no_action"].update(action)
+            is_no_action = self.status_checklist["no_action"].update(agent_pose)
             if is_no_action:
                 traffic_status = ScenarioStatus.NO_ACTION
                 return scenario_status, traffic_status, None
 
             is_out_bound = self.status_checklist["out_bound"].update(agent_pose)
             if is_out_bound:
                 scenario_status = ScenarioStatus.OUT_BOUND
@@ -409,7 +437,12 @@
             self.status_checklist["time_exceed"].reset()
             self.status_checklist["no_action"].reset()
             self.status_checklist["out_bound"].reset(self.map_.boundary)
             self.status_checklist["collision"].reset(
                 [wall for wall in self.map_.areas.values() if wall.subtype != "target_area"]
             )
             self.status_checklist["completed"].reset(self.target_area)
+
+    def close(self):
+        """This function closes the environment."""
+        self.scenario_manager.render_manager.close()
+        super().close()
```

### Comparing `tactics2d-0.1.6/tactics2d/envs/racing.py` & `tactics2d-0.1.7/tactics2d/envs/racing.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             agent_pose = Polygon(self.agent.get_pose())
 
             is_time_exceed = self.status_checklist["time_exceed"].update()
             if is_time_exceed:
                 scenario_status = ScenarioStatus.TIME_EXCEEDED
                 return scenario_status, traffic_status
 
-            is_no_action = self.status_checklist["no_action"].update(action)
+            is_no_action = self.status_checklist["no_action"].update(agent_pose)
             if is_no_action:
                 traffic_status = ScenarioStatus.NO_ACTION
                 return scenario_status, traffic_status
 
             is_out_bound = self.status_checklist["out_bound"].update(agent_pose)
             if is_out_bound:
                 traffic_status = ScenarioStatus.OUT_BOUND
```

### Comparing `tactics2d-0.1.6/tactics2d/map/element/__init__.py` & `tactics2d-0.1.7/tactics2d/map/element/__init__.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/element/area.py` & `tactics2d-0.1.7/tactics2d/map/element/area.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/element/junction.py` & `tactics2d-0.1.7/tactics2d/map/element/junction.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/element/lane.py` & `tactics2d-0.1.7/tactics2d/map/element/lane.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/element/map.py` & `tactics2d-0.1.7/tactics2d/map/element/map.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/element/node.py` & `tactics2d-0.1.7/tactics2d/map/element/node.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/element/regulatory.py` & `tactics2d-0.1.7/tactics2d/map/element/regulatory.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/element/roadline.py` & `tactics2d-0.1.7/tactics2d/map/element/roadline.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/generator/generate_parking_lot.py` & `tactics2d-0.1.7/tactics2d/map/generator/generate_parking_lot.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,23 @@
         type_proportion (float): The proportion of "bay" parking scenario in all generated scenarios. It should be in the range of [0, 1]. If the input is out of the range, it will be clipped to the range. When it is 0, the generator only generates "parallel" parking scenarios. Defaults to 0.5.
         mode (str): The type of the parking scenario. It can be "bay" or "parallel". Defaults to None.
     """
 
     _origin = Point(0.0, 0.0)
     _scenario_size = 30.0
     _margin = 13.0
-    _dist_to_obstacle = (0.1, 1.0)
+    _dist_to_obstacle = (0.8, 1.6)
     _heading_distribution = {
-        "bay": (np.pi / 2, np.pi / 36, np.pi * 5 / 12, np.pi * 7 / 12),
-        "parallel": (0, np.pi / 36, -np.pi / 12, np.pi / 12),
+        "bay": (np.pi / 2, np.pi / 54, np.pi * 4 / 9, np.pi * 5 / 9),
+        "parallel": (0, np.pi / 54, -np.pi / 18, np.pi / 18),
     }
     _length = {"bay": 7.0, "parallel": 4.5}
     _vehicle_size = (5.3, 2.5)
+    _n_parking_lots_bay = 9
+    _n_parking_lots_parallel = 7
     _target_color = (0, 238, 118, 100)
 
     def __init__(
         self, vehicle_size: Tuple[float, float] = (5.3, 2.5), type_proportion: float = 0.5
     ):
         """Initialize the attributes in the class.
 
@@ -107,29 +109,27 @@
         if self.mode == "bay":
             y_min = -min(bottom_right[1], bottom_left[1]) + self._dist_to_obstacle[0]
         else:
             y_min = -min(bottom_right[1], top_right[1]) + self._dist_to_obstacle[0]
         center_point = Point(0.0, self._truncate_gaussian(y_min + 0.4, 0.2, y_min, y_min + 0.8))
 
         shape = self._get_bbox(center_point, heading, *self.vehicle_size)
-        area = Area(id_=0, geometry=shape, color=self._target_color)
+        area = Area(id_=0, geometry=shape, subtype="target_area", color=self._target_color)
 
         return area, heading
 
     def _get_back_wall(self) -> Area:
         wall_width = np.random.uniform(0.5, 1.5)
         wall_center = Point(self._origin.x, self._origin.y - wall_width / 2)
         shape = self._get_bbox(wall_center, 0, self._scenario_size, wall_width)
         obstacle = Area(id_="0000", type_="obstacle", geometry=shape)
 
         return obstacle
 
-    def _get_left_wall(
-        self, id_: int, target_area: Area, dist_to_obstacle: Tuple[float, float]
-    ) -> Area:
+    def _get_left_wall(self, id_: int, target_area: Area, dist_to_obstacle: np.ndarray) -> Area:
         _, top_left, bottom_left, bottom_right, _ = list(target_area.geometry.exterior.coords)
 
         wall_top_right = self._get_random_position(
             Point(top_left) if self.mode == "bay" else Point(bottom_left),
             (np.pi * 11 / 12, np.pi * 13 / 12),
             dist_to_obstacle,
         )
@@ -146,17 +146,15 @@
                 (self._origin.x - self._scenario_size / 2, self._origin.y),
                 (self._origin.x - self._scenario_size / 2, wall_top_right.y),
             ]
         )
         obstacle = Area(id_="%04d" % id_, type_="obstacle", geometry=shape)
         return obstacle
 
-    def _get_right_wall(
-        self, id_: int, target_area: Area, dist_to_obstacle: Tuple[float, float]
-    ) -> Area:
+    def _get_right_wall(self, id_: int, target_area: Area, dist_to_obstacle: np.ndarray) -> Area:
         top_right, top_left, _, bottom_right, _ = list(target_area.geometry.exterior.coords)
 
         wall_bottom_left = self._get_random_position(
             Point(bottom_right) if self.mode == "bay" else Point(top_right),
             (-np.pi * 1 / 12, np.pi * 1 / 12),
             dist_to_obstacle,
         )
@@ -174,15 +172,15 @@
                 wall_top_left,
             ]
         )
         obstacle = Area(id_="%04d" % id_, type_="obstacle", geometry=shape)
         return obstacle
 
     def _get_side_vehicle(
-        self, id_: int, dist_to_obstacle: Tuple[float, float], left_side: bool = True
+        self, id_: int, dist_to_obstacle: np.ndarray, left_side: bool = True
     ) -> Area:
         heading = self._truncate_gaussian(*self._heading_distribution[self.mode])
 
         side_factor = -1 if left_side else 1
         # get x coordinate of the side vehicle
         if self.mode == "bay":
             x = self._origin.x + side_factor * (
@@ -268,39 +266,67 @@
             # get the target area
             target_area, target_heading = self._get_target_area()
             map_.areas = {target_area.id_: target_area}
 
             back_wall = self._get_back_wall()
 
             # generate a wall / static vehicle as an obstacle on the left side of the target area
-            dist_to_obstacle = (self._dist_to_obstacle[0] + 0.1, self._dist_to_obstacle[1])
-            left_obstacle = (
-                self._get_side_vehicle(1, dist_to_obstacle)
-                if np.random.uniform() < 0.5
-                else self._get_left_wall(1, target_area, dist_to_obstacle)
+            dist_to_obstacle = np.array(
+                (self._dist_to_obstacle[0] + 0.1, self._dist_to_obstacle[1])
             )
+            if np.random.uniform() < 0.2:
+                left_obstacle = self._get_left_wall(1, target_area, dist_to_obstacle)
+            else:
+                left_obstacle = self._get_side_vehicle(1, dist_to_obstacle, True)
+                # generate other vehicle on left
+                next_vehicle_distance = (
+                    self.vehicle_size[1] if self.mode == "bay" else self.vehicle_size[0]
+                )
+                parking_lot_num = (
+                    self._n_parking_lots_bay
+                    if self.mode == "bay"
+                    else self._n_parking_lots_parallel
+                )
+                for i in range(
+                    (parking_lot_num - 3) // 2
+                ):  # 3 is the number of obstacles already generated
+                    dist_to_obstacle += next_vehicle_distance + self._dist_to_obstacle[0]
+                    left_obstacle_ = self._get_side_vehicle(2 * i + 3, dist_to_obstacle, True)
+                    obstacles.append(left_obstacle_)
 
             # generate a wall / static vehicle as an obstacle on the right side of the target area
             dist_target_to_left_obstacle = target_area.geometry.distance(left_obstacle.geometry)
             if self.mode == "bay":
                 min_dist_to_obstacle = (
                     max(0.85 - dist_target_to_left_obstacle, 0) + self._dist_to_obstacle[0]
                 )
             else:
                 min_dist_to_obstacle = (
                     max(0.25 * self.vehicle_size[0] - dist_target_to_left_obstacle, 0)
                     + self._dist_to_obstacle[0]
                 )
-            dist_to_obstacle = (min_dist_to_obstacle, self._dist_to_obstacle[1])
 
-            right_obstacle = (
-                self._get_side_vehicle(2, dist_to_obstacle, False)
-                if np.random.uniform() < 0.5
-                else self._get_right_wall(2, target_area, dist_to_obstacle)
-            )
+            dist_to_obstacle = np.array((min_dist_to_obstacle, self._dist_to_obstacle[1]))
+            if np.random.uniform() < 0.2:
+                right_obstacle = self._get_right_wall(2, target_area, dist_to_obstacle)
+            else:
+                right_obstacle = self._get_side_vehicle(2, dist_to_obstacle, False)
+                # generate other vehicle on right
+                next_vehicle_distance = (
+                    self.vehicle_size[1] if self.mode == "bay" else self.vehicle_size[0]
+                )
+                parking_lot_num = (
+                    self._n_parking_lots_bay
+                    if self.mode == "bay"
+                    else self._n_parking_lots_parallel
+                )
+                for i in range((parking_lot_num - 3) // 2):
+                    dist_to_obstacle += next_vehicle_distance + self._dist_to_obstacle[0]
+                    right_obstacle_ = self._get_side_vehicle(2 * i + 4, dist_to_obstacle, False)
+                    obstacles.append(right_obstacle_)
 
             dist_target_to_right = target_area.geometry.distance(right_obstacle.geometry)
             valid_obstacles = self._verify_obstacles(
                 target_area,
                 [back_wall, left_obstacle, right_obstacle],
                 (dist_target_to_left_obstacle, dist_target_to_right),
             )
@@ -341,15 +367,15 @@
                 self._origin.x + self._scenario_size / 2,
             )
             y_range = (
                 y_max_obstacle + self._length[self.mode] + 2,
                 y_max_obstacle + self._length[self.mode] + 6,
             )
 
-            id_ = 3
+            id_ = len(obstacles) + 1
             for _ in range(3):
                 x = np.random.uniform(*x_range)
                 y = np.random.uniform(*y_range)
                 heading = np.random.uniform() * 2 * np.pi
                 shape = np.array(
                     list(self._get_bbox(Point(x, y), heading, *self.vehicle_size).exterior.coords)[
                         :4
@@ -359,17 +385,15 @@
 
                 if Polygon(bbox).contains(shape):
                     obstacle = Area(id_="%04d" % id_, type_="obstacle", geometry=shape)
                     obstacles.append(obstacle)
                     id_ += 1
 
         # randomly drop the obstacles
-        for obstacle in obstacles:
-            if np.random.uniform() < 0.0:
-                obstacles.remove(obstacle)
+        obstacles = [obstacle for obstacle in obstacles if np.random.uniform() >= 0.05]
 
         # store obstacles in map
         for obstacle in obstacles:
             map_.add_area(obstacle)
 
         # get the start state
         valid_start_state = False
```

### Comparing `tactics2d-0.1.6/tactics2d/map/generator/generate_racing_track.py` & `tactics2d-0.1.7/tactics2d/map/generator/generate_racing_track.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/parser/fix_osm.py` & `tactics2d-0.1.7/tactics2d/map/parser/fix_osm.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/map/parser/parse_osm.py` & `tactics2d-0.1.7/tactics2d/map/parser/parse_osm.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         tags = dict()
         tags["custom_tags"] = dict()
 
         directly_save = {
             "subtype",
             "color",
             "width",
-            "height",
             "location",
             "inferred_participants",
             "speed_limit",
         }
         bool_tags = {"temporary", "speed_limit_mandatory", "dynamic", "fallback", "oneway"}
 
         for tag in xml_node.findall("tag"):
```

### Comparing `tactics2d-0.1.6/tactics2d/map/parser/parse_xodr.py` & `tactics2d-0.1.7/tactics2d/map/parser/parse_xodr.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # @Description: This file defines a class for parsing the OpenDRIVE map format.
 # @Author: Yueyuan Li
 # @Version: 1.0.0
 
 
 import logging
 import xml.etree.ElementTree as ET
+from copy import deepcopy
 from typing import Tuple, Union
 
 import numpy as np
 from pyproj import CRS
 from shapely.affinity import affine_transform, rotate
 from shapely.geometry import LineString, Point, Polygon
 
@@ -61,24 +62,38 @@
         "solid solid": "solid_solid",
         "solid": "solid",
     }
 
     def __init__(self):
         self.id_counter = 0
 
+    def get_headings(self, points):
+        diff = np.diff(np.array(points), axis=0)
+        headings = np.arctan2(diff[:, 1], diff[:, 0]).tolist()
+        headings.append(headings[-1])
+        return headings
+
     def _get_line(self, xml_node: ET.Element) -> list:
         x_start = float(xml_node.attrib["x"])
         y_start = float(xml_node.attrib["y"])
         heading = float(xml_node.attrib["hdg"])
         length = float(xml_node.attrib["length"])
 
-        x_end = x_start + length * np.cos(heading)
-        y_end = y_start + length * np.sin(heading)
+        points = [(x_start, y_start)]
+
+        if length > 0.1:
+            n_interpolate = int(length / 0.1)
 
-        return [(x_start, y_start), (x_end, y_end)]
+            for i in np.linspace(0.1, length, n_interpolate - 1):
+                x_end = x_start + i * np.cos(heading)
+                y_end = y_start + i * np.sin(heading)
+                points.append((x_end, y_end))
+
+        points.append((x_start + length * np.cos(heading), y_start + length * np.sin(heading)))
+        return points
 
     def _get_spiral(self, xml_node: ET.Element) -> list:
         x_start = float(xml_node.attrib["x"])
         y_start = float(xml_node.attrib["y"])
         heading = float(xml_node.attrib["hdg"])
         length = float(xml_node.attrib["length"])
         curv_start = float(xml_node.find("spiral").attrib["curvStart"])
@@ -86,38 +101,37 @@
 
         if length < 0.1:  # TODO: check the threshold/precision 0.1
             points = [(x_start, y_start)]
         else:
             gamma = (curv_end - curv_start) / length
             points = Spiral.get_spiral(length, [x_start, y_start], heading, curv_start, gamma)
             points = [(x, y) for x, y in points]
-
         return points
 
     def _get_arc(self, xml_node: ET.Element) -> list:
         x_start = float(xml_node.attrib["x"])
         y_start = float(xml_node.attrib["y"])
         heading = float(xml_node.attrib["hdg"])
         length = float(xml_node.attrib["length"])
         curvature = float(xml_node.find("arc").attrib["curvature"])
 
         center, radius = Circle.get_circle_by_tangent_vector(
             [x_start, y_start], heading, abs(1 / curvature), "L" if curvature > 0 else "R"
         )
 
         n_interpolate = int(length / 0.1)
-        points = [(x_start, y_start)]
+        points = []
+
         arc_angle = length / radius * np.sign(curvature)
         start_heading = heading - np.pi / 2 * np.sign(curvature)
 
         for i in np.linspace(start_heading, start_heading + arc_angle, n_interpolate):
             x = center[0] + radius * np.cos(i)
             y = center[1] + radius * np.sin(i)
             points.append((x, y))
-
         return points
 
     def _get_poly3(self, xml_node: ET.Element) -> list:
         x_start = float(xml_node.attrib["x"])
         y_start = float(xml_node.attrib["y"])
         heading = float(xml_node.attrib["hdg"])
         length = float(xml_node.attrib["length"])
@@ -166,28 +180,34 @@
         )  # TODO: check the rotation direction
         coords_xy = np.dot(coords_uv, transform.T) + np.array([x_start, y_start])
         points = [(x, y) for x, y in coords_xy]
 
         return points
 
     def _get_geometry(self, xml_node: ET.Element) -> list:
+        """
+        Road Reference line
+        """
         geometry = []
 
         if not xml_node.find("line") is None:
             geometry = self._get_line(xml_node)
         elif not xml_node.find("spiral") is None:
             geometry = self._get_spiral(xml_node)
         elif not xml_node.find("arc") is None:
             geometry = self._get_arc(xml_node)
             # geometry = []
         elif not xml_node.find("poly3") is None:
             geometry = self._get_poly3(xml_node)
         elif not xml_node.find("paramPoly3") is None:
             geometry = self._get_param_poly3(xml_node)
 
+        if len(geometry) >= 2:
+            if geometry[-2] == geometry[-1]:
+                geometry.pop(-1)
         return geometry
 
     def _check_continuity(self, new_points, points):
         if len(points) == 0:
             return True
 
         if len(new_points) == 0:
@@ -343,29 +363,35 @@
             ),
             location=location,
         )
         self.id_counter += 1
 
         return lane, roadline
 
-    def load_object(self, x, y, heading, xml_node: ET.Element):
+    def load_object(self, points, s_points, headings, xml_node: ET.Element):
         s = float(xml_node.attrib["s"])
         t = float(xml_node.attrib["t"])
+
+        # find the closest point on the reference line
+        idx = np.argmin(np.abs(s_points - s))
+        ref_heading = headings[idx]
+        x, y = points[idx]
+
         zOffset = float(xml_node.attrib["zOffset"])
         relative_heading = float(xml_node.attrib["hdg"]) if "hdg" in xml_node.attrib else 0
+
         width = float(xml_node.attrib["width"]) if "width" in xml_node.attrib else None
         length = float(xml_node.attrib["length"]) if "length" in xml_node.attrib else None
         height = float(xml_node.attrib["height"]) if "height" in xml_node.attrib else None
         radius = float(xml_node.attrib["radius"]) if "radius" in xml_node.attrib else None
-        # orientation = xml_node.attrib["orientation"] if "orientation" in xml_node.attrib else "+"
-        # orientation = 1 if orientation == "+" else -1
 
         # convert local coordinate to global coordinate
-        x_origin = x + s * np.cos(heading) - t * np.sin(heading)
-        y_origin = y + s * np.sin(heading) + t * np.cos(heading)
+        heading = ref_heading
+        x_origin = x - t * np.sin(heading)
+        y_origin = y + t * np.cos(heading)
         # object_heading = heading + relative_heading * orientation
 
         if not None in [width, length]:
             shape = Polygon(
                 [
                     [0.5 * width, -0.5 * length],
                     [0.5 * width, 0.5 * length],
@@ -380,22 +406,22 @@
                     (np.cos(theta) * radius, np.sin(theta) * radius)
                     for theta in np.linspace(0, 2 * np.pi, 100)
                 ]
             )
         else:
             shape = Point(s, t)
 
-        shape = rotate(shape, relative_heading, origin=(0, 0))
+        shape = rotate(shape, (relative_heading / np.pi) * 180)
         shape = affine_transform(
             shape,
             [
-                np.cos(heading),
-                -np.sin(heading),
-                np.sin(heading),
-                np.cos(heading),
+                np.cos(heading - np.pi / 2),
+                -np.sin(heading - np.pi / 2),
+                np.sin(heading - np.pi / 2),
+                np.cos(heading - np.pi / 2),
                 x_origin,
                 y_origin,
             ],
         )
 
         # TODO: handle traffic participants and road areas separately
         area = Area(
@@ -407,15 +433,18 @@
 
         return area
 
     def load_road(self, xml_node: ET.Element):
         objects = []
         lanes = []
         roadlines = []
+
+        # refline points
         points = []
+
         link_node = xml_node.find("link")
 
         # type
         type_node = xml_node.find("type")
 
         # plan view
         first_geometry = xml_node.find("planView").find("geometry")
@@ -426,38 +455,76 @@
             new_points = self._get_geometry(geometry_node)
             if self._check_continuity(new_points, points):
                 points.extend(new_points)
             else:
                 logging.warning("The geometry is not continuous.")
                 points.extend(new_points)
 
+        s_points = np.sqrt(
+            np.sum((np.array(points) - np.array([points[0]] + points)[:-1, :]) ** 2, axis=1)
+        )
+        # I suggest you to put forward an issue to numpy to change this function name
+        s_points = np.cumsum(s_points)
+
         # elevation profile
         elevation_profile_node = xml_node.find("elevationProfile")
 
         # lateral profile
         lateral_profile_node = xml_node.find("lateralProfile")
 
         # lanes
         lanes_node = xml_node.find("lanes")
-        lane_sections = []
-        for lane_section_node in lanes_node.findall("laneSection"):
-            # DEBUG: curve processing
-
-            center_line = self.load_roadmark(
-                points, lane_section_node.find("center").find("lane").find("roadMark")
-            )  # RoadLine
-            if center_line is None:
-                raise ValueError("Center line must be defined.")
+        lane_sections_offset = [
+            float(lane_section.attrib["s"]) for lane_section in lanes_node.findall("laneSection")
+        ] + [s_points[-1]]
+        for ls_idx, lane_section_node in enumerate(lanes_node.findall("laneSection")):
+            # Load center line for lanesection
+            ls_start_offset, ls_end_offset = (
+                lane_sections_offset[ls_idx],
+                lane_sections_offset[ls_idx + 1],
+            )
+            center_points = np.array(points)[
+                (s_points >= ls_start_offset - 0.1) & (s_points <= ls_end_offset + 0.1)
+            ].tolist()
+            if len(center_points) == 1:
+                center_points.append(center_points[0])
+
+            center_line = RoadLine(
+                id_=self.id_counter,
+                geometry=LineString(center_points),
+            )
+            self.id_counter += 1
 
-            roadlines.append(center_line)
+            # Load road marks for lanesection
+            road_marks = lane_section_node.find("center").find("lane").findall("roadMark")
+            road_mark_offsets = [float(road_mark.attrib["sOffset"]) for road_mark in road_marks] + [
+                s_points[-1]
+            ]
+            for road_mark_idx, road_mark in enumerate(road_marks):
+                s_offset, e_offset = (
+                    road_mark_offsets[road_mark_idx],
+                    road_mark_offsets[road_mark_idx + 1],
+                )
+                part_refline = np.array(points)[
+                    (s_points >= s_offset - 0.1) & (s_points <= e_offset + 0.1)
+                ].tolist()
+
+                if len(part_refline) == 1:
+                    part_refline.append(part_refline[0])
+
+                part_refline = self.load_roadmark(part_refline, road_mark)  # RoadLine
+                if part_refline is None:
+                    raise ValueError("Center line must be defined.")
+                roadlines.append(part_refline)
 
             if not lane_section_node.find("left") is None:
                 lane_nodes = sorted(
                     lane_section_node.find("left").findall("lane"), key=lambda x: x.attrib["id"]
                 )
+
                 ref_line = center_line
                 for lane_node in lane_nodes:
                     lane, ref_line = self.load_lane(ref_line, lane_node, type_node)
                     lanes.append(lane)
                     roadlines.append(ref_line)
 
             if not lane_section_node.find("right") is None:
@@ -471,16 +538,17 @@
                     roadlines.append(ref_line)
 
         if lanes_node is None:
             raise ValueError("Road must have lanes element.")
 
         objects_node = xml_node.find("objects")
         if not objects_node is None:
+            headings = self.get_headings(points)
             for object_node in objects_node.findall("object"):
-                area = self.load_object(x, y, heading, object_node)
+                area = self.load_object(points, s_points, headings, object_node)
                 objects.append(area)
 
         return lanes, roadlines, objects
 
     def load_junction(self, xml_node: ET.Element):
         junction = Junction(id_=self.id_counter)
         self.id_counter += 1
```

### Comparing `tactics2d-0.1.6/tactics2d/math/geometry/circle.py` & `tactics2d-0.1.7/tactics2d/math/geometry/circle.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/math/geometry/vector.py` & `tactics2d-0.1.7/tactics2d/math/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/math/interpolate/b_spline.py` & `tactics2d-0.1.7/tactics2d/math/interpolate/b_spline.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/math/interpolate/bezier.py` & `tactics2d-0.1.7/tactics2d/math/interpolate/bezier.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/math/interpolate/cubic_spline.py` & `tactics2d-0.1.7/tactics2d/math/interpolate/cubic_spline.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/math/interpolate/dubins.py` & `tactics2d-0.1.7/tactics2d/math/interpolate/dubins.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,24 +40,24 @@
             arc_curve = Circle.get_arc(
                 circle_center, radius, radian, start_angle, clockwise, step_size
             )
 
             end_angle = (start_angle - radian) if clockwise else (start_angle + radian)
             end_point = circle_center + np.array([np.cos(end_angle), np.sin(end_angle)]) * radius
             end_heading = (start_heading - radian) if clockwise else (start_heading + radian)
-            yaw = np.arange(heading, end_heading, (-1 if clockwise else 1) * step_size / radius)
+            yaw = np.linspace(heading, end_heading, arc_curve.shape[0])
 
             return arc_curve, yaw, end_point, end_heading
 
         def get_straight_line(point, heading, radius, length):
             end_point = point + np.array([np.cos(heading), np.sin(heading)]) * radius * length
-            x_step = step_size * np.cos(heading)
-            y_step = step_size * np.sin(heading)
-            x = np.arange(point[0], end_point[0], x_step)
-            y = np.arange(point[1], end_point[1], y_step)
+            total_length = np.linalg.norm(end_point - point)
+            step_num = int(np.ceil(total_length / step_size))
+            x = np.linspace(point[0], end_point[0], step_num)
+            y = np.linspace(point[1], end_point[1], step_num)
             straight_line = np.vstack((x, y)).T
             yaw = np.ones_like(x) * heading
 
             return straight_line, yaw, end_point, heading
 
         next_point = start_point
         next_heading = start_heading
```

### Comparing `tactics2d-0.1.6/tactics2d/math/interpolate/reeds_shepp.py` & `tactics2d-0.1.7/tactics2d/math/interpolate/reeds_shepp.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,26 +71,26 @@
             arc_curve = Circle.get_arc(
                 circle_center, radius, radian, start_angle, clockwise, step_size
             )
 
             end_angle = (start_angle - radian) if clockwise else (start_angle + radian)
             end_point = circle_center + np.array([np.cos(end_angle), np.sin(end_angle)]) * radius
             end_heading = (heading - radian) if clockwise else (heading + radian)
-            yaw = np.arange(heading, end_heading, (-1 if clockwise else 1) * step_size / radius)
+            yaw = np.linspace(heading, end_heading, arc_curve.shape[0])
 
             return arc_curve, yaw, end_point, end_heading
 
         def get_straight_line(point, heading, radius, length, forward):
             end_point = (
                 point + np.array([np.cos(heading), np.sin(heading)]) * radius * length * forward
             )
-            x_step = step_size * np.cos(heading) * forward
-            y_step = step_size * np.sin(heading) * forward
-            x = np.arange(point[0], end_point[0], x_step)
-            y = np.arange(point[1], end_point[1], y_step)
+            total_length = np.linalg.norm(end_point - point)
+            num_points = int(np.ceil(total_length / step_size))
+            x = np.linspace(point[0], end_point[0], num_points)
+            y = np.linspace(point[1], end_point[1], num_points)
             straight_line = np.array([x, y]).T
             yaw = np.ones_like(x) * heading
 
             return straight_line, yaw, end_point, heading
 
         next_point = start_point
         next_heading = start_heading
```

### Comparing `tactics2d-0.1.6/tactics2d/math/interpolate/spiral.py` & `tactics2d-0.1.7/tactics2d/math/interpolate/spiral.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/element/__init__.py` & `tactics2d-0.1.7/tactics2d/participant/element/__init__.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/element/cyclist.py` & `tactics2d-0.1.7/tactics2d/participant/element/cyclist.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/element/other.py` & `tactics2d-0.1.7/tactics2d/participant/element/other.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/element/participant_base.py` & `tactics2d-0.1.7/tactics2d/participant/element/participant_base.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/element/participant_template.py` & `tactics2d-0.1.7/tactics2d/participant/element/participant_template.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/element/pedestrian.py` & `tactics2d-0.1.7/tactics2d/participant/element/pedestrian.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/element/vehicle.py` & `tactics2d-0.1.7/tactics2d/participant/element/vehicle.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/guess_type.py` & `tactics2d-0.1.7/tactics2d/participant/guess_type.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/trajectory/state.py` & `tactics2d-0.1.7/tactics2d/participant/trajectory/state.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/trajectory/trajectory.py` & `tactics2d-0.1.7/tactics2d/participant/trajectory/trajectory.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/participant/trajectory_classifier.m` & `tactics2d-0.1.7/tactics2d/participant/trajectory_classifier.m`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/physics/__init__.py` & `tactics2d-0.1.7/tactics2d/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/physics/physics_model_base.py` & `tactics2d-0.1.7/tactics2d/physics/physics_model_base.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/physics/point_mass.py` & `tactics2d-0.1.7/tactics2d/physics/point_mass.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/physics/single_track_drift.py` & `tactics2d-0.1.7/tactics2d/physics/single_track_drift.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/physics/single_track_dynamics.py` & `tactics2d-0.1.7/tactics2d/physics/single_track_dynamics.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/physics/single_track_kinematics.py` & `tactics2d-0.1.7/tactics2d/physics/single_track_kinematics.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         phi = state.heading
         v = state.speed
 
         for dt in dts:
             dx = v * np.cos(phi + beta)
             dy = v * np.sin(phi + beta)
             dv = accel
-            dphi = v / self.wheel_base * np.tan(delta)
+            dphi = v / self.wheel_base * np.tan(delta) * np.cos(beta)
 
             x += dx * dt
             y += dy * dt
             phi += dphi * dt
             v += dv * dt
 
             v = np.clip(v, *self.speed_range) if not self.speed_range is None else v
```

### Comparing `tactics2d-0.1.6/tactics2d/sensor/camera.py` & `tactics2d-0.1.7/tactics2d/sensor/camera.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/sensor/lidar.py` & `tactics2d-0.1.7/tactics2d/sensor/lidar.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,23 +180,23 @@
 
         # select the true intersections, set the false positive intersections to inf
         tmp_inf = self.perception_range * 10
         tmp_zero = 1e-8
         # the false positive intersections on line L1(not on ray L1)
         lidar_line_x = (np.cos(theta) * self.perception_range).reshape(-1, 1)  # (point_density, 1)
         lidar_line_y = (np.sin(theta) * self.perception_range).reshape(-1, 1)
-        raw_x[raw_x > np.maximum(tmp_zero, lidar_line_x)] = tmp_inf
-        raw_x[raw_x < np.minimum(-tmp_zero, lidar_line_x)] = tmp_inf
-        raw_y[raw_y > np.maximum(tmp_zero, lidar_line_y)] = tmp_inf
-        raw_y[raw_y < np.minimum(-tmp_zero, lidar_line_y)] = tmp_inf
+        raw_x[raw_x > np.maximum(tmp_zero, lidar_line_x) + tmp_zero] = tmp_inf
+        raw_x[raw_x < np.minimum(-tmp_zero, lidar_line_x) - tmp_zero] = tmp_inf
+        raw_y[raw_y > np.maximum(tmp_zero, lidar_line_y) + tmp_zero] = tmp_inf
+        raw_y[raw_y < np.minimum(-tmp_zero, lidar_line_y) - tmp_zero] = tmp_inf
         # the false positive intersections on line L2(not on edge L2)
-        raw_x[raw_x > np.maximum(x1s, x2s)] = tmp_inf
-        raw_x[raw_x < np.minimum(x1s, x2s)] = tmp_inf
-        raw_y[raw_y > np.maximum(y1s, y2s)] = tmp_inf
-        raw_y[raw_y < np.minimum(y1s, y2s)] = tmp_inf
+        raw_x[raw_x > np.maximum(x1s, x2s) + tmp_zero] = tmp_inf
+        raw_x[raw_x < np.minimum(x1s, x2s) - tmp_zero] = tmp_inf
+        raw_y[raw_y > np.maximum(y1s, y2s) + tmp_zero] = tmp_inf
+        raw_y[raw_y < np.minimum(y1s, y2s) - tmp_zero] = tmp_inf
         # the (L1, L2) which are parallel
         raw_x[parallel_line_pos] = tmp_inf
 
         lidar_obs = np.min(np.sqrt(raw_x**2 + raw_y**2), axis=1)  # (point_density,)
         lidar_obs = np.clip(lidar_obs, 0, self.perception_range)
         lidar_obs[lidar_obs == self.perception_range] = float("inf")
         self.scan_result = lidar_obs
```

### Comparing `tactics2d-0.1.6/tactics2d/sensor/render_manager.py` & `tactics2d-0.1.7/tactics2d/sensor/render_manager.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/sensor/render_template.py` & `tactics2d-0.1.7/tactics2d/sensor/render_template.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/sensor/sensor_base.py` & `tactics2d-0.1.7/tactics2d/sensor/sensor_base.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/event_detection/__init__.py` & `tactics2d-0.1.7/tactics2d/traffic/event_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/event_detection/arrival.py` & `tactics2d-0.1.7/tactics2d/traffic/event_detection/arrival.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # @File: completed.py
 # @Description: This script defines the event detector to check whether the agent has arrived at a target area.
 # @Author: Yueyuan Li
 # @Version: 1.0.0
 
 
 from tactics2d.map.element import Area
+from shapely.geometry import Polygon
 
 from .event_base import EventBase
 
 
 class Arrival(EventBase):
     """This class is used to detect whether the agent has arrived at a target area.
 
@@ -25,15 +26,15 @@
         Args:
             target_area (Area): The target area that the agent needs to reach.
             threshold (float, optional): The threshold of the intersection over union (IoU) to determine whether the agent has completed the task.
         """
         self.target_area = target_area
         self.threshold = threshold
 
-    def update(self, agent_pose: Area):
+    def update(self, agent_pose: Polygon):
         """This function updates the status of the task completion.
 
         Args:
             agent_pose (Polygon): The current pose of the agent.
 
         Returns:
             is_completed (bool): Whether the agent has completed the task.
```

### Comparing `tactics2d-0.1.6/tactics2d/traffic/event_detection/collision.py` & `tactics2d-0.1.7/tactics2d/traffic/event_detection/collision.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/event_detection/event_base.py` & `tactics2d-0.1.7/tactics2d/traffic/event_detection/event_base.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/event_detection/off_lane.py` & `tactics2d-0.1.7/tactics2d/traffic/event_detection/off_lane.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/event_detection/off_route.py` & `tactics2d-0.1.7/tactics2d/traffic/event_detection/off_route.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/event_detection/out_bound.py` & `tactics2d-0.1.7/tactics2d/traffic/event_detection/out_bound.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/event_detection/time_exceed.py` & `tactics2d-0.1.7/tactics2d/traffic/event_detection/time_exceed.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/scenario_display.py` & `tactics2d-0.1.7/tactics2d/traffic/scenario_display.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/scenario_manager.py` & `tactics2d-0.1.7/tactics2d/traffic/scenario_manager.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d/traffic/status.py` & `tactics2d-0.1.7/tactics2d/traffic/status.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tactics2d.egg-info/PKG-INFO` & `tactics2d-0.1.7/tactics2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tactics2d
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tactics2D: A Reinforcement Learning Environment Library with Generative Scenarios for Driving Decision-making
 Author-email: Yueyuan Li <rowena.academic@gmail.com>
 Maintainer-email: Yueyuan Li <rowena.academic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `tactics2d-0.1.6/tactics2d.egg-info/SOURCES.txt` & `tactics2d-0.1.7/tactics2d.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
+docs/tutorial/train_racing_agent.py
 tactics2d/__init__.py
 tactics2d.egg-info/PKG-INFO
 tactics2d.egg-info/SOURCES.txt
 tactics2d.egg-info/dependency_links.txt
 tactics2d.egg-info/requires.txt
 tactics2d.egg-info/top_level.txt
 tactics2d/dataset_parser/__init__.py
@@ -113,13 +114,8 @@
 test/test_map_element.py
 test/test_map_generator.py
 test/test_map_parser.py
 test/test_math_interpolate.py
 test/test_participant.py
 test/test_physics.py
 test/test_render.py
-test/test_traffic.py
-tutorial/__init__.py
-tutorial/action_mask.py
-tutorial/rs_planner.py
-tutorial/train_parking_agent.py
-tutorial/train_racing_agent.py
+test/test_traffic.py
```

### Comparing `tactics2d-0.1.6/test/test_dataset_parser.py` & `tactics2d-0.1.7/test/test_dataset_parser.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/test/test_env.py` & `tactics2d-0.1.7/test/test_env.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/test/test_map_element.py` & `tactics2d-0.1.7/test/test_map_element.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/test/test_map_generator.py` & `tactics2d-0.1.7/test/test_map_generator.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/test/test_map_parser.py` & `tactics2d-0.1.7/test/test_map_parser.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/test/test_math_interpolate.py` & `tactics2d-0.1.7/test/test_math_interpolate.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/test/test_participant.py` & `tactics2d-0.1.7/test/test_participant.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/test/test_physics.py` & `tactics2d-0.1.7/test/test_physics.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,22 +391,18 @@
     if RENDER:
         # visualizer = Visualizer(vehicle, int(1000/interval))
         visualizer = Visualizer(vehicle)
         t1 = time.time()
 
     for action, duration in VEHICLE_ACTION_LIST:
         for _ in np.arange(0, duration, interval):
-            (
-                state_constrained,
-                omega_wf,
-                omega_wr,
-                real_accel,
-                real_steer,
-            ) = physics_model_constrained.step(
-                state_constrained, omega_wf, omega_wr, action[0], action[1], interval
+            (state_constrained, omega_wf, omega_wr, real_accel, real_steer) = (
+                physics_model_constrained.step(
+                    state_constrained, omega_wf, omega_wr, action[0], action[1], interval
+                )
             )
             trajectory.append((state_constrained.x, state_constrained.y))
             if RENDER:
                 visualizer.update(state_constrained, action, (real_accel, real_steer), trajectory)
 
     if RENDER:
         t2 = time.time()
```

### Comparing `tactics2d-0.1.6/test/test_render.py` & `tactics2d-0.1.7/test/test_render.py`

 * *Files identical despite different names*

### Comparing `tactics2d-0.1.6/tutorial/train_racing_agent.py` & `tactics2d-0.1.7/docs/tutorial/train_racing_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,18 +214,15 @@
             "actor_kwargs": {
                 "state_dim": 6400,
                 "action_dim": 2,
                 "hidden_size": 32,
                 "continuous": True,
             },
             "critic_net": AgentCritic,
-            "critic_kwargs": {
-                "state_dim": 6400,
-                "hidden_size": 32,
-            },
+            "critic_kwargs": {"state_dim": 6400, "hidden_size": 32},
             "vf_coef": 1,
             "gae_lambda": 0.97,
             "adv_norm": False,
         }
     )
     agent = PPO(agent_configs, device)
```

