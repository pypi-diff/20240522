# Comparing `tmp/ourskyai_platform_api-1.3.3603.tar.gz` & `tmp/ourskyai_platform_api-1.3.3644.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3603.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3644.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3603.tar` & `ourskyai_platform_api-1.3.3644.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     9625 2024-05-17 19:15:26.351834 ourskyai_platform_api-1.3.3603/README.md
--rw-r--r--   0        0        0     6272 2024-05-17 19:15:30.007971 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-05-17 19:15:30.039972 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   199259 2024-05-17 19:15:30.135976 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-05-17 19:15:30.207979 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-17 19:15:30.263980 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-05-17 19:15:30.319983 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-05-17 19:15:30.355984 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     5601 2024-05-17 19:15:30.411986 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-05-17 19:15:30.487989 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-05-17 19:15:30.531991 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-05-17 19:15:30.571992 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     2158 2024-05-17 19:15:30.611994 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-05-17 19:15:30.659995 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-05-17 19:15:30.715998 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-05-17 19:15:30.751999 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-05-17 19:15:30.800001 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-05-17 19:15:30.852003 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-05-17 19:15:30.904005 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-05-17 19:15:30.968007 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-05-17 19:15:31.000008 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     2622 2024-05-17 19:15:31.048010 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_auto_focus_instruction.py
--rw-r--r--   0        0        0     2366 2024-05-17 19:15:31.116013 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
--rw-r--r--   0        0        0     4920 2024-05-17 19:15:31.180015 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-05-17 19:15:31.228017 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-05-17 19:15:31.288019 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-05-17 19:15:31.348021 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-05-17 19:15:31.404024 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-05-17 19:15:31.448025 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-05-17 19:15:31.512028 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2710 2024-05-17 19:15:31.548029 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-05-17 19:15:31.604031 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-05-17 19:15:31.644033 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-05-17 19:15:31.692034 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-05-17 19:15:31.732036 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-05-17 19:15:31.804039 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0      719 2024-05-17 19:15:31.896042 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_file_type.py
--rw-r--r--   0        0        0     3298 2024-05-17 19:15:31.944044 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-05-17 19:15:31.988046 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-05-17 19:15:32.064048 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-05-17 19:15:32.120051 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-05-17 19:15:32.164052 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-05-17 19:15:32.248055 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-05-17 19:15:32.308057 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     2675 2024-05-17 19:15:32.380060 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
--rw-r--r--   0        0        0     3985 2024-05-17 19:15:32.476064 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-05-17 19:15:32.516065 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5170 2024-05-17 19:15:32.552067 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3763 2024-05-17 19:15:32.612069 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-05-17 19:15:32.656071 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-05-17 19:15:32.716073 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-05-17 19:15:32.780075 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-05-17 19:15:32.812076 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1655 2024-05-17 19:15:32.876079 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-05-17 19:15:32.932081 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-05-17 19:15:32.980083 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-05-17 19:15:33.024084 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2135 2024-05-17 19:15:33.072086 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
--rw-r--r--   0        0        0     2648 2024-05-17 19:15:33.112088 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
--rw-r--r--   0        0        0     2054 2024-05-17 19:15:33.168090 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2401 2024-05-17 19:15:33.216092 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_release.py
--rw-r--r--   0        0        0     2053 2024-05-17 19:15:33.268094 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-05-17 19:15:33.316095 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-05-17 19:15:33.364097 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-05-17 19:15:33.420099 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-05-17 19:15:33.484102 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-05-17 19:15:33.532104 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-05-17 19:15:33.580105 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-05-17 19:15:33.648108 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-05-17 19:15:33.696110 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-05-17 19:15:33.768113 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-05-17 19:15:33.804114 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-05-17 19:15:33.860116 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-05-17 19:15:33.912118 ourskyai_platform_api-1.3.3603/pyproject.toml
--rw-r--r--   0        0        0    10602 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3603/PKG-INFO
+-rw-r--r--   0        0        0     9661 2024-05-22 19:37:35.329255 ourskyai_platform_api-1.3.3644/README.md
+-rw-r--r--   0        0        0     6336 2024-05-22 19:37:39.181297 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-22 19:37:39.221298 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   199259 2024-05-22 19:37:39.325299 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-05-22 19:37:39.381300 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-22 19:37:39.437300 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-05-22 19:37:39.497301 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-05-22 19:37:39.569301 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5665 2024-05-22 19:37:39.617302 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-22 19:37:39.677303 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-05-22 19:37:39.725303 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-05-22 19:37:39.769304 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     1933 2024-05-22 19:37:39.821304 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/fits_header.py
+-rw-r--r--   0        0        0     2158 2024-05-22 19:37:39.865305 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-05-22 19:37:39.909305 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-05-22 19:37:39.977306 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-05-22 19:37:40.029307 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-05-22 19:37:40.077307 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-05-22 19:37:40.125308 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-05-22 19:37:40.177308 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-05-22 19:37:40.241309 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-05-22 19:37:40.297309 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2622 2024-05-22 19:37:40.353310 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_auto_focus_instruction.py
+-rw-r--r--   0        0        0     2366 2024-05-22 19:37:40.393311 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
+-rw-r--r--   0        0        0     4920 2024-05-22 19:37:40.441311 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-05-22 19:37:40.577313 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-05-22 19:37:40.613313 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-05-22 19:37:40.669314 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-05-22 19:37:40.737314 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-05-22 19:37:40.785315 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-05-22 19:37:40.833315 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2710 2024-05-22 19:37:40.909316 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-05-22 19:37:40.961317 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-05-22 19:37:41.029318 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-05-22 19:37:41.085318 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-05-22 19:37:41.121319 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-05-22 19:37:41.165319 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0      719 2024-05-22 19:37:41.217320 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_file_type.py
+-rw-r--r--   0        0        0     3298 2024-05-22 19:37:41.317321 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-05-22 19:37:41.365321 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-05-22 19:37:41.409322 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-05-22 19:37:41.489323 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-05-22 19:37:41.569324 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-05-22 19:37:41.637324 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-05-22 19:37:41.701325 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2675 2024-05-22 19:37:41.761326 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-05-22 19:37:41.825326 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-05-22 19:37:41.881327 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5803 2024-05-22 19:37:41.957328 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3763 2024-05-22 19:37:41.997328 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-05-22 19:37:42.053329 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-05-22 19:37:42.097329 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-05-22 19:37:42.145330 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-05-22 19:37:42.185330 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1655 2024-05-22 19:37:42.233331 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-05-22 19:37:42.273331 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-05-22 19:37:42.329332 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-05-22 19:37:42.385332 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-05-22 19:37:42.433333 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2648 2024-05-22 19:37:42.533334 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0     2054 2024-05-22 19:37:42.585335 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2401 2024-05-22 19:37:42.649335 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_release.py
+-rw-r--r--   0        0        0     2053 2024-05-22 19:37:42.689336 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-05-22 19:37:42.737336 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-05-22 19:37:42.801337 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-05-22 19:37:42.849338 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-05-22 19:37:42.897338 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-05-22 19:37:42.933338 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-05-22 19:37:42.997339 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-05-22 19:37:43.041340 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-05-22 19:37:43.121341 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-05-22 19:37:43.153341 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:37:43.193341 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-05-22 19:37:43.253342 ourskyai_platform_api-1.3.3644/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-05-22 19:37:43.309343 ourskyai_platform_api-1.3.3644/pyproject.toml
+-rw-r--r--   0        0        0    10638 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3644/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3603/README.md` & `ourskyai_platform_api-1.3.3644/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3603
-- Package version: 1.3.3603
+- API version: 1.3.3644
+- Package version: 1.3.3644
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -115,14 +115,15 @@
 
 
 ## Documentation For Models
 
  - [CameraMode](docs/CameraMode.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
+ - [FitsHeader](docs/FitsHeader.md)
  - [Location](docs/Location.md)
  - [MetricType](docs/MetricType.md)
  - [MountType](docs/MountType.md)
  - [NodeState](docs/NodeState.md)
  - [OpticalTubeType](docs/OpticalTubeType.md)
  - [PlateSolveParameters](docs/PlateSolveParameters.md)
  - [ShutterType](docs/ShutterType.md)
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3603"
+__version__ = "1.3.3644"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
@@ -30,14 +30,15 @@
 from ourskyai_platform_api.exceptions import ApiAttributeError
 from ourskyai_platform_api.exceptions import ApiException
 
 # import models into sdk package
 from ourskyai_platform_api.models.camera_mode import CameraMode
 from ourskyai_platform_api.models.empty_success import EmptySuccess
 from ourskyai_platform_api.models.filter_type import FilterType
+from ourskyai_platform_api.models.fits_header import FitsHeader
 from ourskyai_platform_api.models.location import Location
 from ourskyai_platform_api.models.metric_type import MetricType
 from ourskyai_platform_api.models.mount_type import MountType
 from ourskyai_platform_api.models.node_state import NodeState
 from ourskyai_platform_api.models.optical_tube_type import OpticalTubeType
 from ourskyai_platform_api.models.plate_solve_parameters import PlateSolveParameters
 from ourskyai_platform_api.models.shutter_type import ShutterType
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3603/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3644/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3603\n"\
-               "SDK Package Version: 1.3.3603".\
+               "Version of the API: 1.3.3644\n"\
+               "SDK Package Version: 1.3.3644".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from ourskyai_platform_api.models.camera_mode import CameraMode
 from ourskyai_platform_api.models.empty_success import EmptySuccess
 from ourskyai_platform_api.models.filter_type import FilterType
+from ourskyai_platform_api.models.fits_header import FitsHeader
 from ourskyai_platform_api.models.location import Location
 from ourskyai_platform_api.models.metric_type import MetricType
 from ourskyai_platform_api.models.mount_type import MountType
 from ourskyai_platform_api.models.node_state import NodeState
 from ourskyai_platform_api.models.optical_tube_type import OpticalTubeType
 from ourskyai_platform_api.models.plate_solve_parameters import PlateSolveParameters
 from ourskyai_platform_api.models.shutter_type import ShutterType
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/camera_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/empty_success.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/filter_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/metric_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/mount_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/node_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/shutter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/tracking_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_auto_focus_instruction.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_auto_focus_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_file_type.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_file_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Optional, Union
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr
+from typing import List, Optional, Union
+from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist
+from ourskyai_platform_api.models.fits_header import FitsHeader
 
 class V1ImageSetImage(BaseModel):
     """
     Image Set Image  # noqa: E501
     """
     id: StrictStr = Field(...)
     thumbnail_url: Optional[StrictStr] = Field(None, alias="thumbnailUrl")
@@ -45,15 +46,16 @@
     total_offset: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="totalOffset")
     total_offset_std_dev: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="totalOffsetStdDev")
     total_offset_rms: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="totalOffsetRMS")
     captured_at: datetime = Field(..., alias="capturedAt")
     created_at: datetime = Field(..., alias="createdAt")
     binning: Optional[StrictInt] = None
     exposure_length: Union[StrictFloat, StrictInt] = Field(..., alias="exposureLength")
