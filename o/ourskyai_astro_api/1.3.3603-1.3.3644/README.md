# Comparing `tmp/ourskyai_astro_api-1.3.3603.tar.gz` & `tmp/ourskyai_astro_api-1.3.3644.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3603.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3644.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3603.tar` & `ourskyai_astro_api-1.3.3644.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0    11057 2024-05-17 19:15:26.315833 ourskyai_astro_api-1.3.3603/README.md
--rw-r--r--   0        0        0     5741 2024-05-17 19:15:29.771962 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-05-17 19:15:29.803963 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   253842 2024-05-17 19:15:29.883966 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-05-17 19:15:29.923968 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-17 19:15:29.967970 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-05-17 19:15:30.019971 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-05-17 19:15:30.083974 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5100 2024-05-17 19:15:30.131976 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-05-17 19:15:30.179978 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-05-17 19:15:30.239980 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-05-17 19:15:30.283981 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     1904 2024-05-17 19:15:30.355984 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-05-17 19:15:30.403986 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     2155 2024-05-17 19:15:30.443987 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-05-17 19:15:30.491989 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-05-17 19:15:30.527990 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-05-17 19:15:30.587993 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-05-17 19:15:30.635995 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-05-17 19:15:30.679996 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-05-17 19:15:30.755999 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-05-17 19:15:30.804001 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-05-17 19:15:30.852003 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-05-17 19:15:30.892004 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-05-17 19:15:30.948006 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-05-17 19:15:31.000008 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-05-17 19:15:31.052010 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-05-17 19:15:31.088012 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-05-17 19:15:31.156014 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-05-17 19:15:31.208016 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-05-17 19:15:31.272019 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-05-17 19:15:31.340021 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-05-17 19:15:31.432025 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-05-17 19:15:31.488027 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-05-17 19:15:31.592031 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-05-17 19:15:31.672034 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-05-17 19:15:31.760037 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-05-17 19:15:31.812039 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-05-17 19:15:31.872041 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-05-17 19:15:31.940044 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-05-17 19:15:31.992045 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-05-17 19:15:32.048048 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-05-17 19:15:32.092049 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-05-17 19:15:32.168052 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-05-17 19:15:32.212054 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-05-17 19:15:32.272056 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-05-17 19:15:32.308057 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-05-17 19:15:32.360059 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-05-17 19:15:32.408061 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5167 2024-05-17 19:15:32.464063 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-05-17 19:15:32.516065 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-05-17 19:15:32.564067 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-05-17 19:15:32.612069 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-05-17 19:15:32.660071 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-05-17 19:15:32.712073 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-05-17 19:15:32.752074 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-05-17 19:15:32.832077 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-05-17 19:15:32.880079 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-05-17 19:15:32.932081 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-05-17 19:15:32.976083 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-05-17 19:15:33.024084 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-05-17 19:15:33.056086 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-05-17 19:15:33.124088 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-05-17 19:15:33.156089 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-05-17 19:15:33.212092 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-05-17 19:15:33.268094 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-05-17 19:15:33.308095 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-05-17 19:15:33.388098 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-05-17 19:15:33.416099 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-05-17 19:15:33.476101 ourskyai_astro_api-1.3.3603/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-05-17 19:15:33.520103 ourskyai_astro_api-1.3.3603/pyproject.toml
--rw-r--r--   0        0        0    12025 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3603/PKG-INFO
+-rw-r--r--   0        0        0    11093 2024-05-22 19:37:35.265254 ourskyai_astro_api-1.3.3644/README.md
+-rw-r--r--   0        0        0     5802 2024-05-22 19:37:38.657292 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-22 19:37:38.689292 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   253842 2024-05-22 19:37:38.929294 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-05-22 19:37:38.993295 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-22 19:37:39.041296 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-05-22 19:37:39.101297 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-05-22 19:37:39.189297 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5161 2024-05-22 19:37:39.233298 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-22 19:37:39.361299 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-05-22 19:37:39.449300 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-05-22 19:37:39.509301 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     1904 2024-05-22 19:37:39.549301 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-05-22 19:37:39.637302 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     1930 2024-05-22 19:37:39.689303 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/fits_header.py
+-rw-r--r--   0        0        0     2155 2024-05-22 19:37:39.781304 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-05-22 19:37:39.833305 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-05-22 19:37:39.897305 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-05-22 19:37:39.949306 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-05-22 19:37:40.021307 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-05-22 19:37:40.077307 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-05-22 19:37:40.129308 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-05-22 19:37:40.229309 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-05-22 19:37:40.285309 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-05-22 19:37:40.333310 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-05-22 19:37:40.425311 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-05-22 19:37:40.469311 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-05-22 19:37:40.529312 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-05-22 19:37:40.609313 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-05-22 19:37:40.653313 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-05-22 19:37:40.693314 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-05-22 19:37:40.745314 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-05-22 19:37:40.797315 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-05-22 19:37:40.861316 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-05-22 19:37:40.929317 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-05-22 19:37:40.981317 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-05-22 19:37:41.053318 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-05-22 19:37:41.161319 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-05-22 19:37:41.209320 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-05-22 19:37:41.245320 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-05-22 19:37:41.289321 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-05-22 19:37:41.337321 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-05-22 19:37:41.377321 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-05-22 19:37:41.433322 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-05-22 19:37:41.481323 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-05-22 19:37:41.537323 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-05-22 19:37:41.577324 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-05-22 19:37:41.629324 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-05-22 19:37:41.689325 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-05-22 19:37:41.785326 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5797 2024-05-22 19:37:41.825326 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-05-22 19:37:41.893327 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-05-22 19:37:41.945328 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-05-22 19:37:42.153330 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-05-22 19:37:42.237331 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-05-22 19:37:42.325332 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-05-22 19:37:42.377332 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-05-22 19:37:42.461333 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-05-22 19:37:42.529334 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-05-22 19:37:42.597335 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-05-22 19:37:42.653335 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-05-22 19:37:42.705336 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-05-22 19:37:42.745336 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-05-22 19:37:42.813337 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-05-22 19:37:42.869338 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-05-22 19:37:42.925338 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-05-22 19:37:42.973339 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-05-22 19:37:43.029340 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-05-22 19:37:43.073340 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:37:43.105340 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-05-22 19:37:43.145341 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-05-22 19:37:43.205341 ourskyai_astro_api-1.3.3644/pyproject.toml
+-rw-r--r--   0        0        0    12061 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3644/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3603/README.md` & `ourskyai_astro_api-1.3.3644/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
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
@@ -134,14 +134,15 @@
 ## Documentation For Models
 
  - [AssetFileType](docs/AssetFileType.md)
  - [AssetType](docs/AssetType.md)
  - [CalibrationMasterType](docs/CalibrationMasterType.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
+ - [FitsHeader](docs/FitsHeader.md)
  - [Location](docs/Location.md)
  - [MountType](docs/MountType.md)
  - [NodeState](docs/NodeState.md)
  - [OpticalTubeType](docs/OpticalTubeType.md)
  - [ShutterType](docs/ShutterType.md)
  - [SuccessfulCreate](docs/SuccessfulCreate.md)
  - [TrackingType](docs/TrackingType.md)
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3603"
+__version__ = "1.3.3644"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
@@ -32,14 +32,15 @@
 
 # import models into sdk package
 from ourskyai_astro_api.models.asset_file_type import AssetFileType
 from ourskyai_astro_api.models.asset_type import AssetType
 from ourskyai_astro_api.models.calibration_master_type import CalibrationMasterType
 from ourskyai_astro_api.models.empty_success import EmptySuccess
 from ourskyai_astro_api.models.filter_type import FilterType
+from ourskyai_astro_api.models.fits_header import FitsHeader
 from ourskyai_astro_api.models.location import Location
 from ourskyai_astro_api.models.mount_type import MountType
 from ourskyai_astro_api.models.node_state import NodeState
 from ourskyai_astro_api.models.optical_tube_type import OpticalTubeType
 from ourskyai_astro_api.models.shutter_type import ShutterType
 from ourskyai_astro_api.models.successful_create import SuccessfulCreate
 from ourskyai_astro_api.models.tracking_type import TrackingType
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
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

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
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

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from ourskyai_astro_api.models.asset_file_type import AssetFileType
 from ourskyai_astro_api.models.asset_type import AssetType
 from ourskyai_astro_api.models.calibration_master_type import CalibrationMasterType
 from ourskyai_astro_api.models.empty_success import EmptySuccess
 from ourskyai_astro_api.models.filter_type import FilterType
+from ourskyai_astro_api.models.fits_header import FitsHeader
 from ourskyai_astro_api.models.location import Location
 from ourskyai_astro_api.models.mount_type import MountType
 from ourskyai_astro_api.models.node_state import NodeState
 from ourskyai_astro_api.models.optical_tube_type import OpticalTubeType
 from ourskyai_astro_api.models.shutter_type import ShutterType
 from ourskyai_astro_api.models.successful_create import SuccessfulCreate
 from ourskyai_astro_api.models.tracking_type import TrackingType
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/asset_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/filter_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/mount_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/shutter_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/successful_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/tracking_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
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
+from ourskyai_astro_api.models.fits_header import FitsHeader
 
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

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_job_status.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,23 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1PlatformCreditType(str, Enum):
+class V1PlatformCreditUnit(str, Enum):
     """
-    V1PlatformCreditType
+    V1PlatformCreditUnit
     """
 
     """
     allowed enum values
     """
-    ASTRO_PLATFORM_USAGE = 'ASTRO_PLATFORM_USAGE'
+    MEGABYTE = 'MEGABYTE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1PlatformCreditType:
-        """Create an instance of V1PlatformCreditType from a JSON string"""
-        return V1PlatformCreditType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1PlatformCreditUnit:
+        """Create an instance of V1PlatformCreditUnit from a JSON string"""
+        return V1PlatformCreditUnit(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,23 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1PlatformCreditUnit(str, Enum):
+class V1PlatformCreditType(str, Enum):
     """
-    V1PlatformCreditUnit
+    V1PlatformCreditType
     """
 
     """
     allowed enum values
     """
-    MEGABYTE = 'MEGABYTE'
+    ASTRO_PLATFORM_USAGE = 'ASTRO_PLATFORM_USAGE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1PlatformCreditUnit:
-        """Create an instance of V1PlatformCreditUnit from a JSON string"""
-        return V1PlatformCreditUnit(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1PlatformCreditType:
+        """Create an instance of V1PlatformCreditType from a JSON string"""
+        return V1PlatformCreditType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3603/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3603/pyproject.toml` & `ourskyai_astro_api-1.3.3644/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3603"
+version = "1.3.3644"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3603/PKG-INFO` & `ourskyai_astro_api-1.3.3644/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3603
+Version: 1.3.3644
 Summary: OurSky Astro
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Astro
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-astro-api
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
@@ -159,14 +159,15 @@
 ## Documentation For Models
 
  - [AssetFileType](docs/AssetFileType.md)
  - [AssetType](docs/AssetType.md)
  - [CalibrationMasterType](docs/CalibrationMasterType.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
+ - [FitsHeader](docs/FitsHeader.md)
  - [Location](docs/Location.md)
  - [MountType](docs/MountType.md)
  - [NodeState](docs/NodeState.md)
  - [OpticalTubeType](docs/OpticalTubeType.md)
  - [ShutterType](docs/ShutterType.md)
  - [SuccessfulCreate](docs/SuccessfulCreate.md)
  - [TrackingType](docs/TrackingType.md)
```

