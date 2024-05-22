# Comparing `tmp/ourskyai_sda_api-1.3.3603.tar.gz` & `tmp/ourskyai_sda_api-1.3.3644.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_sda_api-1.3.3603.tar", max compression
+gzip compressed data, was "ourskyai_sda_api-1.3.3644.tar", max compression
```

## Comparing `ourskyai_sda_api-1.3.3603.tar` & `ourskyai_sda_api-1.3.3644.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0    10115 2024-05-17 19:15:26.271831 ourskyai_sda_api-1.3.3603/README.md
--rw-r--r--   0        0        0     5163 2024-05-17 19:15:28.983932 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/__init__.py
--rw-r--r--   0        0        0      104 2024-05-17 19:15:29.019934 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api/__init__.py
--rw-r--r--   0        0        0   220784 2024-05-17 19:15:29.099937 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api/default_api.py
--rw-r--r--   0        0        0    30830 2024-05-17 19:15:29.147939 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-17 19:15:29.187940 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api_response.py
--rw-r--r--   0        0        0    15175 2024-05-17 19:15:29.267943 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/configuration.py
--rw-r--r--   0        0        0     5923 2024-05-17 19:15:29.359947 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/exceptions.py
--rw-r--r--   0        0        0     4542 2024-05-17 19:15:29.399948 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/__init__.py
--rw-r--r--   0        0        0     4311 2024-05-17 19:15:29.435949 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/astrometric_offsets.py
--rw-r--r--   0        0        0     2394 2024-05-17 19:15:29.479951 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/empty_success.py
--rw-r--r--   0        0        0     1676 2024-05-17 19:15:29.531953 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/filter_type.py
--rw-r--r--   0        0        0     2645 2024-05-17 19:15:29.595955 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/location.py
--rw-r--r--   0        0        0     1237 2024-05-17 19:15:29.643957 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/mount_type.py
--rw-r--r--   0        0        0     2756 2024-05-17 19:15:29.715960 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_bounding_box.py
--rw-r--r--   0        0        0     3713 2024-05-17 19:15:29.775962 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_quality.py
--rw-r--r--   0        0        0     6381 2024-05-17 19:15:29.835965 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_result.py
--rw-r--r--   0        0        0     1320 2024-05-17 19:15:29.871966 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_state.py
--rw-r--r--   0        0        0     1529 2024-05-17 19:15:29.923968 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/orbit_type.py
--rw-r--r--   0        0        0     1361 2024-05-17 19:15:29.999971 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/satellite_target_tracking_status.py
--rw-r--r--   0        0        0     1241 2024-05-17 19:15:30.079974 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/shutter_type.py
--rw-r--r--   0        0        0     2382 2024-05-17 19:15:30.135976 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/successful_create.py
--rw-r--r--   0        0        0     1258 2024-05-17 19:15:30.211979 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/tracking_type.py
--rw-r--r--   0        0        0     2534 2024-05-17 19:15:30.271981 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2605 2024-05-17 19:15:30.343984 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     3169 2024-05-17 19:15:30.407986 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2609 2024-05-17 19:15:30.479989 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_organization_target_request.py
--rw-r--r--   0        0        0     2761 2024-05-17 19:15:30.535991 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_satellite_target_request.py
--rw-r--r--   0        0        0     3373 2024-05-17 19:15:30.587993 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_search_instruction_request.py
--rw-r--r--   0        0        0     3353 2024-05-17 19:15:30.639995 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
--rw-r--r--   0        0        0     3017 2024-05-17 19:15:30.691997 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
--rw-r--r--   0        0        0     4457 2024-05-17 19:15:30.723998 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3922 2024-05-17 19:15:30.768000 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5657 2024-05-17 19:15:30.808001 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     4676 2024-05-17 19:15:30.856003 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_feature.py
--rw-r--r--   0        0        0     3748 2024-05-17 19:15:30.912005 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_sequence_result.py
--rw-r--r--   0        0        0     4306 2024-05-17 19:15:30.968007 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
--rw-r--r--   0        0        0     4637 2024-05-17 19:15:31.016009 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_status.py
--rw-r--r--   0        0        0     3192 2024-05-17 19:15:31.092012 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_organization_target.py
--rw-r--r--   0        0        0     3644 2024-05-17 19:15:31.144014 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_satellite_potential.py
--rw-r--r--   0        0        0     3528 2024-05-17 19:15:31.188015 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_satellite_target.py
--rw-r--r--   0        0        0     3733 2024-05-17 19:15:31.312020 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_search_instruction.py
--rw-r--r--   0        0        0     3407 2024-05-17 19:15:31.364022 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_search_instruction_step.py
--rw-r--r--   0        0        0     3634 2024-05-17 19:15:31.408024 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_survey_instruction.py
--rw-r--r--   0        0        0     2799 2024-05-17 19:15:31.460026 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_survey_instruction_step.py
--rw-r--r--   0        0        0     2695 2024-05-17 19:15:31.536028 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_target_correlation.py
--rw-r--r--   0        0        0     3185 2024-05-17 19:15:31.600031 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_tdm.py
--rw-r--r--   0        0        0     2575 2024-05-17 19:15:31.656033 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_email_configuration_request.py
--rw-r--r--   0        0        0     2913 2024-05-17 19:15:31.716035 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_satellite_target_request.py
--rw-r--r--   0        0        0     3146 2024-05-17 19:15:31.772037 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
--rw-r--r--   0        0        0     2963 2024-05-17 19:15:31.832040 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_webhook_configuration.py
--rw-r--r--   0        0        0     1386 2024-05-17 19:15:31.884042 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/weather_condition.py
--rw-r--r--   0        0        0     1350 2024-05-17 19:15:31.920043 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/webhook_auth_type.py
--rw-r--r--   0        0        0     1734 2024-05-17 19:15:31.956044 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/webhook_event.py
--rw-r--r--   0        0        0        0 2024-05-17 19:15:31.988046 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/py.typed
--rw-r--r--   0        0        0    13423 2024-05-17 19:15:32.060048 ourskyai_sda_api-1.3.3603/ourskyai_sda_api/rest.py
--rw-r--r--   0        0        0      731 2024-05-17 19:15:32.104050 ourskyai_sda_api-1.3.3603/pyproject.toml
--rw-r--r--   0        0        0    11077 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3603/PKG-INFO
+-rw-r--r--   0        0        0    10151 2024-05-22 19:37:35.277254 ourskyai_sda_api-1.3.3644/README.md
+-rw-r--r--   0        0        0     5222 2024-05-22 19:37:38.077285 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-22 19:37:38.113286 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/api/__init__.py
+-rw-r--r--   0        0        0   220784 2024-05-22 19:37:38.281288 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/api/default_api.py
+-rw-r--r--   0        0        0    30830 2024-05-22 19:37:38.333288 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-22 19:37:38.377288 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/api_response.py
+-rw-r--r--   0        0        0    15175 2024-05-22 19:37:38.409289 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/configuration.py
+-rw-r--r--   0        0        0     5923 2024-05-22 19:37:38.441289 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/exceptions.py
+-rw-r--r--   0        0        0     4601 2024-05-22 19:37:38.525290 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/__init__.py
+-rw-r--r--   0        0        0     4311 2024-05-22 19:37:38.593291 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/astrometric_offsets.py
+-rw-r--r--   0        0        0     2394 2024-05-22 19:37:38.633291 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/empty_success.py
+-rw-r--r--   0        0        0     1676 2024-05-22 19:37:38.689292 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/filter_type.py
+-rw-r--r--   0        0        0     2420 2024-05-22 19:37:38.733292 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/fits_header.py
+-rw-r--r--   0        0        0     2645 2024-05-22 19:37:38.765293 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/location.py
+-rw-r--r--   0        0        0     1237 2024-05-22 19:37:38.821293 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/mount_type.py
+-rw-r--r--   0        0        0     2756 2024-05-22 19:37:38.889294 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/observation_bounding_box.py
+-rw-r--r--   0        0        0     3713 2024-05-22 19:37:38.937295 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/observation_quality.py
+-rw-r--r--   0        0        0     6381 2024-05-22 19:37:39.005295 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/observation_result.py
+-rw-r--r--   0        0        0     1320 2024-05-22 19:37:39.053296 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/observation_state.py
+-rw-r--r--   0        0        0     1529 2024-05-22 19:37:39.105296 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/orbit_type.py
+-rw-r--r--   0        0        0     1361 2024-05-22 19:37:39.169297 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/satellite_target_tracking_status.py
+-rw-r--r--   0        0        0     1241 2024-05-22 19:37:39.213298 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/shutter_type.py
+-rw-r--r--   0        0        0     2382 2024-05-22 19:37:39.269298 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/successful_create.py
+-rw-r--r--   0        0        0     1258 2024-05-22 19:37:39.309299 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2534 2024-05-22 19:37:39.365299 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2605 2024-05-22 19:37:39.417300 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     3169 2024-05-22 19:37:39.469300 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2609 2024-05-22 19:37:39.517301 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_organization_target_request.py
+-rw-r--r--   0        0        0     2761 2024-05-22 19:37:39.569301 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_satellite_target_request.py
+-rw-r--r--   0        0        0     3373 2024-05-22 19:37:39.621302 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_search_instruction_request.py
+-rw-r--r--   0        0        0     3353 2024-05-22 19:37:39.661303 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_survey_instruction_request.py
+-rw-r--r--   0        0        0     3017 2024-05-22 19:37:39.701303 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_get_satellite_targets_response.py
+-rw-r--r--   0        0        0     4457 2024-05-22 19:37:39.753304 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3922 2024-05-22 19:37:39.849305 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     6285 2024-05-22 19:37:39.913305 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     4676 2024-05-22 19:37:39.973306 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_observation_feature.py
+-rw-r--r--   0        0        0     3748 2024-05-22 19:37:40.029307 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_observation_sequence_result.py
+-rw-r--r--   0        0        0     4306 2024-05-22 19:37:40.101307 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py
+-rw-r--r--   0        0        0     4637 2024-05-22 19:37:40.149308 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_observation_status.py
+-rw-r--r--   0        0        0     3192 2024-05-22 19:37:40.213309 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_organization_target.py
+-rw-r--r--   0        0        0     3644 2024-05-22 19:37:40.273309 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_satellite_potential.py
+-rw-r--r--   0        0        0     3528 2024-05-22 19:37:40.329310 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_satellite_target.py
+-rw-r--r--   0        0        0     3733 2024-05-22 19:37:40.385311 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_search_instruction.py
+-rw-r--r--   0        0        0     3407 2024-05-22 19:37:40.417311 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_search_instruction_step.py
+-rw-r--r--   0        0        0     3634 2024-05-22 19:37:40.469311 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_survey_instruction.py
+-rw-r--r--   0        0        0     2799 2024-05-22 19:37:40.513312 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_survey_instruction_step.py
+-rw-r--r--   0        0        0     3716 2024-05-22 19:37:40.569312 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_target_correlation.py
+-rw-r--r--   0        0        0     3185 2024-05-22 19:37:40.625313 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_tdm.py
+-rw-r--r--   0        0        0     2575 2024-05-22 19:37:40.717314 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_update_email_configuration_request.py
+-rw-r--r--   0        0        0     2913 2024-05-22 19:37:40.765315 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_update_satellite_target_request.py
+-rw-r--r--   0        0        0     3146 2024-05-22 19:37:40.821315 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py
+-rw-r--r--   0        0        0     2963 2024-05-22 19:37:40.881316 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_webhook_configuration.py
+-rw-r--r--   0        0        0     1386 2024-05-22 19:37:40.929317 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/weather_condition.py
+-rw-r--r--   0        0        0     1350 2024-05-22 19:37:40.985317 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/webhook_auth_type.py
+-rw-r--r--   0        0        0     1734 2024-05-22 19:37:41.029318 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/webhook_event.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:37:41.061318 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/py.typed
+-rw-r--r--   0        0        0    13423 2024-05-22 19:37:41.109319 ourskyai_sda_api-1.3.3644/ourskyai_sda_api/rest.py
+-rw-r--r--   0        0        0      731 2024-05-22 19:37:41.165319 ourskyai_sda_api-1.3.3644/pyproject.toml
+-rw-r--r--   0        0        0    11113 1970-01-01 00:00:00.000000 ourskyai_sda_api-1.3.3644/PKG-INFO
```

### Comparing `ourskyai_sda_api-1.3.3603/README.md` & `ourskyai_sda_api-1.3.3644/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3603
-- Package version: 1.3.3603
+- API version: 1.3.3644
+- Package version: 1.3.3644
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -121,14 +121,15 @@
 
 
 ## Documentation For Models
 
  - [AstrometricOffsets](docs/AstrometricOffsets.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
+ - [FitsHeader](docs/FitsHeader.md)
  - [Location](docs/Location.md)
  - [MountType](docs/MountType.md)
  - [ObservationBoundingBox](docs/ObservationBoundingBox.md)
  - [ObservationQuality](docs/ObservationQuality.md)
  - [ObservationResult](docs/ObservationResult.md)
  - [ObservationState](docs/ObservationState.md)
  - [OrbitType](docs/OrbitType.md)
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/__init__.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3603"
+__version__ = "1.3.3644"
 
 # import apis into sdk package
 from ourskyai_sda_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_sda_api.api_response import ApiResponse
 from ourskyai_sda_api.api_client import ApiClient
@@ -30,14 +30,15 @@
 from ourskyai_sda_api.exceptions import ApiAttributeError
 from ourskyai_sda_api.exceptions import ApiException
 
 # import models into sdk package
 from ourskyai_sda_api.models.astrometric_offsets import AstrometricOffsets
 from ourskyai_sda_api.models.empty_success import EmptySuccess
 from ourskyai_sda_api.models.filter_type import FilterType
+from ourskyai_sda_api.models.fits_header import FitsHeader
 from ourskyai_sda_api.models.location import Location
 from ourskyai_sda_api.models.mount_type import MountType
 from ourskyai_sda_api.models.observation_bounding_box import ObservationBoundingBox
 from ourskyai_sda_api.models.observation_quality import ObservationQuality
 from ourskyai_sda_api.models.observation_result import ObservationResult
 from ourskyai_sda_api.models.observation_state import ObservationState
 from ourskyai_sda_api.models.orbit_type import OrbitType
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api/default_api.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api_client.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/api_response.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/configuration.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/exceptions.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/__init__.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 # flake8: noqa
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from ourskyai_sda_api.models.astrometric_offsets import AstrometricOffsets
 from ourskyai_sda_api.models.empty_success import EmptySuccess
 from ourskyai_sda_api.models.filter_type import FilterType
+from ourskyai_sda_api.models.fits_header import FitsHeader
 from ourskyai_sda_api.models.location import Location
 from ourskyai_sda_api.models.mount_type import MountType
 from ourskyai_sda_api.models.observation_bounding_box import ObservationBoundingBox
 from ourskyai_sda_api.models.observation_quality import ObservationQuality
 from ourskyai_sda_api.models.observation_result import ObservationResult
 from ourskyai_sda_api.models.observation_state import ObservationState
 from ourskyai_sda_api.models.orbit_type import OrbitType
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/astrometric_offsets.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/astrometric_offsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/empty_success.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/empty_success.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/filter_type.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/location.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/mount_type.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/mount_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_bounding_box.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/observation_bounding_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_quality.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/observation_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_result.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/observation_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/observation_state.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/observation_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/orbit_type.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/orbit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/satellite_target_tracking_status.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/satellite_target_tracking_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/shutter_type.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/shutter_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/successful_create.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/successful_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/tracking_type.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/tracking_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_image_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_image_set_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_image_response.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_image_set_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_organization_target_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_organization_target_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_satellite_target_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_satellite_target_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_search_instruction_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_search_instruction_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_create_survey_instruction_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_create_survey_instruction_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_get_satellite_targets_response.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_get_satellite_targets_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_ground_station_participant.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_ground_station_participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_image_set.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_image_set_image.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_image_set_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
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
+from ourskyai_sda_api.models.fits_header import FitsHeader
 
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

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_feature.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_observation_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_sequence_result.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_observation_sequence_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_observation_sequence_result_image_sets_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_observation_status.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_observation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_organization_target.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_organization_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_satellite_potential.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_satellite_potential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_satellite_target.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_satellite_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_search_instruction.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_search_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_search_instruction_step.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_search_instruction_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_survey_instruction.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_survey_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_survey_instruction_step.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_survey_instruction_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_target_correlation.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/fits_header.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
 
-class V1TargetCorrelation(BaseModel):
+from pydantic import BaseModel, Field, StrictStr
+
+class FitsHeader(BaseModel):
     """
-    Target Correlation  # noqa: E501
+    FitsHeader
     """
-    target_id: StrictStr = Field(..., alias="targetId")
-    ra: Union[StrictFloat, StrictInt] = Field(...)
-    dec: Union[StrictFloat, StrictInt] = Field(...)
-    __properties = ["targetId", "ra", "dec"]
+    key: StrictStr = Field(...)
+    value: StrictStr = Field(...)
+    __properties = ["key", "value"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,36 +39,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1TargetCorrelation:
-        """Create an instance of V1TargetCorrelation from a JSON string"""
+    def from_json(cls, json_str: str) -> FitsHeader:
+        """Create an instance of FitsHeader from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1TargetCorrelation:
-        """Create an instance of V1TargetCorrelation from a dict"""
+    def from_dict(cls, obj: dict) -> FitsHeader:
+        """Create an instance of FitsHeader from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return V1TargetCorrelation.parse_obj(obj)
+            return FitsHeader.parse_obj(obj)
 
-        _obj = V1TargetCorrelation.parse_obj({
-            "target_id": obj.get("targetId"),
-            "ra": obj.get("ra"),
-            "dec": obj.get("dec")
+        _obj = FitsHeader.parse_obj({
+            "key": obj.get("key"),
+            "value": obj.get("value")
         })
         return _obj
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_tdm.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_tdm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_email_configuration_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_update_email_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_satellite_target_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_update_satellite_target_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_update_webhook_configuration_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/v1_webhook_configuration.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/v1_webhook_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/weather_condition.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/weather_condition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/webhook_auth_type.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/webhook_auth_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/models/webhook_event.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/models/webhook_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_sda_api-1.3.3603/ourskyai_sda_api/rest.py` & `ourskyai_sda_api-1.3.3644/ourskyai_sda_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky SDA
 
     The basic flow for a new organization is as follows: 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe. 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above. 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
-    The version of the OpenAPI document: 1.3.3603
+    The version of the OpenAPI document: 1.3.3644
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_sda_api-1.3.3603/pyproject.toml` & `ourskyai_sda_api-1.3.3644/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_sda_api"
-version = "1.3.3603"
+version = "1.3.3644"
 description = "OurSky SDA"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky SDA"]
 include = ["ourskyai_sda_api/py.typed"]
```

### Comparing `ourskyai_sda_api-1.3.3603/PKG-INFO` & `ourskyai_sda_api-1.3.3644/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_sda_api
-Version: 1.3.3603
+Version: 1.3.3644
 Summary: OurSky SDA
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky SDA
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -27,16 +27,16 @@
 The basic flow for a new organization is as follows:
 1. View the available satellite targets with the [satellite targets](#tag/satellite-targets/[get]/v1/satellite-targets) endpoint. Copy the id of the target you want to observe.
 2. Create an organization target with the [organization target](#tag/organization-targets/[get]/v1/organization-targets) endpoint. Use the id copied from above.
 3. Create a webhook with the [webhook](#tag/webhooks/[post]/v1/communications/webhook) endpoint to receive TDMs automatically (preferred) or use the [tdms](#tag/tdms/[get]/v1/tdms) endpoint to poll for TDMs.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3603
-- Package version: 1.3.3603
+- API version: 1.3.3644
+- Package version: 1.3.3644
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -146,14 +146,15 @@
 
 
 ## Documentation For Models
 
  - [AstrometricOffsets](docs/AstrometricOffsets.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
+ - [FitsHeader](docs/FitsHeader.md)
  - [Location](docs/Location.md)
  - [MountType](docs/MountType.md)
  - [ObservationBoundingBox](docs/ObservationBoundingBox.md)
  - [ObservationQuality](docs/ObservationQuality.md)
  - [ObservationResult](docs/ObservationResult.md)
  - [ObservationState](docs/ObservationState.md)
  - [OrbitType](docs/OrbitType.md)
```