-    __properties = ["id", "thumbnailUrl", "imageUrl", "fullJpgUrl", "nodeId", "targetId", "ra", "dec", "imageSetId", "darkCalibrated", "flatCalibrated", "biasCalibrated", "fwhmAverage", "fwhmStdDev", "fwhmAngle", "raOffset", "decOffset", "totalOffset", "totalOffsetStdDev", "totalOffsetRMS", "capturedAt", "createdAt", "binning", "exposureLength"]
+    fits_headers: conlist(FitsHeader) = Field(..., alias="fitsHeaders")
+    __properties = ["id", "thumbnailUrl", "imageUrl", "fullJpgUrl", "nodeId", "targetId", "ra", "dec", "imageSetId", "darkCalibrated", "flatCalibrated", "biasCalibrated", "fwhmAverage", "fwhmStdDev", "fwhmAngle", "raOffset", "decOffset", "totalOffset", "totalOffsetStdDev", "totalOffsetRMS", "capturedAt", "createdAt", "binning", "exposureLength", "fitsHeaders"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -71,14 +73,21 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in fits_headers (list)
+        _items = []
+        if self.fits_headers:
+            for _item in self.fits_headers:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['fitsHeaders'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> V1ImageSetImage:
         """Create an instance of V1ImageSetImage from a dict"""
         if obj is None:
             return None
@@ -106,12 +115,13 @@
             "dec_offset": obj.get("decOffset"),
             "total_offset": obj.get("totalOffset"),
             "total_offset_std_dev": obj.get("totalOffsetStdDev"),
             "total_offset_rms": obj.get("totalOffsetRMS"),
             "captured_at": obj.get("capturedAt"),
             "created_at": obj.get("createdAt"),
             "binning": obj.get("binning"),
-            "exposure_length": obj.get("exposureLength")
+            "exposure_length": obj.get("exposureLength"),
+            "fits_headers": [FitsHeader.from_dict(_item) for _item in obj.get("fitsHeaders")] if obj.get("fitsHeaders") is not None else None
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_release.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3644/ourskyai_platform_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3603/pyproject.toml` & `ourskyai_platform_api-1.3.3644/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3603"
+version = "1.3.3644"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3603/PKG-INFO` & `ourskyai_platform_api-1.3.3644/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3603
+Version: 1.3.3644
 Summary: OurSky Platform
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3603
-- Package version: 1.3.3603
+- API version: 1.3.3644
+- Package version: 1.3.3644
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -140,14 +140,15 @@
 
 
 ## Documentation For Models
 
  - [CameraMode](docs/CameraMode.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
+ - [FitsHeader](docs/FitsHeader.md)
  - [Location](docs/Location.md)
  - [MetricType](docs/MetricType.md)
  - [MountType](docs/MountType.md)
  - [NodeState](docs/NodeState.md)
  - [OpticalTubeType](docs/OpticalTubeType.md)
  - [PlateSolveParameters](docs/PlateSolveParameters.md)
  - [ShutterType](docs/ShutterType.md)
```

