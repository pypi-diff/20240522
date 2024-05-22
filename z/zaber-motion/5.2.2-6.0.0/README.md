# Comparing `tmp/zaber_motion-5.2.2.tar.gz` & `tmp/zaber_motion-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-5.2.2.tar", last modified: Thu May 16 18:25:41 2024, max compression
+gzip compressed data, was "zaber_motion-6.0.0.tar", last modified: Tue May 21 23:06:58 2024, max compression
```

## Comparing `zaber_motion-5.2.2.tar` & `zaber_motion-6.0.0.tar`

### file list

```diff
@@ -1,221 +1,449 @@
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.898795 zaber_motion-5.2.2/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)   109244 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/LICENSE.txt
--rw-rw-rw-   0 ubuntu    (1001) root         (0)       66 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/MANIFEST.in
--rw-r--r--   0 ubuntu    (1001) root         (0)   128259 2024-05-16 18:25:41.898795 zaber_motion-5.2.2/PKG-INFO
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      470 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/README.md
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1474 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/pyproject.toml
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      105 2024-05-16 18:25:41.898795 zaber_motion-5.2.2/setup.cfg
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1359 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/setup.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.889795 zaber_motion-5.2.2/zaber_motion/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     6891 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/__init__.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.892795 zaber_motion-5.2.2/zaber_motion/ascii/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3721 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2185 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/alert_event.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     8708 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/all_axes.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    52240 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/axis.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    13661 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/axis_group.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2681 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/axis_identity.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    16542 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/axis_settings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      301 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/axis_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1265 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/can_set_state_axis_response.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1530 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/can_set_state_device_response.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    35017 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/connection.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1959 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/conversion_factor.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    25265 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/device.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2801 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/device_identity.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    38262 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/device_io.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2077 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/device_io_info.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    15418 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/device_settings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      274 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/digital_output_action.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1629 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/get_axis_setting.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1435 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/get_axis_setting_result.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2013 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/get_setting.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1501 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/get_setting_result.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1439 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/io_port_label.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/io_port_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    37243 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/lockstep.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1671 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/lockstep_axes.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      386 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/message_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    20711 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/oscilloscope.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2423 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     7109 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/oscilloscope_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      268 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/oscilloscope_data_source.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1601 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/paramset_info.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2078 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/pid_tuning.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2848 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/pvt.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2071 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/pvt_axis_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      256 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/pvt_axis_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3190 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/pvt_buffer.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      247 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/pvt_mode.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    33848 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/pvt_sequence.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2896 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/response.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    20870 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/servo_tuner.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1782 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/servo_tuning_param.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      384 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/servo_tuning_paramset.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    26300 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/setting_constants.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2166 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/simple_tuning.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2340 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    26082 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/storage.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    83863 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/stream.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2110 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/stream_axis_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      253 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/stream_axis_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3084 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/stream_buffer.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      273 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/stream_mode.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2836 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/streams.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     5345 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/transport.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    26434 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/trigger.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      244 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/trigger_action.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/trigger_condition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1429 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/trigger_enabled_state.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      275 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/trigger_operation.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2231 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/trigger_state.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     6058 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/triggers.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2966 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/unknown_response_event.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2855 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/warning_flags.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     5066 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/ascii/warnings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1505 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/async_utils.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1664 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/axis_address.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.892795 zaber_motion-5.2.2/zaber_motion/binary/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      653 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1941 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/binary_settings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3133 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/command_code.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    19670 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/connection.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    29083 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/device.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3361 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/device_identity.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3513 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/device_settings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      276 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/device_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3116 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/error_code.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1498 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/message.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      415 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/reply_code.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1552 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/reply_only_event.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1588 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/binary/unknown_response_event.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1442 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/bindings.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4187 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/call.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     7475 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/convert_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      257 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/device_db_source_type.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2190 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/events.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.895795 zaber_motion-5.2.2/zaber_motion/exceptions/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     7583 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1121 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      991 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1045 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/command_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3097 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/command_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/command_preempted_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1129 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/command_too_long_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1971 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      304 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/connection_closed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/connection_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/conversion_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1158 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1126 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      314 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/device_busy_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1092 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/device_db_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      911 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      283 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      335 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/device_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      317 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/device_not_identified_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1065 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/g_code_execution_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1321 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1036 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1300 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      309 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/internal_error_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      295 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_argument_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      300 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_data_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      310 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_operation_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1058 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_packet_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1198 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      282 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1140 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_pvt_point.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1091 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_response_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      928 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      342 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/io_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      322 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      329 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      386 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/motion_lib_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1070 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/movement_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1852 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1137 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1875 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/no_device_found_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/not_supported_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1095 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/operation_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1861 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/operation_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/os_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      317 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      323 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_discontinuity_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1037 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_execution_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1749 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_execution_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      326 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_mode_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1102 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_movement_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1292 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1169 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1327 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      285 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/pvt_setup_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      300 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/request_timeout_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      349 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3563 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1085 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2372 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1120 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/setting_not_found_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_discontinuity_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1060 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_execution_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1232 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      323 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_mode_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1134 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1313 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1199 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1348 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      282 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      341 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/timeout_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/transport_already_used_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      335 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/exceptions/unknown_request_exception.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2088 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/firmware_version.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.896795 zaber_motion-5.2.2/zaber_motion/gcode/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      578 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2340 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/axis_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1547 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/axis_mapping.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2250 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/axis_transformation.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2360 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/device_definition.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    12481 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/offline_translator.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1555 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/translate_message.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1401 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/translate_result.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    13105 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/translator.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2206 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/gcode/translator_config.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     3346 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/library.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      279 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/log_output_mode.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1937 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/measurement.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.896795 zaber_motion-5.2.2/zaber_motion/microscopy/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      370 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/microscopy/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4647 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/microscopy/filter_changer.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4175 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/microscopy/illuminator.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    19521 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/microscopy/illuminator_channel.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     7395 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/microscopy/microscope.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4844 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/microscopy/microscope_config.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    13576 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.896795 zaber_motion-5.2.2/zaber_motion/product/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      394 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/product/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    26843 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/product/process.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     4171 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/product/process_controller.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/product/process_controller_mode.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2074 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/product/process_controller_source.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      281 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/product/process_controller_source_sensor.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.896795 zaber_motion-5.2.2/zaber_motion/protobufs/
--rw-rw-rw-   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/protobufs/__init__.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    83532 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/protobufs/main_pb2.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)   257403 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/protobufs/main_pb2.pyi
--rw-rw-rw-   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/py.typed
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      278 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/rotation_direction.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)      987 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/serialization.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     2108 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/tools.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)     1553 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/unit_table.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)    10446 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/units.py
--rw-rw-rw-   0 ubuntu    (1001) root         (0)       22 2024-05-16 18:23:58.000000 zaber_motion-5.2.2/zaber_motion/version.py
-drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-16 18:25:41.897795 zaber_motion-5.2.2/zaber_motion.egg-info/
--rw-r--r--   0 ubuntu    (1001) root         (0)   128259 2024-05-16 18:25:41.000000 zaber_motion-5.2.2/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1001) root         (0)     8939 2024-05-16 18:25:41.000000 zaber_motion-5.2.2/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1001) root         (0)        1 2024-05-16 18:25:41.000000 zaber_motion-5.2.2/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1001) root         (0)      212 2024-05-16 18:25:41.000000 zaber_motion-5.2.2/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1001) root         (0)       27 2024-05-16 18:25:41.000000 zaber_motion-5.2.2/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.452649 zaber_motion-6.0.0/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)   109244 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/LICENSE.txt
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)       58 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1001) root         (0)   128206 2024-05-21 23:06:58.452649 zaber_motion-6.0.0/PKG-INFO
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      470 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/README.md
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1461 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/pyproject.toml
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      105 2024-05-21 23:06:58.453649 zaber_motion-6.0.0/setup.cfg
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1359 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/setup.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.406649 zaber_motion-6.0.0/zaber_motion/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     9326 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/__init__.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.410649 zaber_motion-6.0.0/zaber_motion/ascii/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4237 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     8639 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/all_axes.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    50531 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/axis.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    12927 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/axis_group.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    15954 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/axis_settings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    35743 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/connection.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    24912 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/device.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    37408 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/device_io.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    14987 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/device_settings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    35688 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/lockstep.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    20306 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/oscilloscope.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     7031 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/oscilloscope_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2865 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/pvt.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3165 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/pvt_buffer.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    32398 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/pvt_sequence.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    20111 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/servo_tuner.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    26300 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/setting_constants.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    26073 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/storage.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    78560 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/stream.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3079 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/stream_buffer.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2853 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/streams.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     5397 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/transport.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    25402 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/trigger.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     6035 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/triggers.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2855 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/warning_flags.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     5061 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/ascii/warnings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1505 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/async_utils.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.410649 zaber_motion-6.0.0/zaber_motion/binary/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      859 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/binary/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    20359 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/binary/connection.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    28512 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/binary/device.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3349 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/binary/device_settings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1442 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/bindings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     5206 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/call.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     7589 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/convert_exception.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.411649 zaber_motion-6.0.0/zaber_motion/dto/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      458 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/__init__.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.415649 zaber_motion-6.0.0/zaber_motion/dto/ascii/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2582 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2190 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/alert_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2597 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/axis_identity.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      237 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/axis_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1581 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/can_set_state_axis_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1791 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/can_set_state_device_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1748 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/conversion_factor.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2637 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/device_identity.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2116 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/device_io_info.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      210 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/digital_output_action.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1616 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/get_axis_setting.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1694 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/get_axis_setting_result.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1778 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/get_setting.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1687 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/get_setting_result.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1661 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/io_port_label.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      243 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/io_port_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1778 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/lockstep_axes.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      322 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/message_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2510 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/oscilloscope_capture_properties.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      204 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/oscilloscope_data_source.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1756 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/paramset_info.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2027 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/pid_tuning.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1637 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/pvt_axis_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      192 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/pvt_axis_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      183 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/pvt_mode.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2729 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1415 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/servo_tuning_param.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/servo_tuning_paramset.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2151 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/simple_tuning.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2262 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/simple_tuning_param_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1664 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/stream_axis_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      189 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/stream_axis_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      209 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/stream_mode.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      180 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/trigger_action.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      233 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/trigger_condition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1714 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/trigger_enabled_state.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      211 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/trigger_operation.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2163 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/trigger_state.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2825 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/ascii/unknown_response_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1320 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/axis_address.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.416649 zaber_motion-6.0.0/zaber_motion/dto/binary/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      586 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1877 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/binary_settings.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3069 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/command_code.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3116 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/device_identity.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      212 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/device_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3052 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/error_code.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1681 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/message.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      351 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/reply_code.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1742 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/reply_only_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1784 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/binary/unknown_response_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      193 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/device_db_source_type.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.419649 zaber_motion-6.0.0/zaber_motion/dto/exceptions/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2354 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1381 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/binary_command_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2842 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/command_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2089 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/command_too_long_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1447 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/device_address_conflict_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1308 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/device_db_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1613 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/g_code_execution_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1589 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/g_code_syntax_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1505 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/invalid_packet_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1437 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/invalid_pvt_point.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1322 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/invalid_response_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1915 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/movement_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1943 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/movement_interrupted_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1925 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/operation_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1902 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/pvt_execution_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1532 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/pvt_movement_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1572 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3164 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/set_device_state_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2299 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/set_peripheral_state_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1535 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/stream_execution_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1556 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/stream_movement_failed_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1596 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/exceptions/stream_movement_interrupted_exception_data.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1548 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/firmware_version.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.420649 zaber_motion-6.0.0/zaber_motion/dto/gcode/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      539 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/gcode/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1629 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/gcode/axis_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1436 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/gcode/axis_mapping.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1875 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/gcode/axis_transformation.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1994 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/gcode/device_definition.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1748 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/gcode/translate_message.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1618 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/gcode/translate_result.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2061 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/gcode/translator_config.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      215 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/log_output_mode.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1579 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/measurement.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.420649 zaber_motion-6.0.0/zaber_motion/dto/microscopy/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      149 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/microscopy/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2872 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/microscopy/microscope_config.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.420649 zaber_motion-6.0.0/zaber_motion/dto/product/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      364 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/product/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      228 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/product/process_controller_mode.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1634 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/product/process_controller_source.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      217 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/product/process_controller_source_sensor.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.444649 zaber_motion-6.0.0/zaber_motion/dto/requests/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    19921 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1432 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/alert_event_wrapper.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1498 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/axes_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1979 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/axes_get_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1786 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/axes_move_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1403 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/axis_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      174 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/axis_move_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1599 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/axis_to_string_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1412 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_device_detect_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1224 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_device_detect_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1929 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_device_get_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1728 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_device_home_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2108 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_device_move_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2058 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_device_set_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1728 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_device_stop_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2409 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_generic_with_units_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1317 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_message_collection.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1528 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/binary_reply_only_event_wrapper.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1090 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/bool_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1335 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/can_set_state_axis_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1546 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/can_set_state_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1472 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/channel_on.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1577 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/channel_set_intensity.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1401 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/custom_interface_close_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1226 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/custom_interface_open_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1219 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/custom_interface_read_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1367 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/custom_interface_write_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1750 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_cancel_all_outputs_schedule_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1722 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_cancel_output_schedule_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2176 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_convert_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1620 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_detect_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1182 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_detect_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1296 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1528 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_all_analog_io_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1234 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_all_analog_io_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1535 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_all_digital_io_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1240 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_all_digital_io_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1686 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_analog_io_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1693 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_digital_io_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1849 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1711 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_storage_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1595 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_warnings_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1205 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_get_warnings_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1602 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_home_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1704 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_identify_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3201 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_move_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2128 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_multi_get_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1355 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_on_all_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1227 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_on_all_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1357 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_renumber_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1562 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_all_analog_outputs_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2211 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_all_analog_outputs_schedule_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1710 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_all_digital_outputs_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2438 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_all_digital_outputs_schedule_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1674 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_analog_output_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2284 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_analog_output_schedule_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1870 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_digital_output_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2607 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_digital_output_schedule_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1978 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1743 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_setting_str_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1733 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_storage_bool_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1740 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_storage_number_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1840 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_storage_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1965 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_set_unit_conversions_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1602 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_stop_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1622 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_storage_list_keys_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1548 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_storage_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      137 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1693 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/device_wait_until_idle_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1846 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/disconnected_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1171 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/double_array_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1097 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/double_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      954 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1560 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/errors.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1335 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/find_device_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1135 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/find_device_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1083 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/gateway_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1109 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/gateway_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1695 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/gateway_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2030 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/generic_binary_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1894 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/generic_command_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1389 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/generic_command_response_collection.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1343 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/get_all_io_port_labels_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1351 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/get_axis_setting_results.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1782 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/get_io_port_label_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1306 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/get_setting_results.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1492 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/get_simple_tuning_param_definition_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1148 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/int_array_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1067 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/int_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1074 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/int_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1184 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/interface_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      182 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/interface_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2029 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/load_paramset.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1711 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_disable_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1505 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1666 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_enable_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1234 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_get_axis_numbers_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1747 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_get_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1690 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_home_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3152 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_move_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2031 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_set_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1690 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_stop_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1781 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/lockstep_wait_until_idle_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1361 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/microscope_config_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1514 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/microscope_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1643 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/microscope_init_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2252 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/objective_changer_change_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1541 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/objective_changer_create_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1235 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/objective_changer_get_current_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1705 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/objective_changer_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2111 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/objective_changer_set_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2142 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/open_binary_interface_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3012 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/open_interface_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1184 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/open_interface_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1816 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_add_io_channel_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1684 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_add_setting_channel_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1445 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_data_get_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1642 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_data_get_sample_time_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1264 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_data_get_samples_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1189 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_data_identifier.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1214 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_read_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1303 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1517 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/oscilloscope_start_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1938 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/prepare_command_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1875 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/process_on.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2712 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/pvt_point_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      125 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/response_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1395 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/servo_tuning_paramset_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1753 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/servo_tuning_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1568 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_device_db_source_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1439 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_interface_checksum_enabled_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1358 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_interface_timeout_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1154 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_internal_mode_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1911 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_io_port_label_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1424 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_log_output_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1836 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_process_controller_source.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2221 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_servo_tuning_pid_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2125 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_servo_tuning_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2425 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_simple_tuning.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1695 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/set_state_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3734 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_arc_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1611 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_buffer_erase_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1646 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_buffer_get_content_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1280 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_buffer_get_content_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1406 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_buffer_list.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1890 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_call_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3028 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_circle_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1569 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1827 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_generic_command_batch_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1773 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_generic_command_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1657 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_get_axes_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1993 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_get_max_centripetal_acceleration_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1867 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_get_max_speed_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1986 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_get_max_tangential_acceleration_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2390 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_line_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1554 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_mode_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      129 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_segment_type.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1835 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_set_all_analog_outputs_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1983 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_set_all_digital_outputs_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1947 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_set_analog_output_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2143 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_set_digital_output_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2256 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_set_max_centripetal_acceleration_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2018 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_set_max_speed_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2243 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_set_max_tangential_acceleration_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2300 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_setup_live_composite_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1751 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_setup_live_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2178 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_setup_store_arbitrary_axes_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2635 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_setup_store_composite_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2086 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_setup_store_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2100 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_wait_analog_input_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1961 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_wait_digital_input_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1941 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_wait_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1845 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/stream_wait_until_idle_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1169 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/string_array_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1097 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/string_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1056 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/test_event.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1506 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/test_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1105 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/test_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1164 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/test_response_long.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1391 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/toggle_device_db_store_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1226 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/tools_list_serial_ports_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1891 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_create_from_device_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1844 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_create_live_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1709 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_create_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1211 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_create_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1197 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1417 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_flush_live_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1209 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_flush_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1831 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_get_axis_offset_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1646 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_get_axis_position_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1793 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_set_axis_position_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1460 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_set_feed_rate_override_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1698 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_set_traverse_rate_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1354 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/translator_translate_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1811 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_clear_action_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1482 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_empty_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1616 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_enable_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1333 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_enabled_states.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1948 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_fire_at_interval_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2146 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_fire_when_distance_travelled_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2440 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_fire_when_io_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1656 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_fire_when_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2568 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_fire_when_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2038 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_on_fire_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2767 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_on_fire_set_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2763 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_on_fire_set_to_setting_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1255 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/trigger_states.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1131 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/unit_get_enum_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1259 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/unit_get_enum_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1266 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/unit_get_symbol_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1152 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/unit_get_symbol_response.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1670 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/unknown_binary_response_event_wrapper.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1627 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/unknown_response_event_wrapper.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1820 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/wait_to_clear_warnings_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1451 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/requests/wait_to_respond_request.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      214 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto/rotation_direction.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      254 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/dto_object.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2691 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/events.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.450649 zaber_motion-6.0.0/zaber_motion/exceptions/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     7973 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      976 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      906 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/command_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/command_preempted_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      989 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/command_too_long_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      304 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/connection_closed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/connection_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1011 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      314 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/device_busy_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      952 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      283 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      335 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/device_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      317 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      925 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      899 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      309 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/internal_error_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      295 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      300 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/invalid_data_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      310 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      919 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      282 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      381 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/invalid_request_data_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      950 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/invalid_response_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      342 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/io_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      322 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      329 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      386 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/motion_lib_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      930 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/movement_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      992 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      292 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/no_device_found_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      297 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      308 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/not_supported_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      954 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/operation_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/os_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      317 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      323 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      899 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      326 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      959 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1021 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      285 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      300 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/request_timeout_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      349 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      945 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      976 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      307 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      919 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/stream_execution_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      323 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/stream_mode_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      988 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1048 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      282 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      341 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/timeout_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      320 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      335 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/exceptions/unknown_request_exception.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.450649 zaber_motion-6.0.0/zaber_motion/gcode/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      753 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/gcode/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    12118 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/gcode/offline_translator.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    12835 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/gcode/translator.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     3327 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/library.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.451649 zaber_motion-6.0.0/zaber_motion/microscopy/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      484 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/microscopy/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4651 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/microscopy/filter_changer.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4151 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/microscopy/illuminator.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    19265 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/microscopy/illuminator_channel.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     7191 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/microscopy/microscope.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    13373 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.451649 zaber_motion-6.0.0/zaber_motion/product/
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      531 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/product/__init__.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    26272 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/product/process.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     4185 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/product/process_controller.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/py.typed
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)      987 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/serialization.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     2213 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/tools.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)     1540 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/unit_table.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)    10446 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/units.py
+-rw-rw-rw-   0 ubuntu    (1001) root         (0)       22 2024-05-21 23:05:42.000000 zaber_motion-6.0.0/zaber_motion/version.py
+drwxr-xr-x   0 ubuntu    (1001) root         (0)        0 2024-05-21 23:06:58.451649 zaber_motion-6.0.0/zaber_motion.egg-info/
+-rw-r--r--   0 ubuntu    (1001) root         (0)   128206 2024-05-21 23:06:58.000000 zaber_motion-6.0.0/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1001) root         (0)    21650 2024-05-21 23:06:58.000000 zaber_motion-6.0.0/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1001) root         (0)        1 2024-05-21 23:06:58.000000 zaber_motion-6.0.0/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1001) root         (0)      190 2024-05-21 23:06:58.000000 zaber_motion-6.0.0/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1001) root         (0)       18 2024-05-21 23:06:58.000000 zaber_motion-6.0.0/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-5.2.2/LICENSE.txt` & `zaber_motion-6.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.2/PKG-INFO` & `zaber_motion-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 5.2.2
+Version: 6.0.0
 Summary: An official library for communicating with Zaber devices.
 Author-email: "Zaber Technologies Inc." <contact@zaber.com>
 License: The MIT License (MIT)
         
         Copyright 2018-2022 Zaber Technologies Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -2133,20 +2133,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: protobuf<4.22.0,>=3.20.0
-Requires-Dist: rx>=3.0.0
+Requires-Dist: reactivex~=4.0.0
+Requires-Dist: bson~=0.5
 Provides-Extra: dev
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mypy-protobuf; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pycodestyle; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
```

### Comparing `zaber_motion-5.2.2/pyproject.toml` & `zaber_motion-6.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zaber_motion"
-version = "5.2.2"
+version = "6.0.0"
 description = "An official library for communicating with Zaber devices."
 authors = [{ name = "Zaber Technologies Inc.", email = "contact@zaber.com" }]
 license = { file = "LICENSE.txt" }
 readme = { file = "README.md", content-type = "text/markdown" }
 dependencies = [
-  "protobuf>=3.20.0,<4.22.0",
-  "rx>=3.0.0",
+    "reactivex~=4.0.0",
+    "bson~=0.5",
 ]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Libraries",
   "Programming Language :: Python :: 3",
@@ -31,22 +31,21 @@
 Changelog = "https://gitlab.com/ZaberTech/zaber-motion-lib/-/blob/master/CHANGELOG.md"
 
 
 [project.optional-dependencies]
 dev = [
     "invoke",
     "mypy",
-    "mypy-protobuf",
     "pylint",
     "pycodestyle",
     "pytest",
     "pytest-asyncio",
     "setuptools",
     "build",
     "wheel",
     "packaging",
     "twine; sys_platform == 'linux' and platform_machine == 'x86_64'",
 ]
 
 
 [tool.setuptools.packages.find]
-exclude = ["test"]
+exclude = ["test", "examples"]
```

### Comparing `zaber_motion-5.2.2/setup.py` & `zaber_motion-6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/__init__.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,40 @@
-from .connection import Connection as Connection
-from .device import Device as Device
-from .axis import Axis as Axis
-from .all_axes import AllAxes as AllAxes
-from .axis_settings import AxisSettings as AxisSettings
-from .device_settings import DeviceSettings as DeviceSettings
-from .get_setting import GetSetting as GetSetting
-from .get_axis_setting import GetAxisSetting as GetAxisSetting
-from .get_setting_result import GetSettingResult as GetSettingResult
-from .get_axis_setting_result import GetAxisSettingResult as GetAxisSettingResult
-from .io_port_type import IoPortType as IoPortType
-from .io_port_label import IoPortLabel as IoPortLabel
-from .warnings import Warnings as Warnings
-from .warning_flags import WarningFlags as WarningFlags
-from .unknown_response_event import UnknownResponseEvent as UnknownResponseEvent
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long
+from .response import Response as Response
 from .device_identity import DeviceIdentity as DeviceIdentity
-from .device_io import DeviceIO as DeviceIO
-from .device_io_info import DeviceIOInfo as DeviceIOInfo
 from .axis_identity import AxisIdentity as AxisIdentity
-from .message_type import MessageType as MessageType
-from .axis_type import AxisType as AxisType
+from .device_io_info import DeviceIOInfo as DeviceIOInfo
+from .io_port_label import IoPortLabel as IoPortLabel
+from .unknown_response_event import UnknownResponseEvent as UnknownResponseEvent
 from .alert_event import AlertEvent as AlertEvent
 from .lockstep_axes import LockstepAxes as LockstepAxes
-from .lockstep import Lockstep as Lockstep
-from .oscilloscope import Oscilloscope as Oscilloscope
-from .oscilloscope_data import OscilloscopeData as OscilloscopeData
-from .oscilloscope_data_source import OscilloscopeDataSource as OscilloscopeDataSource
 from .oscilloscope_capture_properties import OscilloscopeCaptureProperties as OscilloscopeCaptureProperties
-from .response import Response as Response
-from .setting_constants import SettingConstants as SettingConstants
-from .stream import Stream as Stream
-from .stream_buffer import StreamBuffer as StreamBuffer
-from .stream_mode import StreamMode as StreamMode
-from .stream_axis_type import StreamAxisType as StreamAxisType
 from .stream_axis_definition import StreamAxisDefinition as StreamAxisDefinition
-from .transport import Transport as Transport
-from .servo_tuner import ServoTuner as ServoTuner
-from .servo_tuning_paramset import ServoTuningParamset as ServoTuningParamset
+from .pvt_axis_definition import PvtAxisDefinition as PvtAxisDefinition
+from .can_set_state_axis_response import CanSetStateAxisResponse as CanSetStateAxisResponse
+from .can_set_state_device_response import CanSetStateDeviceResponse as CanSetStateDeviceResponse
+from .servo_tuning_param import ServoTuningParam as ServoTuningParam
 from .paramset_info import ParamsetInfo as ParamsetInfo
 from .pid_tuning import PidTuning as PidTuning
-from .servo_tuning_param import ServoTuningParam as ServoTuningParam
-from .simple_tuning import SimpleTuning as SimpleTuning
 from .simple_tuning_param_definition import SimpleTuningParamDefinition as SimpleTuningParamDefinition
-from .storage import AxisStorage as AxisStorage, DeviceStorage as DeviceStorage
+from .simple_tuning import SimpleTuning as SimpleTuning
 from .conversion_factor import ConversionFactor as ConversionFactor
-from .can_set_state_axis_response import CanSetStateAxisResponse as CanSetStateAxisResponse
-from .can_set_state_device_response import CanSetStateDeviceResponse as CanSetStateDeviceResponse
-from .pvt import Pvt as Pvt
-from .pvt_sequence import PvtSequence as PvtSequence
-from .pvt_buffer import PvtBuffer as PvtBuffer
-from .pvt_mode import PvtMode as PvtMode
-from .pvt_axis_type import PvtAxisType as PvtAxisType
-from .pvt_axis_definition import PvtAxisDefinition as PvtAxisDefinition
-from .axis_group import AxisGroup as AxisGroup
-from .triggers import Triggers as Triggers
-from .trigger import Trigger as Trigger
+from .get_setting import GetSetting as GetSetting
+from .get_axis_setting import GetAxisSetting as GetAxisSetting
+from .get_setting_result import GetSettingResult as GetSettingResult
+from .get_axis_setting_result import GetAxisSettingResult as GetAxisSettingResult
 from .trigger_state import TriggerState as TriggerState
 from .trigger_enabled_state import TriggerEnabledState as TriggerEnabledState
-from .trigger_action import TriggerAction as TriggerAction
+from .stream_axis_type import StreamAxisType as StreamAxisType
+from .pvt_axis_type import PvtAxisType as PvtAxisType
+from .message_type import MessageType as MessageType
+from .axis_type import AxisType as AxisType
+from .stream_mode import StreamMode as StreamMode
+from .pvt_mode import PvtMode as PvtMode
+from .servo_tuning_paramset import ServoTuningParamset as ServoTuningParamset
+from .io_port_type import IoPortType as IoPortType
+from .oscilloscope_data_source import OscilloscopeDataSource as OscilloscopeDataSource
 from .trigger_condition import TriggerCondition as TriggerCondition
+from .trigger_action import TriggerAction as TriggerAction
 from .trigger_operation import TriggerOperation as TriggerOperation
-from .streams import Streams as Streams
 from .digital_output_action import DigitalOutputAction as DigitalOutputAction
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/axis.py` & `zaber_motion-6.0.0/zaber_motion/ascii/axis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Optional
 from ..call import call, call_async, call_sync
 
-from ..protobufs import main_pb2
-from ..units import Units, units_from_literals, LengthUnits, VelocityUnits, AccelerationUnits
+from ..dto import requests as dto
+from ..units import Units, LengthUnits, VelocityUnits, AccelerationUnits
 from .warnings import Warnings
 from .axis_settings import AxisSettings
-from .axis_identity import AxisIdentity
+from ..dto.ascii.axis_identity import AxisIdentity
 from .storage import AxisStorage
-from .axis_type import AxisType
-from .response import Response
-from ..measurement import Measurement
+from ..dto.ascii.axis_type import AxisType
+from ..dto.ascii.response import Response
+from ..dto.measurement import Measurement
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class Axis:
     """
@@ -122,256 +122,284 @@
     ) -> None:
         """
         Homes axis. Axis returns to its homing position.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
         """
-        request = main_pb2.DeviceHomeRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.wait_until_idle = wait_until_idle
+        request = dto.DeviceHomeRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            wait_until_idle=wait_until_idle,
+        )
         call("device/home", request)
 
     async def home_async(
             self,
             wait_until_idle: bool = True
     ) -> None:
         """
         Homes axis. Axis returns to its homing position.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
         """
-        request = main_pb2.DeviceHomeRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.wait_until_idle = wait_until_idle
+        request = dto.DeviceHomeRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            wait_until_idle=wait_until_idle,
+        )
         await call_async("device/home", request)
 
     def stop(
             self,
             wait_until_idle: bool = True
     ) -> None:
         """
         Stops ongoing axis movement. Decelerates until zero speed.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
         """
-        request = main_pb2.DeviceStopRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.wait_until_idle = wait_until_idle
+        request = dto.DeviceStopRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            wait_until_idle=wait_until_idle,
+        )
         call("device/stop", request)
 
     async def stop_async(
             self,
             wait_until_idle: bool = True
     ) -> None:
         """
         Stops ongoing axis movement. Decelerates until zero speed.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
         """
-        request = main_pb2.DeviceStopRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.wait_until_idle = wait_until_idle
+        request = dto.DeviceStopRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            wait_until_idle=wait_until_idle,
+        )
         await call_async("device/stop", request)
 
     def park(
             self
     ) -> None:
         """
         Parks the axis in anticipation of turning the power off.
         It can later be powered on, unparked, and moved without first having to home it.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         call("device/park", request)
 
     async def park_async(
             self
     ) -> None:
         """
         Parks the axis in anticipation of turning the power off.
         It can later be powered on, unparked, and moved without first having to home it.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         await call_async("device/park", request)
 
     def unpark(
             self
     ) -> None:
         """
         Unparks axis. Axis will now be able to move.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         call("device/unpark", request)
 
     async def unpark_async(
             self
     ) -> None:
         """
         Unparks axis. Axis will now be able to move.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         await call_async("device/unpark", request)
 
     def is_parked(
             self
     ) -> bool:
         """
         Returns bool indicating whether the axis is parked or not.
 
         Returns:
             True if the axis is currently parked. False otherwise.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.BoolResponse()
-        call("device/is_parked", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call(
+            "device/is_parked",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_parked_async(
             self
     ) -> bool:
         """
         Returns bool indicating whether the axis is parked or not.
 
         Returns:
             True if the axis is currently parked. False otherwise.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.BoolResponse()
-        await call_async("device/is_parked", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = await call_async(
+            "device/is_parked",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def wait_until_idle(
             self,
             throw_error_on_fault: bool = True
     ) -> None:
         """
         Waits until axis stops moving.
 
         Args:
             throw_error_on_fault: Determines whether to throw error when fault is observed.
         """
-        request = main_pb2.DeviceWaitUntilIdleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.throw_error_on_fault = throw_error_on_fault
+        request = dto.DeviceWaitUntilIdleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            throw_error_on_fault=throw_error_on_fault,
+        )
         call("device/wait_until_idle", request)
 
     async def wait_until_idle_async(
             self,
             throw_error_on_fault: bool = True
     ) -> None:
         """
         Waits until axis stops moving.
 
         Args:
             throw_error_on_fault: Determines whether to throw error when fault is observed.
         """
-        request = main_pb2.DeviceWaitUntilIdleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.throw_error_on_fault = throw_error_on_fault
+        request = dto.DeviceWaitUntilIdleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            throw_error_on_fault=throw_error_on_fault,
+        )
         await call_async("device/wait_until_idle", request)
 
     def is_busy(
             self
     ) -> bool:
         """
         Returns bool indicating whether the axis is executing a motion command.
 
         Returns:
             True if the axis is currently executing a motion command.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.BoolResponse()
-        call("device/is_busy", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call(
+            "device/is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_busy_async(
             self
     ) -> bool:
         """
         Returns bool indicating whether the axis is executing a motion command.
 
         Returns:
             True if the axis is currently executing a motion command.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.BoolResponse()
-        await call_async("device/is_busy", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = await call_async(
+            "device/is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def is_homed(
             self
     ) -> bool:
         """
         Returns bool indicating whether the axis has position reference and was homed.
 
         Returns:
             True if the axis has position reference and was homed.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.BoolResponse()
-        call("device/is_homed", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call(
+            "device/is_homed",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_homed_async(
             self
     ) -> bool:
         """
         Returns bool indicating whether the axis has position reference and was homed.
 
         Returns:
             True if the axis has position reference and was homed.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.BoolResponse()
-        await call_async("device/is_homed", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = await call_async(
+            "device/is_homed",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def move_absolute(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
@@ -392,26 +420,27 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.ABS
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.ABS,
+            arg=position,
+            unit=unit,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/move", request)
 
     async def move_absolute_async(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
@@ -432,26 +461,27 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.ABS
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.ABS,
+            arg=position,
+            unit=unit,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/move", request)
 
     def move_max(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
             velocity_unit: VelocityUnits = Units.NATIVE,
@@ -468,24 +498,25 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.MAX
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.MAX,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/move", request)
 
     async def move_max_async(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
             velocity_unit: VelocityUnits = Units.NATIVE,
@@ -502,24 +533,25 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.MAX
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.MAX,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/move", request)
 
     def move_min(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
             velocity_unit: VelocityUnits = Units.NATIVE,
@@ -536,24 +568,25 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.MIN
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.MIN,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/move", request)
 
     async def move_min_async(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
             velocity_unit: VelocityUnits = Units.NATIVE,
@@ -570,24 +603,25 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.MIN
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.MIN,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/move", request)
 
     def move_relative(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
@@ -608,26 +642,27 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.REL
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.REL,
+            arg=position,
+            unit=unit,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/move", request)
 
     async def move_relative_async(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
@@ -648,26 +683,27 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.REL
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.REL,
+            arg=position,
+            unit=unit,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/move", request)
 
     def move_velocity(
             self,
             velocity: float,
             unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
@@ -680,23 +716,24 @@
             velocity: Movement velocity.
             unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.VEL
-        request.arg = velocity
-        request.unit = units_from_literals(unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.VEL,
+            arg=velocity,
+            unit=unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/move", request)
 
     async def move_velocity_async(
             self,
             velocity: float,
             unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
@@ -709,23 +746,24 @@
             velocity: Movement velocity.
             unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.VEL
-        request.arg = velocity
-        request.unit = units_from_literals(unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.VEL,
+            arg=velocity,
+            unit=unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/move", request)
 
     def get_position(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
@@ -733,22 +771,25 @@
 
         Args:
             unit: Units of position.
 
         Returns:
             Axis position.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.setting = "pos"
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("device/get_setting", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            setting="pos",
+            unit=unit,
+        )
+        response = call(
+            "device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_position_async(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
@@ -756,90 +797,105 @@
 
         Args:
             unit: Units of position.
 
         Returns:
             Axis position.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.setting = "pos"
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("device/get_setting", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            setting="pos",
+            unit=unit,
+        )
+        response = await call_async(
+            "device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_number_of_index_positions(
             self
     ) -> int:
         """
         Gets number of index positions of the axis.
 
         Returns:
             Number of index positions.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.IntResponse()
-        call("device/get_index_count", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call(
+            "device/get_index_count",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     async def get_number_of_index_positions_async(
             self
     ) -> int:
         """
         Gets number of index positions of the axis.
 
         Returns:
             Number of index positions.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.IntResponse()
-        await call_async("device/get_index_count", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = await call_async(
+            "device/get_index_count",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     def get_index_position(
             self
     ) -> int:
         """
         Returns current axis index position.
 
         Returns:
             Index position starting from 1 or 0 if the position is not an index position.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.IntResponse()
-        call("device/get_index_position", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call(
+            "device/get_index_position",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     async def get_index_position_async(
             self
     ) -> int:
         """
         Returns current axis index position.
 
         Returns:
             Index position starting from 1 or 0 if the position is not an index position.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.IntResponse()
-        await call_async("device/get_index_position", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = await call_async(
+            "device/get_index_position",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     def move_index(
             self,
             index: int,
             wait_until_idle: bool = True,
             velocity: float = 0,
@@ -858,25 +914,26 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.INDEX
-        request.arg_int = index
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.INDEX,
+            arg_int=index,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/move", request)
 
     async def move_index_async(
             self,
             index: int,
             wait_until_idle: bool = True,
             velocity: float = 0,
@@ -895,25 +952,26 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.type = main_pb2.DeviceMoveRequest.INDEX
-        request.arg_int = index
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            type=dto.AxisMoveType.INDEX,
+            arg_int=index,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/move", request)
 
     def generic_command(
             self,
             command: str,
             check_errors: bool = True,
             timeout: int = 0
@@ -927,24 +985,27 @@
             check_errors: Controls whether to throw an exception when the device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             A response to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.command = command
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponse()
-        call("interface/generic_command", request, response)
-        return Response.from_protobuf(response)
+        request = dto.GenericCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            command=command,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = call(
+            "interface/generic_command",
+            request,
+            Response.from_binary)
+        return response
 
     async def generic_command_async(
             self,
             command: str,
             check_errors: bool = True,
             timeout: int = 0
     ) -> Response:
@@ -957,24 +1018,27 @@
             check_errors: Controls whether to throw an exception when the device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             A response to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.command = command
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponse()
-        await call_async("interface/generic_command", request, response)
-        return Response.from_protobuf(response)
+        request = dto.GenericCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            command=command,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "interface/generic_command",
+            request,
+            Response.from_binary)
+        return response
 
     def generic_command_multi_response(
             self,
             command: str,
             check_errors: bool = True,
             timeout: int = 0
     ) -> List[Response]:
@@ -988,24 +1052,27 @@
             check_errors: Controls whether to throw an exception when a device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             All responses to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.command = command
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponseCollection()
-        call("interface/generic_command_multi_response", request, response)
-        return [Response.from_protobuf(a) for a in response.responses]
+        request = dto.GenericCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            command=command,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = call(
+            "interface/generic_command_multi_response",
+            request,
+            dto.GenericCommandResponseCollection.from_binary)
+        return response.responses
 
     async def generic_command_multi_response_async(
             self,
             command: str,
             check_errors: bool = True,
             timeout: int = 0
     ) -> List[Response]:
@@ -1019,59 +1086,64 @@
             check_errors: Controls whether to throw an exception when a device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             All responses to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.command = command
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponseCollection()
-        await call_async("interface/generic_command_multi_response", request, response)
-        return [Response.from_protobuf(a) for a in response.responses]
+        request = dto.GenericCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            command=command,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "interface/generic_command_multi_response",
+            request,
+            dto.GenericCommandResponseCollection.from_binary)
+        return response.responses
 
     def generic_command_no_response(
             self,
             command: str
     ) -> None:
         """
         Sends a generic ASCII command to this axis without expecting a response and without adding a message ID
         For more information refer to: [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_commands).
 
         Args:
             command: Command and its parameters.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.command = command
+        request = dto.GenericCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            command=command,
+        )
         call("interface/generic_command_no_response", request)
 
     async def generic_command_no_response_async(
             self,
             command: str
     ) -> None:
         """
         Sends a generic ASCII command to this axis without expecting a response and without adding a message ID
         For more information refer to: [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_commands).
 
         Args:
             command: Command and its parameters.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.command = command
+        request = dto.GenericCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            command=command,
+        )
         await call_async("interface/generic_command_no_response", request)
 
     def prepare_command(
             self,
             command_template: str,
             *parameters: Measurement
     ) -> str:
@@ -1084,299 +1156,333 @@
         Args:
             command_template: Template of a command to prepare. Parameters are denoted by question marks.
             parameters: Variable number of command parameters.
 
         Returns:
             Command with converted parameters.
         """
-        request = main_pb2.PrepareCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.command_template = command_template
-        request.parameters.extend([Measurement.to_protobuf(a) for a in parameters])
-        response = main_pb2.StringResponse()
-        call_sync("device/prepare_command", request, response)
+        request = dto.PrepareCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            command_template=command_template,
+            parameters=list(parameters),
+        )
+        response = call_sync(
+            "device/prepare_command",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def set_label(
             self,
             label: str
     ) -> None:
         """
         Sets the user-assigned peripheral label.
         The label is stored on the controller and recognized by other software.
 
         Args:
             label: Label to set.
         """
-        request = main_pb2.DeviceSetStorageRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.value = label
+        request = dto.DeviceSetStorageRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            value=label,
+        )
         call("device/set_label", request)
 
     async def set_label_async(
             self,
             label: str
     ) -> None:
         """
         Sets the user-assigned peripheral label.
         The label is stored on the controller and recognized by other software.
 
         Args:
             label: Label to set.
         """
-        request = main_pb2.DeviceSetStorageRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.value = label
+        request = dto.DeviceSetStorageRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            value=label,
+        )
         await call_async("device/set_label", request)
 
     def __retrieve_label(
             self
     ) -> str:
         """
         Gets the peripheral name.
 
         Returns:
             The label.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.StringResponse()
-        call_sync("device/get_label", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call_sync(
+            "device/get_label",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the axis.
 
         Returns:
             A string that represents the axis.
         """
-        request = main_pb2.AxisToStringRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.StringResponse()
-        call_sync("device/axis_to_string", request, response)
+        request = dto.AxisToStringRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call_sync(
+            "device/axis_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def get_state(
             self
     ) -> str:
         """
         Returns a serialization of the current axis state that can be saved and reapplied.
 
         Returns:
             A serialization of the current state of the axis.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.StringResponse()
-        call("device/get_state", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call(
+            "device/get_state",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     async def get_state_async(
             self
     ) -> str:
         """
         Returns a serialization of the current axis state that can be saved and reapplied.
 
         Returns:
             A serialization of the current state of the axis.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.StringResponse()
-        await call_async("device/get_state", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = await call_async(
+            "device/get_state",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def set_state(
             self,
             state: str
     ) -> None:
         """
         Applies a saved state to this axis.
 
         Args:
             state: The state object to apply to this axis.
         """
-        request = main_pb2.SetStateRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.state = state
+        request = dto.SetStateRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            state=state,
+        )
         call("device/set_state", request)
 
     async def set_state_async(
             self,
             state: str
     ) -> None:
         """
         Applies a saved state to this axis.
 
         Args:
             state: The state object to apply to this axis.
         """
-        request = main_pb2.SetStateRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.state = state
+        request = dto.SetStateRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            state=state,
+        )
         await call_async("device/set_state", request)
 
     def can_set_state(
             self,
             state: str
-    ) -> str:
+    ) -> Optional[str]:
         """
         Checks if a state can be applied to this axis.
         This only covers exceptions that can be determined statically such as mismatches of ID or version,
         the process of applying the state can still fail when running.
 
         Args:
             state: The state object to check against.
 
         Returns:
             An explanation of why this state cannot be set to this axis.
         """
-        request = main_pb2.CanSetStateRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.state = state
-        response = main_pb2.CanSetStateAxisResponse()
-        call("device/can_set_axis_state", request, response)
+        request = dto.CanSetStateRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            state=state,
+        )
+        response = call(
+            "device/can_set_axis_state",
+            request,
+            dto.CanSetStateAxisResponse.from_binary)
         return response.error
 
     async def can_set_state_async(
             self,
             state: str
-    ) -> str:
+    ) -> Optional[str]:
         """
         Checks if a state can be applied to this axis.
         This only covers exceptions that can be determined statically such as mismatches of ID or version,
         the process of applying the state can still fail when running.
 
         Args:
             state: The state object to check against.
 
         Returns:
             An explanation of why this state cannot be set to this axis.
         """
-        request = main_pb2.CanSetStateRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        request.state = state
-        response = main_pb2.CanSetStateAxisResponse()
-        await call_async("device/can_set_axis_state", request, response)
+        request = dto.CanSetStateRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+            state=state,
+        )
+        response = await call_async(
+            "device/can_set_axis_state",
+            request,
+            dto.CanSetStateAxisResponse.from_binary)
         return response.error
 
     def __retrieve_identity(
             self
     ) -> AxisIdentity:
         """
         Returns identity.
 
         Returns:
             Axis identity.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
-        response = main_pb2.AxisIdentity()
-        call_sync("device/get_axis_identity", request, response)
-        return AxisIdentity.from_protobuf(response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
+        response = call_sync(
+            "device/get_axis_identity",
+            request,
+            AxisIdentity.from_binary)
+        return response
 
     def driver_disable(
             self
     ) -> None:
         """
         Disables the driver, which prevents current from being sent to the motor or load.
         If the driver is already disabled, the driver remains disabled.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         call("device/driver_disable", request)
 
     async def driver_disable_async(
             self
     ) -> None:
         """
         Disables the driver, which prevents current from being sent to the motor or load.
         If the driver is already disabled, the driver remains disabled.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         await call_async("device/driver_disable", request)
 
     def driver_enable(
             self
     ) -> None:
         """
         Attempts to enable the driver.
         If the driver is already enabled, the driver remains enabled.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         call("device/driver_enable", request)
 
     async def driver_enable_async(
             self
     ) -> None:
         """
         Attempts to enable the driver.
         If the driver is already enabled, the driver remains enabled.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         await call_async("device/driver_enable", request)
 
     def activate(
             self
     ) -> None:
         """
         Activates a peripheral on this axis.
         Removes all identity information for the device.
         Run the identify method on the device after activating to refresh the information.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         call("device/activate", request)
 
     async def activate_async(
             self
     ) -> None:
         """
         Activates a peripheral on this axis.
         Removes all identity information for the device.
         Run the identify method on the device after activating to refresh the information.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = self.axis_number
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=self.axis_number,
+        )
         await call_async("device/activate", request)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/axis_group.py` & `zaber_motion-6.0.0/zaber_motion/ascii/axis_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import List
 from ..call import call, call_async, call_sync
 
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from .axis import Axis
-from ..measurement import Measurement
-from ..units import units_from_literals, LengthUnits
+from ..dto.measurement import Measurement
+from ..units import LengthUnits
 
 
 class AxisGroup:
     """
     Groups multiple axes across devices into a single group to allow for simultaneous movement.
     Note that the movement is not coordinated and trajectory is inconsistent and not repeatable between calls.
     Make sure that any possible trajectory is clear of potential obstacles.
@@ -34,262 +34,288 @@
 
     def home(
             self
     ) -> None:
         """
         Homes the axes.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         call("axes/home", request)
 
     async def home_async(
             self
     ) -> None:
         """
         Homes the axes.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         await call_async("axes/home", request)
 
     def stop(
             self
     ) -> None:
         """
         Stops the axes.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         call("axes/stop", request)
 
     async def stop_async(
             self
     ) -> None:
         """
         Stops the axes.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         await call_async("axes/stop", request)
 
     def move_absolute(
             self,
             *position: Measurement
     ) -> None:
         """
         Moves the axes to absolute position.
 
         Args:
             position: Position.
         """
-        request = main_pb2.AxesMoveRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        request.position.extend([Measurement.to_protobuf(a) for a in position])
+        request = dto.AxesMoveRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+            position=list(position),
+        )
         call("axes/move_absolute", request)
 
     async def move_absolute_async(
             self,
             *position: Measurement
     ) -> None:
         """
         Moves the axes to absolute position.
 
         Args:
             position: Position.
         """
-        request = main_pb2.AxesMoveRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        request.position.extend([Measurement.to_protobuf(a) for a in position])
+        request = dto.AxesMoveRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+            position=list(position),
+        )
         await call_async("axes/move_absolute", request)
 
     def move_relative(
             self,
             *position: Measurement
     ) -> None:
         """
         Move axes to position relative to the current position.
 
         Args:
             position: Position.
         """
-        request = main_pb2.AxesMoveRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        request.position.extend([Measurement.to_protobuf(a) for a in position])
+        request = dto.AxesMoveRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+            position=list(position),
+        )
         call("axes/move_relative", request)
 
     async def move_relative_async(
             self,
             *position: Measurement
     ) -> None:
         """
         Move axes to position relative to the current position.
 
         Args:
             position: Position.
         """
-        request = main_pb2.AxesMoveRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        request.position.extend([Measurement.to_protobuf(a) for a in position])
+        request = dto.AxesMoveRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+            position=list(position),
+        )
         await call_async("axes/move_relative", request)
 
     def move_min(
             self
     ) -> None:
         """
         Moves axes to the minimum position as specified by limit.min.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         call("axes/move_min", request)
 
     async def move_min_async(
             self
     ) -> None:
         """
         Moves axes to the minimum position as specified by limit.min.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         await call_async("axes/move_min", request)
 
     def move_max(
             self
     ) -> None:
         """
         Moves axes to the maximum position as specified by limit.max.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         call("axes/move_max", request)
 
     async def move_max_async(
             self
     ) -> None:
         """
         Moves axes to the maximum position as specified by limit.max.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         await call_async("axes/move_max", request)
 
     def wait_until_idle(
             self
     ) -> None:
         """
         Waits until all the axes stop moving.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         call("axes/wait_until_idle", request)
 
     async def wait_until_idle_async(
             self
     ) -> None:
         """
         Waits until all the axes stop moving.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
         await call_async("axes/wait_until_idle", request)
 
     def is_busy(
             self
     ) -> bool:
         """
         Returns bool indicating whether any of the axes is executing a motion command.
 
         Returns:
             True if any of the axes is currently executing a motion command. False otherwise.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        response = main_pb2.BoolResponse()
-        call("axes/is_busy", request, response)
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
+        response = call(
+            "axes/is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_busy_async(
             self
     ) -> bool:
         """
         Returns bool indicating whether any of the axes is executing a motion command.
 
         Returns:
             True if any of the axes is currently executing a motion command. False otherwise.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        response = main_pb2.BoolResponse()
-        await call_async("axes/is_busy", request, response)
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
+        response = await call_async(
+            "axes/is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def is_homed(
             self
     ) -> bool:
         """
         Returns bool indicating whether all the axes are homed.
 
         Returns:
             True if all the axes are homed. False otherwise.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        response = main_pb2.BoolResponse()
-        call("axes/is_homed", request, response)
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
+        response = call(
+            "axes/is_homed",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_homed_async(
             self
     ) -> bool:
         """
         Returns bool indicating whether all the axes are homed.
 
         Returns:
             True if all the axes are homed. False otherwise.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        response = main_pb2.BoolResponse()
-        await call_async("axes/is_homed", request, response)
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
+        response = await call_async(
+            "axes/is_homed",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def get_position(
             self,
             *unit: LengthUnits
     ) -> List[float]:
         """
@@ -299,23 +325,26 @@
 
         Args:
             unit: Units of position. You can specify units once or for each axis separately.
 
         Returns:
             Axes position.
         """
-        request = main_pb2.AxesGetSettingRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        request.setting = "pos"
-        request.unit.extend([units_from_literals(u).value for u in unit])
-        response = main_pb2.DoubleArrayResponse()
-        call("axes/get_setting", request, response)
-        return list(response.values)
+        request = dto.AxesGetSettingRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+            setting="pos",
+            unit=list(unit),
+        )
+        response = call(
+            "axes/get_setting",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     async def get_position_async(
             self,
             *unit: LengthUnits
     ) -> List[float]:
         """
         Returns current axes position.
@@ -324,33 +353,39 @@
 
         Args:
             unit: Units of position. You can specify units once or for each axis separately.
 
         Returns:
             Axes position.
         """
-        request = main_pb2.AxesGetSettingRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        request.setting = "pos"
-        request.unit.extend([units_from_literals(u).value for u in unit])
-        response = main_pb2.DoubleArrayResponse()
-        await call_async("axes/get_setting", request, response)
-        return list(response.values)
+        request = dto.AxesGetSettingRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+            setting="pos",
+            unit=list(unit),
+        )
+        response = await call_async(
+            "axes/get_setting",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the axes.
 
         Returns:
             A string that represents the axes.
         """
-        request = main_pb2.AxesEmptyRequest()
-        request.interfaces.extend([axis.device.connection.interface_id for axis in self._axes])
-        request.devices.extend([axis.device.device_address for axis in self._axes])
-        request.axes.extend([axis.axis_number for axis in self._axes])
-        response = main_pb2.StringResponse()
-        call_sync("axes/to_string", request, response)
+        request = dto.AxesEmptyRequest(
+            interfaces=[axis.device.connection.interface_id for axis in self._axes],
+            devices=[axis.device.device_address for axis in self._axes],
+            axes=[axis.axis_number for axis in self._axes],
+        )
+        response = call_sync(
+            "axes/to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/axis_settings.py` & `zaber_motion-6.0.0/zaber_motion/ascii/axis_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING, List
 from ..call import call, call_async, call_sync
 
-from ..protobufs import main_pb2
-from ..units import UnitsAndLiterals, Units, units_from_literals
-from .conversion_factor import ConversionFactor
-
-from .get_axis_setting import GetAxisSetting
-from .get_axis_setting_result import GetAxisSettingResult
+from ..dto import requests as dto
+from ..units import UnitsAndLiterals, Units
+from ..dto.ascii.conversion_factor import ConversionFactor
+from ..dto.ascii.get_axis_setting import GetAxisSetting
+from ..dto.ascii.get_axis_setting_result import GetAxisSettingResult
 
 if TYPE_CHECKING:
     from .axis import Axis
 
 
 class AxisSettings:
     """
@@ -35,22 +34,25 @@
         Args:
             setting: Name of the setting.
             unit: Units of setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("device/get_setting", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+            unit=unit,
+        )
+        response = call(
+            "device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_async(
             self,
             setting: str,
             unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
@@ -61,22 +63,25 @@
         Args:
             setting: Name of the setting.
             unit: Units of setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("device/get_setting", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+            unit=unit,
+        )
+        response = await call_async(
+            "device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set(
             self,
             setting: str,
             value: float,
             unit: UnitsAndLiterals = Units.NATIVE
@@ -86,21 +91,22 @@
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
             value: Value of the setting.
             unit: Units of setting.
         """
-        request = main_pb2.DeviceSetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
         call("device/set_setting", request)
 
     async def set_async(
             self,
             setting: str,
             value: float,
             unit: UnitsAndLiterals = Units.NATIVE
@@ -110,21 +116,22 @@
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
             value: Value of the setting.
             unit: Units of setting.
         """
-        request = main_pb2.DeviceSetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
         await call_async("device/set_setting", request)
 
     def get_string(
             self,
             setting: str
     ) -> str:
         """
@@ -133,21 +140,24 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        response = main_pb2.StringResponse()
-        call("device/get_setting_str", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+        )
+        response = call(
+            "device/get_setting_str",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     async def get_string_async(
             self,
             setting: str
     ) -> str:
         """
@@ -156,21 +166,24 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        response = main_pb2.StringResponse()
-        await call_async("device/get_setting_str", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+        )
+        response = await call_async(
+            "device/get_setting_str",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def set_string(
             self,
             setting: str,
             value: str
     ) -> None:
@@ -178,20 +191,21 @@
         Sets any axis setting as a string.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
             value: Value of the setting.
         """
-        request = main_pb2.DeviceSetSettingStrRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        request.value = value
+        request = dto.DeviceSetSettingStrRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+            value=value,
+        )
         call("device/set_setting_str", request)
 
     async def set_string_async(
             self,
             setting: str,
             value: str
     ) -> None:
@@ -199,20 +213,21 @@
         Sets any axis setting as a string.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
             value: Value of the setting.
         """
-        request = main_pb2.DeviceSetSettingStrRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        request.value = value
+        request = dto.DeviceSetSettingStrRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+            value=value,
+        )
         await call_async("device/set_setting_str", request)
 
     def convert_to_native_units(
             self,
             setting: str,
             value: float,
             unit: UnitsAndLiterals
@@ -224,23 +239,26 @@
             setting: Name of the setting.
             value: Value of the setting in units specified by following argument.
             unit: Units of the value.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceConvertSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        request.value = value
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("device/convert_setting", request, response)
+        request = dto.DeviceConvertSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
+        response = call_sync(
+            "device/convert_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def convert_from_native_units(
             self,
             setting: str,
             value: float,
             unit: UnitsAndLiterals
@@ -252,24 +270,27 @@
             setting: Name of the setting.
             value: Value of the setting in Zaber native units.
             unit: Units to convert value to.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceConvertSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.from_native = True
-        request.setting = setting
-        request.value = value
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("device/convert_setting", request, response)
+        request = dto.DeviceConvertSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            from_native=True,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
+        response = call_sync(
+            "device/convert_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_default(
             self,
             setting: str,
             unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
@@ -279,22 +300,25 @@
         Args:
             setting: Name of the setting.
             unit: Units of setting.
 
         Returns:
             Default setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("device/get_setting_default", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+            unit=unit,
+        )
+        response = call_sync(
+            "device/get_setting_default",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_default_string(
             self,
             setting: str
     ) -> str:
         """
@@ -302,21 +326,24 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             Default setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        response = main_pb2.StringResponse()
-        call_sync("device/get_setting_default_str", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+        )
+        response = call_sync(
+            "device/get_setting_default_str",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def can_convert_native_units(
             self,
             setting: str
     ) -> bool:
         """
@@ -324,143 +351,160 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             True if unit conversion can be performed.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.setting = setting
-        response = main_pb2.BoolResponse()
-        call_sync("device/can_convert_setting", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            setting=setting,
+        )
+        response = call_sync(
+            "device/can_convert_setting",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def set_custom_unit_conversions(
             self,
             conversions: List[ConversionFactor]
     ) -> None:
         """
         Overrides default unit conversions.
         Conversion factors are specified by setting names representing underlying dimensions.
         Requires at least Firmware 7.30.
 
         Args:
             conversions: Factors of all conversions to override.
         """
-        request = main_pb2.DeviceSetUnitConversionsRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.conversions.extend([ConversionFactor.to_protobuf(a) for a in conversions])
+        request = dto.DeviceSetUnitConversionsRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            conversions=conversions,
+        )
         call("device/set_unit_conversions", request)
 
     async def set_custom_unit_conversions_async(
             self,
             conversions: List[ConversionFactor]
     ) -> None:
         """
         Overrides default unit conversions.
         Conversion factors are specified by setting names representing underlying dimensions.
         Requires at least Firmware 7.30.
 
         Args:
             conversions: Factors of all conversions to override.
         """
-        request = main_pb2.DeviceSetUnitConversionsRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.conversions.extend([ConversionFactor.to_protobuf(a) for a in conversions])
+        request = dto.DeviceSetUnitConversionsRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            conversions=conversions,
+        )
         await call_async("device/set_unit_conversions", request)
 
     def get_many(
             self,
-            *settings: GetAxisSetting
+            *axis_settings: GetAxisSetting
     ) -> List[GetAxisSettingResult]:
         """
         Gets many setting values in as few requests as possible.
 
         Args:
-            settings: The settings to read.
+            axis_settings: The settings to read.
 
         Returns:
             The setting values read.
         """
-        request = main_pb2.DeviceMultiGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.settings.extend([GetAxisSetting.to_protobuf(a) for a in settings])
-        response = main_pb2.GetSettingResults()
-        call("device/get_many_settings", request, response)
-        return [GetAxisSettingResult.from_protobuf(a) for a in response.results]
+        request = dto.DeviceMultiGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            axis_settings=list(axis_settings),
+        )
+        response = call(
+            "device/get_many_settings",
+            request,
+            dto.GetAxisSettingResults.from_binary)
+        return response.results
 
     async def get_many_async(
             self,
-            *settings: GetAxisSetting
+            *axis_settings: GetAxisSetting
     ) -> List[GetAxisSettingResult]:
         """
         Gets many setting values in as few requests as possible.
 
         Args:
-            settings: The settings to read.
+            axis_settings: The settings to read.
 
         Returns:
             The setting values read.
         """
-        request = main_pb2.DeviceMultiGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.settings.extend([GetAxisSetting.to_protobuf(a) for a in settings])
-        response = main_pb2.GetSettingResults()
-        await call_async("device/get_many_settings", request, response)
-        return [GetAxisSettingResult.from_protobuf(a) for a in response.results]
+        request = dto.DeviceMultiGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            axis_settings=list(axis_settings),
+        )
+        response = await call_async(
+            "device/get_many_settings",
+            request,
+            dto.GetAxisSettingResults.from_binary)
+        return response.results
 
     def get_synchronized(
             self,
-            *settings: GetAxisSetting
+            *axis_settings: GetAxisSetting
     ) -> List[GetAxisSettingResult]:
         """
         Gets many setting values in the same tick, ensuring their values are synchronized.
         Requires at least Firmware 7.35.
 
         Args:
-            settings: The settings to read.
+            axis_settings: The settings to read.
 
         Returns:
             The setting values read.
         """
-        request = main_pb2.DeviceMultiGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.settings.extend([GetAxisSetting.to_protobuf(a) for a in settings])
-        response = main_pb2.GetSettingResults()
-        call("device/get_sync_settings", request, response)
-        return [GetAxisSettingResult.from_protobuf(a) for a in response.results]
+        request = dto.DeviceMultiGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            axis_settings=list(axis_settings),
+        )
+        response = call(
+            "device/get_sync_settings",
+            request,
+            dto.GetAxisSettingResults.from_binary)
+        return response.results
 
     async def get_synchronized_async(
             self,
-            *settings: GetAxisSetting
+            *axis_settings: GetAxisSetting
     ) -> List[GetAxisSettingResult]:
         """
         Gets many setting values in the same tick, ensuring their values are synchronized.
         Requires at least Firmware 7.35.
 
         Args:
-            settings: The settings to read.
+            axis_settings: The settings to read.
 
         Returns:
             The setting values read.
         """
-        request = main_pb2.DeviceMultiGetSettingRequest()
-        request.interface_id = self._axis.device.connection.interface_id
-        request.device = self._axis.device.device_address
-        request.axis = self._axis.axis_number
-        request.settings.extend([GetAxisSetting.to_protobuf(a) for a in settings])
-        response = main_pb2.GetSettingResults()
-        await call_async("device/get_sync_settings", request, response)
-        return [GetAxisSettingResult.from_protobuf(a) for a in response.results]
+        request = dto.DeviceMultiGetSettingRequest(
+            interface_id=self._axis.device.connection.interface_id,
+            device=self._axis.device.device_address,
+            axis=self._axis.axis_number,
+            axis_settings=list(axis_settings),
+        )
+        response = await call_async(
+            "device/get_sync_settings",
+            request,
+            dto.GetAxisSettingResults.from_binary)
+        return response.results
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/can_set_state_axis_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
 
+@dataclass
 class CanSetStateAxisResponse:
     """
     An object containing any setup issues that will prevent setting a state to a given axis.
     """
 
-    @property
-    def error(self) -> str:
-        """
-        The error blocking applying this state to the given axis.
-        """
-
-        return self._error
-
-    @error.setter
-    def error(self, value: str) -> None:
-        self._error = value
-
-    @property
-    def axis_number(self) -> int:
-        """
-        The number of the axis that cannot be set.
-        """
-
-        return self._axis_number
-
-    @axis_number.setter
-    def axis_number(self, value: int) -> None:
-        self._axis_number = value
+    axis_number: int
+    """
+    The number of the axis that cannot be set.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    error: Optional[str] = None
+    """
+    The error blocking applying this state to the given axis.
+    """
+
+    @staticmethod
+    def zero_values() -> 'CanSetStateAxisResponse':
+        return CanSetStateAxisResponse(
+            error=None,
+            axis_number=0,
+        )
+
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'CanSetStateAxisResponse':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return CanSetStateAxisResponse.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'error': self.error,
+            'axisNumber': self.axis_number,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.CanSetStateAxisResponse
-    ) -> 'CanSetStateAxisResponse':
-        instance = CanSetStateAxisResponse.__new__(
-            CanSetStateAxisResponse
-        )  # type: CanSetStateAxisResponse
-        instance.error = pb_data.error
-        instance.axis_number = pb_data.axis_number
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'CanSetStateAxisResponse':
+        return CanSetStateAxisResponse(
+            error=data.get('error'),  # type: ignore
+            axis_number=data.get('axisNumber'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-6.0.0/zaber_motion/dto/requests/can_set_state_axis_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from typing import List  # pylint: disable=unused-import
-from ..protobufs import main_pb2
-from .can_set_state_axis_response import CanSetStateAxisResponse
-
-
-class CanSetStateDeviceResponse:
-    """
-    An object containing any setup issues that will prevent setting a state to a given device.
-    """
-
-    @property
-    def error(self) -> str:
-        """
-        The error blocking applying this state to the given device.
-        """
-
-        return self._error
-
-    @error.setter
-    def error(self, value: str) -> None:
-        self._error = value
-
-    @property
-    def axis_errors(self) -> List[CanSetStateAxisResponse]:
-        """
-        A list of errors that block setting state of device's axes.
-        """
-
-        return self._axis_errors
-
-    @axis_errors.setter
-    def axis_errors(self, value: List[CanSetStateAxisResponse]) -> None:
-        self._axis_errors = value
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+
+@dataclass
+class CanSetStateAxisResponse:
+
+    axis_number: int = 0
+
+    error: Optional[str] = None
+
+    @staticmethod
+    def zero_values() -> 'CanSetStateAxisResponse':
+        return CanSetStateAxisResponse(
+            error=None,
+            axis_number=0,
+        )
+
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'CanSetStateAxisResponse':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return CanSetStateAxisResponse.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'error': self.error,
+            'axisNumber': self.axis_number,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.CanSetStateDeviceResponse
-    ) -> 'CanSetStateDeviceResponse':
-        instance = CanSetStateDeviceResponse.__new__(
-            CanSetStateDeviceResponse
-        )  # type: CanSetStateDeviceResponse
-        instance.error = pb_data.error
-        instance.axis_errors = [CanSetStateAxisResponse.from_protobuf(item) for item in pb_data.axis_errors]
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'CanSetStateAxisResponse':
+        return CanSetStateAxisResponse(
+            error=data.get('error'),  # type: ignore
+            axis_number=data.get('axisNumber'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/connection.py` & `zaber_motion-6.0.0/zaber_motion/ascii/connection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
-from typing import Generator, List, Any, Callable, Optional
+from typing import Generator, List, Any, Callable, Optional, Union
 import asyncio
-from rx.subject import ReplaySubject
-from rx.core import Observable
-from rx import operators as rxop
+from reactivex.subject import ReplaySubject
+from reactivex import operators as rxop, Observable
 
 from ..call import call, call_async, call_sync
 from ..convert_exception import convert_exception
-from ..events import events
+from ..events import events, Event
 from ..exceptions.motion_lib_exception import MotionLibException
 
 from .device import Device
-from .response import Response
 from .transport import Transport
-from .unknown_response_event import UnknownResponseEvent
-from .alert_event import AlertEvent
-from ..protobufs import main_pb2
+from ..dto.ascii.response import Response
+from ..dto.ascii.unknown_response_event import UnknownResponseEvent
+from ..dto.ascii.alert_event import AlertEvent
+from ..dto import requests as dto
 
 
 class Connection:
     """
     Class representing access to particular connection (serial port, TCP connection).
     """
 
     @property
-    def unknown_response(self) -> Observable:
+    def unknown_response(self) -> Observable[UnknownResponseEvent]:
         """
         Event invoked when a response from a device cannot be matched to any known request.
         """
         return self._unknown_response
 
     @property
-    def alert(self) -> Observable:
+    def alert(self) -> Observable[AlertEvent]:
         """
         Event invoked when an alert is received from a device.
         """
         return self._alert
 
     @property
-    def disconnected(self) -> Observable:
+    def disconnected(self) -> Observable[MotionLibException]:
         """
         Event invoked when connection is interrupted or closed.
         """
         return self._disconnected
 
     DEFAULT_BAUD_RATE = 115200
     """
@@ -128,21 +127,24 @@
             baud_rate: Optional baud rate (defaults to 115200).
             direct: If true will connect to the serial port directly,
                 failing if the connection is already opened by a message router instance.
 
         Returns:
             An object representing the port.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.SERIAL_PORT
-        request.port_name = port_name
-        request.baud_rate = baud_rate
-        request.reject_routed_connection = direct
-        response = main_pb2.OpenInterfaceResponse()
-        call("interface/open", request, response)
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.SERIAL_PORT,
+            port_name=port_name,
+            baud_rate=baud_rate,
+            reject_routed_connection=direct,
+        )
+        response = call(
+            "interface/open",
+            request,
+            dto.OpenInterfaceResponse.from_binary)
         return Connection(response.interface_id)
 
     @staticmethod
     def open_serial_port_async(
             port_name: str,
             baud_rate: int = DEFAULT_BAUD_RATE,
             direct: bool = False
@@ -157,19 +159,20 @@
             baud_rate: Optional baud rate (defaults to 115200).
             direct: If true will connect to the serial port directly,
                 failing if the connection is already opened by a message router instance.
 
         Returns:
             An object representing the port.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.SERIAL_PORT
-        request.port_name = port_name
-        request.baud_rate = baud_rate
-        request.reject_routed_connection = direct
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.SERIAL_PORT,
+            port_name=port_name,
+            baud_rate=baud_rate,
+            reject_routed_connection=direct,
+        )
         return AsyncConnectionOpener(request)
 
     @staticmethod
     def open_tcp(
             host_name: str,
             port: int = TCP_PORT_CHAIN
     ) -> 'Connection':
@@ -179,20 +182,23 @@
         Args:
             host_name: Hostname or IP address.
             port: Optional port number (defaults to 55550).
 
         Returns:
             An object representing the connection.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.TCP
-        request.host_name = host_name
-        request.port = port
-        response = main_pb2.OpenInterfaceResponse()
-        call("interface/open", request, response)
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.TCP,
+            host_name=host_name,
+            port=port,
+        )
+        response = call(
+            "interface/open",
+            request,
+            dto.OpenInterfaceResponse.from_binary)
         return Connection(response.interface_id)
 
     @staticmethod
     def open_tcp_async(
             host_name: str,
             port: int = TCP_PORT_CHAIN
     ) -> 'AsyncConnectionOpener':
@@ -202,18 +208,19 @@
         Args:
             host_name: Hostname or IP address.
             port: Optional port number (defaults to 55550).
 
         Returns:
             An object representing the connection.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.TCP
-        request.host_name = host_name
-        request.port = port
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.TCP,
+            host_name=host_name,
+            port=port,
+        )
         return AsyncConnectionOpener(request)
 
     @staticmethod
     def open_custom(
             transport: Transport
     ) -> 'Connection':
         """
@@ -221,19 +228,22 @@
 
         Args:
             transport: The custom connection transport.
 
         Returns:
             An object representing the connection.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.CUSTOM
-        request.transport = transport.transport_id
-        response = main_pb2.OpenInterfaceResponse()
-        call("interface/open", request, response)
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.CUSTOM,
+            transport=transport.transport_id,
+        )
+        response = call(
+            "interface/open",
+            request,
+            dto.OpenInterfaceResponse.from_binary)
         return Connection(response.interface_id)
 
     @staticmethod
     def open_custom_async(
             transport: Transport
     ) -> 'AsyncConnectionOpener':
         """
@@ -241,17 +251,18 @@
 
         Args:
             transport: The custom connection transport.
 
         Returns:
             An object representing the connection.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.CUSTOM
-        request.transport = transport.transport_id
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.CUSTOM,
+            transport=transport.transport_id,
+        )
         return AsyncConnectionOpener(request)
 
     @staticmethod
     def open_iot(
             cloud_id: str,
             token: str = "unauthenticated",
             connection_name: str = "",
@@ -271,23 +282,26 @@
             realm: The realm to connect to.
                 Can be left empty for the default account realm.
             api: The URL of the API to receive connection info from.
 
         Returns:
             An object representing the connection.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.IOT
-        request.cloud_id = cloud_id
-        request.token = token
-        request.connection_name = connection_name
-        request.realm = realm
-        request.api = api
-        response = main_pb2.OpenInterfaceResponse()
-        call("interface/open", request, response)
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.IOT,
+            cloud_id=cloud_id,
+            token=token,
+            connection_name=connection_name,
+            realm=realm,
+            api=api,
+        )
+        response = call(
+            "interface/open",
+            request,
+            dto.OpenInterfaceResponse.from_binary)
         return Connection(response.interface_id)
 
     @staticmethod
     def open_iot_async(
             cloud_id: str,
             token: str = "unauthenticated",
             connection_name: str = "",
@@ -307,21 +321,22 @@
             realm: The realm to connect to.
                 Can be left empty for the default account realm.
             api: The URL of the API to receive connection info from.
 
         Returns:
             An object representing the connection.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.IOT
-        request.cloud_id = cloud_id
-        request.token = token
-        request.connection_name = connection_name
-        request.realm = realm
-        request.api = api
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.IOT,
+            cloud_id=cloud_id,
+            token=token,
+            connection_name=connection_name,
+            realm=realm,
+            api=api,
+        )
         return AsyncConnectionOpener(request)
 
     @staticmethod
     def open_network_share(
             host_name: str,
             port: int = NETWORK_SHARE_PORT,
             connection_name: str = ""
@@ -336,21 +351,24 @@
             connection_name: The name of the connection to open.
                 Can be left empty to default to the only connection present.
                 Otherwise, use serial port name for serial port connection or hostname:port for TCP connection.
 
         Returns:
             An object representing the connection.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.NETWORK_SHARE
-        request.host_name = host_name
-        request.port = port
-        request.connection_name = connection_name
-        response = main_pb2.OpenInterfaceResponse()
-        call("interface/open", request, response)
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.NETWORK_SHARE,
+            host_name=host_name,
+            port=port,
+            connection_name=connection_name,
+        )
+        response = call(
+            "interface/open",
+            request,
+            dto.OpenInterfaceResponse.from_binary)
         return Connection(response.interface_id)
 
     @staticmethod
     def open_network_share_async(
             host_name: str,
             port: int = NETWORK_SHARE_PORT,
             connection_name: str = ""
@@ -365,19 +383,20 @@
             connection_name: The name of the connection to open.
                 Can be left empty to default to the only connection present.
                 Otherwise, use serial port name for serial port connection or hostname:port for TCP connection.
 
         Returns:
             An object representing the connection.
         """
-        request = main_pb2.OpenInterfaceRequest()
-        request.interface_type = main_pb2.NETWORK_SHARE
-        request.host_name = host_name
-        request.port = port
-        request.connection_name = connection_name
+        request = dto.OpenInterfaceRequest(
+            interface_type=dto.InterfaceType.NETWORK_SHARE,
+            host_name=host_name,
+            port=port,
+            connection_name=connection_name,
+        )
         return AsyncConnectionOpener(request)
 
     def generic_command(
             self,
             command: str,
             device: int = 0,
             axis: int = 0,
@@ -395,24 +414,27 @@
             check_errors: Controls whether to throw an exception when the device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             A response to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = command
-        request.device = device
-        request.axis = axis
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponse()
-        call("interface/generic_command", request, response)
-        return Response.from_protobuf(response)
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command=command,
+            device=device,
+            axis=axis,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = call(
+            "interface/generic_command",
+            request,
+            Response.from_binary)
+        return response
 
     async def generic_command_async(
             self,
             command: str,
             device: int = 0,
             axis: int = 0,
             check_errors: bool = True,
@@ -429,24 +451,27 @@
             check_errors: Controls whether to throw an exception when the device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             A response to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = command
-        request.device = device
-        request.axis = axis
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponse()
-        await call_async("interface/generic_command", request, response)
-        return Response.from_protobuf(response)
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command=command,
+            device=device,
+            axis=axis,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "interface/generic_command",
+            request,
+            Response.from_binary)
+        return response
 
     def generic_command_no_response(
             self,
             command: str,
             device: int = 0,
             axis: int = 0
     ) -> None:
@@ -457,19 +482,20 @@
         Args:
             command: Command and its parameters.
             device: Optional device address to send the command to.
                 Specifying -1 omits the number completely.
             axis: Optional axis number to send the command to.
                 Specifying -1 omits the number completely.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = command
-        request.device = device
-        request.axis = axis
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command=command,
+            device=device,
+            axis=axis,
+        )
         call("interface/generic_command_no_response", request)
 
     async def generic_command_no_response_async(
             self,
             command: str,
             device: int = 0,
             axis: int = 0
@@ -481,19 +507,20 @@
         Args:
             command: Command and its parameters.
             device: Optional device address to send the command to.
                 Specifying -1 omits the number completely.
             axis: Optional axis number to send the command to.
                 Specifying -1 omits the number completely.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = command
-        request.device = device
-        request.axis = axis
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command=command,
+            device=device,
+            axis=axis,
+        )
         await call_async("interface/generic_command_no_response", request)
 
     def generic_command_multi_response(
             self,
             command: str,
             device: int = 0,
             axis: int = 0,
@@ -513,24 +540,27 @@
             check_errors: Controls whether to throw an exception when a device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             All responses to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = command
-        request.device = device
-        request.axis = axis
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponseCollection()
-        call("interface/generic_command_multi_response", request, response)
-        return [Response.from_protobuf(a) for a in response.responses]
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command=command,
+            device=device,
+            axis=axis,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = call(
+            "interface/generic_command_multi_response",
+            request,
+            dto.GenericCommandResponseCollection.from_binary)
+        return response.responses
 
     async def generic_command_multi_response_async(
             self,
             command: str,
             device: int = 0,
             axis: int = 0,
             check_errors: bool = True,
@@ -549,101 +579,111 @@
             check_errors: Controls whether to throw an exception when a device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             All responses to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = command
-        request.device = device
-        request.axis = axis
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponseCollection()
-        await call_async("interface/generic_command_multi_response", request, response)
-        return [Response.from_protobuf(a) for a in response.responses]
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command=command,
+            device=device,
+            axis=axis,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "interface/generic_command_multi_response",
+            request,
+            dto.GenericCommandResponseCollection.from_binary)
+        return response.responses
 
     def enable_alerts(
             self
     ) -> None:
         """
         Enables alerts for all devices on the connection.
         This will change the "comm.alert" setting to 1 on all supported devices.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = "set comm.alert 1"
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command="set comm.alert 1",
+        )
         call("interface/generic_command_no_response", request)
 
     async def enable_alerts_async(
             self
     ) -> None:
         """
         Enables alerts for all devices on the connection.
         This will change the "comm.alert" setting to 1 on all supported devices.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = "set comm.alert 1"
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command="set comm.alert 1",
+        )
         await call_async("interface/generic_command_no_response", request)
 
     def disable_alerts(
             self
     ) -> None:
         """
         Disables alerts for all devices on the connection.
         This will change the "comm.alert" setting to 0 on all supported devices.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = "set comm.alert 0"
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command="set comm.alert 0",
+        )
         call("interface/generic_command_no_response", request)
 
     async def disable_alerts_async(
             self
     ) -> None:
         """
         Disables alerts for all devices on the connection.
         This will change the "comm.alert" setting to 0 on all supported devices.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.interface_id
-        request.command = "set comm.alert 0"
+        request = dto.GenericCommandRequest(
+            interface_id=self.interface_id,
+            command="set comm.alert 0",
+        )
         await call_async("interface/generic_command_no_response", request)
 
     def reset_ids(
             self
     ) -> None:
         """
         Resets ASCII protocol message IDs. Only for testing purposes.
         """
-        request = main_pb2.InterfaceEmptyRequest()
-        request.interface_id = self.interface_id
+        request = dto.InterfaceEmptyRequest(
+            interface_id=self.interface_id,
+        )
         call_sync("interface/reset_ids", request)
 
     def close(
             self
     ) -> None:
         """
         Close the connection.
         """
-        request = main_pb2.InterfaceEmptyRequest()
-        request.interface_id = self.interface_id
+        request = dto.InterfaceEmptyRequest(
+            interface_id=self.interface_id,
+        )
         call("interface/close", request)
 
     async def close_async(
             self
     ) -> None:
         """
         Close the connection.
         """
-        request = main_pb2.InterfaceEmptyRequest()
-        request.interface_id = self.interface_id
+        request = dto.InterfaceEmptyRequest(
+            interface_id=self.interface_id,
+        )
         await call_async("interface/close", request)
 
     def get_device(
             self,
             device_address: int
     ) -> Device:
         """
@@ -674,19 +714,22 @@
 
         Returns:
             Total number of devices that responded to the renumber.
         """
         if first_address <= 0:
             raise ValueError('Invalid value; device addresses are numbered from 1.')
 
-        request = main_pb2.DeviceRenumberRequest()
-        request.interface_id = self.interface_id
-        request.first_address = first_address
-        response = main_pb2.IntResponse()
-        call("device/renumber", request, response)
+        request = dto.DeviceRenumberRequest(
+            interface_id=self.interface_id,
+            first_address=first_address,
+        )
+        response = call(
+            "device/renumber",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     async def renumber_devices_async(
             self,
             first_address: int = 1
     ) -> int:
         """
@@ -698,19 +741,22 @@
 
         Returns:
             Total number of devices that responded to the renumber.
         """
         if first_address <= 0:
             raise ValueError('Invalid value; device addresses are numbered from 1.')
 
-        request = main_pb2.DeviceRenumberRequest()
-        request.interface_id = self.interface_id
-        request.first_address = first_address
-        response = main_pb2.IntResponse()
-        await call_async("device/renumber", request, response)
+        request = dto.DeviceRenumberRequest(
+            interface_id=self.interface_id,
+            first_address=first_address,
+        )
+        response = await call_async(
+            "device/renumber",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     def detect_devices(
             self,
             identify_devices: bool = True
     ) -> List[Device]:
         """
@@ -718,19 +764,22 @@
 
         Args:
             identify_devices: Determines whether device identification should be performed as well.
 
         Returns:
             Array of detected devices.
         """
-        request = main_pb2.DeviceDetectRequest()
-        request.interface_id = self.interface_id
-        request.identify_devices = identify_devices
-        response = main_pb2.DeviceDetectResponse()
-        call("device/detect", request, response)
+        request = dto.DeviceDetectRequest(
+            interface_id=self.interface_id,
+            identify_devices=identify_devices,
+        )
+        response = call(
+            "device/detect",
+            request,
+            dto.DeviceDetectResponse.from_binary)
         return list(map(self.get_device, response.devices))
 
     async def detect_devices_async(
             self,
             identify_devices: bool = True
     ) -> List[Device]:
         """
@@ -738,19 +787,22 @@
 
         Args:
             identify_devices: Determines whether device identification should be performed as well.
 
         Returns:
             Array of detected devices.
         """
-        request = main_pb2.DeviceDetectRequest()
-        request.interface_id = self.interface_id
-        request.identify_devices = identify_devices
-        response = main_pb2.DeviceDetectResponse()
-        await call_async("device/detect", request, response)
+        request = dto.DeviceDetectRequest(
+            interface_id=self.interface_id,
+            identify_devices=identify_devices,
+        )
+        response = await call_async(
+            "device/detect",
+            request,
+            dto.DeviceDetectResponse.from_binary)
         return list(map(self.get_device, response.devices))
 
     def stop_all(
             self,
             wait_until_idle: bool = True
     ) -> List[int]:
         """
@@ -759,20 +811,23 @@
         Args:
             wait_until_idle: Determines whether the function should return immediately
                 or wait until the devices are stopped.
 
         Returns:
             The addresses of the devices that were stopped by this command.
         """
-        request = main_pb2.DeviceOnAllRequest()
-        request.interface_id = self.interface_id
-        request.wait_until_idle = wait_until_idle
-        response = main_pb2.DeviceOnAllResponse()
-        call("device/stop_all", request, response)
-        return list(response.device_addresses)
+        request = dto.DeviceOnAllRequest(
+            interface_id=self.interface_id,
+            wait_until_idle=wait_until_idle,
+        )
+        response = call(
+            "device/stop_all",
+            request,
+            dto.DeviceOnAllResponse.from_binary)
+        return response.device_addresses
 
     async def stop_all_async(
             self,
             wait_until_idle: bool = True
     ) -> List[int]:
         """
         Stops all of the devices on this connection.
@@ -780,20 +835,23 @@
         Args:
             wait_until_idle: Determines whether the function should return immediately
                 or wait until the devices are stopped.
 
         Returns:
             The addresses of the devices that were stopped by this command.
         """
-        request = main_pb2.DeviceOnAllRequest()
-        request.interface_id = self.interface_id
-        request.wait_until_idle = wait_until_idle
-        response = main_pb2.DeviceOnAllResponse()
-        await call_async("device/stop_all", request, response)
-        return list(response.device_addresses)
+        request = dto.DeviceOnAllRequest(
+            interface_id=self.interface_id,
+            wait_until_idle=wait_until_idle,
+        )
+        response = await call_async(
+            "device/stop_all",
+            request,
+            dto.DeviceOnAllResponse.from_binary)
+        return response.device_addresses
 
     def home_all(
             self,
             wait_until_idle: bool = True
     ) -> List[int]:
         """
         Homes all of the devices on this connection.
@@ -801,20 +859,23 @@
         Args:
             wait_until_idle: Determines whether the function should return immediately
                 or wait until the devices are homed.
 
         Returns:
             The addresses of the devices that were homed by this command.
         """
-        request = main_pb2.DeviceOnAllRequest()
-        request.interface_id = self.interface_id
-        request.wait_until_idle = wait_until_idle
-        response = main_pb2.DeviceOnAllResponse()
-        call("device/home_all", request, response)
-        return list(response.device_addresses)
+        request = dto.DeviceOnAllRequest(
+            interface_id=self.interface_id,
+            wait_until_idle=wait_until_idle,
+        )
+        response = call(
+            "device/home_all",
+            request,
+            dto.DeviceOnAllResponse.from_binary)
+        return response.device_addresses
 
     async def home_all_async(
             self,
             wait_until_idle: bool = True
     ) -> List[int]:
         """
         Homes all of the devices on this connection.
@@ -822,147 +883,169 @@
         Args:
             wait_until_idle: Determines whether the function should return immediately
                 or wait until the devices are homed.
 
         Returns:
             The addresses of the devices that were homed by this command.
         """
-        request = main_pb2.DeviceOnAllRequest()
-        request.interface_id = self.interface_id
-        request.wait_until_idle = wait_until_idle
-        response = main_pb2.DeviceOnAllResponse()
-        await call_async("device/home_all", request, response)
-        return list(response.device_addresses)
+        request = dto.DeviceOnAllRequest(
+            interface_id=self.interface_id,
+            wait_until_idle=wait_until_idle,
+        )
+        response = await call_async(
+            "device/home_all",
+            request,
+            dto.DeviceOnAllResponse.from_binary)
+        return response.device_addresses
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the connection.
 
         Returns:
             A string that represents the connection.
         """
-        request = main_pb2.InterfaceEmptyRequest()
-        request.interface_id = self.interface_id
-        response = main_pb2.StringResponse()
-        call_sync("interface/to_string", request, response)
+        request = dto.InterfaceEmptyRequest(
+            interface_id=self.interface_id,
+        )
+        response = call_sync(
+            "interface/to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def __retrieve_timeout(
             self
     ) -> int:
         """
         Returns default request timeout.
 
         Returns:
             Default request timeout.
         """
-        request = main_pb2.InterfaceEmptyRequest()
-        request.interface_id = self.interface_id
-        response = main_pb2.IntResponse()
-        call_sync("interface/get_timeout", request, response)
+        request = dto.InterfaceEmptyRequest(
+            interface_id=self.interface_id,
+        )
+        response = call_sync(
+            "interface/get_timeout",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     def __change_timeout(
             self,
             timeout: int
     ) -> None:
         """
         Sets default request timeout.
 
         Args:
             timeout: Default request timeout.
         """
-        request = main_pb2.SetInterfaceTimeoutRequest()
-        request.interface_id = self.interface_id
-        request.timeout = timeout
+        request = dto.SetInterfaceTimeoutRequest(
+            interface_id=self.interface_id,
+            timeout=timeout,
+        )
         call_sync("interface/set_timeout", request)
 
     def __retrieve_checksum_enabled(
             self
     ) -> bool:
         """
         Returns checksum enabled.
 
         Returns:
             Checksum enabled.
         """
-        request = main_pb2.InterfaceEmptyRequest()
-        request.interface_id = self.interface_id
-        response = main_pb2.BoolResponse()
-        call_sync("interface/get_checksum_enabled", request, response)
+        request = dto.InterfaceEmptyRequest(
+            interface_id=self.interface_id,
+        )
+        response = call_sync(
+            "interface/get_checksum_enabled",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def __change_checksum_enabled(
             self,
             is_enabled: bool
     ) -> None:
         """
         Sets checksum enabled.
 
         Args:
             is_enabled: Checksum enabled.
         """
-        request = main_pb2.SetInterfaceChecksumEnabledRequest()
-        request.interface_id = self.interface_id
-        request.is_enabled = is_enabled
+        request = dto.SetInterfaceChecksumEnabledRequest(
+            interface_id=self.interface_id,
+            is_enabled=is_enabled,
+        )
         call_sync("interface/set_checksum_enabled", request)
 
     def __enter__(self) -> 'Connection':
         """ __enter__ """
         return self
 
     def __exit__(self, _type: Any, _value: Any, _traceback: Any) -> None:
         """ __exit__ """
         self.close()
 
-    def __filter_event(self, event_name: str) -> Callable[[Any], bool]:
-        def filter_event(event: Any) -> bool:
-            return event[0] == event_name and event[1].interface_id == self._interface_id  # type: ignore
+    def __filter_event(self, event_name: str) -> Callable[[Event[Any]], bool]:
+        def filter_event(
+            event: Event[Union[
+                dto.UnknownResponseEventWrapper,
+                dto.AlertEventWrapper,
+                dto.DisconnectedEvent,
+            ]],
+        ) -> bool:
+            return event.name == event_name and event.data.interface_id == self._interface_id
         return filter_event
 
     def __setup_events(self) -> None:
-        self._disconnected = ReplaySubject()  # terminates all the events
+        self._disconnected = ReplaySubject[MotionLibException]()  # terminates all the events
 
         self._unknown_response = events.pipe(
             rxop.take_until(self.disconnected),
             rxop.filter(self.__filter_event('interface/unknown_response')),
-            rxop.map(lambda ev: UnknownResponseEvent.from_protobuf(ev[1]))
-        )
+            rxop.map(event_unknown_response)
+        )  # type: Observable[UnknownResponseEvent]
 
         self._alert = events.pipe(
             rxop.take_until(self.disconnected),
             rxop.filter(self.__filter_event('interface/alert')),
-            rxop.map(lambda ev: AlertEvent.from_protobuf(ev[1]))
-        )
+            rxop.map(event_alert)
+        )  # type: Observable[AlertEvent]
 
         events.pipe(
             rxop.filter(self.__filter_event('interface/disconnected')),
             rxop.take(1),
-            rxop.map(lambda ev: convert_exception(ev[1].error_type, ev[1].error_message))
-        ).subscribe(self._disconnected)
+            rxop.map(event_disconnect)
+        ).subscribe(self._disconnected)  # type: ignore
 
 
 class AsyncConnectionOpener:
     '''Provides a connection in an asynchronous context using `await` or `async with`'''
-    def __init__(self, request: main_pb2.OpenInterfaceRequest) -> None:
+    def __init__(self, request: dto.OpenInterfaceRequest) -> None:
         self._request = request
         self._resource: Optional[Connection] = None
 
     async def _create_resource(self) -> Connection:
-        response = main_pb2.OpenInterfaceResponse()
-        task = asyncio.ensure_future(call_async("interface/open", self._request, response))
+        task = asyncio.ensure_future(call_async(
+            "interface/open",
+            self._request,
+            dto.OpenInterfaceResponse.from_binary))
 
         try:
-            await asyncio.shield(task)
+            response = await asyncio.shield(task)
         except asyncio.CancelledError:
             async def cancel() -> None:
                 try:
-                    await task
+                    response = await task
                     await Connection(response.interface_id).close_async()
                 except MotionLibException:
                     pass
 
             asyncio.ensure_future(cancel())
             raise
 
@@ -974,7 +1057,19 @@
     async def __aenter__(self) -> 'Connection':
         self._resource = await self._create_resource()
         return self._resource
 
     async def __aexit__(self, exc_type: Any, exc: Any, trace: Any) -> None:
         if self._resource is not None:
             await self._resource.close_async()
+
+
+def event_unknown_response(event: Event[dto.UnknownResponseEventWrapper]) -> UnknownResponseEvent:
+    return event.data.unknown_response
+
+
+def event_alert(event: Event[dto.AlertEventWrapper]) -> AlertEvent:
+    return event.data.alert
+
+
+def event_disconnect(event: Event[dto.DisconnectedEvent]) -> MotionLibException:
+    return convert_exception(event.data.error_type, event.data.error_message)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/get_setting_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,61 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
+from ...units import Units, UnitsAndLiterals, units_from_literals
 
-from typing import Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
-from ..units import UnitsAndLiterals, Units, units_from_literals
 
-
-class ConversionFactor:
+@dataclass
+class GetSettingResult:
     """
-    Represents unit conversion factor for a single dimension.
+    The response from a multi-get command.
     """
 
-    def __init__(
-            self: 'ConversionFactor',
-            setting: str,
-            value: float,
-            unit: UnitsAndLiterals
-    ) -> None:
-        self._setting = setting
-        self._value = value
-        self._unit = unit
-
-    @property
-    def setting(self) -> str:
-        """
-        Setting representing the dimension.
-        """
-
-        return self._setting
-
-    @setting.setter
-    def setting(self, value: str) -> None:
-        self._setting = value
-
-    @property
-    def value(self) -> float:
-        """
-        Value representing 1 native device unit in specified real-word units.
-        """
-
-        return self._value
-
-    @value.setter
-    def value(self, value: float) -> None:
-        self._value = value
-
-    @property
-    def unit(self) -> UnitsAndLiterals:
-        """
-        Units of the value.
-        """
-
-        return self._unit
+    setting: str
+    """
+    The setting read.
+    """
 
-    @unit.setter
-    def unit(self, value: UnitsAndLiterals) -> None:
-        self._unit = value
+    values: List[float]
+    """
+    The list of values returned.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    unit: UnitsAndLiterals
+    """
+    The unit of the values.
+    """
 
     @staticmethod
-    def to_protobuf(source: 'Optional[ConversionFactor]') -> main_pb2.ConversionFactor:
-        pb_data = main_pb2.ConversionFactor()
-
-        if source is None:
-            return pb_data
+    def zero_values() -> 'GetSettingResult':
+        return GetSettingResult(
+            setting="",
+            values=[],
+            unit=Units.NATIVE,
+        )
 
-        if not isinstance(source, ConversionFactor):
-            raise TypeError("Provided value is not ConversionFactor.")
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'GetSettingResult':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return GetSettingResult.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'setting': self.setting,
+            'values': self.values,
+            'unit': units_from_literals(self.unit).value,
+        }
 
-        pb_data.setting = source.setting
-        pb_data.value = source.value
-        pb_data.unit = units_from_literals(source.unit or Units.NATIVE).value
-        return pb_data
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> 'GetSettingResult':
+        return GetSettingResult(
+            setting=data.get('setting'),  # type: ignore
+            values=data.get('values'),  # type: ignore
+            unit=Units(data.get('unit')),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/device.py` & `zaber_motion-6.0.0/zaber_motion/ascii/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING, List, Optional
 from ..call import call, call_async, call_sync
 
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from .device_settings import DeviceSettings
 from .axis import Axis
 from .all_axes import AllAxes
 from .warnings import Warnings
-from .device_identity import DeviceIdentity
+from ..dto.ascii.device_identity import DeviceIdentity
 from .device_io import DeviceIO
-from .response import Response
+from ..dto.ascii.response import Response
 from .lockstep import Lockstep
 from .oscilloscope import Oscilloscope
 from .storage import DeviceStorage
-from .can_set_state_device_response import CanSetStateDeviceResponse
+from ..dto.ascii.can_set_state_device_response import CanSetStateDeviceResponse
 from .pvt import Pvt
 from .triggers import Triggers
 from .streams import Streams
-from ..firmware_version import FirmwareVersion
-from ..measurement import Measurement
+from ..dto.firmware_version import FirmwareVersion
+from ..dto.measurement import Measurement
 
 if TYPE_CHECKING:
     from .connection import Connection
 
 
 class Device:
     """
@@ -204,21 +204,24 @@
             assume_version: The identification assumes the specified firmware version
                 instead of the version queried from the device.
                 Providing this argument can lead to unexpected compatibility issues.
 
         Returns:
             Device identification data.
         """
-        request = main_pb2.DeviceIdentifyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.assume_version.CopyFrom(FirmwareVersion.to_protobuf(assume_version))
-        response = main_pb2.DeviceIdentity()
-        call("device/identify", request, response)
-        return DeviceIdentity.from_protobuf(response)
+        request = dto.DeviceIdentifyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            assume_version=assume_version,
+        )
+        response = call(
+            "device/identify",
+            request,
+            DeviceIdentity.from_binary)
+        return response
 
     async def identify_async(
             self,
             assume_version: Optional[FirmwareVersion] = None
     ) -> DeviceIdentity:
         """
         Queries the device and the database, gathering information about the product.
@@ -229,21 +232,24 @@
             assume_version: The identification assumes the specified firmware version
                 instead of the version queried from the device.
                 Providing this argument can lead to unexpected compatibility issues.
 
         Returns:
             Device identification data.
         """
-        request = main_pb2.DeviceIdentifyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.assume_version.CopyFrom(FirmwareVersion.to_protobuf(assume_version))
-        response = main_pb2.DeviceIdentity()
-        await call_async("device/identify", request, response)
-        return DeviceIdentity.from_protobuf(response)
+        request = dto.DeviceIdentifyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            assume_version=assume_version,
+        )
+        response = await call_async(
+            "device/identify",
+            request,
+            DeviceIdentity.from_binary)
+        return response
 
     def generic_command(
             self,
             command: str,
             axis: int = 0,
             check_errors: bool = True,
             timeout: int = 0
@@ -258,24 +264,27 @@
             check_errors: Controls whether to throw an exception when the device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             A response to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command
-        request.axis = axis
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponse()
-        call("interface/generic_command", request, response)
-        return Response.from_protobuf(response)
+        request = dto.GenericCommandRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            axis=axis,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = call(
+            "interface/generic_command",
+            request,
+            Response.from_binary)
+        return response
 
     async def generic_command_async(
             self,
             command: str,
             axis: int = 0,
             check_errors: bool = True,
             timeout: int = 0
@@ -290,24 +299,27 @@
             check_errors: Controls whether to throw an exception when the device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             A response to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command
-        request.axis = axis
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponse()
-        await call_async("interface/generic_command", request, response)
-        return Response.from_protobuf(response)
+        request = dto.GenericCommandRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            axis=axis,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "interface/generic_command",
+            request,
+            Response.from_binary)
+        return response
 
     def generic_command_multi_response(
             self,
             command: str,
             axis: int = 0,
             check_errors: bool = True,
             timeout: int = 0
@@ -323,24 +335,27 @@
             check_errors: Controls whether to throw an exception when a device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             All responses to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command
-        request.axis = axis
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponseCollection()
-        call("interface/generic_command_multi_response", request, response)
-        return [Response.from_protobuf(a) for a in response.responses]
+        request = dto.GenericCommandRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            axis=axis,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = call(
+            "interface/generic_command_multi_response",
+            request,
+            dto.GenericCommandResponseCollection.from_binary)
+        return response.responses
 
     async def generic_command_multi_response_async(
             self,
             command: str,
             axis: int = 0,
             check_errors: bool = True,
             timeout: int = 0
@@ -356,24 +371,27 @@
             check_errors: Controls whether to throw an exception when a device rejects the command.
             timeout: The timeout, in milliseconds, for a device to respond to the command.
                 Overrides the connection default request timeout.
 
         Returns:
             All responses to the command.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command
-        request.axis = axis
-        request.check_errors = check_errors
-        request.timeout = timeout
-        response = main_pb2.GenericCommandResponseCollection()
-        await call_async("interface/generic_command_multi_response", request, response)
-        return [Response.from_protobuf(a) for a in response.responses]
+        request = dto.GenericCommandRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            axis=axis,
+            check_errors=check_errors,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "interface/generic_command_multi_response",
+            request,
+            dto.GenericCommandResponseCollection.from_binary)
+        return response.responses
 
     def generic_command_no_response(
             self,
             command: str,
             axis: int = 0
     ) -> None:
         """
@@ -381,19 +399,20 @@
         For more information refer to: [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_commands).
 
         Args:
             command: Command and its parameters.
             axis: Optional axis number to send the command to.
                 Specifying -1 omits the number completely.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command
-        request.axis = axis
+        request = dto.GenericCommandRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            axis=axis,
+        )
         call("interface/generic_command_no_response", request)
 
     async def generic_command_no_response_async(
             self,
             command: str,
             axis: int = 0
     ) -> None:
@@ -402,19 +421,20 @@
         For more information refer to: [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_commands).
 
         Args:
             command: Command and its parameters.
             axis: Optional axis number to send the command to.
                 Specifying -1 omits the number completely.
         """
-        request = main_pb2.GenericCommandRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command
-        request.axis = axis
+        request = dto.GenericCommandRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            axis=axis,
+        )
         await call_async("interface/generic_command_no_response", request)
 
     def get_axis(
             self,
             axis_number: int
     ) -> Axis:
         """
@@ -466,157 +486,176 @@
         Args:
             command_template: Template of a command to prepare. Parameters are denoted by question marks.
             parameters: Variable number of command parameters.
 
         Returns:
             Command with converted parameters.
         """
-        request = main_pb2.PrepareCommandRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command_template = command_template
-        request.parameters.extend([Measurement.to_protobuf(a) for a in parameters])
-        response = main_pb2.StringResponse()
-        call_sync("device/prepare_command", request, response)
+        request = dto.PrepareCommandRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command_template=command_template,
+            parameters=list(parameters),
+        )
+        response = call_sync(
+            "device/prepare_command",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def set_label(
             self,
             label: str
     ) -> None:
         """
         Sets the user-assigned device label.
         The label is stored on the controller and recognized by other software.
 
         Args:
             label: Label to set.
         """
-        request = main_pb2.DeviceSetStorageRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.value = label
+        request = dto.DeviceSetStorageRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            value=label,
+        )
         call("device/set_label", request)
 
     async def set_label_async(
             self,
             label: str
     ) -> None:
         """
         Sets the user-assigned device label.
         The label is stored on the controller and recognized by other software.
 
         Args:
             label: Label to set.
         """
-        request = main_pb2.DeviceSetStorageRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.value = label
+        request = dto.DeviceSetStorageRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            value=label,
+        )
         await call_async("device/set_label", request)
 
     def __retrieve_label(
             self
     ) -> str:
         """
         Gets the device name.
 
         Returns:
             The label.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.StringResponse()
-        call_sync("device/get_label", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call_sync(
+            "device/get_label",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the device.
 
         Returns:
             A string that represents the device.
         """
-        request = main_pb2.AxisToStringRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.StringResponse()
-        call_sync("device/device_to_string", request, response)
+        request = dto.AxisToStringRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call_sync(
+            "device/device_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def get_state(
             self
     ) -> str:
         """
         Returns a serialization of the current device state that can be saved and reapplied.
 
         Returns:
             A serialization of the current state of the device.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.StringResponse()
-        call("device/get_state", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call(
+            "device/get_state",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     async def get_state_async(
             self
     ) -> str:
         """
         Returns a serialization of the current device state that can be saved and reapplied.
 
         Returns:
             A serialization of the current state of the device.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.StringResponse()
-        await call_async("device/get_state", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = await call_async(
+            "device/get_state",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def set_state(
             self,
             state: str,
             device_only: bool = False
     ) -> None:
         """
         Applies a saved state to this device.
 
         Args:
             state: The state object to apply to this device.
             device_only: If true, only device scope settings and features will be set.
         """
-        request = main_pb2.SetStateRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.state = state
-        request.device_only = device_only
+        request = dto.SetStateRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            state=state,
+            device_only=device_only,
+        )
         call("device/set_state", request)
 
     async def set_state_async(
             self,
             state: str,
             device_only: bool = False
     ) -> None:
         """
         Applies a saved state to this device.
 
         Args:
             state: The state object to apply to this device.
             device_only: If true, only device scope settings and features will be set.
         """
-        request = main_pb2.SetStateRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.state = state
-        request.device_only = device_only
+        request = dto.SetStateRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            state=state,
+            device_only=device_only,
+        )
         await call_async("device/set_state", request)
 
     def can_set_state(
             self,
             state: str
     ) -> CanSetStateDeviceResponse:
         """
@@ -626,21 +665,24 @@
 
         Args:
             state: The state object to check against.
 
         Returns:
             An object listing errors that come up when trying to set the state.
         """
-        request = main_pb2.CanSetStateRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.state = state
-        response = main_pb2.CanSetStateDeviceResponse()
-        call("device/can_set_state", request, response)
-        return CanSetStateDeviceResponse.from_protobuf(response)
+        request = dto.CanSetStateRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            state=state,
+        )
+        response = call(
+            "device/can_set_state",
+            request,
+            CanSetStateDeviceResponse.from_binary)
+        return response
 
     async def can_set_state_async(
             self,
             state: str
     ) -> CanSetStateDeviceResponse:
         """
         Checks if a state can be applied to this device.
@@ -649,82 +691,93 @@
 
         Args:
             state: The state object to check against.
 
         Returns:
             An object listing errors that come up when trying to set the state.
         """
-        request = main_pb2.CanSetStateRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.state = state
-        response = main_pb2.CanSetStateDeviceResponse()
-        await call_async("device/can_set_state", request, response)
-        return CanSetStateDeviceResponse.from_protobuf(response)
+        request = dto.CanSetStateRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            state=state,
+        )
+        response = await call_async(
+            "device/can_set_state",
+            request,
+            CanSetStateDeviceResponse.from_binary)
+        return response
 
     def wait_to_respond(
             self,
             timeout: float
     ) -> None:
         """
         Waits for the device to start responding to messages.
         Useful to call after resetting the device.
         Throws RequestTimeoutException upon timeout.
 
         Args:
             timeout: For how long to wait in milliseconds for the device to start responding.
         """
-        request = main_pb2.WaitToRespondRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.timeout = timeout
+        request = dto.WaitToRespondRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            timeout=timeout,
+        )
         call("device/wait_to_respond", request)
 
     async def wait_to_respond_async(
             self,
             timeout: float
     ) -> None:
         """
         Waits for the device to start responding to messages.
         Useful to call after resetting the device.
         Throws RequestTimeoutException upon timeout.
 
         Args:
             timeout: For how long to wait in milliseconds for the device to start responding.
         """
-        request = main_pb2.WaitToRespondRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.timeout = timeout
+        request = dto.WaitToRespondRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            timeout=timeout,
+        )
         await call_async("device/wait_to_respond", request)
 
     def __retrieve_identity(
             self
     ) -> DeviceIdentity:
         """
         Returns identity.
 
         Returns:
             Device identity.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.DeviceIdentity()
-        call_sync("device/get_identity", request, response)
-        return DeviceIdentity.from_protobuf(response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call_sync(
+            "device/get_identity",
+            request,
+            DeviceIdentity.from_binary)
+        return response
 
     def __retrieve_is_identified(
             self
     ) -> bool:
         """
         Returns whether or not the device have been identified.
 
         Returns:
             True if the device has already been identified. False otherwise.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BoolResponse()
-        call_sync("device/get_is_identified", request, response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call_sync(
+            "device/get_is_identified",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/device_io.py` & `zaber_motion-6.0.0/zaber_motion/ascii/device_io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ﻿# pylint: disable=dangerous-default-value
 # ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING, List
 from ..call import call, call_async
-from ..units import Units, units_from_literals, TimeUnits
-from .device_io_info import DeviceIOInfo
-from .digital_output_action import DigitalOutputAction
-from .io_port_type import IoPortType
-from .io_port_label import IoPortLabel
+from ..units import Units, TimeUnits
+from ..dto.ascii.device_io_info import DeviceIOInfo
+from ..dto.ascii.digital_output_action import DigitalOutputAction
+from ..dto.ascii.io_port_type import IoPortType
+from ..dto.ascii.io_port_label import IoPortLabel
 
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class DeviceIO:
     """
@@ -29,161 +29,188 @@
     ) -> List[bool]:
         """
         Returns the current values of all digital input channels.
 
         Returns:
             True if voltage is present on the input channel and false otherwise.
         """
-        request = main_pb2.DeviceGetAllDigitalIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "di"
-        response = main_pb2.DeviceGetAllDigitalIOResponse()
-        call("device/get_all_digital_io", request, response)
-        return list(response.values)
+        request = dto.DeviceGetAllDigitalIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="di",
+        )
+        response = call(
+            "device/get_all_digital_io",
+            request,
+            dto.DeviceGetAllDigitalIOResponse.from_binary)
+        return response.values
 
     async def get_all_digital_inputs_async(
             self
     ) -> List[bool]:
         """
         Returns the current values of all digital input channels.
 
         Returns:
             True if voltage is present on the input channel and false otherwise.
         """
-        request = main_pb2.DeviceGetAllDigitalIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "di"
-        response = main_pb2.DeviceGetAllDigitalIOResponse()
-        await call_async("device/get_all_digital_io", request, response)
-        return list(response.values)
+        request = dto.DeviceGetAllDigitalIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="di",
+        )
+        response = await call_async(
+            "device/get_all_digital_io",
+            request,
+            dto.DeviceGetAllDigitalIOResponse.from_binary)
+        return response.values
 
     def get_all_digital_outputs(
             self
     ) -> List[bool]:
         """
         Returns the current values of all digital output channels.
 
         Returns:
             True if the output channel is conducting and false otherwise.
         """
-        request = main_pb2.DeviceGetAllDigitalIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "do"
-        response = main_pb2.DeviceGetAllDigitalIOResponse()
-        call("device/get_all_digital_io", request, response)
-        return list(response.values)
+        request = dto.DeviceGetAllDigitalIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="do",
+        )
+        response = call(
+            "device/get_all_digital_io",
+            request,
+            dto.DeviceGetAllDigitalIOResponse.from_binary)
+        return response.values
 
     async def get_all_digital_outputs_async(
             self
     ) -> List[bool]:
         """
         Returns the current values of all digital output channels.
 
         Returns:
             True if the output channel is conducting and false otherwise.
         """
-        request = main_pb2.DeviceGetAllDigitalIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "do"
-        response = main_pb2.DeviceGetAllDigitalIOResponse()
-        await call_async("device/get_all_digital_io", request, response)
-        return list(response.values)
+        request = dto.DeviceGetAllDigitalIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="do",
+        )
+        response = await call_async(
+            "device/get_all_digital_io",
+            request,
+            dto.DeviceGetAllDigitalIOResponse.from_binary)
+        return response.values
 
     def get_all_analog_inputs(
             self
     ) -> List[float]:
         """
         Returns the current values of all analog input channels.
 
         Returns:
              Measurements of the voltage present on the input channels.
         """
-        request = main_pb2.DeviceGetAllAnalogIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "ai"
-        response = main_pb2.DeviceGetAllAnalogIOResponse()
-        call("device/get_all_analog_io", request, response)
-        return list(response.values)
+        request = dto.DeviceGetAllAnalogIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="ai",
+        )
+        response = call(
+            "device/get_all_analog_io",
+            request,
+            dto.DeviceGetAllAnalogIOResponse.from_binary)
+        return response.values
 
     async def get_all_analog_inputs_async(
             self
     ) -> List[float]:
         """
         Returns the current values of all analog input channels.
 
         Returns:
              Measurements of the voltage present on the input channels.
         """
-        request = main_pb2.DeviceGetAllAnalogIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "ai"
-        response = main_pb2.DeviceGetAllAnalogIOResponse()
-        await call_async("device/get_all_analog_io", request, response)
-        return list(response.values)
+        request = dto.DeviceGetAllAnalogIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="ai",
+        )
+        response = await call_async(
+            "device/get_all_analog_io",
+            request,
+            dto.DeviceGetAllAnalogIOResponse.from_binary)
+        return response.values
 
     def get_all_analog_outputs(
             self
     ) -> List[float]:
         """
         Returns the current values of all analog output channels.
 
         Returns:
              Measurements of voltage that the output channels are conducting.
         """
-        request = main_pb2.DeviceGetAllAnalogIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "ao"
-        response = main_pb2.DeviceGetAllAnalogIOResponse()
-        call("device/get_all_analog_io", request, response)
-        return list(response.values)
+        request = dto.DeviceGetAllAnalogIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="ao",
+        )
+        response = call(
+            "device/get_all_analog_io",
+            request,
+            dto.DeviceGetAllAnalogIOResponse.from_binary)
+        return response.values
 
     async def get_all_analog_outputs_async(
             self
     ) -> List[float]:
         """
         Returns the current values of all analog output channels.
 
         Returns:
              Measurements of voltage that the output channels are conducting.
         """
-        request = main_pb2.DeviceGetAllAnalogIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "ao"
-        response = main_pb2.DeviceGetAllAnalogIOResponse()
-        await call_async("device/get_all_analog_io", request, response)
-        return list(response.values)
+        request = dto.DeviceGetAllAnalogIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="ao",
+        )
+        response = await call_async(
+            "device/get_all_analog_io",
+            request,
+            dto.DeviceGetAllAnalogIOResponse.from_binary)
+        return response.values
 
     def get_digital_input(
             self,
             channel_number: int
     ) -> bool:
         """
         Returns the current value of the specified digital input channel.
 
         Args:
             channel_number: Channel number starting at 1.
 
         Returns:
             True if voltage is present on the input channel and false otherwise.
         """
-        request = main_pb2.DeviceGetDigitalIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "di"
-        request.channel_number = channel_number
-        response = main_pb2.BoolResponse()
-        call("device/get_digital_io", request, response)
+        request = dto.DeviceGetDigitalIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="di",
+            channel_number=channel_number,
+        )
+        response = call(
+            "device/get_digital_io",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def get_digital_input_async(
             self,
             channel_number: int
     ) -> bool:
         """
@@ -191,21 +218,24 @@
 
         Args:
             channel_number: Channel number starting at 1.
 
         Returns:
             True if voltage is present on the input channel and false otherwise.
         """
-        request = main_pb2.DeviceGetDigitalIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "di"
-        request.channel_number = channel_number
-        response = main_pb2.BoolResponse()
-        await call_async("device/get_digital_io", request, response)
+        request = dto.DeviceGetDigitalIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="di",
+            channel_number=channel_number,
+        )
+        response = await call_async(
+            "device/get_digital_io",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def get_digital_output(
             self,
             channel_number: int
     ) -> bool:
         """
@@ -213,21 +243,24 @@
 
         Args:
             channel_number: Channel number starting at 1.
 
         Returns:
             True if the output channel is conducting and false otherwise.
         """
-        request = main_pb2.DeviceGetDigitalIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "do"
-        request.channel_number = channel_number
-        response = main_pb2.BoolResponse()
-        call("device/get_digital_io", request, response)
+        request = dto.DeviceGetDigitalIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="do",
+            channel_number=channel_number,
+        )
+        response = call(
+            "device/get_digital_io",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def get_digital_output_async(
             self,
             channel_number: int
     ) -> bool:
         """
@@ -235,21 +268,24 @@
 
         Args:
             channel_number: Channel number starting at 1.
 
         Returns:
             True if the output channel is conducting and false otherwise.
         """
-        request = main_pb2.DeviceGetDigitalIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "do"
-        request.channel_number = channel_number
-        response = main_pb2.BoolResponse()
-        await call_async("device/get_digital_io", request, response)
+        request = dto.DeviceGetDigitalIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="do",
+            channel_number=channel_number,
+        )
+        response = await call_async(
+            "device/get_digital_io",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def get_analog_input(
             self,
             channel_number: int
     ) -> float:
         """
@@ -257,21 +293,24 @@
 
         Args:
             channel_number: Channel number starting at 1.
 
         Returns:
              A measurementsof the voltage present on the input channel.
         """
-        request = main_pb2.DeviceGetAnalogIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "ai"
-        request.channel_number = channel_number
-        response = main_pb2.DoubleResponse()
-        call("device/get_analog_io", request, response)
+        request = dto.DeviceGetAnalogIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="ai",
+            channel_number=channel_number,
+        )
+        response = call(
+            "device/get_analog_io",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_analog_input_async(
             self,
             channel_number: int
     ) -> float:
         """
@@ -279,21 +318,24 @@
 
         Args:
             channel_number: Channel number starting at 1.
 
         Returns:
              A measurementsof the voltage present on the input channel.
         """
-        request = main_pb2.DeviceGetAnalogIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "ai"
-        request.channel_number = channel_number
-        response = main_pb2.DoubleResponse()
-        await call_async("device/get_analog_io", request, response)
+        request = dto.DeviceGetAnalogIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="ai",
+            channel_number=channel_number,
+        )
+        response = await call_async(
+            "device/get_analog_io",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_analog_output(
             self,
             channel_number: int
     ) -> float:
         """
@@ -301,21 +343,24 @@
 
         Args:
             channel_number: Channel number starting at 1.
 
         Returns:
             A measurement of voltage that the output channel is conducting.
         """
-        request = main_pb2.DeviceGetAnalogIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "ao"
-        request.channel_number = channel_number
-        response = main_pb2.DoubleResponse()
-        call("device/get_analog_io", request, response)
+        request = dto.DeviceGetAnalogIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="ao",
+            channel_number=channel_number,
+        )
+        response = call(
+            "device/get_analog_io",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_analog_output_async(
             self,
             channel_number: int
     ) -> float:
         """
@@ -323,53 +368,58 @@
 
         Args:
             channel_number: Channel number starting at 1.
 
         Returns:
             A measurement of voltage that the output channel is conducting.
         """
-        request = main_pb2.DeviceGetAnalogIORequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_type = "ao"
-        request.channel_number = channel_number
-        response = main_pb2.DoubleResponse()
-        await call_async("device/get_analog_io", request, response)
+        request = dto.DeviceGetAnalogIORequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_type="ao",
+            channel_number=channel_number,
+        )
+        response = await call_async(
+            "device/get_analog_io",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set_all_digital_outputs(
             self,
             values: List[DigitalOutputAction]
     ) -> None:
         """
         Sets values for all digital output channels.
 
         Args:
             values: The type of action to perform on the channel.
         """
-        request = main_pb2.DeviceSetAllDigitalOutputsRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.values.extend([x.value for x in values])
+        request = dto.DeviceSetAllDigitalOutputsRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            values=values,
+        )
         call("device/set_all_digital_outputs", request)
 
     async def set_all_digital_outputs_async(
             self,
             values: List[DigitalOutputAction]
     ) -> None:
         """
         Sets values for all digital output channels.
 
         Args:
             values: The type of action to perform on the channel.
         """
-        request = main_pb2.DeviceSetAllDigitalOutputsRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.values.extend([x.value for x in values])
+        request = dto.DeviceSetAllDigitalOutputsRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            values=values,
+        )
         await call_async("device/set_all_digital_outputs", request)
 
     def set_all_digital_outputs_schedule(
             self,
             values: List[DigitalOutputAction],
             future_values: List[DigitalOutputAction],
             delay: float,
@@ -384,21 +434,22 @@
             future_values: The type of actions to perform in the future on output channels.
             delay: Delay between setting current values and setting future values.
             unit: Units of time.
         """
         if delay <= 0:
             raise ValueError('Delay must be a positive value.')
 
-        request = main_pb2.DeviceSetAllDigitalOutputsScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.values.extend([x.value for x in values])
-        request.future_values.extend([x.value for x in future_values])
-        request.delay = delay
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetAllDigitalOutputsScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            values=values,
+            future_values=future_values,
+            delay=delay,
+            unit=unit,
+        )
         call("device/set_all_digital_outputs_schedule", request)
 
     async def set_all_digital_outputs_schedule_async(
             self,
             values: List[DigitalOutputAction],
             future_values: List[DigitalOutputAction],
             delay: float,
@@ -413,21 +464,22 @@
             future_values: The type of actions to perform in the future on output channels.
             delay: Delay between setting current values and setting future values.
             unit: Units of time.
         """
         if delay <= 0:
             raise ValueError('Delay must be a positive value.')
 
-        request = main_pb2.DeviceSetAllDigitalOutputsScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.values.extend([x.value for x in values])
-        request.future_values.extend([x.value for x in future_values])
-        request.delay = delay
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetAllDigitalOutputsScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            values=values,
+            future_values=future_values,
+            delay=delay,
+            unit=unit,
+        )
         await call_async("device/set_all_digital_outputs_schedule", request)
 
     def cancel_all_digital_outputs_schedule(
             self,
             channels: List[bool] = []
     ) -> None:
         """
@@ -435,19 +487,20 @@
         Requires at least Firmware 7.37.
 
         Args:
             channels: Optionally specify which channels to cancel.
                 Array length must be empty or equal to the number of channels on device.
                 Specifying "True" for a channel will cancel the scheduled digital output action for that channel.
         """
-        request = main_pb2.DeviceCancelAllOutputsScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.analog = False
-        request.channels.extend(channels)
+        request = dto.DeviceCancelAllOutputsScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            analog=False,
+            channels=channels,
+        )
         call("device/cancel_all_outputs_schedule", request)
 
     async def cancel_all_digital_outputs_schedule_async(
             self,
             channels: List[bool] = []
     ) -> None:
         """
@@ -455,19 +508,20 @@
         Requires at least Firmware 7.37.
 
         Args:
             channels: Optionally specify which channels to cancel.
                 Array length must be empty or equal to the number of channels on device.
                 Specifying "True" for a channel will cancel the scheduled digital output action for that channel.
         """
-        request = main_pb2.DeviceCancelAllOutputsScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.analog = False
-        request.channels.extend(channels)
+        request = dto.DeviceCancelAllOutputsScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            analog=False,
+            channels=channels,
+        )
         await call_async("device/cancel_all_outputs_schedule", request)
 
     def cancel_all_analog_outputs_schedule(
             self,
             channels: List[bool] = []
     ) -> None:
         """
@@ -475,19 +529,20 @@
         Requires at least Firmware 7.38.
 
         Args:
             channels: Optionally specify which channels to cancel.
                 Array length must be empty or equal to the number of channels on device.
                 Specifying "True" for a channel will cancel the scheduled analog output value for that channel.
         """
-        request = main_pb2.DeviceCancelAllOutputsScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.analog = True
-        request.channels.extend(channels)
+        request = dto.DeviceCancelAllOutputsScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            analog=True,
+            channels=channels,
+        )
         call("device/cancel_all_outputs_schedule", request)
 
     async def cancel_all_analog_outputs_schedule_async(
             self,
             channels: List[bool] = []
     ) -> None:
         """
@@ -495,51 +550,54 @@
         Requires at least Firmware 7.38.
 
         Args:
             channels: Optionally specify which channels to cancel.
                 Array length must be empty or equal to the number of channels on device.
                 Specifying "True" for a channel will cancel the scheduled analog output value for that channel.
         """
-        request = main_pb2.DeviceCancelAllOutputsScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.analog = True
-        request.channels.extend(channels)
+        request = dto.DeviceCancelAllOutputsScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            analog=True,
+            channels=channels,
+        )
         await call_async("device/cancel_all_outputs_schedule", request)
 
     def set_all_analog_outputs(
             self,
             values: List[float]
     ) -> None:
         """
         Sets values for all analog output channels.
 
         Args:
             values: Voltage values to set the output channels to.
         """
-        request = main_pb2.DeviceSetAllAnalogOutputsRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.values.extend(values)
+        request = dto.DeviceSetAllAnalogOutputsRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            values=values,
+        )
         call("device/set_all_analog_outputs", request)
 
     async def set_all_analog_outputs_async(
             self,
             values: List[float]
     ) -> None:
         """
         Sets values for all analog output channels.
 
         Args:
             values: Voltage values to set the output channels to.
         """
-        request = main_pb2.DeviceSetAllAnalogOutputsRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.values.extend(values)
+        request = dto.DeviceSetAllAnalogOutputsRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            values=values,
+        )
         await call_async("device/set_all_analog_outputs", request)
 
     def set_all_analog_outputs_schedule(
             self,
             values: List[float],
             future_values: List[float],
             delay: float,
@@ -554,21 +612,22 @@
             future_values: Voltage values to set the output channels to in the future.
             delay: Delay between setting current values and setting future values.
             unit: Units of time.
         """
         if delay <= 0:
             raise ValueError('Delay must be a positive value.')
 
-        request = main_pb2.DeviceSetAllAnalogOutputsScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.values.extend(values)
-        request.future_values.extend(future_values)
-        request.delay = delay
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetAllAnalogOutputsScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            values=values,
+            future_values=future_values,
+            delay=delay,
+            unit=unit,
+        )
         call("device/set_all_analog_outputs_schedule", request)
 
     async def set_all_analog_outputs_schedule_async(
             self,
             values: List[float],
             future_values: List[float],
             delay: float,
@@ -583,59 +642,62 @@
             future_values: Voltage values to set the output channels to in the future.
             delay: Delay between setting current values and setting future values.
             unit: Units of time.
         """
         if delay <= 0:
             raise ValueError('Delay must be a positive value.')
 
-        request = main_pb2.DeviceSetAllAnalogOutputsScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.values.extend(values)
-        request.future_values.extend(future_values)
-        request.delay = delay
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetAllAnalogOutputsScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            values=values,
+            future_values=future_values,
+            delay=delay,
+            unit=unit,
+        )
         await call_async("device/set_all_analog_outputs_schedule", request)
 
     def set_digital_output(
             self,
             channel_number: int,
             value: DigitalOutputAction
     ) -> None:
         """
         Sets value for the specified digital output channel.
 
         Args:
             channel_number: Channel number starting at 1.
             value: The type of action to perform on the channel.
         """
-        request = main_pb2.DeviceSetDigitalOutputRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_number = channel_number
-        request.value = value.value
+        request = dto.DeviceSetDigitalOutputRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_number=channel_number,
+            value=value,
+        )
         call("device/set_digital_output", request)
 
     async def set_digital_output_async(
             self,
             channel_number: int,
             value: DigitalOutputAction
     ) -> None:
         """
         Sets value for the specified digital output channel.
 
         Args:
             channel_number: Channel number starting at 1.
             value: The type of action to perform on the channel.
         """
-        request = main_pb2.DeviceSetDigitalOutputRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_number = channel_number
-        request.value = value.value
+        request = dto.DeviceSetDigitalOutputRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_number=channel_number,
+            value=value,
+        )
         await call_async("device/set_digital_output", request)
 
     def set_digital_output_schedule(
             self,
             channel_number: int,
             value: DigitalOutputAction,
             future_value: DigitalOutputAction,
@@ -652,22 +714,23 @@
             future_value: The type of action to perform in the future on the channel.
             delay: Delay between setting current value and setting future value.
             unit: Units of time.
         """
         if delay <= 0:
             raise ValueError('Delay must be a positive value.')
 
-        request = main_pb2.DeviceSetDigitalOutputScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_number = channel_number
-        request.value = value.value
-        request.future_value = future_value.value
-        request.delay = delay
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetDigitalOutputScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_number=channel_number,
+            value=value,
+            future_value=future_value,
+            delay=delay,
+            unit=unit,
+        )
         call("device/set_digital_output_schedule", request)
 
     async def set_digital_output_schedule_async(
             self,
             channel_number: int,
             value: DigitalOutputAction,
             future_value: DigitalOutputAction,
@@ -684,132 +747,139 @@
             future_value: The type of action to perform in the future on the channel.
             delay: Delay between setting current value and setting future value.
             unit: Units of time.
         """
         if delay <= 0:
             raise ValueError('Delay must be a positive value.')
 
-        request = main_pb2.DeviceSetDigitalOutputScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_number = channel_number
-        request.value = value.value
-        request.future_value = future_value.value
-        request.delay = delay
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetDigitalOutputScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_number=channel_number,
+            value=value,
+            future_value=future_value,
+            delay=delay,
+            unit=unit,
+        )
         await call_async("device/set_digital_output_schedule", request)
 
     def cancel_digital_output_schedule(
             self,
             channel_number: int
     ) -> None:
         """
         Cancels a scheduled digital output action.
         Requires at least Firmware 7.37.
 
         Args:
             channel_number: Channel number starting at 1.
         """
-        request = main_pb2.DeviceCancelOutputScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.analog = False
-        request.channel_number = channel_number
+        request = dto.DeviceCancelOutputScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            analog=False,
+            channel_number=channel_number,
+        )
         call("device/cancel_output_schedule", request)
 
     async def cancel_digital_output_schedule_async(
             self,
             channel_number: int
     ) -> None:
         """
         Cancels a scheduled digital output action.
         Requires at least Firmware 7.37.
 
         Args:
             channel_number: Channel number starting at 1.
         """
-        request = main_pb2.DeviceCancelOutputScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.analog = False
-        request.channel_number = channel_number
+        request = dto.DeviceCancelOutputScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            analog=False,
+            channel_number=channel_number,
+        )
         await call_async("device/cancel_output_schedule", request)
 
     def cancel_analog_output_schedule(
             self,
             channel_number: int
     ) -> None:
         """
         Cancels a scheduled analog output value.
         Requires at least Firmware 7.38.
 
         Args:
             channel_number: Channel number starting at 1.
         """
-        request = main_pb2.DeviceCancelOutputScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.analog = True
-        request.channel_number = channel_number
+        request = dto.DeviceCancelOutputScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            analog=True,
+            channel_number=channel_number,
+        )
         call("device/cancel_output_schedule", request)
 
     async def cancel_analog_output_schedule_async(
             self,
             channel_number: int
     ) -> None:
         """
         Cancels a scheduled analog output value.
         Requires at least Firmware 7.38.
 
         Args:
             channel_number: Channel number starting at 1.
         """
-        request = main_pb2.DeviceCancelOutputScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.analog = True
-        request.channel_number = channel_number
+        request = dto.DeviceCancelOutputScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            analog=True,
+            channel_number=channel_number,
+        )
         await call_async("device/cancel_output_schedule", request)
 
     def set_analog_output(
             self,
             channel_number: int,
             value: float
     ) -> None:
         """
         Sets value for the specified analog output channel.
 
         Args:
             channel_number: Channel number starting at 1.
             value: Value to set the output channel voltage to.
         """
-        request = main_pb2.DeviceSetAnalogOutputRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_number = channel_number
-        request.value = value
+        request = dto.DeviceSetAnalogOutputRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_number=channel_number,
+            value=value,
+        )
         call("device/set_analog_output", request)
 
     async def set_analog_output_async(
             self,
             channel_number: int,
             value: float
     ) -> None:
         """
         Sets value for the specified analog output channel.
 
         Args:
             channel_number: Channel number starting at 1.
             value: Value to set the output channel voltage to.
         """
-        request = main_pb2.DeviceSetAnalogOutputRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_number = channel_number
-        request.value = value
+        request = dto.DeviceSetAnalogOutputRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_number=channel_number,
+            value=value,
+        )
         await call_async("device/set_analog_output", request)
 
     def set_analog_output_schedule(
             self,
             channel_number: int,
             value: float,
             future_value: float,
@@ -826,22 +896,23 @@
             future_value: Value to set the output channel voltage to in the future.
             delay: Delay between setting current value and setting future value.
             unit: Units of time.
         """
         if delay <= 0:
             raise ValueError('Delay must be a positive value.')
 
-        request = main_pb2.DeviceSetAnalogOutputScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_number = channel_number
-        request.value = value
-        request.future_value = future_value
-        request.delay = delay
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetAnalogOutputScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_number=channel_number,
+            value=value,
+            future_value=future_value,
+            delay=delay,
+            unit=unit,
+        )
         call("device/set_analog_output_schedule", request)
 
     async def set_analog_output_schedule_async(
             self,
             channel_number: int,
             value: float,
             future_value: float,
@@ -858,55 +929,62 @@
             future_value: Value to set the output channel voltage to in the future.
             delay: Delay between setting current value and setting future value.
             unit: Units of time.
         """
         if delay <= 0:
             raise ValueError('Delay must be a positive value.')
 
-        request = main_pb2.DeviceSetAnalogOutputScheduleRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.channel_number = channel_number
-        request.value = value
-        request.future_value = future_value
-        request.delay = delay
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetAnalogOutputScheduleRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            channel_number=channel_number,
+            value=value,
+            future_value=future_value,
+            delay=delay,
+            unit=unit,
+        )
         await call_async("device/set_analog_output_schedule", request)
 
     def get_channels_info(
             self
     ) -> DeviceIOInfo:
         """
         Returns the number of I/O channels the device has.
 
         Returns:
             An object containing the number of I/O channels the device has.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        response = main_pb2.DeviceIOInfo()
-        call("device/get_io_info", request, response)
-        return DeviceIOInfo.from_protobuf(response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+        )
+        response = call(
+            "device/get_io_info",
+            request,
+            DeviceIOInfo.from_binary)
+        return response
 
     async def get_channels_info_async(
             self
     ) -> DeviceIOInfo:
         """
         Returns the number of I/O channels the device has.
 
         Returns:
             An object containing the number of I/O channels the device has.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        response = main_pb2.DeviceIOInfo()
-        await call_async("device/get_io_info", request, response)
-        return DeviceIOInfo.from_protobuf(response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+        )
+        response = await call_async(
+            "device/get_io_info",
+            request,
+            DeviceIOInfo.from_binary)
+        return response
 
     def set_label(
             self,
             port_type: IoPortType,
             channel_number: int,
             label: str
     ) -> None:
@@ -914,20 +992,21 @@
         Sets the label of the specified channel.
 
         Args:
             port_type: The type of channel to set the label of.
             channel_number: Channel number starting at 1.
             label: The label to set for the specified channel.
         """
-        request = main_pb2.SetIoPortLabel()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.port_type = port_type.value
-        request.channel_number = channel_number
-        request.label = label
+        request = dto.SetIoPortLabelRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            port_type=port_type,
+            channel_number=channel_number,
+            label=label,
+        )
         call("device/set_io_label", request)
 
     async def set_label_async(
             self,
             port_type: IoPortType,
             channel_number: int,
             label: str
@@ -936,20 +1015,21 @@
         Sets the label of the specified channel.
 
         Args:
             port_type: The type of channel to set the label of.
             channel_number: Channel number starting at 1.
             label: The label to set for the specified channel.
         """
-        request = main_pb2.SetIoPortLabel()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.port_type = port_type.value
-        request.channel_number = channel_number
-        request.label = label
+        request = dto.SetIoPortLabelRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            port_type=port_type,
+            channel_number=channel_number,
+            label=label,
+        )
         await call_async("device/set_io_label", request)
 
     def get_label(
             self,
             port_type: IoPortType,
             channel_number: int
     ) -> str:
@@ -959,21 +1039,24 @@
         Args:
             port_type: The type of channel to get the label of.
             channel_number: Channel number starting at 1.
 
         Returns:
             The label of the specified channel.
         """
-        request = main_pb2.GetIoPortLabel()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.port_type = port_type.value
-        request.channel_number = channel_number
-        response = main_pb2.StringResponse()
-        call("device/get_io_label", request, response)
+        request = dto.GetIoPortLabelRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            port_type=port_type,
+            channel_number=channel_number,
+        )
+        response = call(
+            "device/get_io_label",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     async def get_label_async(
             self,
             port_type: IoPortType,
             channel_number: int
     ) -> str:
@@ -983,47 +1066,56 @@
         Args:
             port_type: The type of channel to get the label of.
             channel_number: Channel number starting at 1.
 
         Returns:
             The label of the specified channel.
         """
-        request = main_pb2.GetIoPortLabel()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.port_type = port_type.value
-        request.channel_number = channel_number
-        response = main_pb2.StringResponse()
-        await call_async("device/get_io_label", request, response)
+        request = dto.GetIoPortLabelRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            port_type=port_type,
+            channel_number=channel_number,
+        )
+        response = await call_async(
+            "device/get_io_label",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def get_all_labels(
             self
     ) -> List[IoPortLabel]:
         """
         Returns every label assigned to an IO port on this device.
 
         Returns:
             The labels set for this device's IO.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        response = main_pb2.GetAllIoPortLabelsResponse()
-        call("device/get_all_io_labels", request, response)
-        return [IoPortLabel.from_protobuf(a) for a in response.labels]
+        request = dto.DeviceEmptyRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+        )
+        response = call(
+            "device/get_all_io_labels",
+            request,
+            dto.GetAllIoPortLabelsResponse.from_binary)
+        return response.labels
 
     async def get_all_labels_async(
             self
     ) -> List[IoPortLabel]:
         """
         Returns every label assigned to an IO port on this device.
 
         Returns:
             The labels set for this device's IO.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        response = main_pb2.GetAllIoPortLabelsResponse()
-        await call_async("device/get_all_io_labels", request, response)
-        return [IoPortLabel.from_protobuf(a) for a in response.labels]
+        request = dto.DeviceEmptyRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+        )
+        response = await call_async(
+            "device/get_all_io_labels",
+            request,
+            dto.GetAllIoPortLabelsResponse.from_binary)
+        return response.labels
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/device_settings.py` & `zaber_motion-6.0.0/zaber_motion/ascii/device_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING, List
 from ..call import call, call_async, call_sync
 
-from ..protobufs import main_pb2
-from ..units import UnitsAndLiterals, Units, units_from_literals
+from ..dto import requests as dto
+from ..units import UnitsAndLiterals, Units
 
-from .get_setting import GetSetting
-from .get_setting_result import GetSettingResult
+from ..dto.ascii.get_setting import GetSetting
+from ..dto.ascii.get_setting_result import GetSettingResult
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class DeviceSettings:
     """
@@ -34,21 +34,24 @@
         Args:
             setting: Name of the setting.
             unit: Units of setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("device/get_setting", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            unit=unit,
+        )
+        response = call(
+            "device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_async(
             self,
             setting: str,
             unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
@@ -59,21 +62,24 @@
         Args:
             setting: Name of the setting.
             unit: Units of setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("device/get_setting", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            unit=unit,
+        )
+        response = await call_async(
+            "device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set(
             self,
             setting: str,
             value: float,
             unit: UnitsAndLiterals = Units.NATIVE
@@ -83,20 +89,21 @@
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
             value: Value of the setting.
             unit: Units of setting.
         """
-        request = main_pb2.DeviceSetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
         call("device/set_setting", request)
 
     async def set_async(
             self,
             setting: str,
             value: float,
             unit: UnitsAndLiterals = Units.NATIVE
@@ -106,20 +113,21 @@
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
             value: Value of the setting.
             unit: Units of setting.
         """
-        request = main_pb2.DeviceSetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.DeviceSetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
         await call_async("device/set_setting", request)
 
     def get_string(
             self,
             setting: str
     ) -> str:
         """
@@ -128,20 +136,23 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        response = main_pb2.StringResponse()
-        call("device/get_setting_str", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+        )
+        response = call(
+            "device/get_setting_str",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     async def get_string_async(
             self,
             setting: str
     ) -> str:
         """
@@ -150,20 +161,23 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        response = main_pb2.StringResponse()
-        await call_async("device/get_setting_str", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+        )
+        response = await call_async(
+            "device/get_setting_str",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def set_string(
             self,
             setting: str,
             value: str
     ) -> None:
@@ -171,19 +185,20 @@
         Sets any device setting as a string.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
             value: Value of the setting.
         """
-        request = main_pb2.DeviceSetSettingStrRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        request.value = value
+        request = dto.DeviceSetSettingStrRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            value=value,
+        )
         call("device/set_setting_str", request)
 
     async def set_string_async(
             self,
             setting: str,
             value: str
     ) -> None:
@@ -191,19 +206,20 @@
         Sets any device setting as a string.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
             value: Value of the setting.
         """
-        request = main_pb2.DeviceSetSettingStrRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        request.value = value
+        request = dto.DeviceSetSettingStrRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            value=value,
+        )
         await call_async("device/set_setting_str", request)
 
     def convert_to_native_units(
             self,
             setting: str,
             value: float,
             unit: UnitsAndLiterals
@@ -215,22 +231,25 @@
             setting: Name of the setting.
             value: Value of the setting in units specified by following argument.
             unit: Units of the value.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceConvertSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        request.value = value
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("device/convert_setting", request, response)
+        request = dto.DeviceConvertSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
+        response = call_sync(
+            "device/convert_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def convert_from_native_units(
             self,
             setting: str,
             value: float,
             unit: UnitsAndLiterals
@@ -242,23 +261,26 @@
             setting: Name of the setting.
             value: Value of the setting in Zaber native units.
             unit: Units to convert value to.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.DeviceConvertSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.from_native = True
-        request.setting = setting
-        request.value = value
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("device/convert_setting", request, response)
+        request = dto.DeviceConvertSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            from_native=True,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
+        response = call_sync(
+            "device/convert_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_default(
             self,
             setting: str,
             unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
@@ -268,21 +290,24 @@
         Args:
             setting: Name of the setting.
             unit: Units of setting.
 
         Returns:
             Default setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("device/get_setting_default", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            unit=unit,
+        )
+        response = call_sync(
+            "device/get_setting_default",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_default_string(
             self,
             setting: str
     ) -> str:
         """
@@ -290,20 +315,23 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             Default setting value.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        response = main_pb2.StringResponse()
-        call_sync("device/get_setting_default_str", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+        )
+        response = call_sync(
+            "device/get_setting_default_str",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def can_convert_native_units(
             self,
             setting: str
     ) -> bool:
         """
@@ -311,20 +339,23 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             True if unit conversion can be performed.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        response = main_pb2.BoolResponse()
-        call_sync("device/can_convert_setting", request, response)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+        )
+        response = call_sync(
+            "device/can_convert_setting",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def get_from_all_axes(
             self,
             setting: str
     ) -> List[float]:
         """
@@ -333,21 +364,24 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             The setting values on each axis.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        response = main_pb2.DoubleArrayResponse()
-        call("device/get_setting_from_all_axes", request, response)
-        return list(response.values)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+        )
+        response = call(
+            "device/get_setting_from_all_axes",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     async def get_from_all_axes_async(
             self,
             setting: str
     ) -> List[float]:
         """
         Gets the value of an axis scope setting for each axis on the device.
@@ -355,63 +389,72 @@
 
         Args:
             setting: Name of the setting.
 
         Returns:
             The setting values on each axis.
         """
-        request = main_pb2.DeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting
-        response = main_pb2.DoubleArrayResponse()
-        await call_async("device/get_setting_from_all_axes", request, response)
-        return list(response.values)
+        request = dto.DeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+        )
+        response = await call_async(
+            "device/get_setting_from_all_axes",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     def get_many(
             self,
             *settings: GetSetting
     ) -> List[GetSettingResult]:
         """
         Gets many setting values in as few device requests as possible.
 
         Args:
             settings: The settings to read.
 
         Returns:
             The setting values read.
         """
-        request = main_pb2.DeviceMultiGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.settings.extend([GetSetting.to_protobuf(a) for a in settings])
-        response = main_pb2.GetSettingResults()
-        call("device/get_many_settings", request, response)
-        return [GetSettingResult.from_protobuf(a) for a in response.results]
+        request = dto.DeviceMultiGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            settings=list(settings),
+        )
+        response = call(
+            "device/get_many_settings",
+            request,
+            dto.GetSettingResults.from_binary)
+        return response.results
 
     async def get_many_async(
             self,
             *settings: GetSetting
     ) -> List[GetSettingResult]:
         """
         Gets many setting values in as few device requests as possible.
 
         Args:
             settings: The settings to read.
 
         Returns:
             The setting values read.
         """
-        request = main_pb2.DeviceMultiGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.settings.extend([GetSetting.to_protobuf(a) for a in settings])
-        response = main_pb2.GetSettingResults()
-        await call_async("device/get_many_settings", request, response)
-        return [GetSettingResult.from_protobuf(a) for a in response.results]
+        request = dto.DeviceMultiGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            settings=list(settings),
+        )
+        response = await call_async(
+            "device/get_many_settings",
+            request,
+            dto.GetSettingResults.from_binary)
+        return response.results
 
     def get_synchronized(
             self,
             *settings: GetSetting
     ) -> List[GetSettingResult]:
         """
         Gets many setting values in the same tick, ensuring their values are synchronized.
@@ -419,21 +462,24 @@
 
         Args:
             settings: The settings to read.
 
         Returns:
             The setting values read.
         """
-        request = main_pb2.DeviceMultiGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.settings.extend([GetSetting.to_protobuf(a) for a in settings])
-        response = main_pb2.GetSettingResults()
-        call("device/get_sync_settings", request, response)
-        return [GetSettingResult.from_protobuf(a) for a in response.results]
+        request = dto.DeviceMultiGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            settings=list(settings),
+        )
+        response = call(
+            "device/get_sync_settings",
+            request,
+            dto.GetSettingResults.from_binary)
+        return response.results
 
     async def get_synchronized_async(
             self,
             *settings: GetSetting
     ) -> List[GetSettingResult]:
         """
         Gets many setting values in the same tick, ensuring their values are synchronized.
@@ -441,14 +487,17 @@
 
         Args:
             settings: The settings to read.
 
         Returns:
             The setting values read.
         """
-        request = main_pb2.DeviceMultiGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.settings.extend([GetSetting.to_protobuf(a) for a in settings])
-        response = main_pb2.GetSettingResults()
-        await call_async("device/get_sync_settings", request, response)
-        return [GetSettingResult.from_protobuf(a) for a in response.results]
+        request = dto.DeviceMultiGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            settings=list(settings),
+        )
+        response = await call_async(
+            "device/get_sync_settings",
+            request,
+            dto.GetSettingResults.from_binary)
+        return response.results
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/get_axis_setting.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/get_axis_setting_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
+from ...units import Units, UnitsAndLiterals, units_from_literals
 
-from typing import Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
-from ..units import UnitsAndLiterals, Units, units_from_literals
 
-
-class GetAxisSetting:
+@dataclass
+class GetAxisSettingResult:
     """
-    Specifies a setting to get with one of the multi-get commands.
+    The response from a multi-get axis command.
     """
 
-    def __init__(
-            self: 'GetAxisSetting',
-            setting: str,
-            unit: Optional[UnitsAndLiterals] = None
-    ) -> None:
-        self._setting = setting
-        self._unit = unit
-
-    @property
-    def setting(self) -> str:
-        """
-        The setting to read.
-        """
-
-        return self._setting
-
-    @setting.setter
-    def setting(self, value: str) -> None:
-        self._setting = value
-
-    @property
-    def unit(self) -> Optional[UnitsAndLiterals]:
-        """
-        The unit to convert the read setting to.
-        """
-
-        return self._unit
+    setting: str
+    """
+    The setting read.
+    """
 
-    @unit.setter
-    def unit(self, value: Optional[UnitsAndLiterals]) -> None:
-        self._unit = value
+    value: float
+    """
+    The value read.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    unit: UnitsAndLiterals
+    """
+    The unit of the values.
+    """
 
     @staticmethod
-    def to_protobuf(source: 'Optional[GetAxisSetting]') -> main_pb2.GetSetting:
-        pb_data = main_pb2.GetSetting()
+    def zero_values() -> 'GetAxisSettingResult':
+        return GetAxisSettingResult(
+            setting="",
+            value=0,
+            unit=Units.NATIVE,
+        )
 
-        if source is None:
-            return pb_data
-
-        if not isinstance(source, GetAxisSetting):
-            raise TypeError("Provided value is not GetAxisSetting.")
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'GetAxisSettingResult':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return GetAxisSettingResult.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'setting': self.setting,
+            'value': self.value,
+            'unit': units_from_literals(self.unit).value,
+        }
 
-        pb_data.setting = source.setting
-        pb_data.unit = units_from_literals(source.unit or Units.NATIVE).value
-        return pb_data
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> 'GetAxisSettingResult':
+        return GetAxisSettingResult(
+            setting=data.get('setting'),  # type: ignore
+            value=data.get('value'),  # type: ignore
+            unit=Units(data.get('unit')),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/get_axis_setting_result.py` & `zaber_motion-6.0.0/zaber_motion/dto/requests/get_axis_setting_results.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,39 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
+from ..ascii.get_axis_setting_result import GetAxisSettingResult
 
-from ..protobufs import main_pb2
-from ..units import UnitsAndLiterals, Units
 
+@dataclass
+class GetAxisSettingResults:
 
-class GetAxisSettingResult:
-    """
-    The response from a multi-get axis command.
-    """
+    results: List[GetAxisSettingResult] = field(default_factory=list)
 
-    @property
-    def setting(self) -> str:
-        """
-        The setting read.
-        """
-
-        return self._setting
-
-    @setting.setter
-    def setting(self, value: str) -> None:
-        self._setting = value
-
-    @property
-    def value(self) -> float:
-        """
-        The value read.
-        """
-
-        return self._value
-
-    @value.setter
-    def value(self, value: float) -> None:
-        self._value = value
-
-    @property
-    def unit(self) -> UnitsAndLiterals:
-        """
-        The unit of the values.
-        """
-
-        return self._unit
-
-    @unit.setter
-    def unit(self, value: UnitsAndLiterals) -> None:
-        self._unit = value
+    @staticmethod
+    def zero_values() -> 'GetAxisSettingResults':
+        return GetAxisSettingResults(
+            results=[],
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'GetAxisSettingResults':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return GetAxisSettingResults.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'results': [item.to_dict() for item in self.results],
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.GetSettingResult
-    ) -> 'GetAxisSettingResult':
-        instance = GetAxisSettingResult.__new__(
-            GetAxisSettingResult
-        )  # type: GetAxisSettingResult
-        instance.setting = pb_data.setting
-        instance.value = pb_data.values[0]
-        instance.unit = Units(pb_data.unit)
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'GetAxisSettingResults':
+        return GetAxisSettingResults(
+            results=[GetAxisSettingResult.from_dict(item) for item in data.get('results')],  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/get_setting.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/get_axis_setting.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,53 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
+from ...units import Units, UnitsAndLiterals, units_from_literals
 
-from typing import List, Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
-from ..units import UnitsAndLiterals, Units, units_from_literals
 
-
-class GetSetting:
+@dataclass
+class GetAxisSetting:
     """
     Specifies a setting to get with one of the multi-get commands.
     """
 
-    def __init__(
-            self: 'GetSetting',
-            setting: str,
-            axes: Optional[List[int]] = None,
-            unit: Optional[UnitsAndLiterals] = None
-    ) -> None:
-        self._setting = setting
-        self._axes = axes
-        self._unit = unit
-
-    @property
-    def setting(self) -> str:
-        """
-        The setting to read.
-        """
-
-        return self._setting
-
-    @setting.setter
-    def setting(self, value: str) -> None:
-        self._setting = value
-
-    @property
-    def axes(self) -> Optional[List[int]]:
-        """
-        The list of axes to read.
-        """
-
-        return self._axes
-
-    @axes.setter
-    def axes(self, value: Optional[List[int]]) -> None:
-        self._axes = value
-
-    @property
-    def unit(self) -> Optional[UnitsAndLiterals]:
-        """
-        The unit to convert the read settings to.
-        """
-
-        return self._unit
-
-    @unit.setter
-    def unit(self, value: Optional[UnitsAndLiterals]) -> None:
-        self._unit = value
+    setting: str
+    """
+    The setting to read.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    unit: Optional[UnitsAndLiterals] = None
+    """
+    The unit to convert the read setting to.
+    """
 
     @staticmethod
-    def to_protobuf(source: 'Optional[GetSetting]') -> main_pb2.GetSetting:
-        pb_data = main_pb2.GetSetting()
-
-        if source is None:
-            return pb_data
+    def zero_values() -> 'GetAxisSetting':
+        return GetAxisSetting(
+            setting="",
+            unit=None,
+        )
 
-        if not isinstance(source, GetSetting):
-            raise TypeError("Provided value is not GetSetting.")
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'GetAxisSetting':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return GetAxisSetting.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'setting': self.setting,
+            'unit': units_from_literals(self.unit).value if self.unit is not None else None,
+        }
 
-        pb_data.setting = source.setting
-        if source.axes is not None:
-            pb_data.axes.extend(source.axes)
-        pb_data.unit = units_from_literals(source.unit or Units.NATIVE).value
-        return pb_data
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> 'GetAxisSetting':
+        return GetAxisSetting(
+            setting=data.get('setting'),  # type: ignore
+            unit=Units(data.get('unit')) if data.get('unit') is not None else None,  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/io_port_label.py` & `zaber_motion-6.0.0/zaber_motion/dto/requests/get_io_port_label_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,54 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
+from ..ascii.io_port_type import IoPortType
 
-from ..protobufs import main_pb2
-from .io_port_type import IoPortType
 
+@dataclass
+class GetIoPortLabelRequest:
 
-class IoPortLabel:
-    """
-    The label of an IO port.
-    """
+    interface_id: int = 0
 
-    @property
-    def port_type(self) -> IoPortType:
-        """
-        The type of the port.
-        """
+    device: int = 0
 
-        return self._port_type
+    port_type: IoPortType = next(first for first in IoPortType)
 
-    @port_type.setter
-    def port_type(self, value: IoPortType) -> None:
-        self._port_type = value
+    channel_number: int = 0
 
-    @property
-    def channel_number(self) -> int:
-        """
-        The number of the port.
-        """
-
-        return self._channel_number
-
-    @channel_number.setter
-    def channel_number(self, value: int) -> None:
-        self._channel_number = value
-
-    @property
-    def label(self) -> str:
-        """
-        The label of the port.
-        """
-
-        return self._label
-
-    @label.setter
-    def label(self, value: str) -> None:
-        self._label = value
+    @staticmethod
+    def zero_values() -> 'GetIoPortLabelRequest':
+        return GetIoPortLabelRequest(
+            interface_id=0,
+            device=0,
+            port_type=next(first for first in IoPortType),
+            channel_number=0,
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'GetIoPortLabelRequest':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return GetIoPortLabelRequest.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'interfaceId': self.interface_id,
+            'device': self.device,
+            'portType': self.port_type.value,
+            'channelNumber': self.channel_number,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.IoPortLabel
-    ) -> 'IoPortLabel':
-        instance = IoPortLabel.__new__(
-            IoPortLabel
-        )  # type: IoPortLabel
-        instance.port_type = IoPortType(pb_data.port_type)
-        instance.channel_number = pb_data.channel_number
-        instance.label = pb_data.label
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'GetIoPortLabelRequest':
+        return GetIoPortLabelRequest(
+            interface_id=data.get('interfaceId'),  # type: ignore
+            device=data.get('device'),  # type: ignore
+            port_type=IoPortType(data.get('portType')),  # type: ignore
+            channel_number=data.get('channelNumber'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/lockstep.py` & `zaber_motion-6.0.0/zaber_motion/ascii/lockstep.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
-from ..protobufs import main_pb2
-from ..units import Units, units_from_literals, LengthUnits, VelocityUnits, AccelerationUnits
+from ..dto import requests as dto
+from ..units import Units, LengthUnits, VelocityUnits, AccelerationUnits
 from ..call import call, call_async, call_sync
-from .lockstep_axes import LockstepAxes
+from ..dto.ascii.lockstep_axes import LockstepAxes
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class Lockstep:
     """
@@ -41,128 +41,136 @@
     ) -> None:
         """
         Activate the lockstep group on the axes specified.
 
         Args:
             axes: The numbers of axes in the lockstep group.
         """
-        request = main_pb2.LockstepEnableRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.axes.extend(axes)
+        request = dto.LockstepEnableRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            axes=list(axes),
+        )
         call("device/lockstep_enable", request)
 
     async def enable_async(
             self,
             *axes: int
     ) -> None:
         """
         Activate the lockstep group on the axes specified.
 
         Args:
             axes: The numbers of axes in the lockstep group.
         """
-        request = main_pb2.LockstepEnableRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.axes.extend(axes)
+        request = dto.LockstepEnableRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            axes=list(axes),
+        )
         await call_async("device/lockstep_enable", request)
 
     def disable(
             self
     ) -> None:
         """
         Disable the lockstep group.
         """
-        request = main_pb2.LockstepDisableRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
+        request = dto.LockstepDisableRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
         call("device/lockstep_disable", request)
 
     async def disable_async(
             self
     ) -> None:
         """
         Disable the lockstep group.
         """
-        request = main_pb2.LockstepDisableRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
+        request = dto.LockstepDisableRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
         await call_async("device/lockstep_disable", request)
 
     def stop(
             self,
             wait_until_idle: bool = True
     ) -> None:
         """
         Stops ongoing lockstep group movement. Decelerates until zero speed.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
         """
-        request = main_pb2.LockstepStopRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.wait_until_idle = wait_until_idle
+        request = dto.LockstepStopRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            wait_until_idle=wait_until_idle,
+        )
         call("device/lockstep_stop", request)
 
     async def stop_async(
             self,
             wait_until_idle: bool = True
     ) -> None:
         """
         Stops ongoing lockstep group movement. Decelerates until zero speed.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
         """
-        request = main_pb2.LockstepStopRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.wait_until_idle = wait_until_idle
+        request = dto.LockstepStopRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            wait_until_idle=wait_until_idle,
+        )
         await call_async("device/lockstep_stop", request)
 
     def home(
             self,
             wait_until_idle: bool = True
     ) -> None:
         """
         Retracts the axes of the lockstep group until a home associated with an individual axis is detected.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
         """
-        request = main_pb2.LockstepHomeRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.wait_until_idle = wait_until_idle
+        request = dto.LockstepHomeRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            wait_until_idle=wait_until_idle,
+        )
         call("device/lockstep_home", request)
 
     async def home_async(
             self,
             wait_until_idle: bool = True
     ) -> None:
         """
         Retracts the axes of the lockstep group until a home associated with an individual axis is detected.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
         """
-        request = main_pb2.LockstepHomeRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.wait_until_idle = wait_until_idle
+        request = dto.LockstepHomeRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            wait_until_idle=wait_until_idle,
+        )
         await call_async("device/lockstep_home", request)
 
     def move_absolute(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
@@ -184,26 +192,27 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.ABS
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.ABS,
+            arg=position,
+            unit=unit,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/lockstep_move", request)
 
     async def move_absolute_async(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
@@ -225,26 +234,27 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.ABS
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.ABS,
+            arg=position,
+            unit=unit,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/lockstep_move", request)
 
     def move_relative(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
@@ -266,26 +276,27 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.REL
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.REL,
+            arg=position,
+            unit=unit,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/lockstep_move", request)
 
     async def move_relative_async(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
@@ -307,26 +318,27 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.REL
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.REL,
+            arg=position,
+            unit=unit,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/lockstep_move", request)
 
     def move_velocity(
             self,
             velocity: float,
             unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
@@ -340,23 +352,24 @@
             velocity: Movement velocity.
             unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.VEL
-        request.arg = velocity
-        request.unit = units_from_literals(unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.VEL,
+            arg=velocity,
+            unit=unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/lockstep_move", request)
 
     async def move_velocity_async(
             self,
             velocity: float,
             unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
@@ -370,23 +383,24 @@
             velocity: Movement velocity.
             unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.VEL
-        request.arg = velocity
-        request.unit = units_from_literals(unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.VEL,
+            arg=velocity,
+            unit=unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/lockstep_move", request)
 
     def move_max(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
             velocity_unit: VelocityUnits = Units.NATIVE,
@@ -405,24 +419,25 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.MAX
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.MAX,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/lockstep_move", request)
 
     async def move_max_async(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
             velocity_unit: VelocityUnits = Units.NATIVE,
@@ -441,24 +456,25 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.MAX
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.MAX,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/lockstep_move", request)
 
     def move_min(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
             velocity_unit: VelocityUnits = Units.NATIVE,
@@ -477,24 +493,25 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.MIN
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.MIN,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         call("device/lockstep_move", request)
 
     async def move_min_async(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
             velocity_unit: VelocityUnits = Units.NATIVE,
@@ -513,165 +530,186 @@
                 Requires at least Firmware 7.25.
             velocity_unit: Units of velocity.
             acceleration: Movement acceleration.
                 Default value of 0 indicates that the accel setting is used instead.
                 Requires at least Firmware 7.25.
             acceleration_unit: Units of acceleration.
         """
-        request = main_pb2.LockstepMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.type = main_pb2.LockstepMoveRequest.MIN
-        request.wait_until_idle = wait_until_idle
-        request.velocity = velocity
-        request.velocity_unit = units_from_literals(velocity_unit).value
-        request.acceleration = acceleration
-        request.acceleration_unit = units_from_literals(acceleration_unit).value
+        request = dto.LockstepMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            type=dto.AxisMoveType.MIN,
+            wait_until_idle=wait_until_idle,
+            velocity=velocity,
+            velocity_unit=velocity_unit,
+            acceleration=acceleration,
+            acceleration_unit=acceleration_unit,
+        )
         await call_async("device/lockstep_move", request)
 
     def wait_until_idle(
             self,
             throw_error_on_fault: bool = True
     ) -> None:
         """
         Waits until the lockstep group stops moving.
 
         Args:
             throw_error_on_fault: Determines whether to throw error when fault is observed.
         """
-        request = main_pb2.LockstepWaitUntilIdleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.throw_error_on_fault = throw_error_on_fault
+        request = dto.LockstepWaitUntilIdleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            throw_error_on_fault=throw_error_on_fault,
+        )
         call("device/lockstep_wait_until_idle", request)
 
     async def wait_until_idle_async(
             self,
             throw_error_on_fault: bool = True
     ) -> None:
         """
         Waits until the lockstep group stops moving.
 
         Args:
             throw_error_on_fault: Determines whether to throw error when fault is observed.
         """
-        request = main_pb2.LockstepWaitUntilIdleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.throw_error_on_fault = throw_error_on_fault
+        request = dto.LockstepWaitUntilIdleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            throw_error_on_fault=throw_error_on_fault,
+        )
         await call_async("device/lockstep_wait_until_idle", request)
 
     def is_busy(
             self
     ) -> bool:
         """
         Returns bool indicating whether the lockstep group is executing a motion command.
 
         Returns:
             True if the axes are currently executing a motion command.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.BoolResponse()
-        call("device/lockstep_is_busy", request, response)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = call(
+            "device/lockstep_is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_busy_async(
             self
     ) -> bool:
         """
         Returns bool indicating whether the lockstep group is executing a motion command.
 
         Returns:
             True if the axes are currently executing a motion command.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.BoolResponse()
-        await call_async("device/lockstep_is_busy", request, response)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = await call_async(
+            "device/lockstep_is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def get_axes(
             self
     ) -> LockstepAxes:
         """
         Deprecated: Use GetAxisNumbers instead.
 
         Gets the axes of the lockstep group.
 
         Returns:
             LockstepAxes instance which contains the axes numbers of the lockstep group.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.LockstepAxes()
-        call("device/lockstep_get_axes", request, response)
-        return LockstepAxes.from_protobuf(response)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = call(
+            "device/lockstep_get_axes",
+            request,
+            LockstepAxes.from_binary)
+        return response
 
     async def get_axes_async(
             self
     ) -> LockstepAxes:
         """
         Deprecated: Use GetAxisNumbers instead.
 
         Gets the axes of the lockstep group.
 
         Returns:
             LockstepAxes instance which contains the axes numbers of the lockstep group.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.LockstepAxes()
-        await call_async("device/lockstep_get_axes", request, response)
-        return LockstepAxes.from_protobuf(response)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = await call_async(
+            "device/lockstep_get_axes",
+            request,
+            LockstepAxes.from_binary)
+        return response
 
     def get_axis_numbers(
             self
     ) -> List[int]:
         """
         Gets the axis numbers of the lockstep group.
 
         Returns:
             Axis numbers in order specified when enabling lockstep.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.LockstepGetAxisNumbersResponse()
-        call("device/lockstep_get_axis_numbers", request, response)
-        return list(response.axes)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = call(
+            "device/lockstep_get_axis_numbers",
+            request,
+            dto.LockstepGetAxisNumbersResponse.from_binary)
+        return response.axes
 
     async def get_axis_numbers_async(
             self
     ) -> List[int]:
         """
         Gets the axis numbers of the lockstep group.
 
         Returns:
             Axis numbers in order specified when enabling lockstep.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.LockstepGetAxisNumbersResponse()
-        await call_async("device/lockstep_get_axis_numbers", request, response)
-        return list(response.axes)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = await call_async(
+            "device/lockstep_get_axis_numbers",
+            request,
+            dto.LockstepGetAxisNumbersResponse.from_binary)
+        return response.axes
 
     def get_offsets(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> List[float]:
         """
         Gets the initial offsets of secondary axes of an enabled lockstep group.
@@ -679,22 +717,25 @@
         Args:
             unit: Units of position.
                 Uses primary axis unit conversion.
 
         Returns:
             Initial offset for each axis of the lockstep group.
         """
-        request = main_pb2.LockstepGetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleArrayResponse()
-        call("device/lockstep_get_offsets", request, response)
-        return list(response.values)
+        request = dto.LockstepGetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            unit=unit,
+        )
+        response = call(
+            "device/lockstep_get_offsets",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     async def get_offsets_async(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> List[float]:
         """
         Gets the initial offsets of secondary axes of an enabled lockstep group.
@@ -702,22 +743,25 @@
         Args:
             unit: Units of position.
                 Uses primary axis unit conversion.
 
         Returns:
             Initial offset for each axis of the lockstep group.
         """
-        request = main_pb2.LockstepGetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleArrayResponse()
-        await call_async("device/lockstep_get_offsets", request, response)
-        return list(response.values)
+        request = dto.LockstepGetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            unit=unit,
+        )
+        response = await call_async(
+            "device/lockstep_get_offsets",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     def get_twists(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> List[float]:
         """
         Gets the twists of secondary axes of an enabled lockstep group.
@@ -725,22 +769,25 @@
         Args:
             unit: Units of position.
                 Uses primary axis unit conversion.
 
         Returns:
             Difference between the initial offset and the actual offset for each axis of the lockstep group.
         """
-        request = main_pb2.LockstepGetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleArrayResponse()
-        call("device/lockstep_get_twists", request, response)
-        return list(response.values)
+        request = dto.LockstepGetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            unit=unit,
+        )
+        response = call(
+            "device/lockstep_get_twists",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     async def get_twists_async(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> List[float]:
         """
         Gets the twists of secondary axes of an enabled lockstep group.
@@ -748,43 +795,49 @@
         Args:
             unit: Units of position.
                 Uses primary axis unit conversion.
 
         Returns:
             Difference between the initial offset and the actual offset for each axis of the lockstep group.
         """
-        request = main_pb2.LockstepGetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleArrayResponse()
-        await call_async("device/lockstep_get_twists", request, response)
-        return list(response.values)
+        request = dto.LockstepGetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            unit=unit,
+        )
+        response = await call_async(
+            "device/lockstep_get_twists",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     def get_position(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
         Returns current position of the primary axis.
 
         Args:
             unit: Units of the position.
 
         Returns:
             Primary axis position.
         """
-        request = main_pb2.LockstepGetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("device/lockstep_get_pos", request, response)
+        request = dto.LockstepGetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            unit=unit,
+        )
+        response = call(
+            "device/lockstep_get_pos",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_position_async(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
@@ -792,21 +845,24 @@
 
         Args:
             unit: Units of the position.
 
         Returns:
             Primary axis position.
         """
-        request = main_pb2.LockstepGetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("device/lockstep_get_pos", request, response)
+        request = dto.LockstepGetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            unit=unit,
+        )
+        response = await call_async(
+            "device/lockstep_get_pos",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set_tolerance(
             self,
             tolerance: float,
             unit: LengthUnits = Units.NATIVE,
             axis_index: int = 0
@@ -819,21 +875,22 @@
             tolerance: Twist tolerance.
             unit: Units of the tolerance.
                 Uses primary axis unit conversion when setting to all axes,
                 otherwise uses specified secondary axis unit conversion.
             axis_index: Optional index of a secondary axis to set the tolerance for.
                 If left empty or set to 0, the tolerance is set to all the secondary axes.
         """
-        request = main_pb2.LockstepSetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.value = tolerance
-        request.unit = units_from_literals(unit).value
-        request.axis_index = axis_index
+        request = dto.LockstepSetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            value=tolerance,
+            unit=unit,
+            axis_index=axis_index,
+        )
         call("device/lockstep_set_tolerance", request)
 
     async def set_tolerance_async(
             self,
             tolerance: float,
             unit: LengthUnits = Units.NATIVE,
             axis_index: int = 0
@@ -846,66 +903,76 @@
             tolerance: Twist tolerance.
             unit: Units of the tolerance.
                 Uses primary axis unit conversion when setting to all axes,
                 otherwise uses specified secondary axis unit conversion.
             axis_index: Optional index of a secondary axis to set the tolerance for.
                 If left empty or set to 0, the tolerance is set to all the secondary axes.
         """
-        request = main_pb2.LockstepSetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        request.value = tolerance
-        request.unit = units_from_literals(unit).value
-        request.axis_index = axis_index
+        request = dto.LockstepSetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+            value=tolerance,
+            unit=unit,
+            axis_index=axis_index,
+        )
         await call_async("device/lockstep_set_tolerance", request)
 
     def is_enabled(
             self
     ) -> bool:
         """
         Checks if the lockstep group is currently enabled on the device.
 
         Returns:
             True if a lockstep group with this ID is enabled on the device.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.BoolResponse()
-        call("device/lockstep_is_enabled", request, response)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = call(
+            "device/lockstep_is_enabled",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_enabled_async(
             self
     ) -> bool:
         """
         Checks if the lockstep group is currently enabled on the device.
 
         Returns:
             True if a lockstep group with this ID is enabled on the device.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.BoolResponse()
-        await call_async("device/lockstep_is_enabled", request, response)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = await call_async(
+            "device/lockstep_is_enabled",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string which represents the enabled lockstep group.
 
         Returns:
             String which represents the enabled lockstep group.
         """
-        request = main_pb2.LockstepEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.lockstep_group_id = self.lockstep_group_id
-        response = main_pb2.StringResponse()
-        call_sync("device/lockstep_to_string", request, response)
+        request = dto.LockstepEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            lockstep_group_id=self.lockstep_group_id,
+        )
+        response = call_sync(
+            "device/lockstep_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-6.0.0/zaber_motion/ascii/oscilloscope_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import List
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from ..call import call_sync
-from ..units import UnitsAndLiterals, Units, units_from_literals, TimeUnits, FrequencyUnits
-from .io_port_type import IoPortType
-from .oscilloscope_data_source import OscilloscopeDataSource
-from .oscilloscope_capture_properties import OscilloscopeCaptureProperties
+from ..units import UnitsAndLiterals, Units, TimeUnits, FrequencyUnits
+from ..dto.ascii.io_port_type import IoPortType
+from ..dto.ascii.oscilloscope_data_source import OscilloscopeDataSource
+from ..dto.ascii.oscilloscope_capture_properties import OscilloscopeCaptureProperties
 
 
 class OscilloscopeData:
     """
     Contains a block of contiguous recorded data for one channel of the device's oscilloscope.
     """
 
@@ -68,19 +68,22 @@
 
         Args:
             unit: Unit of measure to represent the timebase in.
 
         Returns:
             The timebase setting at the time the data was recorded.
         """
-        request = main_pb2.OscilloscopeDataGetRequest()
-        request.data_id = self.data_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("oscilloscopedata/get_timebase", request, response)
+        request = dto.OscilloscopeDataGetRequest(
+            data_id=self.data_id,
+            unit=unit,
+        )
+        response = call_sync(
+            "oscilloscopedata/get_timebase",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_frequency(
             self,
             unit: FrequencyUnits = Units.NATIVE
     ) -> float:
         """
@@ -88,19 +91,22 @@
 
         Args:
             unit: Unit of measure to represent the frequency in.
 
         Returns:
             The frequency (inverse of the timebase setting) at the time the data was recorded.
         """
-        request = main_pb2.OscilloscopeDataGetRequest()
-        request.data_id = self.data_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("oscilloscopedata/get_frequency", request, response)
+        request = dto.OscilloscopeDataGetRequest(
+            data_id=self.data_id,
+            unit=unit,
+        )
+        response = call_sync(
+            "oscilloscopedata/get_frequency",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_delay(
             self,
             unit: TimeUnits = Units.NATIVE
     ) -> float:
         """
@@ -109,19 +115,22 @@
 
         Args:
             unit: Unit of measure to represent the delay in.
 
         Returns:
             The delay setting at the time the data was recorded.
         """
-        request = main_pb2.OscilloscopeDataGetRequest()
-        request.data_id = self.data_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("oscilloscopedata/get_delay", request, response)
+        request = dto.OscilloscopeDataGetRequest(
+            data_id=self.data_id,
+            unit=unit,
+        )
+        response = call_sync(
+            "oscilloscopedata/get_delay",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_sample_time(
             self,
             index: int,
             unit: TimeUnits = Units.NATIVE
     ) -> float:
@@ -131,20 +140,23 @@
         Args:
             index: 0-based index of the sample to calculate the time of.
             unit: Unit of measure to represent the calculated time in.
 
         Returns:
             The calculated time offset of the data sample at the given index.
         """
-        request = main_pb2.OscilloscopeDataGetSampleTimeRequest()
-        request.data_id = self.data_id
-        request.index = index
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("oscilloscopedata/get_sample_time", request, response)
+        request = dto.OscilloscopeDataGetSampleTimeRequest(
+            data_id=self.data_id,
+            index=index,
+            unit=unit,
+        )
+        response = call_sync(
+            "oscilloscopedata/get_sample_time",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def get_sample_times(
             self,
             unit: TimeUnits = Units.NATIVE
     ) -> List[float]:
         """
@@ -152,65 +164,75 @@
 
         Args:
             unit: Unit of measure to represent the calculated time in.
 
         Returns:
             The calculated time offsets of all data samples.
         """
-        request = main_pb2.OscilloscopeDataGetSampleTimeRequest()
-        request.data_id = self.data_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleArrayResponse()
-        call_sync("oscilloscopedata/get_sample_times", request, response)
-        return list(response.values)
+        request = dto.OscilloscopeDataGetSampleTimeRequest(
+            data_id=self.data_id,
+            unit=unit,
+        )
+        response = call_sync(
+            "oscilloscopedata/get_sample_times",
+            request,
+            dto.DoubleArrayResponse.from_binary)
+        return response.values
 
     def get_data(
             self,
             unit: UnitsAndLiterals = Units.NATIVE
     ) -> List[float]:
         """
         Get the recorded data as an array of doubles.
 
         Args:
             unit: Unit of measure to convert the data to.
 
         Returns:
             The recorded data for one oscilloscope channel, converted to the units specified.
         """
-        request = main_pb2.OscilloscopeDataGetRequest()
-        request.data_id = self.data_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.OscilloscopeDataGetSamplesResponse()
-        call_sync("oscilloscopedata/get_samples", request, response)
-        return list(response.data)
+        request = dto.OscilloscopeDataGetRequest(
+            data_id=self.data_id,
+            unit=unit,
+        )
+        response = call_sync(
+            "oscilloscopedata/get_samples",
+            request,
+            dto.OscilloscopeDataGetSamplesResponse.from_binary)
+        return response.data
 
     @staticmethod
     def __free(
             data_id: int
     ) -> None:
         """
         Releases native resources of an oscilloscope data buffer.
 
         Args:
             data_id: The ID of the data buffer to delete.
         """
-        request = main_pb2.OscilloscopeDataIdentifier()
-        request.data_id = data_id
+        request = dto.OscilloscopeDataIdentifier(
+            data_id=data_id,
+        )
         call_sync("oscilloscopedata/free", request)
 
     def __retrieve_properties(
             self
     ) -> OscilloscopeCaptureProperties:
         """
         Returns recording properties.
 
         Returns:
             Capture properties.
         """
-        request = main_pb2.OscilloscopeDataIdentifier()
-        request.data_id = self.data_id
-        response = main_pb2.OscilloscopeCaptureProperties()
-        call_sync("oscilloscopedata/get_properties", request, response)
-        return OscilloscopeCaptureProperties.from_protobuf(response)
+        request = dto.OscilloscopeDataIdentifier(
+            data_id=self.data_id,
+        )
+        response = call_sync(
+            "oscilloscopedata/get_properties",
+            request,
+            OscilloscopeCaptureProperties.from_binary)
+        return response
 
     def __del__(self) -> None:
         OscilloscopeData.__free(self.data_id)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/paramset_info.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/paramset_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,61 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from typing import List  # pylint: disable=unused-import
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 from .servo_tuning_param import ServoTuningParam
 
 
+@dataclass
 class ParamsetInfo:
     """
     The raw parameters currently saved to a given paramset.
     """
 
-    @property
-    def type(self) -> str:
-        """
-        The tuning algorithm used for this axis.
-        """
-
-        return self._type
-
-    @type.setter
-    def type(self, value: str) -> None:
-        self._type = value
-
-    @property
-    def version(self) -> int:
-        """
-        The version of the tuning algorithm used for this axis.
-        """
-
-        return self._version
-
-    @version.setter
-    def version(self, value: int) -> None:
-        self._version = value
-
-    @property
-    def params(self) -> List[ServoTuningParam]:
-        """
-        The raw tuning parameters of this device.
-        """
-
-        return self._params
-
-    @params.setter
-    def params(self, value: List[ServoTuningParam]) -> None:
-        self._params = value
+    type: str
+    """
+    The tuning algorithm used for this axis.
+    """
+
+    version: int
+    """
+    The version of the tuning algorithm used for this axis.
+    """
+
+    params: List[ServoTuningParam]
+    """
+    The raw tuning parameters of this device.
+    """
+
+    @staticmethod
+    def zero_values() -> 'ParamsetInfo':
+        return ParamsetInfo(
+            type="",
+            version=0,
+            params=[],
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'ParamsetInfo':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return ParamsetInfo.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'type': self.type,
+            'version': self.version,
+            'params': [item.to_dict() for item in self.params],
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.ParamsetInfo
-    ) -> 'ParamsetInfo':
-        instance = ParamsetInfo.__new__(
-            ParamsetInfo
-        )  # type: ParamsetInfo
-        instance.type = pb_data.type
-        instance.version = pb_data.version
-        instance.params = [ServoTuningParam.from_protobuf(item) for item in pb_data.params]
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'ParamsetInfo':
+        return ParamsetInfo(
+            type=data.get('type'),  # type: ignore
+            version=data.get('version'),  # type: ignore
+            params=[ServoTuningParam.from_dict(item) for item in data.get('params')],  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/pvt.py` & `zaber_motion-6.0.0/zaber_motion/ascii/pvt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
 
 from ..call import call, call_async
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 
 from .pvt_sequence import PvtSequence
 from .pvt_buffer import PvtBuffer
 
 if TYPE_CHECKING:
     from .device import Device
 
@@ -69,31 +69,37 @@
     ) -> List[int]:
         """
         Get a list of buffer IDs that are currently in use.
 
         Returns:
             List of buffer IDs.
         """
-        request = main_pb2.StreamBufferList()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.pvt = True
-        response = main_pb2.IntArrayResponse()
-        call("device/stream_buffer_list", request, response)
-        return list(response.values)
+        request = dto.StreamBufferList(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            pvt=True,
+        )
+        response = call(
+            "device/stream_buffer_list",
+            request,
+            dto.IntArrayResponse.from_binary)
+        return response.values
 
     async def list_buffer_ids_async(
             self
     ) -> List[int]:
         """
         Get a list of buffer IDs that are currently in use.
 
         Returns:
             List of buffer IDs.
         """
-        request = main_pb2.StreamBufferList()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.pvt = True
-        response = main_pb2.IntArrayResponse()
-        await call_async("device/stream_buffer_list", request, response)
-        return list(response.values)
+        request = dto.StreamBufferList(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            pvt=True,
+        )
+        response = await call_async(
+            "device/stream_buffer_list",
+            request,
+            dto.IntArrayResponse.from_binary)
+        return response.values
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/pvt_axis_definition.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/pvt_axis_definition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,53 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from typing import Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 from .pvt_axis_type import PvtAxisType
 
 
+@dataclass
 class PvtAxisDefinition:
     """
     Defines an axis of the PVT sequence.
     """
 
-    def __init__(
-            self: 'PvtAxisDefinition',
-            axis_number: int,
-            axis_type: Optional[PvtAxisType] = None
-    ) -> None:
-        self._axis_number = axis_number
-        self._axis_type = axis_type
-
-    @property
-    def axis_number(self) -> int:
-        """
-        Number of a physical axis or a lockstep group.
-        """
-
-        return self._axis_number
-
-    @axis_number.setter
-    def axis_number(self, value: int) -> None:
-        self._axis_number = value
-
-    @property
-    def axis_type(self) -> Optional[PvtAxisType]:
-        """
-        Defines the type of the axis.
-        """
-
-        return self._axis_type
-
-    @axis_type.setter
-    def axis_type(self, value: Optional[PvtAxisType]) -> None:
-        self._axis_type = value
+    axis_number: int
+    """
+    Number of a physical axis or a lockstep group.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    axis_type: Optional[PvtAxisType] = None
+    """
+    Defines the type of the axis.
+    """
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.StreamAxisDefinition
-    ) -> 'PvtAxisDefinition':
-        instance = PvtAxisDefinition.__new__(
-            PvtAxisDefinition
-        )  # type: PvtAxisDefinition
-        instance.axis_number = pb_data.axis_number
-        instance.axis_type = PvtAxisType(pb_data.axis_type)
-        return instance
+    def zero_values() -> 'PvtAxisDefinition':
+        return PvtAxisDefinition(
+            axis_number=0,
+            axis_type=None,
+        )
 
     @staticmethod
-    def to_protobuf(source: 'Optional[PvtAxisDefinition]') -> main_pb2.StreamAxisDefinition:
-        pb_data = main_pb2.StreamAxisDefinition()
-
-        if source is None:
-            return pb_data
+    def from_binary(data_bytes: bytes) -> 'PvtAxisDefinition':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return PvtAxisDefinition.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'axisNumber': self.axis_number,
+            'axisType': self.axis_type.value if self.axis_type is not None else None,
+        }
 
-        if not isinstance(source, PvtAxisDefinition):
-            raise TypeError("Provided value is not PvtAxisDefinition.")
-
-        pb_data.axis_number = source.axis_number
-        pb_data.axis_type = source.axis_type.value if source.axis_type is not None else 0
-        return pb_data
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> 'PvtAxisDefinition':
+        return PvtAxisDefinition(
+            axis_number=data.get('axisNumber'),  # type: ignore
+            axis_type=PvtAxisType(data.get('axisType')) if data.get('axisType') is not None else None,  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/pvt_buffer.py` & `zaber_motion-6.0.0/zaber_motion/ascii/pvt_buffer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from ..call import call, call_async
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class PvtBuffer:
@@ -37,61 +37,69 @@
     ) -> List[str]:
         """
         Gets the buffer contents as an array of strings.
 
         Returns:
             A string array containing all the PVT commands stored in the buffer.
         """
-        request = main_pb2.StreamBufferGetContentRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.buffer_id = self.buffer_id
-        request.pvt = True
-        response = main_pb2.StreamBufferGetContentResponse()
-        call("device/stream_buffer_get_content", request, response)
-        return list(response.buffer_lines)
+        request = dto.StreamBufferGetContentRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            buffer_id=self.buffer_id,
+            pvt=True,
+        )
+        response = call(
+            "device/stream_buffer_get_content",
+            request,
+            dto.StreamBufferGetContentResponse.from_binary)
+        return response.buffer_lines
 
     async def get_content_async(
             self
     ) -> List[str]:
         """
         Gets the buffer contents as an array of strings.
 
         Returns:
             A string array containing all the PVT commands stored in the buffer.
         """
-        request = main_pb2.StreamBufferGetContentRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.buffer_id = self.buffer_id
-        request.pvt = True
-        response = main_pb2.StreamBufferGetContentResponse()
-        await call_async("device/stream_buffer_get_content", request, response)
-        return list(response.buffer_lines)
+        request = dto.StreamBufferGetContentRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            buffer_id=self.buffer_id,
+            pvt=True,
+        )
+        response = await call_async(
+            "device/stream_buffer_get_content",
+            request,
+            dto.StreamBufferGetContentResponse.from_binary)
+        return response.buffer_lines
 
     def erase(
             self
     ) -> None:
         """
         Erases the contents of the buffer.
         This method fails if there is a PVT sequence writing to the buffer.
         """
-        request = main_pb2.StreamBufferEraseRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.buffer_id = self.buffer_id
-        request.pvt = True
+        request = dto.StreamBufferEraseRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            buffer_id=self.buffer_id,
+            pvt=True,
+        )
         call("device/stream_buffer_erase", request)
 
     async def erase_async(
             self
     ) -> None:
         """
         Erases the contents of the buffer.
         This method fails if there is a PVT sequence writing to the buffer.
         """
-        request = main_pb2.StreamBufferEraseRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.buffer_id = self.buffer_id
-        request.pvt = True
+        request = dto.StreamBufferEraseRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            buffer_id=self.buffer_id,
+            pvt=True,
+        )
         await call_async("device/stream_buffer_erase", request)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-6.0.0/zaber_motion/ascii/servo_tuner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
-from typing import List
-from ..protobufs import main_pb2
+from typing import List, Optional
+from ..dto import requests as dto
 from ..call import call, call_async
 from .axis import Axis
-from .servo_tuning_paramset import ServoTuningParamset
-from .paramset_info import ParamsetInfo
-from .servo_tuning_param import ServoTuningParam
-from .simple_tuning import SimpleTuning
-from .simple_tuning_param_definition import SimpleTuningParamDefinition
-from .pid_tuning import PidTuning
+from ..dto.ascii.servo_tuning_paramset import ServoTuningParamset
+from ..dto.ascii.paramset_info import ParamsetInfo
+from ..dto.ascii.servo_tuning_param import ServoTuningParam
+from ..dto.ascii.simple_tuning import SimpleTuning
+from ..dto.ascii.simple_tuning_param_definition import SimpleTuningParamDefinition
+from ..dto.ascii.pid_tuning import PidTuning
 
 
 class ServoTuner:
     """
     Exposes the capabilities to inspect and edit an axis' servo tuning.
     Requires at least Firmware 6.25 or 7.00.
     """
@@ -36,111 +36,121 @@
     ) -> ServoTuningParamset:
         """
         Get the paramset that this device uses by default when it starts up.
 
         Returns:
             The paramset used when the device restarts.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        response = main_pb2.IntResponse()
-        call("servotuning/get_startup_set", request, response)
-        return ServoTuningParamset(response.value)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+        )
+        response = call(
+            "servotuning/get_startup_set",
+            request,
+            dto.ServoTuningParamsetResponse.from_binary)
+        return response.paramset
 
     async def get_startup_paramset_async(
             self
     ) -> ServoTuningParamset:
         """
         Get the paramset that this device uses by default when it starts up.
 
         Returns:
             The paramset used when the device restarts.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        response = main_pb2.IntResponse()
-        await call_async("servotuning/get_startup_set", request, response)
-        return ServoTuningParamset(response.value)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+        )
+        response = await call_async(
+            "servotuning/get_startup_set",
+            request,
+            dto.ServoTuningParamsetResponse.from_binary)
+        return response.paramset
 
     def set_startup_paramset(
             self,
             paramset: ServoTuningParamset
     ) -> None:
         """
         Set the paramset that this device uses by default when it starts up.
 
         Args:
             paramset: The paramset to use at startup.
         """
-        request = main_pb2.ServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
+        request = dto.ServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+        )
         call("servotuning/set_startup_set", request)
 
     async def set_startup_paramset_async(
             self,
             paramset: ServoTuningParamset
     ) -> None:
         """
         Set the paramset that this device uses by default when it starts up.
 
         Args:
             paramset: The paramset to use at startup.
         """
-        request = main_pb2.ServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
+        request = dto.ServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+        )
         await call_async("servotuning/set_startup_set", request)
 
     def load_paramset(
             self,
             to_paramset: ServoTuningParamset,
             from_paramset: ServoTuningParamset
     ) -> None:
         """
         Load the values from one paramset into another.
 
         Args:
             to_paramset: The paramset to load into.
             from_paramset: The paramset to load from.
         """
-        request = main_pb2.LoadParamset()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.to_paramset = to_paramset.value
-        request.from_paramset = from_paramset.value
+        request = dto.LoadParamset(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            to_paramset=to_paramset,
+            from_paramset=from_paramset,
+        )
         call("servotuning/load_paramset", request)
 
     async def load_paramset_async(
             self,
             to_paramset: ServoTuningParamset,
             from_paramset: ServoTuningParamset
     ) -> None:
         """
         Load the values from one paramset into another.
 
         Args:
             to_paramset: The paramset to load into.
             from_paramset: The paramset to load from.
         """
-        request = main_pb2.LoadParamset()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.to_paramset = to_paramset.value
-        request.from_paramset = from_paramset.value
+        request = dto.LoadParamset(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            to_paramset=to_paramset,
+            from_paramset=from_paramset,
+        )
         await call_async("servotuning/load_paramset", request)
 
     def get_tuning(
             self,
             paramset: ServoTuningParamset
     ) -> ParamsetInfo:
         """
@@ -148,64 +158,71 @@
 
         Args:
             paramset: The paramset to get tuning for.
 
         Returns:
             The raw representation of the current tuning.
         """
-        request = main_pb2.ServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        response = main_pb2.ParamsetInfo()
-        call("servotuning/get_raw", request, response)
-        return ParamsetInfo.from_protobuf(response)
+        request = dto.ServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+        )
+        response = call(
+            "servotuning/get_raw",
+            request,
+            ParamsetInfo.from_binary)
+        return response
 
     async def get_tuning_async(
             self,
             paramset: ServoTuningParamset
     ) -> ParamsetInfo:
         """
         Get the full set of tuning parameters used by the firmware driving this axis.
 
         Args:
             paramset: The paramset to get tuning for.
 
         Returns:
             The raw representation of the current tuning.
         """
-        request = main_pb2.ServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        response = main_pb2.ParamsetInfo()
-        await call_async("servotuning/get_raw", request, response)
-        return ParamsetInfo.from_protobuf(response)
+        request = dto.ServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+        )
+        response = await call_async(
+            "servotuning/get_raw",
+            request,
+            ParamsetInfo.from_binary)
+        return response
 
     def set_tuning(
             self,
             paramset: ServoTuningParamset,
             tuning_params: List[ServoTuningParam]
     ) -> None:
         """
         Set individual tuning parameters.
         Only use this method if you have a strong understanding of Zaber specific tuning parameters.
 
         Args:
             paramset: The paramset to set tuning of.
             tuning_params: The params to set.
         """
-        request = main_pb2.SetServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        request.tuning_params.extend([ServoTuningParam.to_protobuf(a) for a in tuning_params])
+        request = dto.SetServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+            tuning_params=tuning_params,
+        )
         call("servotuning/set_raw", request)
 
     async def set_tuning_async(
             self,
             paramset: ServoTuningParamset,
             tuning_params: List[ServoTuningParam]
     ) -> None:
@@ -213,20 +230,21 @@
         Set individual tuning parameters.
         Only use this method if you have a strong understanding of Zaber specific tuning parameters.
 
         Args:
             paramset: The paramset to set tuning of.
             tuning_params: The params to set.
         """
-        request = main_pb2.SetServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        request.tuning_params.extend([ServoTuningParam.to_protobuf(a) for a in tuning_params])
+        request = dto.SetServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+            tuning_params=tuning_params,
+        )
         await call_async("servotuning/set_raw", request)
 
     def set_pid_tuning(
             self,
             paramset: ServoTuningParamset,
             p: float,
             i: float,
@@ -242,26 +260,29 @@
             i: The integral gain. Must be in units of N/m⋅s.
             d: The derivative gain. Must be in units of N⋅s/m.
             fc: The cutoff frequency. Must be in units of Hz.
 
         Returns:
             The PID representation of the current tuning after your changes have been applied.
         """
-        request = main_pb2.SetServoTuningPIDRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        request.p = p
-        request.i = i
-        request.d = d
-        request.fc = fc
-        response = main_pb2.PidTuning()
-        call("servotuning/set_pid", request, response)
-        return PidTuning.from_protobuf(response)
+        request = dto.SetServoTuningPIDRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+            p=p,
+            i=i,
+            d=d,
+            fc=fc,
+        )
+        response = call(
+            "servotuning/set_pid",
+            request,
+            PidTuning.from_binary)
+        return response
 
     async def set_pid_tuning_async(
             self,
             paramset: ServoTuningParamset,
             p: float,
             i: float,
             d: float,
@@ -276,159 +297,176 @@
             i: The integral gain. Must be in units of N/m⋅s.
             d: The derivative gain. Must be in units of N⋅s/m.
             fc: The cutoff frequency. Must be in units of Hz.
 
         Returns:
             The PID representation of the current tuning after your changes have been applied.
         """
-        request = main_pb2.SetServoTuningPIDRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        request.p = p
-        request.i = i
-        request.d = d
-        request.fc = fc
-        response = main_pb2.PidTuning()
-        await call_async("servotuning/set_pid", request, response)
-        return PidTuning.from_protobuf(response)
+        request = dto.SetServoTuningPIDRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+            p=p,
+            i=i,
+            d=d,
+            fc=fc,
+        )
+        response = await call_async(
+            "servotuning/set_pid",
+            request,
+            PidTuning.from_binary)
+        return response
 
     def get_pid_tuning(
             self,
             paramset: ServoTuningParamset
     ) -> PidTuning:
         """
         Gets the PID representation of this paramset's servo tuning.
 
         Args:
             paramset: The paramset to get tuning for.
 
         Returns:
             The PID representation of the current tuning.
         """
-        request = main_pb2.ServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        response = main_pb2.PidTuning()
-        call("servotuning/get_pid", request, response)
-        return PidTuning.from_protobuf(response)
+        request = dto.ServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+        )
+        response = call(
+            "servotuning/get_pid",
+            request,
+            PidTuning.from_binary)
+        return response
 
     async def get_pid_tuning_async(
             self,
             paramset: ServoTuningParamset
     ) -> PidTuning:
         """
         Gets the PID representation of this paramset's servo tuning.
 
         Args:
             paramset: The paramset to get tuning for.
 
         Returns:
             The PID representation of the current tuning.
         """
-        request = main_pb2.ServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        response = main_pb2.PidTuning()
-        await call_async("servotuning/get_pid", request, response)
-        return PidTuning.from_protobuf(response)
+        request = dto.ServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+        )
+        response = await call_async(
+            "servotuning/get_pid",
+            request,
+            PidTuning.from_binary)
+        return response
 
     def get_simple_tuning_param_definitions(
             self
     ) -> List[SimpleTuningParamDefinition]:
         """
         Gets the parameters that are required to tune this device.
 
         Returns:
             The tuning parameters.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        response = main_pb2.GetSimpleTuningParamDefinitionResponse()
-        call("servotuning/get_simple_params_definition", request, response)
-        return [SimpleTuningParamDefinition.from_protobuf(a) for a in response.params]
+        request = dto.AxisEmptyRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+        )
+        response = call(
+            "servotuning/get_simple_params_definition",
+            request,
+            dto.GetSimpleTuningParamDefinitionResponse.from_binary)
+        return response.params
 
     async def get_simple_tuning_param_definitions_async(
             self
     ) -> List[SimpleTuningParamDefinition]:
         """
         Gets the parameters that are required to tune this device.
 
         Returns:
             The tuning parameters.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        response = main_pb2.GetSimpleTuningParamDefinitionResponse()
-        await call_async("servotuning/get_simple_params_definition", request, response)
-        return [SimpleTuningParamDefinition.from_protobuf(a) for a in response.params]
+        request = dto.AxisEmptyRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+        )
+        response = await call_async(
+            "servotuning/get_simple_params_definition",
+            request,
+            dto.GetSimpleTuningParamDefinitionResponse.from_binary)
+        return response.params
 
     def set_simple_tuning(
             self,
             paramset: ServoTuningParamset,
             tuning_params: List[ServoTuningParam],
             load_mass: float,
-            carriage_mass: float = -1.0
+            carriage_mass: Optional[float] = None
     ) -> None:
         """
         Set the tuning of this device using the simple input method.
 
         Args:
             paramset: The paramset to set tuning for.
             tuning_params: The params used to tune this device.
                 To get what parameters are expected, call GetSimpleTuningParamList.
                 All values must be between 0 and 1.
             load_mass: The mass loaded on the stage (excluding the mass of the carriage itself) in kg.
             carriage_mass: The mass of the carriage in kg. If this value is not set the default carriage mass is used.
         """
-        request = main_pb2.SetSimpleTuning()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        request.tuning_params.extend([ServoTuningParam.to_protobuf(a) for a in tuning_params])
-        request.load_mass = load_mass
-        request.carriage_mass = carriage_mass
+        request = dto.SetSimpleTuning(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+            tuning_params=tuning_params,
+            load_mass=load_mass,
+            carriage_mass=carriage_mass,
+        )
         call("servotuning/set_simple_tuning", request)
 
     async def set_simple_tuning_async(
             self,
             paramset: ServoTuningParamset,
             tuning_params: List[ServoTuningParam],
             load_mass: float,
-            carriage_mass: float = -1.0
+            carriage_mass: Optional[float] = None
     ) -> None:
         """
         Set the tuning of this device using the simple input method.
 
         Args:
             paramset: The paramset to set tuning for.
             tuning_params: The params used to tune this device.
                 To get what parameters are expected, call GetSimpleTuningParamList.
                 All values must be between 0 and 1.
             load_mass: The mass loaded on the stage (excluding the mass of the carriage itself) in kg.
             carriage_mass: The mass of the carriage in kg. If this value is not set the default carriage mass is used.
         """
-        request = main_pb2.SetSimpleTuning()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        request.tuning_params.extend([ServoTuningParam.to_protobuf(a) for a in tuning_params])
-        request.load_mass = load_mass
-        request.carriage_mass = carriage_mass
+        request = dto.SetSimpleTuning(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+            tuning_params=tuning_params,
+            load_mass=load_mass,
+            carriage_mass=carriage_mass,
+        )
         await call_async("servotuning/set_simple_tuning", request)
 
     def get_simple_tuning(
             self,
             paramset: ServoTuningParamset
     ) -> SimpleTuning:
         """
@@ -436,51 +474,57 @@
 
         Args:
             paramset: The paramset to get tuning for.
 
         Returns:
             The simple tuning parameters.
         """
-        request = main_pb2.ServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        response = main_pb2.SimpleTuning()
-        call("servotuning/get_simple_tuning", request, response)
-        return SimpleTuning.from_protobuf(response)
+        request = dto.ServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+        )
+        response = call(
+            "servotuning/get_simple_tuning",
+            request,
+            SimpleTuning.from_binary)
+        return response
 
     async def get_simple_tuning_async(
             self,
             paramset: ServoTuningParamset
     ) -> SimpleTuning:
         """
         Get the simple tuning parameters for this device.
 
         Args:
             paramset: The paramset to get tuning for.
 
         Returns:
             The simple tuning parameters.
         """
-        request = main_pb2.ServoTuningRequest()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        response = main_pb2.SimpleTuning()
-        await call_async("servotuning/get_simple_tuning", request, response)
-        return SimpleTuning.from_protobuf(response)
+        request = dto.ServoTuningRequest(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+        )
+        response = await call_async(
+            "servotuning/get_simple_tuning",
+            request,
+            SimpleTuning.from_binary)
+        return response
 
     def is_using_simple_tuning(
             self,
             paramset: ServoTuningParamset,
             tuning_params: List[ServoTuningParam],
             load_mass: float,
-            carriage_mass: float = -1.0
+            carriage_mass: Optional[float] = None
     ) -> bool:
         """
         Deprecated: Use GetSimpleTuning instead.
 
         Checks if the provided simple tuning is being stored by this paramset.
 
         Args:
@@ -490,32 +534,35 @@
                 All values must be between 0 and 1.
             load_mass: The mass loaded on the stage (excluding the mass of the carriage itself) in kg.
             carriage_mass: The mass of the carriage in kg. If this value is not set the default carriage mass is used.
 
         Returns:
             True if the provided simple tuning is currently stored in this paramset.
         """
-        request = main_pb2.SetSimpleTuning()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        request.tuning_params.extend([ServoTuningParam.to_protobuf(a) for a in tuning_params])
-        request.load_mass = load_mass
-        request.carriage_mass = carriage_mass
-        response = main_pb2.BoolResponse()
-        call("servotuning/is_using_simple_tuning", request, response)
+        request = dto.SetSimpleTuning(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+            tuning_params=tuning_params,
+            load_mass=load_mass,
+            carriage_mass=carriage_mass,
+        )
+        response = call(
+            "servotuning/is_using_simple_tuning",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_using_simple_tuning_async(
             self,
             paramset: ServoTuningParamset,
             tuning_params: List[ServoTuningParam],
             load_mass: float,
-            carriage_mass: float = -1.0
+            carriage_mass: Optional[float] = None
     ) -> bool:
         """
         Deprecated: Use GetSimpleTuning instead.
 
         Checks if the provided simple tuning is being stored by this paramset.
 
         Args:
@@ -525,18 +572,21 @@
                 All values must be between 0 and 1.
             load_mass: The mass loaded on the stage (excluding the mass of the carriage itself) in kg.
             carriage_mass: The mass of the carriage in kg. If this value is not set the default carriage mass is used.
 
         Returns:
             True if the provided simple tuning is currently stored in this paramset.
         """
-        request = main_pb2.SetSimpleTuning()
-        request.interface_id = self.axis.device.connection.interface_id
-        request.device = self.axis.device.device_address
-        request.axis = self.axis.axis_number
-        request.paramset = paramset.value
-        request.tuning_params.extend([ServoTuningParam.to_protobuf(a) for a in tuning_params])
-        request.load_mass = load_mass
-        request.carriage_mass = carriage_mass
-        response = main_pb2.BoolResponse()
-        await call_async("servotuning/is_using_simple_tuning", request, response)
+        request = dto.SetSimpleTuning(
+            interface_id=self.axis.device.connection.interface_id,
+            device=self.axis.device.device_address,
+            axis=self.axis.axis_number,
+            paramset=paramset,
+            tuning_params=tuning_params,
+            load_mass=load_mass,
+            carriage_mass=carriage_mass,
+        )
+        response = await call_async(
+            "servotuning/is_using_simple_tuning",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/servo_tuning_param.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,52 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from typing import Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
 
+@dataclass
 class ServoTuningParam:
     """
     A parameter used to establish the servo tuning of an axis.
     """
 
-    def __init__(
-            self: 'ServoTuningParam',
-            name: str,
-            value: float
-    ) -> None:
-        self._name = name
-        self._value = value
-
-    @property
-    def name(self) -> str:
-        """
-        The name of the parameter to set.
-        """
-
-        return self._name
-
-    @name.setter
-    def name(self, value: str) -> None:
-        self._name = value
-
-    @property
-    def value(self) -> float:
-        """
-        The value to use for this parameter.
-        """
-
-        return self._value
-
-    @value.setter
-    def value(self, value: float) -> None:
-        self._value = value
+    name: str
+    """
+    The name of the parameter to set.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    value: float
+    """
+    The value to use for this parameter.
+    """
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.ServoTuningParam
-    ) -> 'ServoTuningParam':
-        instance = ServoTuningParam.__new__(
-            ServoTuningParam
-        )  # type: ServoTuningParam
-        instance.name = pb_data.name
-        instance.value = pb_data.value
-        return instance
+    def zero_values() -> 'ServoTuningParam':
+        return ServoTuningParam(
+            name="",
+            value=0,
+        )
 
     @staticmethod
-    def to_protobuf(source: 'Optional[ServoTuningParam]') -> main_pb2.ServoTuningParam:
-        pb_data = main_pb2.ServoTuningParam()
-
-        if source is None:
-            return pb_data
+    def from_binary(data_bytes: bytes) -> 'ServoTuningParam':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return ServoTuningParam.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'name': self.name,
+            'value': self.value,
+        }
 
-        if not isinstance(source, ServoTuningParam):
-            raise TypeError("Provided value is not ServoTuningParam.")
-
-        pb_data.name = source.name
-        pb_data.value = source.value
-        return pb_data
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> 'ServoTuningParam':
+        return ServoTuningParam(
+            name=data.get('name'),  # type: ignore
+            value=data.get('value'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/setting_constants.py` & `zaber_motion-6.0.0/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/simple_tuning.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/simple_tuning_param_definition.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,76 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
-from typing import List, Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
-from .servo_tuning_param import ServoTuningParam
 
-
-class SimpleTuning:
+@dataclass
+class SimpleTuningParamDefinition:
     """
-    The masses and parameters last used by simple tuning.
+    Information about a parameter used for the simple tuning method.
     """
 
-    @property
-    def is_used(self) -> bool:
-        """
-        Whether the tuning returned is currently in use by this paramset,
-        or if it has been overwritten by a later change.
-        """
-
-        return self._is_used
-
-    @is_used.setter
-    def is_used(self, value: bool) -> None:
-        self._is_used = value
-
-    @property
-    def carriage_mass(self) -> Optional[float]:
-        """
-        The mass of the carriage in kg.
-        """
-
-        return self._carriage_mass
-
-    @carriage_mass.setter
-    def carriage_mass(self, value: Optional[float]) -> None:
-        self._carriage_mass = value
-
-    @property
-    def load_mass(self) -> float:
-        """
-        The mass of the load in kg, excluding the mass of the carriage.
-        """
+    name: str
+    """
+    The name of the parameter.
+    """
 
-        return self._load_mass
+    min_label: str
+    """
+    The human readable description of the effect of a lower value on this setting.
+    """
 
-    @load_mass.setter
-    def load_mass(self, value: float) -> None:
-        self._load_mass = value
+    max_label: str
+    """
+    The human readable description of the effect of a higher value on this setting.
+    """
 
-    @property
-    def tuning_params(self) -> List[ServoTuningParam]:
-        """
-        The parameters used by simple tuning.
-        """
+    data_type: str
+    """
+    How this parameter will be parsed by the tuner.
+    """
 
-        return self._tuning_params
+    default_value: Optional[float] = None
+    """
+    The default value of this parameter.
+    """
 
-    @tuning_params.setter
-    def tuning_params(self, value: List[ServoTuningParam]) -> None:
-        self._tuning_params = value
+    @staticmethod
+    def zero_values() -> 'SimpleTuningParamDefinition':
+        return SimpleTuningParamDefinition(
+            name="",
+            min_label="",
+            max_label="",
+            data_type="",
+            default_value=None,
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'SimpleTuningParamDefinition':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return SimpleTuningParamDefinition.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'name': self.name,
+            'minLabel': self.min_label,
+            'maxLabel': self.max_label,
+            'dataType': self.data_type,
+            'defaultValue': self.default_value,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.SimpleTuning
-    ) -> 'SimpleTuning':
-        instance = SimpleTuning.__new__(
-            SimpleTuning
-        )  # type: SimpleTuning
-        instance.is_used = pb_data.is_used
-        instance.carriage_mass = pb_data.carriage_mass if pb_data.has_carriage_mass else None
-        instance.load_mass = pb_data.load_mass
-        instance.tuning_params = [ServoTuningParam.from_protobuf(item) for item in pb_data.tuning_params]
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'SimpleTuningParamDefinition':
+        return SimpleTuningParamDefinition(
+            name=data.get('name'),  # type: ignore
+            min_label=data.get('minLabel'),  # type: ignore
+            max_label=data.get('maxLabel'),  # type: ignore
+            data_type=data.get('dataType'),  # type: ignore
+            default_value=data.get('defaultValue'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-6.0.0/zaber_motion/dto/exceptions/stream_movement_failed_exception_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,52 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
-from typing import Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
 
-
-class SimpleTuningParamDefinition:
+@dataclass
+class StreamMovementFailedExceptionData:
     """
-    Information about a parameter used for the simple tuning method.
+    Contains additional data for StreamMovementFailedException.
     """
 
-    @property
-    def name(self) -> str:
-        """
-        The name of the parameter.
-        """
-
-        return self._name
-
-    @name.setter
-    def name(self, value: str) -> None:
-        self._name = value
-
-    @property
-    def min_label(self) -> str:
-        """
-        The human readable description of the effect of a lower value on this setting.
-        """
-
-        return self._min_label
-
-    @min_label.setter
-    def min_label(self, value: str) -> None:
-        self._min_label = value
-
-    @property
-    def max_label(self) -> str:
-        """
-        The human readable description of the effect of a higher value on this setting.
-        """
-
-        return self._max_label
-
-    @max_label.setter
-    def max_label(self, value: str) -> None:
-        self._max_label = value
-
-    @property
-    def data_type(self) -> str:
-        """
-        How this parameter will be parsed by the tuner.
-        """
-
-        return self._data_type
-
-    @data_type.setter
-    def data_type(self, value: str) -> None:
-        self._data_type = value
-
-    @property
-    def default_value(self) -> Optional[float]:
-        """
-        The default value of this parameter.
-        """
+    warnings: List[str]
+    """
+    The full list of warnings.
+    """
 
-        return self._default_value
+    reason: str
+    """
+    The reason for the Exception.
+    """
 
-    @default_value.setter
-    def default_value(self, value: Optional[float]) -> None:
-        self._default_value = value
+    @staticmethod
+    def zero_values() -> 'StreamMovementFailedExceptionData':
+        return StreamMovementFailedExceptionData(
+            warnings=[],
+            reason="",
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'StreamMovementFailedExceptionData':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return StreamMovementFailedExceptionData.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'warnings': self.warnings,
+            'reason': self.reason,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.SimpleTuningParamDefinition
-    ) -> 'SimpleTuningParamDefinition':
-        instance = SimpleTuningParamDefinition.__new__(
-            SimpleTuningParamDefinition
-        )  # type: SimpleTuningParamDefinition
-        instance.name = pb_data.name
-        instance.min_label = pb_data.min_label
-        instance.max_label = pb_data.max_label
-        instance.data_type = pb_data.data_type
-        instance.default_value = pb_data.default_value if pb_data.has_default_value else None
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'StreamMovementFailedExceptionData':
+        return StreamMovementFailedExceptionData(
+            warnings=data.get('warnings'),  # type: ignore
+            reason=data.get('reason'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/stream.py` & `zaber_motion-6.0.0/zaber_motion/ascii/stream.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ﻿# pylint: disable=too-many-arguments, too-many-lines
 
 # ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
-from ..protobufs import main_pb2
-from ..units import Units, units_from_literals, VelocityUnits, AccelerationUnits, TimeUnits
+from ..dto import requests as dto
+from ..units import Units, VelocityUnits, AccelerationUnits, TimeUnits
 from ..call import call, call_async, call_sync
-from ..measurement import Measurement
-from ..rotation_direction import RotationDirection
+from ..dto.measurement import Measurement
+from ..dto.rotation_direction import RotationDirection
 from .stream_buffer import StreamBuffer
-from .stream_mode import StreamMode
-from .stream_axis_definition import StreamAxisDefinition
-from .digital_output_action import DigitalOutputAction
+from ..dto.ascii.stream_mode import StreamMode
+from ..dto.ascii.stream_axis_definition import StreamAxisDefinition
+from ..dto.ascii.digital_output_action import DigitalOutputAction
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class Stream:
     """
@@ -63,71 +63,75 @@
         """
         Setup the stream to control the specified axes and to queue actions on the device.
         Allows use of lockstep axes in a stream.
 
         Args:
             axes: Definition of the stream axes.
         """
-        request = main_pb2.StreamSetupLiveCompositeRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.axes.extend([StreamAxisDefinition.to_protobuf(a) for a in axes])
+        request = dto.StreamSetupLiveCompositeRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            axes=list(axes),
+        )
         call("device/stream_setup_live_composite", request)
 
     async def setup_live_composite_async(
             self,
             *axes: StreamAxisDefinition
     ) -> None:
         """
         Setup the stream to control the specified axes and to queue actions on the device.
         Allows use of lockstep axes in a stream.
 
         Args:
             axes: Definition of the stream axes.
         """
-        request = main_pb2.StreamSetupLiveCompositeRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.axes.extend([StreamAxisDefinition.to_protobuf(a) for a in axes])
+        request = dto.StreamSetupLiveCompositeRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            axes=list(axes),
+        )
         await call_async("device/stream_setup_live_composite", request)
 
     def setup_live(
             self,
             *axes: int
     ) -> None:
         """
         Setup the stream to control the specified axes and to queue actions on the device.
 
         Args:
             axes: Numbers of physical axes to setup the stream on.
         """
-        request = main_pb2.StreamSetupLiveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.axes.extend(axes)
+        request = dto.StreamSetupLiveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            axes=list(axes),
+        )
         call("device/stream_setup_live", request)
 
     async def setup_live_async(
             self,
             *axes: int
     ) -> None:
         """
         Setup the stream to control the specified axes and to queue actions on the device.
 
         Args:
             axes: Numbers of physical axes to setup the stream on.
         """
-        request = main_pb2.StreamSetupLiveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.axes.extend(axes)
+        request = dto.StreamSetupLiveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            axes=list(axes),
+        )
         await call_async("device/stream_setup_live", request)
 
     def setup_store_composite(
             self,
             stream_buffer: StreamBuffer,
             *axes: StreamAxisDefinition
     ) -> None:
@@ -135,20 +139,21 @@
         Setup the stream to control the specified axes and queue actions into a stream buffer.
         Allows use of lockstep axes in a stream.
 
         Args:
             stream_buffer: The stream buffer to queue actions in.
             axes: Definition of the stream axes.
         """
-        request = main_pb2.StreamSetupStoreCompositeRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.stream_buffer = stream_buffer.buffer_id
-        request.axes.extend([StreamAxisDefinition.to_protobuf(a) for a in axes])
+        request = dto.StreamSetupStoreCompositeRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            stream_buffer=stream_buffer.buffer_id,
+            axes=list(axes),
+        )
         call("device/stream_setup_store_composite", request)
 
     async def setup_store_composite_async(
             self,
             stream_buffer: StreamBuffer,
             *axes: StreamAxisDefinition
     ) -> None:
@@ -156,60 +161,63 @@
         Setup the stream to control the specified axes and queue actions into a stream buffer.
         Allows use of lockstep axes in a stream.
 
         Args:
             stream_buffer: The stream buffer to queue actions in.
             axes: Definition of the stream axes.
         """
-        request = main_pb2.StreamSetupStoreCompositeRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.stream_buffer = stream_buffer.buffer_id
-        request.axes.extend([StreamAxisDefinition.to_protobuf(a) for a in axes])
+        request = dto.StreamSetupStoreCompositeRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            stream_buffer=stream_buffer.buffer_id,
+            axes=list(axes),
+        )
         await call_async("device/stream_setup_store_composite", request)
 
     def setup_store(
             self,
             stream_buffer: StreamBuffer,
             *axes: int
     ) -> None:
         """
         Setup the stream to control the specified axes and queue actions into a stream buffer.
 
         Args:
             stream_buffer: The stream buffer to queue actions in.
             axes: Numbers of physical axes to setup the stream on.
         """
-        request = main_pb2.StreamSetupStoreRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.stream_buffer = stream_buffer.buffer_id
-        request.axes.extend(axes)
+        request = dto.StreamSetupStoreRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            stream_buffer=stream_buffer.buffer_id,
+            axes=list(axes),
+        )
         call("device/stream_setup_store", request)
 
     async def setup_store_async(
             self,
             stream_buffer: StreamBuffer,
             *axes: int
     ) -> None:
         """
         Setup the stream to control the specified axes and queue actions into a stream buffer.
 
         Args:
             stream_buffer: The stream buffer to queue actions in.
             axes: Numbers of physical axes to setup the stream on.
         """
-        request = main_pb2.StreamSetupStoreRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.stream_buffer = stream_buffer.buffer_id
-        request.axes.extend(axes)
+        request = dto.StreamSetupStoreRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            stream_buffer=stream_buffer.buffer_id,
+            axes=list(axes),
+        )
         await call_async("device/stream_setup_store", request)
 
     def setup_store_arbitrary_axes(
             self,
             stream_buffer: StreamBuffer,
             axes_count: int
     ) -> None:
@@ -218,20 +226,21 @@
         Afterwards, you may call the resulting stream buffer on arbitrary axes.
         This mode does not allow for unit conversions.
 
         Args:
             stream_buffer: The stream buffer to queue actions in.
             axes_count: The number of axes in the stream.
         """
-        request = main_pb2.StreamSetupStoreArbitraryAxesRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.stream_buffer = stream_buffer.buffer_id
-        request.axes_count = axes_count
+        request = dto.StreamSetupStoreArbitraryAxesRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            stream_buffer=stream_buffer.buffer_id,
+            axes_count=axes_count,
+        )
         call("device/stream_setup_store_arbitrary_axes", request)
 
     async def setup_store_arbitrary_axes_async(
             self,
             stream_buffer: StreamBuffer,
             axes_count: int
     ) -> None:
@@ -240,126 +249,133 @@
         Afterwards, you may call the resulting stream buffer on arbitrary axes.
         This mode does not allow for unit conversions.
 
         Args:
             stream_buffer: The stream buffer to queue actions in.
             axes_count: The number of axes in the stream.
         """
-        request = main_pb2.StreamSetupStoreArbitraryAxesRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.stream_buffer = stream_buffer.buffer_id
-        request.axes_count = axes_count
+        request = dto.StreamSetupStoreArbitraryAxesRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            stream_buffer=stream_buffer.buffer_id,
+            axes_count=axes_count,
+        )
         await call_async("device/stream_setup_store_arbitrary_axes", request)
 
     def call(
             self,
             stream_buffer: StreamBuffer
     ) -> None:
         """
         Append the actions in a stream buffer to the queue.
 
         Args:
             stream_buffer: The stream buffer to call.
         """
-        request = main_pb2.StreamCallRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.stream_buffer = stream_buffer.buffer_id
+        request = dto.StreamCallRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            stream_buffer=stream_buffer.buffer_id,
+        )
         call("device/stream_call", request)
 
     async def call_async(
             self,
             stream_buffer: StreamBuffer
     ) -> None:
         """
         Append the actions in a stream buffer to the queue.
 
         Args:
             stream_buffer: The stream buffer to call.
         """
-        request = main_pb2.StreamCallRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.stream_buffer = stream_buffer.buffer_id
+        request = dto.StreamCallRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            stream_buffer=stream_buffer.buffer_id,
+        )
         await call_async("device/stream_call", request)
 
     def line_absolute(
             self,
             *endpoint: Measurement
     ) -> None:
         """
         Queue an absolute line movement in the stream.
 
         Args:
             endpoint: Positions for the axes to move to, relative to their home positions.
         """
-        request = main_pb2.StreamLineRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamLineRequest.ABS
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamLineRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            endpoint=list(endpoint),
+        )
         call("device/stream_line", request)
 
     async def line_absolute_async(
             self,
             *endpoint: Measurement
     ) -> None:
         """
         Queue an absolute line movement in the stream.
 
         Args:
             endpoint: Positions for the axes to move to, relative to their home positions.
         """
-        request = main_pb2.StreamLineRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamLineRequest.ABS
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamLineRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            endpoint=list(endpoint),
+        )
         await call_async("device/stream_line", request)
 
     def line_relative(
             self,
             *endpoint: Measurement
     ) -> None:
         """
         Queue a relative line movement in the stream.
 
         Args:
             endpoint: Positions for the axes to move to, relative to their positions before movement.
         """
-        request = main_pb2.StreamLineRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamLineRequest.REL
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamLineRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            endpoint=list(endpoint),
+        )
         call("device/stream_line", request)
 
     async def line_relative_async(
             self,
             *endpoint: Measurement
     ) -> None:
         """
         Queue a relative line movement in the stream.
 
         Args:
             endpoint: Positions for the axes to move to, relative to their positions before movement.
         """
-        request = main_pb2.StreamLineRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamLineRequest.REL
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamLineRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            endpoint=list(endpoint),
+        )
         await call_async("device/stream_line", request)
 
     def line_absolute_on(
             self,
             target_axes_indices: List[int],
             endpoint: List[Measurement]
     ) -> None:
@@ -369,21 +385,22 @@
 
         Args:
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             endpoint: Positions for the axes to move to, relative to their home positions.
         """
-        request = main_pb2.StreamLineRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamLineRequest.ABS
-        request.target_axes_indices.extend(target_axes_indices)
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamLineRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            target_axes_indices=target_axes_indices,
+            endpoint=endpoint,
+        )
         call("device/stream_line", request)
 
     async def line_absolute_on_async(
             self,
             target_axes_indices: List[int],
             endpoint: List[Measurement]
     ) -> None:
@@ -393,21 +410,22 @@
 
         Args:
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             endpoint: Positions for the axes to move to, relative to their home positions.
         """
-        request = main_pb2.StreamLineRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamLineRequest.ABS
-        request.target_axes_indices.extend(target_axes_indices)
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamLineRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            target_axes_indices=target_axes_indices,
+            endpoint=endpoint,
+        )
         await call_async("device/stream_line", request)
 
     def line_relative_on(
             self,
             target_axes_indices: List[int],
             endpoint: List[Measurement]
     ) -> None:
@@ -417,21 +435,22 @@
 
         Args:
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             endpoint: Positions for the axes to move to, relative to their positions before movement.
         """
-        request = main_pb2.StreamLineRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamLineRequest.REL
-        request.target_axes_indices.extend(target_axes_indices)
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamLineRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            target_axes_indices=target_axes_indices,
+            endpoint=endpoint,
+        )
         call("device/stream_line", request)
 
     async def line_relative_on_async(
             self,
             target_axes_indices: List[int],
             endpoint: List[Measurement]
     ) -> None:
@@ -441,21 +460,22 @@
 
         Args:
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             endpoint: Positions for the axes to move to, relative to their positions before movement.
         """
-        request = main_pb2.StreamLineRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamLineRequest.REL
-        request.target_axes_indices.extend(target_axes_indices)
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamLineRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            target_axes_indices=target_axes_indices,
+            endpoint=endpoint,
+        )
         await call_async("device/stream_line", request)
 
     def arc_absolute(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement,
@@ -469,24 +489,25 @@
         Args:
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the arc exists.
             center_y: The second dimension of the position of the center of the circle on which the arc exists.
             end_x: The first dimension of the end position of the arc.
             end_y: The second dimension of the end position of the arc.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.ABS
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+        )
         call("device/stream_arc", request)
 
     async def arc_absolute_async(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement,
@@ -500,24 +521,25 @@
         Args:
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the arc exists.
             center_y: The second dimension of the position of the center of the circle on which the arc exists.
             end_x: The first dimension of the end position of the arc.
             end_y: The second dimension of the end position of the arc.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.ABS
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+        )
         await call_async("device/stream_arc", request)
 
     def arc_relative(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement,
@@ -531,24 +553,25 @@
         Args:
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the arc exists.
             center_y: The second dimension of the position of the center of the circle on which the arc exists.
             end_x: The first dimension of the end position of the arc.
             end_y: The second dimension of the end position of the arc.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.REL
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+        )
         call("device/stream_arc", request)
 
     async def arc_relative_async(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement,
@@ -562,24 +585,25 @@
         Args:
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the arc exists.
             center_y: The second dimension of the position of the center of the circle on which the arc exists.
             end_x: The first dimension of the end position of the arc.
             end_y: The second dimension of the end position of the arc.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.REL
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+        )
         await call_async("device/stream_arc", request)
 
     def arc_absolute_on(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -598,25 +622,26 @@
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the arc exists.
             center_y: The second dimension of the position of the center of the circle on which the arc exists.
             end_x: The first dimension of the end position of the arc.
             end_y: The second dimension of the end position of the arc.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.ABS
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+        )
         call("device/stream_arc", request)
 
     async def arc_absolute_on_async(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -635,25 +660,26 @@
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the arc exists.
             center_y: The second dimension of the position of the center of the circle on which the arc exists.
             end_x: The first dimension of the end position of the arc.
             end_y: The second dimension of the end position of the arc.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.ABS
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+        )
         await call_async("device/stream_arc", request)
 
     def arc_relative_on(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -672,25 +698,26 @@
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the arc exists.
             center_y: The second dimension of the position of the center of the circle on which the arc exists.
             end_x: The first dimension of the end position of the arc.
             end_y: The second dimension of the end position of the arc.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.REL
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+        )
         call("device/stream_arc", request)
 
     async def arc_relative_on_async(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -709,25 +736,26 @@
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the arc exists.
             center_y: The second dimension of the position of the center of the circle on which the arc exists.
             end_x: The first dimension of the end position of the arc.
             end_y: The second dimension of the end position of the arc.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.REL
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+        )
         await call_async("device/stream_arc", request)
 
     def helix_absolute_on(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -749,26 +777,27 @@
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the helix projects.
             center_y: The second dimension of the position of the center of the circle on which the helix projects.
             end_x: The first dimension of the end position of the helix's arc component.
             end_y: The second dimension of the end position of the helix's arc component.
             endpoint: Positions for the helix's line component axes, relative to their home positions.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.ABS
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+            endpoint=list(endpoint),
+        )
         call("device/stream_helix", request)
 
     async def helix_absolute_on_async(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -790,26 +819,27 @@
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the helix projects.
             center_y: The second dimension of the position of the center of the circle on which the helix projects.
             end_x: The first dimension of the end position of the helix's arc component.
             end_y: The second dimension of the end position of the helix's arc component.
             endpoint: Positions for the helix's line component axes, relative to their home positions.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.ABS
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+            endpoint=list(endpoint),
+        )
         await call_async("device/stream_helix", request)
 
     def helix_relative_on(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -831,26 +861,27 @@
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the helix projects.
             center_y: The second dimension of the position of the center of the circle on which the helix projects.
             end_x: The first dimension of the end position of the helix's arc component.
             end_y: The second dimension of the end position of the helix's arc component.
             endpoint: Positions for the helix's line component axes, relative to their positions before movement.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.REL
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+            endpoint=list(endpoint),
+        )
         call("device/stream_helix", request)
 
     async def helix_relative_on_async(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -872,26 +903,27 @@
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle on which the helix projects.
             center_y: The second dimension of the position of the center of the circle on which the helix projects.
             end_x: The first dimension of the end position of the helix's arc component.
             end_y: The second dimension of the end position of the helix's arc component.
             endpoint: Positions for the helix's line component axes, relative to their positions before movement.
         """
-        request = main_pb2.StreamArcRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamArcRequest.REL
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
-        request.end_x.CopyFrom(Measurement.to_protobuf(end_x))
-        request.end_y.CopyFrom(Measurement.to_protobuf(end_y))
-        request.endpoint.extend([Measurement.to_protobuf(a) for a in endpoint])
+        request = dto.StreamArcRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+            end_x=end_x,
+            end_y=end_y,
+            endpoint=list(endpoint),
+        )
         await call_async("device/stream_helix", request)
 
     def circle_absolute(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement
@@ -901,22 +933,23 @@
         Absolute meaning that the home positions of the axes are treated as the origin.
 
         Args:
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle.
             center_y: The second dimension of the position of the center of the circle.
         """
-        request = main_pb2.StreamCircleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamCircleRequest.ABS
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request = dto.StreamCircleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+        )
         call("device/stream_circle", request)
 
     async def circle_absolute_async(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement
@@ -926,22 +959,23 @@
         Absolute meaning that the home positions of the axes are treated as the origin.
 
         Args:
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle.
             center_y: The second dimension of the position of the center of the circle.
         """
-        request = main_pb2.StreamCircleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamCircleRequest.ABS
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request = dto.StreamCircleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+        )
         await call_async("device/stream_circle", request)
 
     def circle_relative(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement
@@ -951,22 +985,23 @@
         Relative meaning that the current position of the axes is treated as the origin.
 
         Args:
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle.
             center_y: The second dimension of the position of the center of the circle.
         """
-        request = main_pb2.StreamCircleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamCircleRequest.REL
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request = dto.StreamCircleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+        )
         call("device/stream_circle", request)
 
     async def circle_relative_async(
             self,
             rotation_direction: RotationDirection,
             center_x: Measurement,
             center_y: Measurement
@@ -976,22 +1011,23 @@
         Relative meaning that the current position of the axes is treated as the origin.
 
         Args:
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle.
             center_y: The second dimension of the position of the center of the circle.
         """
-        request = main_pb2.StreamCircleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamCircleRequest.REL
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request = dto.StreamCircleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+        )
         await call_async("device/stream_circle", request)
 
     def circle_absolute_on(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -1006,23 +1042,24 @@
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle.
             center_y: The second dimension of the position of the center of the circle.
         """
-        request = main_pb2.StreamCircleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamCircleRequest.ABS
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request = dto.StreamCircleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+        )
         call("device/stream_circle", request)
 
     async def circle_absolute_on_async(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -1037,23 +1074,24 @@
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle.
             center_y: The second dimension of the position of the center of the circle.
         """
-        request = main_pb2.StreamCircleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamCircleRequest.ABS
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request = dto.StreamCircleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.ABS,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+        )
         await call_async("device/stream_circle", request)
 
     def circle_relative_on(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -1068,23 +1106,24 @@
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle.
             center_y: The second dimension of the position of the center of the circle.
         """
-        request = main_pb2.StreamCircleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamCircleRequest.REL
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request = dto.StreamCircleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+        )
         call("device/stream_circle", request)
 
     async def circle_relative_on_async(
             self,
             target_axes_indices: List[int],
             rotation_direction: RotationDirection,
             center_x: Measurement,
@@ -1099,23 +1138,24 @@
             target_axes_indices: Indices of the axes in the stream the movement targets.
                 Refers to the axes provided during the stream setup or further execution.
                 Indices are zero-based.
             rotation_direction: The direction of the rotation.
             center_x: The first dimension of the position of the center of the circle.
             center_y: The second dimension of the position of the center of the circle.
         """
-        request = main_pb2.StreamCircleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.type = main_pb2.StreamCircleRequest.REL
-        request.target_axes_indices.extend(target_axes_indices)
-        request.rotation_direction = rotation_direction.value
-        request.center_x.CopyFrom(Measurement.to_protobuf(center_x))
-        request.center_y.CopyFrom(Measurement.to_protobuf(center_y))
+        request = dto.StreamCircleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            type=dto.StreamSegmentType.REL,
+            target_axes_indices=target_axes_indices,
+            rotation_direction=rotation_direction,
+            center_x=center_x,
+            center_y=center_y,
+        )
         await call_async("device/stream_circle", request)
 
     def wait_digital_input(
             self,
             channel_number: int,
             value: bool
     ) -> None:
@@ -1123,20 +1163,21 @@
         Wait for a digital input channel to reach a given value.
 
         Args:
             channel_number: The number of the digital input channel.
                 Channel numbers are numbered from one.
             value: The value that the stream should wait for.
         """
-        request = main_pb2.StreamWaitDigitalInputRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.channel_number = channel_number
-        request.value = value
+        request = dto.StreamWaitDigitalInputRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            channel_number=channel_number,
+            value=value,
+        )
         call("device/stream_wait_digital_input", request)
 
     async def wait_digital_input_async(
             self,
             channel_number: int,
             value: bool
     ) -> None:
@@ -1144,20 +1185,21 @@
         Wait for a digital input channel to reach a given value.
 
         Args:
             channel_number: The number of the digital input channel.
                 Channel numbers are numbered from one.
             value: The value that the stream should wait for.
         """
-        request = main_pb2.StreamWaitDigitalInputRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.channel_number = channel_number
-        request.value = value
+        request = dto.StreamWaitDigitalInputRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            channel_number=channel_number,
+            value=value,
+        )
         await call_async("device/stream_wait_digital_input", request)
 
     def wait_analog_input(
             self,
             channel_number: int,
             condition: str,
             value: float
@@ -1167,21 +1209,22 @@
 
         Args:
             channel_number: The number of the analog input channel.
                 Channel numbers are numbered from one.
             condition: A condition (e.g. <, <=, ==, !=).
             value: The value that the condition concerns, in Volts.
         """
-        request = main_pb2.StreamWaitAnalogInputRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.channel_number = channel_number
-        request.condition = condition
-        request.value = value
+        request = dto.StreamWaitAnalogInputRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            channel_number=channel_number,
+            condition=condition,
+            value=value,
+        )
         call("device/stream_wait_analog_input", request)
 
     async def wait_analog_input_async(
             self,
             channel_number: int,
             condition: str,
             value: float
@@ -1191,21 +1234,22 @@
 
         Args:
             channel_number: The number of the analog input channel.
                 Channel numbers are numbered from one.
             condition: A condition (e.g. <, <=, ==, !=).
             value: The value that the condition concerns, in Volts.
         """
-        request = main_pb2.StreamWaitAnalogInputRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.channel_number = channel_number
-        request.condition = condition
-        request.value = value
+        request = dto.StreamWaitAnalogInputRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            channel_number=channel_number,
+            condition=condition,
+            value=value,
+        )
         await call_async("device/stream_wait_analog_input", request)
 
     def set_digital_output(
             self,
             channel_number: int,
             value: DigitalOutputAction
     ) -> None:
@@ -1213,20 +1257,21 @@
         Set the value of a digital output channel.
 
         Args:
             channel_number: The number of the digital output channel.
                 Channel numbers are numbered from one.
             value: The type of action to perform on the channel.
         """
-        request = main_pb2.StreamSetDigitalOutputRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.channel_number = channel_number
-        request.value = value.value
+        request = dto.StreamSetDigitalOutputRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            channel_number=channel_number,
+            value=value,
+        )
         call("device/stream_set_digital_output", request)
 
     async def set_digital_output_async(
             self,
             channel_number: int,
             value: DigitalOutputAction
     ) -> None:
@@ -1234,20 +1279,21 @@
         Set the value of a digital output channel.
 
         Args:
             channel_number: The number of the digital output channel.
                 Channel numbers are numbered from one.
             value: The type of action to perform on the channel.
         """
-        request = main_pb2.StreamSetDigitalOutputRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.channel_number = channel_number
-        request.value = value.value
+        request = dto.StreamSetDigitalOutputRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            channel_number=channel_number,
+            value=value,
+        )
         await call_async("device/stream_set_digital_output", request)
 
     def set_analog_output(
             self,
             channel_number: int,
             value: float
     ) -> None:
@@ -1255,20 +1301,21 @@
         Set the value of an analog output channel.
 
         Args:
             channel_number: The number of the analog output channel.
                 Channel numbers are numbered from one.
             value: The value to set the channel to, in Volts.
         """
-        request = main_pb2.StreamSetAnalogOutputRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.channel_number = channel_number
-        request.value = value
+        request = dto.StreamSetAnalogOutputRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            channel_number=channel_number,
+            value=value,
+        )
         call("device/stream_set_analog_output", request)
 
     async def set_analog_output_async(
             self,
             channel_number: int,
             value: float
     ) -> None:
@@ -1276,252 +1323,271 @@
         Set the value of an analog output channel.
 
         Args:
             channel_number: The number of the analog output channel.
                 Channel numbers are numbered from one.
             value: The value to set the channel to, in Volts.
         """
-        request = main_pb2.StreamSetAnalogOutputRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.channel_number = channel_number
-        request.value = value
+        request = dto.StreamSetAnalogOutputRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            channel_number=channel_number,
+            value=value,
+        )
         await call_async("device/stream_set_analog_output", request)
 
     def set_all_digital_outputs(
             self,
             values: List[DigitalOutputAction]
     ) -> None:
         """
         Sets values for all digital output channels.
 
         Args:
             values: The type of action to perform on the channel.
         """
-        request = main_pb2.StreamSetAllDigitalOutputsRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.values.extend([x.value for x in values])
+        request = dto.StreamSetAllDigitalOutputsRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            values=values,
+        )
         call("device/stream_set_all_digital_outputs", request)
 
     async def set_all_digital_outputs_async(
             self,
             values: List[DigitalOutputAction]
     ) -> None:
         """
         Sets values for all digital output channels.
 
         Args:
             values: The type of action to perform on the channel.
         """
-        request = main_pb2.StreamSetAllDigitalOutputsRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.values.extend([x.value for x in values])
+        request = dto.StreamSetAllDigitalOutputsRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            values=values,
+        )
         await call_async("device/stream_set_all_digital_outputs", request)
 
     def set_all_analog_outputs(
             self,
             values: List[float]
     ) -> None:
         """
         Sets values for all analog output channels.
 
         Args:
             values: The values to set the output channels to, in Volts.
         """
-        request = main_pb2.StreamSetAllAnalogOutputsRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.values.extend(values)
+        request = dto.StreamSetAllAnalogOutputsRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            values=values,
+        )
         call("device/stream_set_all_analog_outputs", request)
 
     async def set_all_analog_outputs_async(
             self,
             values: List[float]
     ) -> None:
         """
         Sets values for all analog output channels.
 
         Args:
             values: The values to set the output channels to, in Volts.
         """
-        request = main_pb2.StreamSetAllAnalogOutputsRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.values.extend(values)
+        request = dto.StreamSetAllAnalogOutputsRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            values=values,
+        )
         await call_async("device/stream_set_all_analog_outputs", request)
 
     def wait(
             self,
             time: float,
             unit: TimeUnits = Units.NATIVE
     ) -> None:
         """
         Wait a specified time.
 
         Args:
             time: Amount of time to wait.
             unit: Units of time.
         """
-        request = main_pb2.StreamWaitRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.time = time
-        request.unit = units_from_literals(unit).value
+        request = dto.StreamWaitRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            time=time,
+            unit=unit,
+        )
         call("device/stream_wait", request)
 
     async def wait_async(
             self,
             time: float,
             unit: TimeUnits = Units.NATIVE
     ) -> None:
         """
         Wait a specified time.
 
         Args:
             time: Amount of time to wait.
             unit: Units of time.
         """
-        request = main_pb2.StreamWaitRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.time = time
-        request.unit = units_from_literals(unit).value
+        request = dto.StreamWaitRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            time=time,
+            unit=unit,
+        )
         await call_async("device/stream_wait", request)
 
     def wait_until_idle(
             self,
             throw_error_on_fault: bool = True
     ) -> None:
         """
         Waits until the live stream executes all queued actions.
 
         Args:
             throw_error_on_fault: Determines whether to throw error when fault is observed.
         """
-        request = main_pb2.StreamWaitUntilIdleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.throw_error_on_fault = throw_error_on_fault
+        request = dto.StreamWaitUntilIdleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            throw_error_on_fault=throw_error_on_fault,
+        )
         call("device/stream_wait_until_idle", request)
 
     async def wait_until_idle_async(
             self,
             throw_error_on_fault: bool = True
     ) -> None:
         """
         Waits until the live stream executes all queued actions.
 
         Args:
             throw_error_on_fault: Determines whether to throw error when fault is observed.
         """
-        request = main_pb2.StreamWaitUntilIdleRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.throw_error_on_fault = throw_error_on_fault
+        request = dto.StreamWaitUntilIdleRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            throw_error_on_fault=throw_error_on_fault,
+        )
         await call_async("device/stream_wait_until_idle", request)
 
     def cork(
             self
     ) -> None:
         """
         Cork the front of the stream's action queue, blocking execution.
         Execution resumes upon uncorking the queue, or when the number of queued actions reaches its limit.
         Corking eliminates discontinuities in motion due to subsequent stream commands reaching the device late.
         You can only cork an idle live stream.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
         call("device/stream_cork", request)
 
     async def cork_async(
             self
     ) -> None:
         """
         Cork the front of the stream's action queue, blocking execution.
         Execution resumes upon uncorking the queue, or when the number of queued actions reaches its limit.
         Corking eliminates discontinuities in motion due to subsequent stream commands reaching the device late.
         You can only cork an idle live stream.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
         await call_async("device/stream_cork", request)
 
     def uncork(
             self
     ) -> None:
         """
         Uncork the front of the queue, unblocking command execution.
         You can only uncork an idle live stream that is corked.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
         call("device/stream_uncork", request)
 
     async def uncork_async(
             self
     ) -> None:
         """
         Uncork the front of the queue, unblocking command execution.
         You can only uncork an idle live stream that is corked.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
         await call_async("device/stream_uncork", request)
 
     def is_busy(
             self
     ) -> bool:
         """
         Returns a boolean value indicating whether the live stream is executing a queued action.
 
         Returns:
             True if the stream is executing a queued action.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        response = main_pb2.BoolResponse()
-        call("device/stream_is_busy", request, response)
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
+        response = call(
+            "device/stream_is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_busy_async(
             self
     ) -> bool:
         """
         Returns a boolean value indicating whether the live stream is executing a queued action.
 
         Returns:
             True if the stream is executing a queued action.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        response = main_pb2.BoolResponse()
-        await call_async("device/stream_is_busy", request, response)
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
+        response = await call_async(
+            "device/stream_is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def get_max_speed(
             self,
             unit: VelocityUnits = Units.NATIVE
     ) -> float:
         """
@@ -1530,21 +1596,24 @@
 
         Args:
             unit: Units of velocity.
 
         Returns:
             The maximum speed of the stream.
         """
-        request = main_pb2.StreamGetMaxSpeedRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("device/stream_get_max_speed", request, response)
+        request = dto.StreamGetMaxSpeedRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            unit=unit,
+        )
+        response = call(
+            "device/stream_get_max_speed",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_max_speed_async(
             self,
             unit: VelocityUnits = Units.NATIVE
     ) -> float:
         """
@@ -1553,21 +1622,24 @@
 
         Args:
             unit: Units of velocity.
 
         Returns:
             The maximum speed of the stream.
         """
-        request = main_pb2.StreamGetMaxSpeedRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("device/stream_get_max_speed", request, response)
+        request = dto.StreamGetMaxSpeedRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            unit=unit,
+        )
+        response = await call_async(
+            "device/stream_get_max_speed",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set_max_speed(
             self,
             max_speed: float,
             unit: VelocityUnits = Units.NATIVE
     ) -> None:
@@ -1575,20 +1647,21 @@
         Sets the maximum speed of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_speed: Maximum speed at which any stream action is executed.
             unit: Units of velocity.
         """
-        request = main_pb2.StreamSetMaxSpeedRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.max_speed = max_speed
-        request.unit = units_from_literals(unit).value
+        request = dto.StreamSetMaxSpeedRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            max_speed=max_speed,
+            unit=unit,
+        )
         call("device/stream_set_max_speed", request)
 
     async def set_max_speed_async(
             self,
             max_speed: float,
             unit: VelocityUnits = Units.NATIVE
     ) -> None:
@@ -1596,20 +1669,21 @@
         Sets the maximum speed of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_speed: Maximum speed at which any stream action is executed.
             unit: Units of velocity.
         """
-        request = main_pb2.StreamSetMaxSpeedRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.max_speed = max_speed
-        request.unit = units_from_literals(unit).value
+        request = dto.StreamSetMaxSpeedRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            max_speed=max_speed,
+            unit=unit,
+        )
         await call_async("device/stream_set_max_speed", request)
 
     def get_max_tangential_acceleration(
             self,
             unit: AccelerationUnits = Units.NATIVE
     ) -> float:
         """
@@ -1618,21 +1692,24 @@
 
         Args:
             unit: Units of acceleration.
 
         Returns:
             The maximum tangential acceleration of the live stream.
         """
-        request = main_pb2.StreamGetMaxTangentialAccelerationRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("device/stream_get_max_tangential_acceleration", request, response)
+        request = dto.StreamGetMaxTangentialAccelerationRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            unit=unit,
+        )
+        response = call(
+            "device/stream_get_max_tangential_acceleration",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_max_tangential_acceleration_async(
             self,
             unit: AccelerationUnits = Units.NATIVE
     ) -> float:
         """
@@ -1641,21 +1718,24 @@
 
         Args:
             unit: Units of acceleration.
 
         Returns:
             The maximum tangential acceleration of the live stream.
         """
-        request = main_pb2.StreamGetMaxTangentialAccelerationRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("device/stream_get_max_tangential_acceleration", request, response)
+        request = dto.StreamGetMaxTangentialAccelerationRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            unit=unit,
+        )
+        response = await call_async(
+            "device/stream_get_max_tangential_acceleration",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set_max_tangential_acceleration(
             self,
             max_tangential_acceleration: float,
             unit: AccelerationUnits = Units.NATIVE
     ) -> None:
@@ -1663,20 +1743,21 @@
         Sets the maximum tangential acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_tangential_acceleration: Maximum tangential acceleration at which any stream action is executed.
             unit: Units of acceleration.
         """
-        request = main_pb2.StreamSetMaxTangentialAccelerationRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.max_tangential_acceleration = max_tangential_acceleration
-        request.unit = units_from_literals(unit).value
+        request = dto.StreamSetMaxTangentialAccelerationRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            max_tangential_acceleration=max_tangential_acceleration,
+            unit=unit,
+        )
         call("device/stream_set_max_tangential_acceleration", request)
 
     async def set_max_tangential_acceleration_async(
             self,
             max_tangential_acceleration: float,
             unit: AccelerationUnits = Units.NATIVE
     ) -> None:
@@ -1684,20 +1765,21 @@
         Sets the maximum tangential acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_tangential_acceleration: Maximum tangential acceleration at which any stream action is executed.
             unit: Units of acceleration.
         """
-        request = main_pb2.StreamSetMaxTangentialAccelerationRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.max_tangential_acceleration = max_tangential_acceleration
-        request.unit = units_from_literals(unit).value
+        request = dto.StreamSetMaxTangentialAccelerationRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            max_tangential_acceleration=max_tangential_acceleration,
+            unit=unit,
+        )
         await call_async("device/stream_set_max_tangential_acceleration", request)
 
     def get_max_centripetal_acceleration(
             self,
             unit: AccelerationUnits = Units.NATIVE
     ) -> float:
         """
@@ -1706,21 +1788,24 @@
 
         Args:
             unit: Units of acceleration.
 
         Returns:
             The maximum centripetal acceleration of the live stream.
         """
-        request = main_pb2.StreamGetMaxCentripetalAccelerationRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("device/stream_get_max_centripetal_acceleration", request, response)
+        request = dto.StreamGetMaxCentripetalAccelerationRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            unit=unit,
+        )
+        response = call(
+            "device/stream_get_max_centripetal_acceleration",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_max_centripetal_acceleration_async(
             self,
             unit: AccelerationUnits = Units.NATIVE
     ) -> float:
         """
@@ -1729,21 +1814,24 @@
 
         Args:
             unit: Units of acceleration.
 
         Returns:
             The maximum centripetal acceleration of the live stream.
         """
-        request = main_pb2.StreamGetMaxCentripetalAccelerationRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("device/stream_get_max_centripetal_acceleration", request, response)
+        request = dto.StreamGetMaxCentripetalAccelerationRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            unit=unit,
+        )
+        response = await call_async(
+            "device/stream_get_max_centripetal_acceleration",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set_max_centripetal_acceleration(
             self,
             max_centripetal_acceleration: float,
             unit: AccelerationUnits = Units.NATIVE
     ) -> None:
@@ -1751,20 +1839,21 @@
         Sets the maximum centripetal acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_centripetal_acceleration: Maximum centripetal acceleration at which any stream action is executed.
             unit: Units of acceleration.
         """
-        request = main_pb2.StreamSetMaxCentripetalAccelerationRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.max_centripetal_acceleration = max_centripetal_acceleration
-        request.unit = units_from_literals(unit).value
+        request = dto.StreamSetMaxCentripetalAccelerationRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            max_centripetal_acceleration=max_centripetal_acceleration,
+            unit=unit,
+        )
         call("device/stream_set_max_centripetal_acceleration", request)
 
     async def set_max_centripetal_acceleration_async(
             self,
             max_centripetal_acceleration: float,
             unit: AccelerationUnits = Units.NATIVE
     ) -> None:
@@ -1772,231 +1861,255 @@
         Sets the maximum centripetal acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_centripetal_acceleration: Maximum centripetal acceleration at which any stream action is executed.
             unit: Units of acceleration.
         """
-        request = main_pb2.StreamSetMaxCentripetalAccelerationRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.max_centripetal_acceleration = max_centripetal_acceleration
-        request.unit = units_from_literals(unit).value
+        request = dto.StreamSetMaxCentripetalAccelerationRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            max_centripetal_acceleration=max_centripetal_acceleration,
+            unit=unit,
+        )
         await call_async("device/stream_set_max_centripetal_acceleration", request)
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string which represents the stream.
 
         Returns:
             String which represents the stream.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        response = main_pb2.StringResponse()
-        call_sync("device/stream_to_string", request, response)
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
+        response = call_sync(
+            "device/stream_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def disable(
             self
     ) -> None:
         """
         Disables the stream.
         If the stream is not setup, this command does nothing.
         Once disabled, the stream will no longer accept stream commands.
         The stream will process the rest of the commands in the queue until it is empty.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
         call("device/stream_disable", request)
 
     async def disable_async(
             self
     ) -> None:
         """
         Disables the stream.
         If the stream is not setup, this command does nothing.
         Once disabled, the stream will no longer accept stream commands.
         The stream will process the rest of the commands in the queue until it is empty.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
         await call_async("device/stream_disable", request)
 
     def generic_command(
             self,
             command: str
     ) -> None:
         """
         Sends a generic ASCII command to the stream.
         Keeps resending the command while the device rejects with AGAIN reason.
 
         Args:
             command: Command and its parameters.
         """
-        request = main_pb2.StreamGenericCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.command = command
+        request = dto.StreamGenericCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            command=command,
+        )
         call("device/stream_generic_command", request)
 
     async def generic_command_async(
             self,
             command: str
     ) -> None:
         """
         Sends a generic ASCII command to the stream.
         Keeps resending the command while the device rejects with AGAIN reason.
 
         Args:
             command: Command and its parameters.
         """
-        request = main_pb2.StreamGenericCommandRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.command = command
+        request = dto.StreamGenericCommandRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            command=command,
+        )
         await call_async("device/stream_generic_command", request)
 
     def generic_command_batch(
             self,
             batch: List[str]
     ) -> None:
         """
         Sends a batch of generic ASCII commands to the stream.
         Keeps resending command while the device rejects with AGAIN reason.
         The batch is atomic in terms of thread safety.
 
         Args:
             batch: Array of commands.
         """
-        request = main_pb2.StreamGenericCommandBatchRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.batch.extend(batch)
+        request = dto.StreamGenericCommandBatchRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            batch=batch,
+        )
         call("device/stream_generic_command_batch", request)
 
     async def generic_command_batch_async(
             self,
             batch: List[str]
     ) -> None:
         """
         Sends a batch of generic ASCII commands to the stream.
         Keeps resending command while the device rejects with AGAIN reason.
         The batch is atomic in terms of thread safety.
 
         Args:
             batch: Array of commands.
         """
-        request = main_pb2.StreamGenericCommandBatchRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        request.batch.extend(batch)
+        request = dto.StreamGenericCommandBatchRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+            batch=batch,
+        )
         await call_async("device/stream_generic_command_batch", request)
 
     def check_disabled(
             self
     ) -> bool:
         """
         Queries the stream status from the device
         and returns boolean indicating whether the stream is disabled.
         Useful to determine if streaming was interrupted by other movements.
 
         Returns:
             True if the stream is disabled.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        response = main_pb2.BoolResponse()
-        call("device/stream_check_disabled", request, response)
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
+        response = call(
+            "device/stream_check_disabled",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def check_disabled_async(
             self
     ) -> bool:
         """
         Queries the stream status from the device
         and returns boolean indicating whether the stream is disabled.
         Useful to determine if streaming was interrupted by other movements.
 
         Returns:
             True if the stream is disabled.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        response = main_pb2.BoolResponse()
-        await call_async("device/stream_check_disabled", request, response)
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
+        response = await call_async(
+            "device/stream_check_disabled",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def treat_discontinuities_as_error(
             self
     ) -> None:
         """
         Makes the stream throw StreamDiscontinuityException when it encounters discontinuities (ND warning flag).
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
         call_sync("device/stream_treat_discontinuities", request)
 
     def ignore_current_discontinuity(
             self
     ) -> None:
         """
         Prevents StreamDiscontinuityException as a result of expected discontinuity when resuming streaming.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
         call_sync("device/stream_ignore_discontinuity", request)
 
     def __retrieve_axes(
             self
     ) -> List[StreamAxisDefinition]:
         """
         Gets the axes of the stream.
 
         Returns:
             An array of axis numbers of the axes the stream is set up to control.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        response = main_pb2.StreamGetAxesResponse()
-        call_sync("device/stream_get_axes", request, response)
-        return [StreamAxisDefinition.from_protobuf(a) for a in response.axes]
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
+        response = call_sync(
+            "device/stream_get_axes",
+            request,
+            dto.StreamGetAxesResponse.from_binary)
+        return response.axes
 
     def __retrieve_mode(
             self
     ) -> StreamMode:
         """
         Get the mode of the stream.
 
         Returns:
             Mode of the stream.
         """
-        request = main_pb2.StreamEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.stream_id = self.stream_id
-        response = main_pb2.IntResponse()
-        call_sync("device/stream_get_mode", request, response)
-        return StreamMode(response.value)
+        request = dto.StreamEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            stream_id=self.stream_id,
+        )
+        response = call_sync(
+            "device/stream_get_mode",
+            request,
+            dto.StreamModeResponse.from_binary)
+        return response.stream_mode
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-6.0.0/zaber_motion/ascii/stream_buffer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from ..call import call, call_async
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class StreamBuffer:
@@ -37,57 +37,65 @@
     ) -> List[str]:
         """
         Get the buffer contents as an array of strings.
 
         Returns:
             A string array containing all the stream commands stored in the buffer.
         """
-        request = main_pb2.StreamBufferGetContentRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.buffer_id = self.buffer_id
-        response = main_pb2.StreamBufferGetContentResponse()
-        call("device/stream_buffer_get_content", request, response)
-        return list(response.buffer_lines)
+        request = dto.StreamBufferGetContentRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            buffer_id=self.buffer_id,
+        )
+        response = call(
+            "device/stream_buffer_get_content",
+            request,
+            dto.StreamBufferGetContentResponse.from_binary)
+        return response.buffer_lines
 
     async def get_content_async(
             self
     ) -> List[str]:
         """
         Get the buffer contents as an array of strings.
 
         Returns:
             A string array containing all the stream commands stored in the buffer.
         """
-        request = main_pb2.StreamBufferGetContentRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.buffer_id = self.buffer_id
-        response = main_pb2.StreamBufferGetContentResponse()
-        await call_async("device/stream_buffer_get_content", request, response)
-        return list(response.buffer_lines)
+        request = dto.StreamBufferGetContentRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            buffer_id=self.buffer_id,
+        )
+        response = await call_async(
+            "device/stream_buffer_get_content",
+            request,
+            dto.StreamBufferGetContentResponse.from_binary)
+        return response.buffer_lines
 
     def erase(
             self
     ) -> None:
         """
         Erase the contents of the buffer.
         This method fails if there is a stream writing to the buffer.
         """
-        request = main_pb2.StreamBufferEraseRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.buffer_id = self.buffer_id
+        request = dto.StreamBufferEraseRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            buffer_id=self.buffer_id,
+        )
         call("device/stream_buffer_erase", request)
 
     async def erase_async(
             self
     ) -> None:
         """
         Erase the contents of the buffer.
         This method fails if there is a stream writing to the buffer.
         """
-        request = main_pb2.StreamBufferEraseRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.buffer_id = self.buffer_id
+        request = dto.StreamBufferEraseRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            buffer_id=self.buffer_id,
+        )
         await call_async("device/stream_buffer_erase", request)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/streams.py` & `zaber_motion-6.0.0/zaber_motion/ascii/streams.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
 
 from ..call import call, call_async
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 
 from .stream import Stream
 from .stream_buffer import StreamBuffer
 
 if TYPE_CHECKING:
     from .device import Device
 
@@ -69,31 +69,37 @@
     ) -> List[int]:
         """
         Get a list of buffer IDs that are currently in use.
 
         Returns:
             List of buffer IDs.
         """
-        request = main_pb2.StreamBufferList()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.pvt = False
-        response = main_pb2.IntArrayResponse()
-        call("device/stream_buffer_list", request, response)
-        return list(response.values)
+        request = dto.StreamBufferList(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            pvt=False,
+        )
+        response = call(
+            "device/stream_buffer_list",
+            request,
+            dto.IntArrayResponse.from_binary)
+        return response.values
 
     async def list_buffer_ids_async(
             self
     ) -> List[int]:
         """
         Get a list of buffer IDs that are currently in use.
 
         Returns:
             List of buffer IDs.
         """
-        request = main_pb2.StreamBufferList()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.pvt = False
-        response = main_pb2.IntArrayResponse()
-        await call_async("device/stream_buffer_list", request, response)
-        return list(response.values)
+        request = dto.StreamBufferList(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            pvt=False,
+        )
+        response = await call_async(
+            "device/stream_buffer_list",
+            request,
+            dto.IntArrayResponse.from_binary)
+        return response.values
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/transport.py` & `zaber_motion-6.0.0/zaber_motion/ascii/transport.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Any
 
 from ..call import call, call_async, call_sync
 
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 
 
 class Transport:
     """
     Connection transport backend allowing to carry Zaber ASCII protocol over arbitrary protocols.
     Can only be used with a single connection.
     """
@@ -28,139 +28,154 @@
     def open() -> 'Transport':
         """
         Creates new instance allowing to read/write messages from/to a single connection.
 
         Returns:
             New instance of transport.
         """
-        request = main_pb2.EmptyRequest()
-        response = main_pb2.CustomInterfaceOpenResponse()
-        call_sync("custom/interface/open", request, response)
+        request = dto.EmptyRequest(
+        )
+        response = call_sync(
+            "custom/interface/open",
+            request,
+            dto.CustomInterfaceOpenResponse.from_binary)
         return Transport(response.transport_id)
 
     def close(
             self
     ) -> None:
         """
         Closes the transport.
         Also closes the connection using the transport.
         """
-        request = main_pb2.CustomInterfaceCloseRequest()
-        request.transport_id = self.transport_id
+        request = dto.CustomInterfaceCloseRequest(
+            transport_id=self.transport_id,
+        )
         call("custom/interface/close", request)
 
     async def close_async(
             self
     ) -> None:
         """
         Closes the transport.
         Also closes the connection using the transport.
         """
-        request = main_pb2.CustomInterfaceCloseRequest()
-        request.transport_id = self.transport_id
+        request = dto.CustomInterfaceCloseRequest(
+            transport_id=self.transport_id,
+        )
         await call_async("custom/interface/close", request)
 
     def close_with_error(
             self,
             error_message: str
     ) -> None:
         """
         Closes the transport with error.
         Also closes the connection using the transport propagating the error.
 
         Args:
             error_message: Error to be propagated.
         """
-        request = main_pb2.CustomInterfaceCloseRequest()
-        request.transport_id = self.transport_id
-        request.error_message = error_message
+        request = dto.CustomInterfaceCloseRequest(
+            transport_id=self.transport_id,
+            error_message=error_message,
+        )
         call("custom/interface/close", request)
 
     async def close_with_error_async(
             self,
             error_message: str
     ) -> None:
         """
         Closes the transport with error.
         Also closes the connection using the transport propagating the error.
 
         Args:
             error_message: Error to be propagated.
         """
-        request = main_pb2.CustomInterfaceCloseRequest()
-        request.transport_id = self.transport_id
-        request.error_message = error_message
+        request = dto.CustomInterfaceCloseRequest(
+            transport_id=self.transport_id,
+            error_message=error_message,
+        )
         await call_async("custom/interface/close", request)
 
     def write(
             self,
             message: str
     ) -> None:
         """
         Writes a single message to the connection.
         The message will be processed as a reply from the device.
 
         Args:
             message: Single message of Zaber ASCII protocol.
         """
-        request = main_pb2.CustomInterfaceWriteRequest()
-        request.transport_id = self.transport_id
-        request.message = message
+        request = dto.CustomInterfaceWriteRequest(
+            transport_id=self.transport_id,
+            message=message,
+        )
         call("custom/interface/write", request)
 
     async def write_async(
             self,
             message: str
     ) -> None:
         """
         Writes a single message to the connection.
         The message will be processed as a reply from the device.
 
         Args:
             message: Single message of Zaber ASCII protocol.
         """
-        request = main_pb2.CustomInterfaceWriteRequest()
-        request.transport_id = self.transport_id
-        request.message = message
+        request = dto.CustomInterfaceWriteRequest(
+            transport_id=self.transport_id,
+            message=message,
+        )
         await call_async("custom/interface/write", request)
 
     def read(
             self
     ) -> str:
         """
         Reads a single message generated by the connection.
         The message is a request for the device.
         Read should be called continuously in a loop to ensure all generated messages are processed.
         Subsequent read call confirms that previous message was delivered to the device.
 
         Returns:
             Message generated by the connection.
         """
-        request = main_pb2.CustomInterfaceReadRequest()
-        request.transport_id = self.transport_id
-        response = main_pb2.StringResponse()
-        call("custom/interface/read", request, response)
+        request = dto.CustomInterfaceReadRequest(
+            transport_id=self.transport_id,
+        )
+        response = call(
+            "custom/interface/read",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     async def read_async(
             self
     ) -> str:
         """
         Reads a single message generated by the connection.
         The message is a request for the device.
         Read should be called continuously in a loop to ensure all generated messages are processed.
         Subsequent read call confirms that previous message was delivered to the device.
 
         Returns:
             Message generated by the connection.
         """
-        request = main_pb2.CustomInterfaceReadRequest()
-        request.transport_id = self.transport_id
-        response = main_pb2.StringResponse()
-        await call_async("custom/interface/read", request, response)
+        request = dto.CustomInterfaceReadRequest(
+            transport_id=self.transport_id,
+        )
+        response = await call_async(
+            "custom/interface/read",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def __enter__(self) -> 'Transport':
         """ __enter__ """
         return self
 
     def __exit__(self, _type: Any, _value: Any, _traceback: Any) -> None:
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/trigger.py` & `zaber_motion-6.0.0/zaber_motion/ascii/trigger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from ..call import call, call_async
-from ..units import Units, LengthUnits, units_from_literals, UnitsAndLiterals, TimeUnits
-from .trigger_state import TriggerState
-from .trigger_enabled_state import TriggerEnabledState
-from .io_port_type import IoPortType
-from .trigger_condition import TriggerCondition
-from .trigger_action import TriggerAction
-from .trigger_operation import TriggerOperation
+from ..units import Units, LengthUnits, UnitsAndLiterals, TimeUnits
+from ..dto.ascii.trigger_state import TriggerState
+from ..dto.ascii.trigger_enabled_state import TriggerEnabledState
+from ..dto.ascii.io_port_type import IoPortType
+from ..dto.ascii.trigger_condition import TriggerCondition
+from ..dto.ascii.trigger_action import TriggerAction
+from ..dto.ascii.trigger_operation import TriggerOperation
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class Trigger:
     """
@@ -53,19 +53,20 @@
         Args:
             count: Number of times the trigger will fire before disabling itself.
                 If count is not specified, or 0, the trigger will fire indefinitely.
         """
         if count < 0:
             raise ValueError('Invalid value; count must be 0 or positive.')
 
-        request = main_pb2.TriggerEnableRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.count = count
+        request = dto.TriggerEnableRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            count=count,
+        )
         call("trigger/enable", request)
 
     async def enable_async(
             self,
             count: int = 0
     ) -> None:
         """
@@ -76,147 +77,164 @@
         Args:
             count: Number of times the trigger will fire before disabling itself.
                 If count is not specified, or 0, the trigger will fire indefinitely.
         """
         if count < 0:
             raise ValueError('Invalid value; count must be 0 or positive.')
 
-        request = main_pb2.TriggerEnableRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.count = count
+        request = dto.TriggerEnableRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            count=count,
+        )
         await call_async("trigger/enable", request)
 
     def disable(
             self
     ) -> None:
         """
         Disables the trigger.
         Once disabled, the trigger will not fire and trigger actions will not run, even if trigger conditions are met.
         """
-        request = main_pb2.TriggerEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
+        request = dto.TriggerEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+        )
         call("trigger/disable", request)
 
     async def disable_async(
             self
     ) -> None:
         """
         Disables the trigger.
         Once disabled, the trigger will not fire and trigger actions will not run, even if trigger conditions are met.
         """
-        request = main_pb2.TriggerEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
+        request = dto.TriggerEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+        )
         await call_async("trigger/disable", request)
 
     def get_state(
             self
     ) -> TriggerState:
         """
         Gets the state of the trigger.
 
         Returns:
             Complete state of the trigger.
         """
-        request = main_pb2.TriggerEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        response = main_pb2.TriggerState()
-        call("trigger/get_state", request, response)
-        return TriggerState.from_protobuf(response)
+        request = dto.TriggerEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+        )
+        response = call(
+            "trigger/get_state",
+            request,
+            TriggerState.from_binary)
+        return response
 
     async def get_state_async(
             self
     ) -> TriggerState:
         """
         Gets the state of the trigger.
 
         Returns:
             Complete state of the trigger.
         """
-        request = main_pb2.TriggerEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        response = main_pb2.TriggerState()
-        await call_async("trigger/get_state", request, response)
-        return TriggerState.from_protobuf(response)
+        request = dto.TriggerEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+        )
+        response = await call_async(
+            "trigger/get_state",
+            request,
+            TriggerState.from_binary)
+        return response
 
     def get_enabled_state(
             self
     ) -> TriggerEnabledState:
         """
         Gets the enabled state of the trigger.
 
         Returns:
             Whether the trigger is enabled and the number of times it will fire.
         """
-        request = main_pb2.TriggerEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        response = main_pb2.TriggerEnabledState()
-        call("trigger/get_enabled_state", request, response)
-        return TriggerEnabledState.from_protobuf(response)
+        request = dto.TriggerEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+        )
+        response = call(
+            "trigger/get_enabled_state",
+            request,
+            TriggerEnabledState.from_binary)
+        return response
 
     async def get_enabled_state_async(
             self
     ) -> TriggerEnabledState:
         """
         Gets the enabled state of the trigger.
 
         Returns:
             Whether the trigger is enabled and the number of times it will fire.
         """
-        request = main_pb2.TriggerEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        response = main_pb2.TriggerEnabledState()
-        await call_async("trigger/get_enabled_state", request, response)
-        return TriggerEnabledState.from_protobuf(response)
+        request = dto.TriggerEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+        )
+        response = await call_async(
+            "trigger/get_enabled_state",
+            request,
+            TriggerEnabledState.from_binary)
+        return response
 
     def fire_when(
             self,
             condition: str
     ) -> None:
         """
         Set a generic trigger condition.
 
         Args:
             condition: The condition to set for this trigger.
         """
-        request = main_pb2.TriggerFireWhenRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.condition = condition
+        request = dto.TriggerFireWhenRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            condition=condition,
+        )
         call("trigger/fire_when", request)
 
     async def fire_when_async(
             self,
             condition: str
     ) -> None:
         """
         Set a generic trigger condition.
 
         Args:
             condition: The condition to set for this trigger.
         """
-        request = main_pb2.TriggerFireWhenRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.condition = condition
+        request = dto.TriggerFireWhenRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            condition=condition,
+        )
         await call_async("trigger/fire_when", request)
 
     def fire_when_encoder_distance_travelled(
             self,
             axis: int,
             distance: float,
             unit: LengthUnits = Units.NATIVE
@@ -229,21 +247,22 @@
                 May be set to 0 on single-axis devices only.
             distance: The measured encoder distance between trigger fires.
             unit: Units of dist.
         """
         if distance <= 0:
             raise ValueError('Invalid value; encoder distance must be a positive value.')
 
-        request = main_pb2.TriggerFireWhenDistanceTravelledRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.axis = axis
-        request.distance = distance
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerFireWhenDistanceTravelledRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            axis=axis,
+            distance=distance,
+            unit=unit,
+        )
         call("trigger/fire_when_encoder_distance_travelled", request)
 
     async def fire_when_encoder_distance_travelled_async(
             self,
             axis: int,
             distance: float,
             unit: LengthUnits = Units.NATIVE
@@ -256,21 +275,22 @@
                 May be set to 0 on single-axis devices only.
             distance: The measured encoder distance between trigger fires.
             unit: Units of dist.
         """
         if distance <= 0:
             raise ValueError('Invalid value; encoder distance must be a positive value.')
 
-        request = main_pb2.TriggerFireWhenDistanceTravelledRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.axis = axis
-        request.distance = distance
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerFireWhenDistanceTravelledRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            axis=axis,
+            distance=distance,
+            unit=unit,
+        )
         await call_async("trigger/fire_when_encoder_distance_travelled", request)
 
     def fire_when_distance_travelled(
             self,
             axis: int,
             distance: float,
             unit: LengthUnits = Units.NATIVE
@@ -283,21 +303,22 @@
                 May be set to 0 on single-axis devices only.
             distance: The measured distance between trigger fires.
             unit: Units of dist.
         """
         if distance <= 0:
             raise ValueError('Invalid value; distance must be a positive value.')
 
-        request = main_pb2.TriggerFireWhenDistanceTravelledRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.axis = axis
-        request.distance = distance
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerFireWhenDistanceTravelledRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            axis=axis,
+            distance=distance,
+            unit=unit,
+        )
         call("trigger/fire_when_distance_travelled", request)
 
     async def fire_when_distance_travelled_async(
             self,
             axis: int,
             distance: float,
             unit: LengthUnits = Units.NATIVE
@@ -310,21 +331,22 @@
                 May be set to 0 on single-axis devices only.
             distance: The measured distance between trigger fires.
             unit: Units of dist.
         """
         if distance <= 0:
             raise ValueError('Invalid value; distance must be a positive value.')
 
-        request = main_pb2.TriggerFireWhenDistanceTravelledRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.axis = axis
-        request.distance = distance
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerFireWhenDistanceTravelledRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            axis=axis,
+            distance=distance,
+            unit=unit,
+        )
         await call_async("trigger/fire_when_distance_travelled", request)
 
     def fire_when_io(
             self,
             port_type: IoPortType,
             channel: int,
             trigger_condition: TriggerCondition,
@@ -338,22 +360,23 @@
             channel: The IO channel to monitor.
             trigger_condition: Comparison operator.
             value: Comparison value.
         """
         if channel <= 0:
             raise ValueError('Invalid value; channel must be a positive value.')
 
-        request = main_pb2.TriggerFireWhenIoRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.port_type = port_type.value
-        request.channel = channel
-        request.trigger_condition = trigger_condition.value
-        request.value = value
+        request = dto.TriggerFireWhenIoRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            port_type=port_type,
+            channel=channel,
+            trigger_condition=trigger_condition,
+            value=value,
+        )
         call("trigger/fire_when_io", request)
 
     async def fire_when_io_async(
             self,
             port_type: IoPortType,
             channel: int,
             trigger_condition: TriggerCondition,
@@ -367,22 +390,23 @@
             channel: The IO channel to monitor.
             trigger_condition: Comparison operator.
             value: Comparison value.
         """
         if channel <= 0:
             raise ValueError('Invalid value; channel must be a positive value.')
 
-        request = main_pb2.TriggerFireWhenIoRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.port_type = port_type.value
-        request.channel = channel
-        request.trigger_condition = trigger_condition.value
-        request.value = value
+        request = dto.TriggerFireWhenIoRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            port_type=port_type,
+            channel=channel,
+            trigger_condition=trigger_condition,
+            value=value,
+        )
         await call_async("trigger/fire_when_io", request)
 
     def fire_when_setting(
             self,
             axis: int,
             setting: str,
             trigger_condition: TriggerCondition,
@@ -396,23 +420,24 @@
             axis: The axis to monitor for this condition.
                 Set to 0 for device-scope settings.
             setting: The setting to monitor.
             trigger_condition: Comparison operator.
             value: Comparison value.
             unit: Units of value.
         """
-        request = main_pb2.TriggerFireWhenSettingRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.axis = axis
-        request.setting = setting
-        request.trigger_condition = trigger_condition.value
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerFireWhenSettingRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            axis=axis,
+            setting=setting,
+            trigger_condition=trigger_condition,
+            value=value,
+            unit=unit,
+        )
         call("trigger/fire_when_setting", request)
 
     async def fire_when_setting_async(
             self,
             axis: int,
             setting: str,
             trigger_condition: TriggerCondition,
@@ -426,23 +451,24 @@
             axis: The axis to monitor for this condition.
                 Set to 0 for device-scope settings.
             setting: The setting to monitor.
             trigger_condition: Comparison operator.
             value: Comparison value.
             unit: Units of value.
         """
-        request = main_pb2.TriggerFireWhenSettingRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.axis = axis
-        request.setting = setting
-        request.trigger_condition = trigger_condition.value
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerFireWhenSettingRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            axis=axis,
+            setting=setting,
+            trigger_condition=trigger_condition,
+            value=value,
+            unit=unit,
+        )
         await call_async("trigger/fire_when_setting", request)
 
     def fire_at_interval(
             self,
             interval: float,
             unit: TimeUnits = Units.NATIVE
     ) -> None:
@@ -452,20 +478,21 @@
         Args:
             interval: The time interval between trigger fires.
             unit: Units of time.
         """
         if interval <= 0:
             raise ValueError('Invalid value; interval must be a positive value.')
 
-        request = main_pb2.TriggerFireAtIntervalRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.interval = interval
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerFireAtIntervalRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            interval=interval,
+            unit=unit,
+        )
         call("trigger/fire_at_interval", request)
 
     async def fire_at_interval_async(
             self,
             interval: float,
             unit: TimeUnits = Units.NATIVE
     ) -> None:
@@ -475,20 +502,21 @@
         Args:
             interval: The time interval between trigger fires.
             unit: Units of time.
         """
         if interval <= 0:
             raise ValueError('Invalid value; interval must be a positive value.')
 
-        request = main_pb2.TriggerFireAtIntervalRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.interval = interval
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerFireAtIntervalRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            interval=interval,
+            unit=unit,
+        )
         await call_async("trigger/fire_at_interval", request)
 
     def on_fire(
             self,
             action: TriggerAction,
             axis: int,
             command: str
@@ -498,21 +526,22 @@
 
         Args:
             action: The action number to assign the command to.
             axis: The axis to on which to run this command.
                 Set to 0 for device-scope settings or to run command on all axes.
             command: The command to run when the action is triggered.
         """
-        request = main_pb2.TriggerOnFireRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.action = action.value
-        request.axis = axis
-        request.command = command
+        request = dto.TriggerOnFireRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            action=action,
+            axis=axis,
+            command=command,
+        )
         call("trigger/on_fire", request)
 
     async def on_fire_async(
             self,
             action: TriggerAction,
             axis: int,
             command: str
@@ -522,21 +551,22 @@
 
         Args:
             action: The action number to assign the command to.
             axis: The axis to on which to run this command.
                 Set to 0 for device-scope settings or to run command on all axes.
             command: The command to run when the action is triggered.
         """
-        request = main_pb2.TriggerOnFireRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.action = action.value
-        request.axis = axis
-        request.command = command
+        request = dto.TriggerOnFireRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            action=action,
+            axis=axis,
+            command=command,
+        )
         await call_async("trigger/on_fire", request)
 
     def on_fire_set(
             self,
             action: TriggerAction,
             axis: int,
             setting: str,
@@ -552,24 +582,25 @@
             axis: The axis on which to change the setting.
                 Set to 0 to change the setting for the device.
             setting: The name of the setting to change.
             operation: The operation to apply to the setting.
             value: Operation value.
             unit: Units of value.
         """
-        request = main_pb2.TriggerOnFireSetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.action = action.value
-        request.axis = axis
-        request.setting = setting
-        request.operation = operation.value
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerOnFireSetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            action=action,
+            axis=axis,
+            setting=setting,
+            operation=operation,
+            value=value,
+            unit=unit,
+        )
         call("trigger/on_fire_set", request)
 
     async def on_fire_set_async(
             self,
             action: TriggerAction,
             axis: int,
             setting: str,
@@ -585,24 +616,25 @@
             axis: The axis on which to change the setting.
                 Set to 0 to change the setting for the device.
             setting: The name of the setting to change.
             operation: The operation to apply to the setting.
             value: Operation value.
             unit: Units of value.
         """
-        request = main_pb2.TriggerOnFireSetRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.action = action.value
-        request.axis = axis
-        request.setting = setting
-        request.operation = operation.value
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.TriggerOnFireSetRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            action=action,
+            axis=axis,
+            setting=setting,
+            operation=operation,
+            value=value,
+            unit=unit,
+        )
         await call_async("trigger/on_fire_set", request)
 
     def on_fire_set_to_setting(
             self,
             action: TriggerAction,
             axis: int,
             setting: str,
@@ -621,24 +653,25 @@
                 Must have either integer or boolean type.
             operation: The operation to apply to the setting.
             from_axis: The axis from which to read the setting.
                 Set to 0 to read the setting from the device.
             from_setting: The name of the setting to read.
                 Must have either integer or boolean type.
         """
-        request = main_pb2.TriggerOnFireSetToSettingRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.action = action.value
-        request.axis = axis
-        request.setting = setting
-        request.operation = operation.value
-        request.from_axis = from_axis
-        request.from_setting = from_setting
+        request = dto.TriggerOnFireSetToSettingRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            action=action,
+            axis=axis,
+            setting=setting,
+            operation=operation,
+            from_axis=from_axis,
+            from_setting=from_setting,
+        )
         call("trigger/on_fire_set_to_setting", request)
 
     async def on_fire_set_to_setting_async(
             self,
             action: TriggerAction,
             axis: int,
             setting: str,
@@ -657,54 +690,57 @@
                 Must have either integer or boolean type.
             operation: The operation to apply to the setting.
             from_axis: The axis from which to read the setting.
                 Set to 0 to read the setting from the device.
             from_setting: The name of the setting to read.
                 Must have either integer or boolean type.
         """
-        request = main_pb2.TriggerOnFireSetToSettingRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.action = action.value
-        request.axis = axis
-        request.setting = setting
-        request.operation = operation.value
-        request.from_axis = from_axis
-        request.from_setting = from_setting
+        request = dto.TriggerOnFireSetToSettingRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            action=action,
+            axis=axis,
+            setting=setting,
+            operation=operation,
+            from_axis=from_axis,
+            from_setting=from_setting,
+        )
         await call_async("trigger/on_fire_set_to_setting", request)
 
     def clear_action(
             self,
             action: TriggerAction = TriggerAction.ALL
     ) -> None:
         """
         Clear a trigger action.
 
         Args:
             action: The action number to clear.
                 The default option is to clear all actions.
         """
-        request = main_pb2.TriggerClearActionRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.action = action.value
+        request = dto.TriggerClearActionRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            action=action,
+        )
         call("trigger/clear_action", request)
 
     async def clear_action_async(
             self,
             action: TriggerAction = TriggerAction.ALL
     ) -> None:
         """
         Clear a trigger action.
 
         Args:
             action: The action number to clear.
                 The default option is to clear all actions.
         """
-        request = main_pb2.TriggerClearActionRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.trigger_number = self.trigger_number
-        request.action = action.value
+        request = dto.TriggerClearActionRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            trigger_number=self.trigger_number,
+            action=action,
+        )
         await call_async("trigger/clear_action", request)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/trigger_state.py` & `zaber_motion-6.0.0/zaber_motion/dto/ascii/trigger_enabled_state.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,55 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
-from typing import List  # pylint: disable=unused-import
-from ..protobufs import main_pb2
 
-
-class TriggerState:
+@dataclass
+class TriggerEnabledState:
     """
-    The complete state of a trigger.
+    The enabled state of a single trigger.
+    Returns whether the given trigger is enabled and the number of times it will fire.
+    This is a subset of the complete state, and is faster to query.
     """
 
-    @property
-    def condition(self) -> str:
-        """
-        The firing condition for a trigger.
-        """
-
-        return self._condition
-
-    @condition.setter
-    def condition(self, value: str) -> None:
-        self._condition = value
-
-    @property
-    def actions(self) -> List[str]:
-        """
-        The actions for a trigger.
-        """
-
-        return self._actions
-
-    @actions.setter
-    def actions(self, value: List[str]) -> None:
-        self._actions = value
-
-    @property
-    def enabled(self) -> bool:
-        """
-        The enabled state for a trigger.
-        """
-
-        return self._enabled
-
-    @enabled.setter
-    def enabled(self, value: bool) -> None:
-        self._enabled = value
-
-    @property
-    def fires_total(self) -> int:
-        """
-        The number of total fires for this trigger.
-        A value of -1 indicates unlimited fires.
-        """
-
-        return self._fires_total
-
-    @fires_total.setter
-    def fires_total(self, value: int) -> None:
-        self._fires_total = value
-
-    @property
-    def fires_remaining(self) -> int:
-        """
-        The number of remaining fires for this trigger.
-        A value of -1 indicates unlimited fires remaining.
-        """
+    enabled: bool
+    """
+    The enabled state for a trigger.
+    """
 
-        return self._fires_remaining
+    fires_remaining: int
+    """
+    The number of remaining fires for this trigger.
+    A value of -1 indicates unlimited fires remaining.
+    """
 
-    @fires_remaining.setter
-    def fires_remaining(self, value: int) -> None:
-        self._fires_remaining = value
+    @staticmethod
+    def zero_values() -> 'TriggerEnabledState':
+        return TriggerEnabledState(
+            enabled=False,
+            fires_remaining=0,
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'TriggerEnabledState':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return TriggerEnabledState.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'enabled': self.enabled,
+            'firesRemaining': self.fires_remaining,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.TriggerState
-    ) -> 'TriggerState':
-        instance = TriggerState.__new__(
-            TriggerState
-        )  # type: TriggerState
-        instance.condition = pb_data.condition
-        instance.actions = list(pb_data.actions)
-        instance.enabled = pb_data.enabled
-        instance.fires_total = pb_data.fires_total
-        instance.fires_remaining = pb_data.fires_remaining
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'TriggerEnabledState':
+        return TriggerEnabledState(
+            enabled=data.get('enabled'),  # type: ignore
+            fires_remaining=data.get('firesRemaining'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/ascii/warning_flags.py` & `zaber_motion-6.0.0/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.2/zaber_motion/async_utils.py` & `zaber_motion-6.0.0/zaber_motion/async_utils.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.2/zaber_motion/binary/binary_settings.py` & `zaber_motion-6.0.0/zaber_motion/dto/binary/binary_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
+# This file is generated. Do not modify by hand.
 from enum import Enum
 
 
 class BinarySettings(Enum):
     """
     Named constants for all Zaber Binary protocol settings.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/binary/command_code.py` & `zaber_motion-6.0.0/zaber_motion/dto/binary/command_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
+# This file is generated. Do not modify by hand.
 from enum import Enum
 
 
 class CommandCode(Enum):
     """
     Named constants for all Zaber Binary protocol commands.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/binary/device.py` & `zaber_motion-6.0.0/zaber_motion/binary/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 # pylint: disable=too-many-arguments
 
 from typing import TYPE_CHECKING
 from ..call import call, call_async, call_sync
 
-from ..protobufs import main_pb2
-from .binary_settings import BinarySettings
-from .device_identity import DeviceIdentity
+from ..dto import requests as dto
+from ..dto.binary.binary_settings import BinarySettings
+from ..dto.binary.device_identity import DeviceIdentity
 from .device_settings import DeviceSettings
-from .command_code import CommandCode
-from .message import Message
-from ..units import UnitsAndLiterals, Units, units_from_literals, LengthUnits, VelocityUnits
-from .device_type import DeviceType
-from ..firmware_version import FirmwareVersion
+from ..dto.binary.command_code import CommandCode
+from ..dto.binary.message import Message
+from ..units import UnitsAndLiterals, Units, LengthUnits, VelocityUnits
+from ..dto.binary.device_type import DeviceType
+from ..dto.firmware_version import FirmwareVersion
 
 if TYPE_CHECKING:
     from .connection import Connection
 
 
 class Device:
     """
@@ -145,24 +145,27 @@
             data: Optional data argument to the command. Defaults to zero.
             timeout: Number of seconds to wait for a response from the device. 0 or negative defaults to 0.5s.
             check_errors: Controls whether to throw an exception when the device rejects the command.
 
         Returns:
             A response to the command.
         """
-        request = main_pb2.GenericBinaryRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command.value
-        request.data = data
-        request.timeout = timeout
-        request.check_errors = check_errors
-        response = main_pb2.BinaryMessage()
-        call("binary/interface/generic_command", request, response)
-        return Message.from_protobuf(response)
+        request = dto.GenericBinaryRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            data=data,
+            timeout=timeout,
+            check_errors=check_errors,
+        )
+        response = call(
+            "binary/interface/generic_command",
+            request,
+            Message.from_binary)
+        return response
 
     async def generic_command_async(
             self,
             command: CommandCode,
             data: int = 0,
             timeout: float = 0.0,
             check_errors: bool = True
@@ -177,24 +180,27 @@
             data: Optional data argument to the command. Defaults to zero.
             timeout: Number of seconds to wait for a response from the device. 0 or negative defaults to 0.5s.
             check_errors: Controls whether to throw an exception when the device rejects the command.
 
         Returns:
             A response to the command.
         """
-        request = main_pb2.GenericBinaryRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command.value
-        request.data = data
-        request.timeout = timeout
-        request.check_errors = check_errors
-        response = main_pb2.BinaryMessage()
-        await call_async("binary/interface/generic_command", request, response)
-        return Message.from_protobuf(response)
+        request = dto.GenericBinaryRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            data=data,
+            timeout=timeout,
+            check_errors=check_errors,
+        )
+        response = await call_async(
+            "binary/interface/generic_command",
+            request,
+            Message.from_binary)
+        return response
 
     def generic_command_no_response(
             self,
             command: CommandCode,
             data: int = 0
     ) -> None:
         """
@@ -202,19 +208,20 @@
         For more information please refer to the
         [Binary Protocol Manual](https://www.zaber.com/protocol-manual?protocol=Binary#topic_quick_command_reference).
 
         Args:
             command: Command to send.
             data: Optional data argument to the command. Defaults to zero.
         """
-        request = main_pb2.GenericBinaryRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command.value
-        request.data = data
+        request = dto.GenericBinaryRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            data=data,
+        )
         call("binary/interface/generic_command_no_response", request)
 
     async def generic_command_no_response_async(
             self,
             command: CommandCode,
             data: int = 0
     ) -> None:
@@ -223,19 +230,20 @@
         For more information please refer to the
         [Binary Protocol Manual](https://www.zaber.com/protocol-manual?protocol=Binary#topic_quick_command_reference).
 
         Args:
             command: Command to send.
             data: Optional data argument to the command. Defaults to zero.
         """
-        request = main_pb2.GenericBinaryRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command.value
-        request.data = data
+        request = dto.GenericBinaryRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            data=data,
+        )
         await call_async("binary/interface/generic_command_no_response", request)
 
     def generic_command_with_units(
             self,
             command: CommandCode,
             data: float = 0,
             from_unit: UnitsAndLiterals = Units.NATIVE,
@@ -251,24 +259,27 @@
             from_unit: Unit to convert sent data from.
             to_unit: Unit to convert retrieved data to.
             timeout: Number of seconds to wait for a response from the device. 0 or negative defaults to 0.5s.
 
         Returns:
             Data that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryGenericWithUnitsRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command.value
-        request.data = data
-        request.from_unit = units_from_literals(from_unit).value
-        request.to_unit = units_from_literals(to_unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        call("binary/device/generic_command_with_units", request, response)
+        request = dto.BinaryGenericWithUnitsRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            data=data,
+            from_unit=from_unit,
+            to_unit=to_unit,
+            timeout=timeout,
+        )
+        response = call(
+            "binary/device/generic_command_with_units",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def generic_command_with_units_async(
             self,
             command: CommandCode,
             data: float = 0,
             from_unit: UnitsAndLiterals = Units.NATIVE,
@@ -284,24 +295,27 @@
             from_unit: Unit to convert sent data from.
             to_unit: Unit to convert retrieved data to.
             timeout: Number of seconds to wait for a response from the device. 0 or negative defaults to 0.5s.
 
         Returns:
             Data that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryGenericWithUnitsRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.command = command.value
-        request.data = data
-        request.from_unit = units_from_literals(from_unit).value
-        request.to_unit = units_from_literals(to_unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        await call_async("binary/device/generic_command_with_units", request, response)
+        request = dto.BinaryGenericWithUnitsRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            command=command,
+            data=data,
+            from_unit=from_unit,
+            to_unit=to_unit,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "binary/device/generic_command_with_units",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def home(
             self,
             unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
@@ -311,21 +325,24 @@
         Args:
             unit: Unit to convert returned position to.
             timeout: Number of seconds to wait for response from the device chain (defaults to 60s).
 
         Returns:
             Current position that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceHomeRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.unit = units_from_literals(unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        call("binary/device/home", request, response)
+        request = dto.BinaryDeviceHomeRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            unit=unit,
+            timeout=timeout,
+        )
+        response = call(
+            "binary/device/home",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def home_async(
             self,
             unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
@@ -335,21 +352,24 @@
         Args:
             unit: Unit to convert returned position to.
             timeout: Number of seconds to wait for response from the device chain (defaults to 60s).
 
         Returns:
             Current position that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceHomeRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.unit = units_from_literals(unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        await call_async("binary/device/home", request, response)
+        request = dto.BinaryDeviceHomeRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            unit=unit,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "binary/device/home",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def stop(
             self,
             unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
@@ -359,21 +379,24 @@
         Args:
             unit: Unit to convert returned position to.
             timeout: Number of seconds to wait for response from the device chain (defaults to 60s).
 
         Returns:
             Current position that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceStopRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.unit = units_from_literals(unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        call("binary/device/stop", request, response)
+        request = dto.BinaryDeviceStopRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            unit=unit,
+            timeout=timeout,
+        )
+        response = call(
+            "binary/device/stop",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def stop_async(
             self,
             unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
@@ -383,21 +406,24 @@
         Args:
             unit: Unit to convert returned position to.
             timeout: Number of seconds to wait for response from the device chain (defaults to 60s).
 
         Returns:
             Current position that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceStopRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.unit = units_from_literals(unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        await call_async("binary/device/stop", request, response)
+        request = dto.BinaryDeviceStopRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            unit=unit,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "binary/device/stop",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def move_absolute(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
@@ -409,23 +435,26 @@
             position: Absolute position.
             unit: Unit for the provided position as well as position returned by the device.
             timeout: Number of seconds to wait for response from the device chain (defaults to 60s).
 
         Returns:
             Current position that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceMoveRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.type = main_pb2.BinaryDeviceMoveRequest.ABS
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        call("binary/device/move", request, response)
+        request = dto.BinaryDeviceMoveRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            type=dto.AxisMoveType.ABS,
+            arg=position,
+            unit=unit,
+            timeout=timeout,
+        )
+        response = call(
+            "binary/device/move",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def move_absolute_async(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
@@ -437,23 +466,26 @@
             position: Absolute position.
             unit: Unit for the provided position as well as position returned by the device.
             timeout: Number of seconds to wait for response from the device chain (defaults to 60s).
 
         Returns:
             Current position that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceMoveRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.type = main_pb2.BinaryDeviceMoveRequest.ABS
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        await call_async("binary/device/move", request, response)
+        request = dto.BinaryDeviceMoveRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            type=dto.AxisMoveType.ABS,
+            arg=position,
+            unit=unit,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "binary/device/move",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def move_relative(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
@@ -465,23 +497,26 @@
             position: Relative position.
             unit: Unit for the provided position as well as position returned by the device.
             timeout: Number of seconds to wait for response from the device chain (defaults to 60s).
 
         Returns:
             Current position that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceMoveRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.type = main_pb2.BinaryDeviceMoveRequest.REL
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        call("binary/device/move", request, response)
+        request = dto.BinaryDeviceMoveRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            type=dto.AxisMoveType.REL,
+            arg=position,
+            unit=unit,
+            timeout=timeout,
+        )
+        response = call(
+            "binary/device/move",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def move_relative_async(
             self,
             position: float,
             unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
@@ -493,23 +528,26 @@
             position: Relative position.
             unit: Unit for the provided position as well as position returned by the device.
             timeout: Number of seconds to wait for response from the device chain (defaults to 60s).
 
         Returns:
             Current position that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceMoveRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.type = main_pb2.BinaryDeviceMoveRequest.REL
-        request.arg = position
-        request.unit = units_from_literals(unit).value
-        request.timeout = timeout
-        response = main_pb2.DoubleResponse()
-        await call_async("binary/device/move", request, response)
+        request = dto.BinaryDeviceMoveRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            type=dto.AxisMoveType.REL,
+            arg=position,
+            unit=unit,
+            timeout=timeout,
+        )
+        response = await call_async(
+            "binary/device/move",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def move_velocity(
             self,
             velocity: float,
             unit: VelocityUnits = Units.NATIVE
     ) -> float:
@@ -519,22 +557,25 @@
         Args:
             velocity: Movement velocity.
             unit: Unit to convert returned velocity to.
 
         Returns:
             Device velocity that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceMoveRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.type = main_pb2.BinaryDeviceMoveRequest.VEL
-        request.arg = velocity
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("binary/device/move", request, response)
+        request = dto.BinaryDeviceMoveRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            type=dto.AxisMoveType.VEL,
+            arg=velocity,
+            unit=unit,
+        )
+        response = call(
+            "binary/device/move",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def move_velocity_async(
             self,
             velocity: float,
             unit: VelocityUnits = Units.NATIVE
     ) -> float:
@@ -544,198 +585,225 @@
         Args:
             velocity: Movement velocity.
             unit: Unit to convert returned velocity to.
 
         Returns:
             Device velocity that has been converted to the provided unit.
         """
-        request = main_pb2.BinaryDeviceMoveRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.type = main_pb2.BinaryDeviceMoveRequest.VEL
-        request.arg = velocity
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("binary/device/move", request, response)
+        request = dto.BinaryDeviceMoveRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            type=dto.AxisMoveType.VEL,
+            arg=velocity,
+            unit=unit,
+        )
+        response = await call_async(
+            "binary/device/move",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def wait_until_idle(
             self
     ) -> None:
         """
         Waits until device stops moving.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
         call("binary/device/wait_until_idle", request)
 
     async def wait_until_idle_async(
             self
     ) -> None:
         """
         Waits until device stops moving.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
         await call_async("binary/device/wait_until_idle", request)
 
     def is_busy(
             self
     ) -> bool:
         """
         Check whether the device is moving.
 
         Returns:
             True if the device is currently executing a motion command.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BoolResponse()
-        call("binary/device/is_busy", request, response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call(
+            "binary/device/is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_busy_async(
             self
     ) -> bool:
         """
         Check whether the device is moving.
 
         Returns:
             True if the device is currently executing a motion command.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BoolResponse()
-        await call_async("binary/device/is_busy", request, response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = await call_async(
+            "binary/device/is_busy",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def identify(
             self
     ) -> DeviceIdentity:
         """
         Queries the device and the database, gathering information about the product.
         Without this information features such as unit conversions will not work.
         Usually, called automatically by detect devices method.
 
         Returns:
             Device identification data.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BinaryDeviceIdentity()
-        call("binary/device/identify", request, response)
-        return DeviceIdentity.from_protobuf(response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call(
+            "binary/device/identify",
+            request,
+            DeviceIdentity.from_binary)
+        return response
 
     async def identify_async(
             self
     ) -> DeviceIdentity:
         """
         Queries the device and the database, gathering information about the product.
         Without this information features such as unit conversions will not work.
         Usually, called automatically by detect devices method.
 
         Returns:
             Device identification data.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BinaryDeviceIdentity()
-        await call_async("binary/device/identify", request, response)
-        return DeviceIdentity.from_protobuf(response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = await call_async(
+            "binary/device/identify",
+            request,
+            DeviceIdentity.from_binary)
+        return response
 
     def park(
             self
     ) -> None:
         """
         Parks the axis.
         Motor drivers remain enabled and hold current continues to be applied until the device is powered off.
         It can later be unparked and moved without first having to home it.
         Requires at least Firmware 6.06.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
         call("binary/device/park", request)
 
     async def park_async(
             self
     ) -> None:
         """
         Parks the axis.
         Motor drivers remain enabled and hold current continues to be applied until the device is powered off.
         It can later be unparked and moved without first having to home it.
         Requires at least Firmware 6.06.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
         await call_async("binary/device/park", request)
 
     def unpark(
             self
     ) -> None:
         """
         Unparks axis. Axis will now be able to move.
         Requires at least Firmware 6.06.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
         call("binary/device/unpark", request)
 
     async def unpark_async(
             self
     ) -> None:
         """
         Unparks axis. Axis will now be able to move.
         Requires at least Firmware 6.06.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
         await call_async("binary/device/unpark", request)
 
     def is_parked(
             self
     ) -> bool:
         """
         Returns bool indicating whether the axis is parked or not.
         Requires at least Firmware 6.06.
 
         Returns:
             True if the axis is currently parked. False otherwise.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BoolResponse()
-        call("binary/device/is_parked", request, response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call(
+            "binary/device/is_parked",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_parked_async(
             self
     ) -> bool:
         """
         Returns bool indicating whether the axis is parked or not.
         Requires at least Firmware 6.06.
 
         Returns:
             True if the axis is currently parked. False otherwise.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BoolResponse()
-        await call_async("binary/device/is_parked", request, response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = await call_async(
+            "binary/device/is_parked",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def get_position(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
@@ -743,21 +811,24 @@
 
         Args:
             unit: Units of position.
 
         Returns:
             Axis position.
         """
-        request = main_pb2.BinaryDeviceGetSettingRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.setting = BinarySettings.CURRENT_POSITION.value
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("binary/device/get_setting", request, response)
+        request = dto.BinaryDeviceGetSettingRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            setting=BinarySettings.CURRENT_POSITION,
+            unit=unit,
+        )
+        response = call(
+            "binary/device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_position_async(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
@@ -765,63 +836,75 @@
 
         Args:
             unit: Units of position.
 
         Returns:
             Axis position.
         """
-        request = main_pb2.BinaryDeviceGetSettingRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        request.setting = BinarySettings.CURRENT_POSITION.value
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("binary/device/get_setting", request, response)
+        request = dto.BinaryDeviceGetSettingRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+            setting=BinarySettings.CURRENT_POSITION,
+            unit=unit,
+        )
+        response = await call_async(
+            "binary/device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the device.
 
         Returns:
             A string that represents the device.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.StringResponse()
-        call_sync("binary/device/device_to_string", request, response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call_sync(
+            "binary/device/device_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def __retrieve_identity(
             self
     ) -> DeviceIdentity:
         """
         Returns identity.
 
         Returns:
             Device identity.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BinaryDeviceIdentity()
-        call_sync("binary/device/get_identity", request, response)
-        return DeviceIdentity.from_protobuf(response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call_sync(
+            "binary/device/get_identity",
+            request,
+            DeviceIdentity.from_binary)
+        return response
 
     def __retrieve_is_identified(
             self
     ) -> bool:
         """
         Returns whether or not the device have been identified.
 
         Returns:
             True if the device has already been identified. False otherwise.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.device = self.device_address
-        response = main_pb2.BoolResponse()
-        call_sync("binary/device/get_is_identified", request, response)
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.connection.interface_id,
+            device=self.device_address,
+        )
+        response = call_sync(
+            "binary/device/get_is_identified",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/binary/device_settings.py` & `zaber_motion-6.0.0/zaber_motion/binary/device_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING
 from ..call import call, call_async
 
-from ..protobufs import main_pb2
-from ..units import UnitsAndLiterals, Units, units_from_literals
-from .binary_settings import BinarySettings
+from ..dto import requests as dto
+from ..units import UnitsAndLiterals, Units
+from ..dto.binary.binary_settings import BinarySettings
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class DeviceSettings:
     """
@@ -31,21 +31,24 @@
         Args:
             setting: Setting to get.
             unit: Units of setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.BinaryDeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting.value
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("binary/device/get_setting", request, response)
+        request = dto.BinaryDeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            unit=unit,
+        )
+        response = call(
+            "binary/device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_async(
             self,
             setting: BinarySettings,
             unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
@@ -55,21 +58,24 @@
         Args:
             setting: Setting to get.
             unit: Units of setting.
 
         Returns:
             Setting value.
         """
-        request = main_pb2.BinaryDeviceGetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting.value
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("binary/device/get_setting", request, response)
+        request = dto.BinaryDeviceGetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            unit=unit,
+        )
+        response = await call_async(
+            "binary/device/get_setting",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set(
             self,
             setting: BinarySettings,
             value: float,
             unit: UnitsAndLiterals = Units.NATIVE
@@ -78,20 +84,21 @@
         Sets any device setting.
 
         Args:
             setting: Setting to set.
             value: Value of the setting.
             unit: Units of setting.
         """
-        request = main_pb2.BinaryDeviceSetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting.value
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.BinaryDeviceSetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
         call("binary/device/set_setting", request)
 
     async def set_async(
             self,
             setting: BinarySettings,
             value: float,
             unit: UnitsAndLiterals = Units.NATIVE
@@ -100,14 +107,15 @@
         Sets any device setting.
 
         Args:
             setting: Setting to set.
             value: Value of the setting.
             unit: Units of setting.
         """
-        request = main_pb2.BinaryDeviceSetSettingRequest()
-        request.interface_id = self._device.connection.interface_id
-        request.device = self._device.device_address
-        request.setting = setting.value
-        request.value = value
-        request.unit = units_from_literals(unit).value
+        request = dto.BinaryDeviceSetSettingRequest(
+            interface_id=self._device.connection.interface_id,
+            device=self._device.device_address,
+            setting=setting,
+            value=value,
+            unit=unit,
+        )
         await call_async("binary/device/set_setting", request)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/binary/error_code.py` & `zaber_motion-6.0.0/zaber_motion/dto/binary/error_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
+# This file is generated. Do not modify by hand.
 from enum import Enum
 
 
 class ErrorCode(Enum):
     """
     Named constants for all Zaber Binary protocol error codes.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/bindings.py` & `zaber_motion-6.0.0/zaber_motion/bindings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.2/zaber_motion/call.py` & `zaber_motion-6.0.0/zaber_motion/call.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from threading import Lock
 import asyncio
 import functools
-from typing import TYPE_CHECKING, Optional, List, Set, Callable, Any  # pylint: disable=unused-import
+from typing import TYPE_CHECKING, Optional, List, Set, Callable, Any, TypeVar, overload  # pylint: disable=unused-import
 from ctypes import c_void_p, c_int64
 import queue
-from google.protobuf.message import Message
+from .dto_object import DtoObject
 
 from .convert_exception import convert_exception
-from .protobufs import main_pb2
+from .dto import requests as dto
 from .serialization import serialize, deserialize
 from .bindings import c_call, CALLBACK
 
+TResponse = TypeVar('TResponse', bound=DtoObject)  # pylint: disable=invalid-name
+
 
 class CallbackWrap:
     def __init__(self, callbackFunc: Callable[[c_void_p, c_int64], None]):
         self._callback = CALLBACK(callbackFunc)
 
     @property
     def callback(self) -> Any:
@@ -22,15 +24,36 @@
 
 
 # we must store callback in a set to prevent garbage collection in case the future gets cancelled
 callbacks: Set[CallbackWrap] = set()
 callbacks_lock = Lock()
 
 
-def call(request: str, data: Optional[Message] = None, response_data: Optional[Message] = None) -> None:
+@overload
+def call(
+    request: str,
+    data: Optional[DtoObject] = None,
+) -> None:
+    ...
+
+
+@overload
+def call(
+    request: str,
+    data: Optional[DtoObject],
+    make_response: Callable[[bytes], TResponse],
+) -> TResponse:
+    ...
+
+
+def call(
+    request: str,
+    data: Optional[DtoObject] = None,
+    make_response: Optional[Callable[[bytes], TResponse]] = None,
+) -> Optional[TResponse]:
     buffer = get_request_buffer(request, data)
 
     promise = queue.Queue(maxsize=1)  # type: ignore
 
     def callback(response_data: c_void_p, _tag: c_int64) -> None:
         resp_buffer = deserialize(response_data)
         promise.put(resp_buffer)
@@ -39,23 +62,44 @@
     result = c_call(buffer, 0, cb, 1)
 
     if result != 0:
         raise RuntimeError(f"Invalid result code: {result}")
 
     response_buffers = promise.get()
 
-    process_response(response_buffers, response_data)
+    return process_response(response_buffers, make_response)
 
 
 def set_result(future: 'asyncio.Future[List[bytes]]', resp_buffer: List[bytes]) -> None:
     if not future.done():
         future.set_result(resp_buffer)
 
 
-async def call_async(request: str, data: Optional[Message] = None, response_data: Optional[Message] = None) -> None:
+@overload
+async def call_async(
+    request: str,
+    data: Optional[DtoObject] = None,
+) -> None:
+    ...
+
+
+@overload
+async def call_async(
+    request: str,
+    data: Optional[DtoObject],
+    make_response: Callable[[bytes], TResponse],
+) -> TResponse:
+    ...
+
+
+async def call_async(
+    request: str,
+    data: Optional[DtoObject] = None,
+    make_response: Optional[Callable[[bytes], TResponse]] = None,
+) -> Optional[TResponse]:
     buffer = get_request_buffer(request, data)
 
     cb: CallbackWrap = None  # type: ignore
     loop = asyncio.get_event_loop()
     future = loop.create_future()
 
     def callback(response_data: c_void_p, _tag: c_int64) -> None:
@@ -77,55 +121,78 @@
     result = c_call(buffer, 0, cb.callback, 1)
 
     if result != 0:
         raise RuntimeError(f"Invalid result code: {result}")
 
     response_buffers = await future
 
-    process_response(response_buffers, response_data)
+    return process_response(response_buffers, make_response)
 
 
-def call_sync(request: str, data: Optional[Message] = None, response_data: Optional[Message] = None) -> None:
+@overload
+def call_sync(
+    request: str,
+    data: Optional[DtoObject] = None,
+) -> None:
+    ...
+
+
+@overload
+def call_sync(
+    request: str,
+    data: Optional[DtoObject],
+    make_response: Callable[[bytes], TResponse],
+) -> TResponse:
+    ...
+
+
+def call_sync(
+    request: str,
+    data: Optional[DtoObject] = None,
+    make_response: Optional[Callable[[bytes], TResponse]] = None,
+) -> Optional[TResponse]:
     buffer = get_request_buffer(request, data)
 
     resp_buffers = [None]  # type: Any
 
     def callback(response_data: c_void_p, _tag: c_int64) -> None:
         resp_buffers[0] = deserialize(response_data)
 
     cb = CALLBACK(callback)
     result = c_call(buffer, 0, cb, 0)
 
     if result != 0:
         raise RuntimeError(f"Invalid result code: {result}")
 
-    process_response(resp_buffers[0], response_data)
+    return process_response(resp_buffers[0], make_response)
 
 
-def get_request_buffer(request: str, data: Optional[Message]) -> bytes:
-    request_proto = main_pb2.Request()
-    request_proto.request = request
+def get_request_buffer(request: str, data: Optional[DtoObject]) -> bytes:
+    request_proto = dto.GatewayRequest(request=request)
 
-    messages = [request_proto.SerializeToString()]
+    messages = [request_proto.to_binary()]
     if data is not None:
-        messages.append(data.SerializeToString())
+        messages.append(data.to_binary())
 
     buffer = serialize(messages)
     return buffer
 
 
-def process_response(response_buffers: List[bytes], response_data: Optional[Message]) -> None:
-    response_proto = main_pb2.Response()
-    response_proto.ParseFromString(response_buffers[0])
+def process_response(
+    response_buffers: List[bytes],
+    make_response: Optional[Callable[[bytes], TResponse]],
+) -> Optional[TResponse]:
+    response_dto = dto.GatewayResponse.from_binary(response_buffers[0])
 
-    if response_proto.response != main_pb2.Response.OK:
+    if response_dto.response != dto.ResponseType.OK:
         if len(response_buffers) > 1:
-            raise convert_exception(response_proto.error_type, response_proto.error_message, response_buffers[1])
-        raise convert_exception(response_proto.error_type, response_proto.error_message)
+            raise convert_exception(response_dto.error_type, response_dto.error_message, response_buffers[1])
+        raise convert_exception(response_dto.error_type, response_dto.error_message)
 
     if len(response_buffers) > 1:
-        if response_data is None:
+        if make_response is None:
             raise RuntimeError("Response from library is ignored, response_data==None")
-        response_data.ParseFromString(response_buffers[1])
+        return make_response(response_buffers[1])
     else:
-        if response_data is not None:
+        if make_response is not None:
             raise RuntimeError("No response from library")
+        return None
```

### Comparing `zaber_motion-5.2.2/zaber_motion/convert_exception.py` & `zaber_motion-6.0.0/zaber_motion/convert_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import Optional
-from .protobufs import main_pb2
+from .dto import requests as dto
 from .exceptions.motion_lib_exception import MotionLibException
 from .exceptions.binary_command_failed_exception import BinaryCommandFailedException
 from .exceptions.command_failed_exception import CommandFailedException
 from .exceptions.command_preempted_exception import CommandPreemptedException
 from .exceptions.command_too_long_exception import CommandTooLongException
 from .exceptions.connection_closed_exception import ConnectionClosedException
 from .exceptions.connection_failed_exception import ConnectionFailedException
@@ -20,14 +20,15 @@
 from .exceptions.g_code_syntax_exception import GCodeSyntaxException
 from .exceptions.internal_error_exception import InternalErrorException
 from .exceptions.invalid_argument_exception import InvalidArgumentException
 from .exceptions.invalid_data_exception import InvalidDataException
 from .exceptions.invalid_operation_exception import InvalidOperationException
 from .exceptions.invalid_packet_exception import InvalidPacketException
 from .exceptions.invalid_park_state_exception import InvalidParkStateException
+from .exceptions.invalid_request_data_exception import InvalidRequestDataException
 from .exceptions.invalid_response_exception import InvalidResponseException
 from .exceptions.io_channel_out_of_range_exception import IoChannelOutOfRangeException
 from .exceptions.io_failed_exception import IoFailedException
 from .exceptions.lockstep_enabled_exception import LockstepEnabledException
 from .exceptions.lockstep_not_enabled_exception import LockstepNotEnabledException
 from .exceptions.movement_failed_exception import MovementFailedException
 from .exceptions.movement_interrupted_exception import MovementInterruptedException
@@ -76,14 +77,15 @@
     "G_CODE_SYNTAX": GCodeSyntaxException,
     "INTERNAL_ERROR": InternalErrorException,
     "INVALID_ARGUMENT": InvalidArgumentException,
     "INVALID_DATA": InvalidDataException,
     "INVALID_OPERATION": InvalidOperationException,
     "INVALID_PACKET": InvalidPacketException,
     "INVALID_PARK_STATE": InvalidParkStateException,
+    "INVALID_REQUEST_DATA": InvalidRequestDataException,
     "INVALID_RESPONSE": InvalidResponseException,
     "IO_CHANNEL_OUT_OF_RANGE": IoChannelOutOfRangeException,
     "IO_FAILED": IoFailedException,
     "LOCKSTEP_ENABLED": LockstepEnabledException,
     "LOCKSTEP_NOT_ENABLED": LockstepNotEnabledException,
     "MOVEMENT_FAILED": MovementFailedException,
     "MOVEMENT_INTERRUPTED": MovementInterruptedException,
@@ -112,11 +114,11 @@
     "STREAM_SETUP_FAILED": StreamSetupFailedException,
     "TIMEOUT": TimeoutException,
     "TRANSPORT_ALREADY_USED": TransportAlreadyUsedException,
     "UNKNOWN_REQUEST": UnknownRequestException,
 }
 
 
-def convert_exception(error_type: int, message: str, custom_data: Optional[bytes] = None) -> MotionLibException:
+def convert_exception(error_type: dto.Errors, message: str, custom_data: Optional[bytes] = None) -> MotionLibException:
     if custom_data:
-        return errorMap[main_pb2.Errors.Name(error_type)](message, custom_data)  # type: ignore
-    return errorMap[main_pb2.Errors.Name(error_type)](message)  # type: ignore
+        return errorMap[error_type.name](message, custom_data)  # type: ignore
+    return errorMap[error_type.name](message)  # type: ignore
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/__init__.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
 # pylint: disable=line-too-long
-
+# The following imports are automatically generated by templates.
 from .binary_command_failed_exception import BinaryCommandFailedException as BinaryCommandFailedException
 from .command_failed_exception import CommandFailedException as CommandFailedException
 from .command_preempted_exception import CommandPreemptedException as CommandPreemptedException
 from .command_too_long_exception import CommandTooLongException as CommandTooLongException
 from .connection_closed_exception import ConnectionClosedException as ConnectionClosedException
 from .connection_failed_exception import ConnectionFailedException as ConnectionFailedException
 from .conversion_failed_exception import ConversionFailedException as ConversionFailedException
@@ -19,19 +17,21 @@
 from .g_code_syntax_exception import GCodeSyntaxException as GCodeSyntaxException
 from .internal_error_exception import InternalErrorException as InternalErrorException
 from .invalid_argument_exception import InvalidArgumentException as InvalidArgumentException
 from .invalid_data_exception import InvalidDataException as InvalidDataException
 from .invalid_operation_exception import InvalidOperationException as InvalidOperationException
 from .invalid_packet_exception import InvalidPacketException as InvalidPacketException
 from .invalid_park_state_exception import InvalidParkStateException as InvalidParkStateException
+from .invalid_request_data_exception import InvalidRequestDataException as InvalidRequestDataException
 from .invalid_response_exception import InvalidResponseException as InvalidResponseException
 from .io_channel_out_of_range_exception import IoChannelOutOfRangeException as IoChannelOutOfRangeException
 from .io_failed_exception import IoFailedException as IoFailedException
 from .lockstep_enabled_exception import LockstepEnabledException as LockstepEnabledException
 from .lockstep_not_enabled_exception import LockstepNotEnabledException as LockstepNotEnabledException
+from .motion_lib_exception import MotionLibException as MotionLibException
 from .movement_failed_exception import MovementFailedException as MovementFailedException
 from .movement_interrupted_exception import MovementInterruptedException as MovementInterruptedException
 from .no_device_found_exception import NoDeviceFoundException as NoDeviceFoundException
 from .no_value_for_key_exception import NoValueForKeyException as NoValueForKeyException
 from .not_supported_exception import NotSupportedException as NotSupportedException
 from .operation_failed_exception import OperationFailedException as OperationFailedException
 from .os_failed_exception import OsFailedException as OsFailedException
@@ -52,30 +52,28 @@
 from .stream_mode_exception import StreamModeException as StreamModeException
 from .stream_movement_failed_exception import StreamMovementFailedException as StreamMovementFailedException
 from .stream_movement_interrupted_exception import StreamMovementInterruptedException as StreamMovementInterruptedException
 from .stream_setup_failed_exception import StreamSetupFailedException as StreamSetupFailedException
 from .timeout_exception import TimeoutException as TimeoutException
 from .transport_already_used_exception import TransportAlreadyUsedException as TransportAlreadyUsedException
 from .unknown_request_exception import UnknownRequestException as UnknownRequestException
-from .motion_lib_exception import MotionLibException as MotionLibException
-
-from .binary_command_failed_exception_data import BinaryCommandFailedExceptionData as BinaryCommandFailedExceptionData
-from .command_failed_exception_data import CommandFailedExceptionData as CommandFailedExceptionData
-from .command_too_long_exception_data import CommandTooLongExceptionData as CommandTooLongExceptionData
-from .device_address_conflict_exception_data import DeviceAddressConflictExceptionData as DeviceAddressConflictExceptionData
-from .device_db_failed_exception_data import DeviceDbFailedExceptionData as DeviceDbFailedExceptionData
-from .g_code_execution_exception_data import GCodeExecutionExceptionData as GCodeExecutionExceptionData
-from .g_code_syntax_exception_data import GCodeSyntaxExceptionData as GCodeSyntaxExceptionData
-from .invalid_packet_exception_data import InvalidPacketExceptionData as InvalidPacketExceptionData
-from .invalid_pvt_point import InvalidPvtPoint as InvalidPvtPoint
-from .invalid_response_exception_data import InvalidResponseExceptionData as InvalidResponseExceptionData
-from .movement_failed_exception_data import MovementFailedExceptionData as MovementFailedExceptionData
-from .movement_interrupted_exception_data import MovementInterruptedExceptionData as MovementInterruptedExceptionData
-from .operation_failed_exception_data import OperationFailedExceptionData as OperationFailedExceptionData
-from .pvt_execution_exception_data import PvtExecutionExceptionData as PvtExecutionExceptionData
-from .pvt_movement_failed_exception_data import PvtMovementFailedExceptionData as PvtMovementFailedExceptionData
-from .pvt_movement_interrupted_exception_data import PvtMovementInterruptedExceptionData as PvtMovementInterruptedExceptionData
-from .set_device_state_exception_data import SetDeviceStateExceptionData as SetDeviceStateExceptionData
-from .set_peripheral_state_exception_data import SetPeripheralStateExceptionData as SetPeripheralStateExceptionData
-from .stream_execution_exception_data import StreamExecutionExceptionData as StreamExecutionExceptionData
-from .stream_movement_failed_exception_data import StreamMovementFailedExceptionData as StreamMovementFailedExceptionData
-from .stream_movement_interrupted_exception_data import StreamMovementInterruptedExceptionData as StreamMovementInterruptedExceptionData
+from ..dto.exceptions.invalid_packet_exception_data import InvalidPacketExceptionData as InvalidPacketExceptionData
+from ..dto.exceptions.device_address_conflict_exception_data import DeviceAddressConflictExceptionData as DeviceAddressConflictExceptionData
+from ..dto.exceptions.movement_interrupted_exception_data import MovementInterruptedExceptionData as MovementInterruptedExceptionData
+from ..dto.exceptions.stream_movement_interrupted_exception_data import StreamMovementInterruptedExceptionData as StreamMovementInterruptedExceptionData
+from ..dto.exceptions.pvt_movement_interrupted_exception_data import PvtMovementInterruptedExceptionData as PvtMovementInterruptedExceptionData
+from ..dto.exceptions.movement_failed_exception_data import MovementFailedExceptionData as MovementFailedExceptionData
+from ..dto.exceptions.stream_movement_failed_exception_data import StreamMovementFailedExceptionData as StreamMovementFailedExceptionData
+from ..dto.exceptions.pvt_movement_failed_exception_data import PvtMovementFailedExceptionData as PvtMovementFailedExceptionData
+from ..dto.exceptions.stream_execution_exception_data import StreamExecutionExceptionData as StreamExecutionExceptionData
+from ..dto.exceptions.pvt_execution_exception_data import PvtExecutionExceptionData as PvtExecutionExceptionData
+from ..dto.exceptions.invalid_pvt_point import InvalidPvtPoint as InvalidPvtPoint
+from ..dto.exceptions.operation_failed_exception_data import OperationFailedExceptionData as OperationFailedExceptionData
+from ..dto.exceptions.invalid_response_exception_data import InvalidResponseExceptionData as InvalidResponseExceptionData
+from ..dto.exceptions.command_failed_exception_data import CommandFailedExceptionData as CommandFailedExceptionData
+from ..dto.exceptions.binary_command_failed_exception_data import BinaryCommandFailedExceptionData as BinaryCommandFailedExceptionData
+from ..dto.exceptions.set_peripheral_state_exception_data import SetPeripheralStateExceptionData as SetPeripheralStateExceptionData
+from ..dto.exceptions.set_device_state_exception_data import SetDeviceStateExceptionData as SetDeviceStateExceptionData
+from ..dto.exceptions.command_too_long_exception_data import CommandTooLongExceptionData as CommandTooLongExceptionData
+from ..dto.exceptions.device_db_failed_exception_data import DeviceDbFailedExceptionData as DeviceDbFailedExceptionData
+from ..dto.exceptions.g_code_syntax_exception_data import GCodeSyntaxExceptionData as GCodeSyntaxExceptionData
+from ..dto.exceptions.g_code_execution_exception_data import GCodeExecutionExceptionData as GCodeExecutionExceptionData
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/operation_failed_exception.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .binary_command_failed_exception_data import BinaryCommandFailedExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.operation_failed_exception_data import OperationFailedExceptionData
 from .motion_lib_exception import MotionLibException
 
 
-class BinaryCommandFailedException(MotionLibException):
+class OperationFailedException(MotionLibException):
     """
-    Thrown when a device rejects a binary command with an error.
+    Thrown when a non-motion device fails to perform a requested operation.
     """
 
     @property
-    def details(self) -> BinaryCommandFailedExceptionData:
+    def details(self) -> OperationFailedExceptionData:
         """
-        Additional data for BinaryCommandFailedException
+        Additional data for OperationFailedException
         """
         return self._details
 
-    def __init__(self, message: str, custom_data: Union[bytes, BinaryCommandFailedExceptionData]):
+    def __init__(self, message: str, custom_data: Union[bytes, OperationFailedExceptionData]):
         MotionLibException.__init__(self, message)
 
-        if isinstance(custom_data, BinaryCommandFailedExceptionData):
+        if isinstance(custom_data, OperationFailedExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.BinaryCommandFailedExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = BinaryCommandFailedExceptionData.from_protobuf(protobuf_obj)
+            self._details = OperationFailedExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-6.0.0/zaber_motion/dto/exceptions/binary_command_failed_exception_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,44 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
 
+@dataclass
 class BinaryCommandFailedExceptionData:
     """
     Contains additional data for BinaryCommandFailedException.
     """
 
-    @property
-    def response_data(self) -> int:
-        """
-        The response data.
-        """
-
-        return self._response_data
-
-    @response_data.setter
-    def response_data(self, value: int) -> None:
-        self._response_data = value
+    response_data: int
+    """
+    The response data.
+    """
+
+    @staticmethod
+    def zero_values() -> 'BinaryCommandFailedExceptionData':
+        return BinaryCommandFailedExceptionData(
+            response_data=0,
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'BinaryCommandFailedExceptionData':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return BinaryCommandFailedExceptionData.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'responseData': self.response_data,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.BinaryCommandFailedExceptionData
-    ) -> 'BinaryCommandFailedExceptionData':
-        instance = BinaryCommandFailedExceptionData.__new__(
-            BinaryCommandFailedExceptionData
-        )  # type: BinaryCommandFailedExceptionData
-        instance.response_data = pb_data.response_data
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'BinaryCommandFailedExceptionData':
+        return BinaryCommandFailedExceptionData(
+            response_data=data.get('responseData'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/command_failed_exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .command_failed_exception_data import CommandFailedExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.command_failed_exception_data import CommandFailedExceptionData
 from .motion_lib_exception import MotionLibException
 
 
 class CommandFailedException(MotionLibException):
     """
     Thrown when a device rejects a command.
     """
@@ -21,10 +20,8 @@
 
     def __init__(self, message: str, custom_data: Union[bytes, CommandFailedExceptionData]):
         MotionLibException.__init__(self, message)
 
         if isinstance(custom_data, CommandFailedExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.CommandFailedExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = CommandFailedExceptionData.from_protobuf(protobuf_obj)
+            self._details = CommandFailedExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .command_too_long_exception_data import CommandTooLongExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.set_device_state_exception_data import SetDeviceStateExceptionData
 from .motion_lib_exception import MotionLibException
 
 
-class CommandTooLongException(MotionLibException):
+class SetDeviceStateFailedException(MotionLibException):
     """
-    Thrown when a command is too long to be written by the ASCII protocol, even when continued across multiple lines.
+    Thrown when a device cannot be set to the supplied state.
     """
 
     @property
-    def details(self) -> CommandTooLongExceptionData:
+    def details(self) -> SetDeviceStateExceptionData:
         """
-        Additional data for CommandTooLongException
+        Additional data for SetDeviceStateFailedException
         """
         return self._details
 
-    def __init__(self, message: str, custom_data: Union[bytes, CommandTooLongExceptionData]):
+    def __init__(self, message: str, custom_data: Union[bytes, SetDeviceStateExceptionData]):
         MotionLibException.__init__(self, message)
 
-        if isinstance(custom_data, CommandTooLongExceptionData):
+        if isinstance(custom_data, SetDeviceStateExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.CommandTooLongExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = CommandTooLongExceptionData.from_protobuf(protobuf_obj)
+            self._details = SetDeviceStateExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .device_address_conflict_exception_data import DeviceAddressConflictExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.device_address_conflict_exception_data import DeviceAddressConflictExceptionData
 from .motion_lib_exception import MotionLibException
 
 
 class DeviceAddressConflictException(MotionLibException):
     """
     Thrown when there is a conflict in device numbers preventing unique addressing.
     """
@@ -21,10 +20,8 @@
 
     def __init__(self, message: str, custom_data: Union[bytes, DeviceAddressConflictExceptionData]):
         MotionLibException.__init__(self, message)
 
         if isinstance(custom_data, DeviceAddressConflictExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.DeviceAddressConflictExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = DeviceAddressConflictExceptionData.from_protobuf(protobuf_obj)
+            self._details = DeviceAddressConflictExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .device_db_failed_exception_data import DeviceDbFailedExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.stream_movement_interrupted_exception_data import StreamMovementInterruptedExceptionData
 from .motion_lib_exception import MotionLibException
 
 
-class DeviceDbFailedException(MotionLibException):
+class StreamMovementInterruptedException(MotionLibException):
     """
-    Thrown when device information cannot be retrieved from the device database.
+    Thrown when ongoing stream movement is interrupted by another command or user input.
     """
 
     @property
-    def details(self) -> DeviceDbFailedExceptionData:
+    def details(self) -> StreamMovementInterruptedExceptionData:
         """
-        Additional data for DeviceDbFailedException
+        Additional data for StreamMovementInterruptedException
         """
         return self._details
 
-    def __init__(self, message: str, custom_data: Union[bytes, DeviceDbFailedExceptionData]):
+    def __init__(self, message: str, custom_data: Union[bytes, StreamMovementInterruptedExceptionData]):
         MotionLibException.__init__(self, message)
 
-        if isinstance(custom_data, DeviceDbFailedExceptionData):
+        if isinstance(custom_data, StreamMovementInterruptedExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.DeviceDbFailedExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = DeviceDbFailedExceptionData.from_protobuf(protobuf_obj)
+            self._details = StreamMovementInterruptedExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
 
-from ..protobufs import main_pb2
+from typing import Union
+from ..dto.exceptions.movement_interrupted_exception_data import MovementInterruptedExceptionData
+from .motion_lib_exception import MotionLibException
 
 
-class DeviceDbFailedExceptionData:
+class MovementInterruptedException(MotionLibException):
     """
-    Contains additional data for a DeviceDbFailedException.
+    Thrown when ongoing movement is interrupted by another command or user input.
     """
 
     @property
-    def code(self) -> str:
+    def details(self) -> MovementInterruptedExceptionData:
         """
-        Code describing type of the error.
+        Additional data for MovementInterruptedException
         """
+        return self._details
 
-        return self._code
+    def __init__(self, message: str, custom_data: Union[bytes, MovementInterruptedExceptionData]):
+        MotionLibException.__init__(self, message)
 
-    @code.setter
-    def code(self, value: str) -> None:
-        self._code = value
-
-    def __repr__(self) -> str:
-        return str(self.__dict__)
-
-    @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.DeviceDbFailedExceptionData
-    ) -> 'DeviceDbFailedExceptionData':
-        instance = DeviceDbFailedExceptionData.__new__(
-            DeviceDbFailedExceptionData
-        )  # type: DeviceDbFailedExceptionData
-        instance.code = pb_data.code
-        return instance
+        if isinstance(custom_data, MovementInterruptedExceptionData):
+            self._details = custom_data
+        else:
+            self._details = MovementInterruptedExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/pvt_execution_exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .g_code_execution_exception_data import GCodeExecutionExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.pvt_execution_exception_data import PvtExecutionExceptionData
 from .motion_lib_exception import MotionLibException
 
 
-class GCodeExecutionException(MotionLibException):
+class PvtExecutionException(MotionLibException):
     """
-    Thrown when a block of G-Code cannot be executed.
+    Thrown when a PVT sequence motion fails.
     """
 
     @property
-    def details(self) -> GCodeExecutionExceptionData:
+    def details(self) -> PvtExecutionExceptionData:
         """
-        Additional data for GCodeExecutionException
+        Additional data for PvtExecutionException
         """
         return self._details
 
-    def __init__(self, message: str, custom_data: Union[bytes, GCodeExecutionExceptionData]):
+    def __init__(self, message: str, custom_data: Union[bytes, PvtExecutionExceptionData]):
         MotionLibException.__init__(self, message)
 
-        if isinstance(custom_data, GCodeExecutionExceptionData):
+        if isinstance(custom_data, PvtExecutionExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.GCodeExecutionExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = GCodeExecutionExceptionData.from_protobuf(protobuf_obj)
+            self._details = PvtExecutionExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
 
-from ..protobufs import main_pb2
+from typing import Union
+from ..dto.exceptions.g_code_execution_exception_data import GCodeExecutionExceptionData
+from .motion_lib_exception import MotionLibException
 
 
-class GCodeExecutionExceptionData:
+class GCodeExecutionException(MotionLibException):
     """
-    Contains additional data for GCodeExecutionException.
+    Thrown when a block of G-Code cannot be executed.
     """
 
     @property
-    def from_block(self) -> int:
+    def details(self) -> GCodeExecutionExceptionData:
         """
-        The index in the block string that caused the exception.
+        Additional data for GCodeExecutionException
         """
+        return self._details
 
-        return self._from_block
+    def __init__(self, message: str, custom_data: Union[bytes, GCodeExecutionExceptionData]):
+        MotionLibException.__init__(self, message)
 
-    @from_block.setter
-    def from_block(self, value: int) -> None:
-        self._from_block = value
-
-    @property
-    def to_block(self) -> int:
-        """
-        The end index in the block string that caused the exception.
-        The end index is exclusive.
-        """
-
-        return self._to_block
-
-    @to_block.setter
-    def to_block(self, value: int) -> None:
-        self._to_block = value
-
-    def __repr__(self) -> str:
-        return str(self.__dict__)
-
-    @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.GCodeExecutionExceptionData
-    ) -> 'GCodeExecutionExceptionData':
-        instance = GCodeExecutionExceptionData.__new__(
-            GCodeExecutionExceptionData
-        )  # type: GCodeExecutionExceptionData
-        instance.from_block = pb_data.from_block
-        instance.to_block = pb_data.to_block
-        return instance
+        if isinstance(custom_data, GCodeExecutionExceptionData):
+            self._details = custom_data
+        else:
+            self._details = GCodeExecutionExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .g_code_syntax_exception_data import GCodeSyntaxExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.g_code_syntax_exception_data import GCodeSyntaxExceptionData
 from .motion_lib_exception import MotionLibException
 
 
 class GCodeSyntaxException(MotionLibException):
     """
     Thrown when a block of G-Code cannot be parsed.
     """
@@ -21,10 +20,8 @@
 
     def __init__(self, message: str, custom_data: Union[bytes, GCodeSyntaxExceptionData]):
         MotionLibException.__init__(self, message)
 
         if isinstance(custom_data, GCodeSyntaxExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.GCodeSyntaxExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = GCodeSyntaxExceptionData.from_protobuf(protobuf_obj)
+            self._details = GCodeSyntaxExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .invalid_packet_exception_data import InvalidPacketExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.invalid_packet_exception_data import InvalidPacketExceptionData
 from .motion_lib_exception import MotionLibException
 
 
 class InvalidPacketException(MotionLibException):
     """
     Thrown when a packet from a device cannot be parsed.
     """
@@ -21,10 +20,8 @@
 
     def __init__(self, message: str, custom_data: Union[bytes, InvalidPacketExceptionData]):
         MotionLibException.__init__(self, message)
 
         if isinstance(custom_data, InvalidPacketExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.InvalidPacketExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = InvalidPacketExceptionData.from_protobuf(protobuf_obj)
+            self._details = InvalidPacketExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-6.0.0/zaber_motion/dto/exceptions/invalid_packet_exception_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
 
+@dataclass
 class InvalidPacketExceptionData:
     """
     Contains additional data for the InvalidPacketException.
     """
 
-    @property
-    def packet(self) -> str:
-        """
-        The invalid packet that caused the exception.
-        """
-
-        return self._packet
-
-    @packet.setter
-    def packet(self, value: str) -> None:
-        self._packet = value
-
-    @property
-    def reason(self) -> str:
-        """
-        The reason for the exception.
-        """
-
-        return self._reason
-
-    @reason.setter
-    def reason(self, value: str) -> None:
-        self._reason = value
+    packet: str
+    """
+    The invalid packet that caused the exception.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    reason: str
+    """
+    The reason for the exception.
+    """
+
+    @staticmethod
+    def zero_values() -> 'InvalidPacketExceptionData':
+        return InvalidPacketExceptionData(
+            packet="",
+            reason="",
+        )
+
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'InvalidPacketExceptionData':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return InvalidPacketExceptionData.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'packet': self.packet,
+            'reason': self.reason,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.InvalidPacketExceptionData
-    ) -> 'InvalidPacketExceptionData':
-        instance = InvalidPacketExceptionData.__new__(
-            InvalidPacketExceptionData
-        )  # type: InvalidPacketExceptionData
-        instance.packet = pb_data.packet
-        instance.reason = pb_data.reason
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'InvalidPacketExceptionData':
+        return InvalidPacketExceptionData(
+            packet=data.get('packet'),  # type: ignore
+            reason=data.get('reason'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .invalid_response_exception_data import InvalidResponseExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.invalid_response_exception_data import InvalidResponseExceptionData
 from .motion_lib_exception import MotionLibException
 
 
 class InvalidResponseException(MotionLibException):
     """
     Thrown when a device sends a response with unexpected type or data.
     """
@@ -21,10 +20,8 @@
 
     def __init__(self, message: str, custom_data: Union[bytes, InvalidResponseExceptionData]):
         MotionLibException.__init__(self, message)
 
         if isinstance(custom_data, InvalidResponseExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.InvalidResponseExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = InvalidResponseExceptionData.from_protobuf(protobuf_obj)
+            self._details = InvalidResponseExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .movement_failed_exception_data import MovementFailedExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.movement_failed_exception_data import MovementFailedExceptionData
 from .motion_lib_exception import MotionLibException
 
 
 class MovementFailedException(MotionLibException):
     """
     Thrown when a device registers a fault during movement.
     """
@@ -21,10 +20,8 @@
 
     def __init__(self, message: str, custom_data: Union[bytes, MovementFailedExceptionData]):
         MotionLibException.__init__(self, message)
 
         if isinstance(custom_data, MovementFailedExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.MovementFailedExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = MovementFailedExceptionData.from_protobuf(protobuf_obj)
+            self._details = MovementFailedExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-6.0.0/zaber_motion/dto/exceptions/pvt_movement_failed_exception_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,52 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
-from typing import List  # pylint: disable=unused-import
-from ..protobufs import main_pb2
 
-
-class MovementFailedExceptionData:
+@dataclass
+class PvtMovementFailedExceptionData:
     """
-    Contains additional data for MovementFailedException.
+    Contains additional data for PvtMovementFailedException.
     """
 
-    @property
-    def warnings(self) -> List[str]:
-        """
-        The full list of warnings.
-        """
-
-        return self._warnings
-
-    @warnings.setter
-    def warnings(self, value: List[str]) -> None:
-        self._warnings = value
-
-    @property
-    def reason(self) -> str:
-        """
-        The reason for the Exception.
-        """
-
-        return self._reason
-
-    @reason.setter
-    def reason(self, value: str) -> None:
-        self._reason = value
-
-    @property
-    def device(self) -> int:
-        """
-        The address of the device that performed the failed movement.
-        """
-
-        return self._device
-
-    @device.setter
-    def device(self, value: int) -> None:
-        self._device = value
-
-    @property
-    def axis(self) -> int:
-        """
-        The number of the axis that performed the failed movement.
-        """
+    warnings: List[str]
+    """
+    The full list of warnings.
+    """
 
-        return self._axis
+    reason: str
+    """
+    The reason for the Exception.
+    """
 
-    @axis.setter
-    def axis(self, value: int) -> None:
-        self._axis = value
+    @staticmethod
+    def zero_values() -> 'PvtMovementFailedExceptionData':
+        return PvtMovementFailedExceptionData(
+            warnings=[],
+            reason="",
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'PvtMovementFailedExceptionData':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return PvtMovementFailedExceptionData.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'warnings': self.warnings,
+            'reason': self.reason,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.MovementFailedExceptionData
-    ) -> 'MovementFailedExceptionData':
-        instance = MovementFailedExceptionData.__new__(
-            MovementFailedExceptionData
-        )  # type: MovementFailedExceptionData
-        instance.warnings = list(pb_data.warnings)
-        instance.reason = pb_data.reason
-        instance.device = pb_data.device
-        instance.axis = pb_data.axis
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'PvtMovementFailedExceptionData':
+        return PvtMovementFailedExceptionData(
+            warnings=data.get('warnings'),  # type: ignore
+            reason=data.get('reason'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .movement_interrupted_exception_data import MovementInterruptedExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.pvt_movement_interrupted_exception_data import PvtMovementInterruptedExceptionData
 from .motion_lib_exception import MotionLibException
 
 
-class MovementInterruptedException(MotionLibException):
+class PvtMovementInterruptedException(MotionLibException):
     """
-    Thrown when ongoing movement is interrupted by another command or user input.
+    Thrown when ongoing PVT movement is interrupted by another command or user input.
     """
 
     @property
-    def details(self) -> MovementInterruptedExceptionData:
+    def details(self) -> PvtMovementInterruptedExceptionData:
         """
-        Additional data for MovementInterruptedException
+        Additional data for PvtMovementInterruptedException
         """
         return self._details
 
-    def __init__(self, message: str, custom_data: Union[bytes, MovementInterruptedExceptionData]):
+    def __init__(self, message: str, custom_data: Union[bytes, PvtMovementInterruptedExceptionData]):
         MotionLibException.__init__(self, message)
 
-        if isinstance(custom_data, MovementInterruptedExceptionData):
+        if isinstance(custom_data, PvtMovementInterruptedExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.MovementInterruptedExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = MovementInterruptedExceptionData.from_protobuf(protobuf_obj)
+            self._details = PvtMovementInterruptedExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/operation_failed_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/pvt_movement_failed_exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .operation_failed_exception_data import OperationFailedExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.pvt_movement_failed_exception_data import PvtMovementFailedExceptionData
 from .motion_lib_exception import MotionLibException
 
 
-class OperationFailedException(MotionLibException):
+class PvtMovementFailedException(MotionLibException):
     """
-    Thrown when a non-motion device fails to perform a requested operation.
+    Thrown when a device registers a fault during PVT movement.
     """
 
     @property
-    def details(self) -> OperationFailedExceptionData:
+    def details(self) -> PvtMovementFailedExceptionData:
         """
-        Additional data for OperationFailedException
+        Additional data for PvtMovementFailedException
         """
         return self._details
 
-    def __init__(self, message: str, custom_data: Union[bytes, OperationFailedExceptionData]):
+    def __init__(self, message: str, custom_data: Union[bytes, PvtMovementFailedExceptionData]):
         MotionLibException.__init__(self, message)
 
-        if isinstance(custom_data, OperationFailedExceptionData):
+        if isinstance(custom_data, PvtMovementFailedExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.OperationFailedExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = OperationFailedExceptionData.from_protobuf(protobuf_obj)
+            self._details = PvtMovementFailedExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/operation_failed_exception_data.py` & `zaber_motion-6.0.0/zaber_motion/dto/exceptions/operation_failed_exception_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,68 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from typing import List  # pylint: disable=unused-import
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
 
+@dataclass
 class OperationFailedExceptionData:
     """
     Contains additional data for OperationFailedException.
     """
 
-    @property
-    def warnings(self) -> List[str]:
-        """
-        The full list of warnings.
-        """
-
-        return self._warnings
-
-    @warnings.setter
-    def warnings(self, value: List[str]) -> None:
-        self._warnings = value
-
-    @property
-    def reason(self) -> str:
-        """
-        The reason for the Exception.
-        """
-
-        return self._reason
-
-    @reason.setter
-    def reason(self, value: str) -> None:
-        self._reason = value
-
-    @property
-    def device(self) -> int:
-        """
-        The address of the device that attempted the failed operation.
-        """
-
-        return self._device
-
-    @device.setter
-    def device(self, value: int) -> None:
-        self._device = value
-
-    @property
-    def axis(self) -> int:
-        """
-        The number of the axis that attempted the failed operation.
-        """
-
-        return self._axis
-
-    @axis.setter
-    def axis(self, value: int) -> None:
-        self._axis = value
+    warnings: List[str]
+    """
+    The full list of warnings.
+    """
+
+    reason: str
+    """
+    The reason for the Exception.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    device: int
+    """
+    The address of the device that attempted the failed operation.
+    """
+
+    axis: int
+    """
+    The number of the axis that attempted the failed operation.
+    """
+
+    @staticmethod
+    def zero_values() -> 'OperationFailedExceptionData':
+        return OperationFailedExceptionData(
+            warnings=[],
+            reason="",
+            device=0,
+            axis=0,
+        )
+
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'OperationFailedExceptionData':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return OperationFailedExceptionData.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'warnings': self.warnings,
+            'reason': self.reason,
+            'device': self.device,
+            'axis': self.axis,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.OperationFailedExceptionData
-    ) -> 'OperationFailedExceptionData':
-        instance = OperationFailedExceptionData.__new__(
-            OperationFailedExceptionData
-        )  # type: OperationFailedExceptionData
-        instance.warnings = list(pb_data.warnings)
-        instance.reason = pb_data.reason
-        instance.device = pb_data.device
-        instance.axis = pb_data.axis
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'OperationFailedExceptionData':
+        return OperationFailedExceptionData(
+            warnings=data.get('warnings'),  # type: ignore
+            reason=data.get('reason'),  # type: ignore
+            device=data.get('device'),  # type: ignore
+            axis=data.get('axis'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/pvt_execution_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .pvt_execution_exception_data import PvtExecutionExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.stream_execution_exception_data import StreamExecutionExceptionData
 from .motion_lib_exception import MotionLibException
 
 
-class PvtExecutionException(MotionLibException):
+class StreamExecutionException(MotionLibException):
     """
-    Thrown when a PVT sequence motion fails.
+    Thrown when a streamed motion fails.
     """
 
     @property
-    def details(self) -> PvtExecutionExceptionData:
+    def details(self) -> StreamExecutionExceptionData:
         """
-        Additional data for PvtExecutionException
+        Additional data for StreamExecutionException
         """
         return self._details
 
-    def __init__(self, message: str, custom_data: Union[bytes, PvtExecutionExceptionData]):
+    def __init__(self, message: str, custom_data: Union[bytes, StreamExecutionExceptionData]):
         MotionLibException.__init__(self, message)
 
-        if isinstance(custom_data, PvtExecutionExceptionData):
+        if isinstance(custom_data, StreamExecutionExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.PvtExecutionExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = PvtExecutionExceptionData.from_protobuf(protobuf_obj)
+            self._details = StreamExecutionExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/pvt_execution_exception_data.py` & `zaber_motion-6.0.0/zaber_motion/dto/exceptions/invalid_pvt_point.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,52 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
-from typing import List  # pylint: disable=unused-import
-from ..protobufs import main_pb2
-from .invalid_pvt_point import InvalidPvtPoint
 
-
-class PvtExecutionExceptionData:
+@dataclass
+class InvalidPvtPoint:
     """
-    Contains additional data for PvtExecutionException.
+    Contains invalid PVT points for PvtExecutionException.
     """
 
-    @property
-    def error_flag(self) -> str:
-        """
-        The error flag that caused the exception.
-        """
-
-        return self._error_flag
-
-    @error_flag.setter
-    def error_flag(self, value: str) -> None:
-        self._error_flag = value
-
-    @property
-    def reason(self) -> str:
-        """
-        The reason for the exception.
-        """
-
-        return self._reason
-
-    @reason.setter
-    def reason(self, value: str) -> None:
-        self._reason = value
-
-    @property
-    def invalid_points(self) -> List[InvalidPvtPoint]:
-        """
-        A list of points that cause the error (if applicable).
-        """
+    index: int
+    """
+    Index of the point numbered from the last submitted point.
+    """
 
-        return self._invalid_points
+    point: str
+    """
+    The textual representation of the point.
+    """
 
-    @invalid_points.setter
-    def invalid_points(self, value: List[InvalidPvtPoint]) -> None:
-        self._invalid_points = value
+    @staticmethod
+    def zero_values() -> 'InvalidPvtPoint':
+        return InvalidPvtPoint(
+            index=0,
+            point="",
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'InvalidPvtPoint':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return InvalidPvtPoint.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'index': self.index,
+            'point': self.point,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.PvtExecutionExceptionData
-    ) -> 'PvtExecutionExceptionData':
-        instance = PvtExecutionExceptionData.__new__(
-            PvtExecutionExceptionData
-        )  # type: PvtExecutionExceptionData
-        instance.error_flag = pb_data.error_flag
-        instance.reason = pb_data.reason
-        instance.invalid_points = [InvalidPvtPoint.from_protobuf(item) for item in pb_data.invalid_points]
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'InvalidPvtPoint':
+        return InvalidPvtPoint(
+            index=data.get('index'),  # type: ignore
+            point=data.get('point'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/pvt_movement_failed_exception_data.py` & `zaber_motion-6.0.0/zaber_motion/dto/exceptions/device_db_failed_exception_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,44 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
-from typing import List  # pylint: disable=unused-import
-from ..protobufs import main_pb2
 
+@dataclass
+class DeviceDbFailedExceptionData:
+    """
+    Contains additional data for a DeviceDbFailedException.
+    """
 
-class PvtMovementFailedExceptionData:
+    code: str
     """
-    Contains additional data for PvtMovementFailedException.
+    Code describing type of the error.
     """
 
-    @property
-    def warnings(self) -> List[str]:
-        """
-        The full list of warnings.
-        """
-
-        return self._warnings
-
-    @warnings.setter
-    def warnings(self, value: List[str]) -> None:
-        self._warnings = value
-
-    @property
-    def reason(self) -> str:
-        """
-        The reason for the Exception.
-        """
-
-        return self._reason
-
-    @reason.setter
-    def reason(self, value: str) -> None:
-        self._reason = value
+    @staticmethod
+    def zero_values() -> 'DeviceDbFailedExceptionData':
+        return DeviceDbFailedExceptionData(
+            code="",
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'DeviceDbFailedExceptionData':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return DeviceDbFailedExceptionData.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'code': self.code,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.PvtMovementFailedExceptionData
-    ) -> 'PvtMovementFailedExceptionData':
-        instance = PvtMovementFailedExceptionData.__new__(
-            PvtMovementFailedExceptionData
-        )  # type: PvtMovementFailedExceptionData
-        instance.warnings = list(pb_data.warnings)
-        instance.reason = pb_data.reason
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'DeviceDbFailedExceptionData':
+        return DeviceDbFailedExceptionData(
+            code=data.get('code'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-6.0.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Union
-from .set_peripheral_state_exception_data import SetPeripheralStateExceptionData
-from ..protobufs import main_pb2
+from ..dto.exceptions.set_peripheral_state_exception_data import SetPeripheralStateExceptionData
 from .motion_lib_exception import MotionLibException
 
 
 class SetPeripheralStateFailedException(MotionLibException):
     """
     Thrown when an axis cannot be set to the supplied state.
     """
@@ -21,10 +20,8 @@
 
     def __init__(self, message: str, custom_data: Union[bytes, SetPeripheralStateExceptionData]):
         MotionLibException.__init__(self, message)
 
         if isinstance(custom_data, SetPeripheralStateExceptionData):
             self._details = custom_data
         else:
-            protobuf_obj = main_pb2.SetPeripheralStateExceptionData()
-            protobuf_obj.ParseFromString(custom_data)
-            self._details = SetPeripheralStateExceptionData.from_protobuf(protobuf_obj)
+            self._details = SetPeripheralStateExceptionData.from_binary(custom_data)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/gcode/axis_definition.py` & `zaber_motion-6.0.0/zaber_motion/dto/gcode/axis_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,54 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from typing import Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
 
+@dataclass
 class AxisDefinition:
     """
     Defines an axis of the translator.
     """
 
-    def __init__(
-            self: 'AxisDefinition',
-            peripheral_id: int,
-            microstep_resolution: Optional[int] = None
-    ) -> None:
-        self._peripheral_id = peripheral_id
-        self._microstep_resolution = microstep_resolution
-
-    @property
-    def peripheral_id(self) -> int:
-        """
-        ID of the peripheral.
-        """
-
-        return self._peripheral_id
-
-    @peripheral_id.setter
-    def peripheral_id(self, value: int) -> None:
-        self._peripheral_id = value
-
-    @property
-    def microstep_resolution(self) -> Optional[int]:
-        """
-        Microstep resolution of the axis.
-        Can be obtained by reading the resolution setting.
-        Leave empty if the axis does not have the setting.
-        """
-
-        return self._microstep_resolution
-
-    @microstep_resolution.setter
-    def microstep_resolution(self, value: Optional[int]) -> None:
-        self._microstep_resolution = value
+    peripheral_id: int
+    """
+    ID of the peripheral.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    microstep_resolution: Optional[int] = None
+    """
+    Microstep resolution of the axis.
+    Can be obtained by reading the resolution setting.
+    Leave empty if the axis does not have the setting.
+    """
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.TranslatorAxisDefinition
-    ) -> 'AxisDefinition':
-        instance = AxisDefinition.__new__(
-            AxisDefinition
-        )  # type: AxisDefinition
-        instance.peripheral_id = pb_data.peripheral_id
-        instance.microstep_resolution = pb_data.microstep_resolution if pb_data.has_microstep_resolution else None
-        return instance
+    def zero_values() -> 'AxisDefinition':
+        return AxisDefinition(
+            peripheral_id=0,
+            microstep_resolution=None,
+        )
 
     @staticmethod
-    def to_protobuf(source: 'Optional[AxisDefinition]') -> main_pb2.TranslatorAxisDefinition:
-        pb_data = main_pb2.TranslatorAxisDefinition()
-
-        if source is None:
-            return pb_data
+    def from_binary(data_bytes: bytes) -> 'AxisDefinition':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return AxisDefinition.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'peripheralId': self.peripheral_id,
+            'microstepResolution': self.microstep_resolution,
+        }
 
-        if not isinstance(source, AxisDefinition):
-            raise TypeError("Provided value is not AxisDefinition.")
-
-        pb_data.peripheral_id = source.peripheral_id
-        if source.microstep_resolution is not None:
-            pb_data.microstep_resolution = source.microstep_resolution
-            pb_data.has_microstep_resolution = True
-        return pb_data
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> 'AxisDefinition':
+        return AxisDefinition(
+            peripheral_id=data.get('peripheralId'),  # type: ignore
+            microstep_resolution=data.get('microstepResolution'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/gcode/translate_result.py` & `zaber_motion-6.0.0/zaber_motion/dto/gcode/translate_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,61 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 
-from typing import List  # pylint: disable=unused-import
-from ..protobufs import main_pb2
-from .translate_message import TranslateMessage
 
-
-class TranslateResult:
+@dataclass
+class TranslateMessage:
     """
-    Represents a result of a G-code block translation.
+    Represents a message from translator regarding a block translation.
     """
 
-    @property
-    def commands(self) -> List[str]:
-        """
-        Stream commands resulting from the block.
-        """
-
-        return self._commands
-
-    @commands.setter
-    def commands(self, value: List[str]) -> None:
-        self._commands = value
+    message: str
+    """
+    The message describing an occurrence.
+    """
 
-    @property
-    def warnings(self) -> List[TranslateMessage]:
-        """
-        Messages informing about unsupported codes and features.
-        """
+    from_block: int
+    """
+    The index in the block string that the message regards to.
+    """
 
-        return self._warnings
+    to_block: int
+    """
+    The end index in the block string that the message regards to.
+    The end index is exclusive.
+    """
 
-    @warnings.setter
-    def warnings(self, value: List[TranslateMessage]) -> None:
-        self._warnings = value
+    @staticmethod
+    def zero_values() -> 'TranslateMessage':
+        return TranslateMessage(
+            message="",
+            from_block=0,
+            to_block=0,
+        )
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'TranslateMessage':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return TranslateMessage.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'message': self.message,
+            'fromBlock': self.from_block,
+            'toBlock': self.to_block,
+        }
 
     @staticmethod
-    def from_protobuf(
-        pb_data: main_pb2.TranslatorTranslateResponse
-    ) -> 'TranslateResult':
-        instance = TranslateResult.__new__(
-            TranslateResult
-        )  # type: TranslateResult
-        instance.commands = list(pb_data.commands)
-        instance.warnings = [TranslateMessage.from_protobuf(item) for item in pb_data.warnings]
-        return instance
+    def from_dict(data: Dict[str, Any]) -> 'TranslateMessage':
+        return TranslateMessage(
+            message=data.get('message'),  # type: ignore
+            from_block=data.get('fromBlock'),  # type: ignore
+            to_block=data.get('toBlock'),  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/gcode/translator.py` & `zaber_motion-6.0.0/zaber_motion/gcode/translator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import List, Optional
 from ..call import call, call_async, call_sync
 
-from ..protobufs import main_pb2
-from ..units import units_from_literals, LengthUnits, VelocityUnits
+from ..dto import requests as dto
+from ..units import LengthUnits, VelocityUnits
 from ..ascii import Stream
-from .translator_config import TranslatorConfig
-from .translate_result import TranslateResult
+from ..dto.gcode.translator_config import TranslatorConfig
+from ..dto.gcode.translate_result import TranslateResult
 
 
 class Translator:
     """
     Represents a live G-Code translator.
     It allows to stream G-Code blocks to a connected device.
     It requires a stream to be setup on the device.
@@ -48,21 +48,24 @@
             stream: The stream to setup the translator on.
                 The stream must be already setup in a live or a store mode.
             config: Configuration of the translator.
 
         Returns:
             New instance of translator.
         """
-        request = main_pb2.TranslatorCreateLiveRequest()
-        request.device = stream.device.device_address
-        request.interface_id = stream.device.connection.interface_id
-        request.stream_id = stream.stream_id
-        request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
-        response = main_pb2.TranslatorCreateResponse()
-        call("gcode/create_live", request, response)
+        request = dto.TranslatorCreateLiveRequest(
+            device=stream.device.device_address,
+            interface_id=stream.device.connection.interface_id,
+            stream_id=stream.stream_id,
+            config=config,
+        )
+        response = call(
+            "gcode/create_live",
+            request,
+            dto.TranslatorCreateResponse.from_binary)
         return Translator(response.translator_id)
 
     @staticmethod
     async def setup_async(
             stream: Stream,
             config: Optional[TranslatorConfig] = None
     ) -> 'Translator':
@@ -73,21 +76,24 @@
             stream: The stream to setup the translator on.
                 The stream must be already setup in a live or a store mode.
             config: Configuration of the translator.
 
         Returns:
             New instance of translator.
         """
-        request = main_pb2.TranslatorCreateLiveRequest()
-        request.device = stream.device.device_address
-        request.interface_id = stream.device.connection.interface_id
-        request.stream_id = stream.stream_id
-        request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
-        response = main_pb2.TranslatorCreateResponse()
-        await call_async("gcode/create_live", request, response)
+        request = dto.TranslatorCreateLiveRequest(
+            device=stream.device.device_address,
+            interface_id=stream.device.connection.interface_id,
+            stream_id=stream.stream_id,
+            config=config,
+        )
+        response = await call_async(
+            "gcode/create_live",
+            request,
+            dto.TranslatorCreateResponse.from_binary)
         return Translator(response.translator_id)
 
     def translate(
             self,
             block: str
     ) -> TranslateResult:
         """
@@ -97,20 +103,23 @@
 
         Args:
             block: Block (line) of G-code.
 
         Returns:
             Result of translation containing the commands sent to the device.
         """
-        request = main_pb2.TranslatorTranslateRequest()
-        request.translator_id = self.translator_id
-        request.block = block
-        response = main_pb2.TranslatorTranslateResponse()
-        call("gcode/translate_live", request, response)
-        return TranslateResult.from_protobuf(response)
+        request = dto.TranslatorTranslateRequest(
+            translator_id=self.translator_id,
+            block=block,
+        )
+        response = call(
+            "gcode/translate_live",
+            request,
+            TranslateResult.from_binary)
+        return response
 
     async def translate_async(
             self,
             block: str
     ) -> TranslateResult:
         """
         Translates a single block (line) of G-code.
@@ -119,20 +128,23 @@
 
         Args:
             block: Block (line) of G-code.
 
         Returns:
             Result of translation containing the commands sent to the device.
         """
-        request = main_pb2.TranslatorTranslateRequest()
-        request.translator_id = self.translator_id
-        request.block = block
-        response = main_pb2.TranslatorTranslateResponse()
-        await call_async("gcode/translate_live", request, response)
-        return TranslateResult.from_protobuf(response)
+        request = dto.TranslatorTranslateRequest(
+            translator_id=self.translator_id,
+            block=block,
+        )
+        response = await call_async(
+            "gcode/translate_live",
+            request,
+            TranslateResult.from_binary)
+        return response
 
     def flush(
             self,
             wait_until_idle: bool = True
     ) -> List[str]:
         """
         Flushes the remaining stream commands waiting in optimization buffer into the underlying stream.
@@ -140,20 +152,23 @@
 
         Args:
             wait_until_idle: Determines whether to wait for the stream to finish all the movements.
 
         Returns:
             The remaining stream commands.
         """
-        request = main_pb2.TranslatorFlushLiveRequest()
-        request.translator_id = self.translator_id
-        request.wait_until_idle = wait_until_idle
-        response = main_pb2.TranslatorFlushResponse()
-        call("gcode/flush_live", request, response)
-        return list(response.commands)
+        request = dto.TranslatorFlushLiveRequest(
+            translator_id=self.translator_id,
+            wait_until_idle=wait_until_idle,
+        )
+        response = call(
+            "gcode/flush_live",
+            request,
+            dto.TranslatorFlushResponse.from_binary)
+        return response.commands
 
     async def flush_async(
             self,
             wait_until_idle: bool = True
     ) -> List[str]:
         """
         Flushes the remaining stream commands waiting in optimization buffer into the underlying stream.
@@ -161,59 +176,65 @@
 
         Args:
             wait_until_idle: Determines whether to wait for the stream to finish all the movements.
 
         Returns:
             The remaining stream commands.
         """
-        request = main_pb2.TranslatorFlushLiveRequest()
-        request.translator_id = self.translator_id
-        request.wait_until_idle = wait_until_idle
-        response = main_pb2.TranslatorFlushResponse()
-        await call_async("gcode/flush_live", request, response)
-        return list(response.commands)
+        request = dto.TranslatorFlushLiveRequest(
+            translator_id=self.translator_id,
+            wait_until_idle=wait_until_idle,
+        )
+        response = await call_async(
+            "gcode/flush_live",
+            request,
+            dto.TranslatorFlushResponse.from_binary)
+        return response.commands
 
     def reset_position(
             self
     ) -> None:
         """
         Resets position of the translator from the underlying stream.
         Call this method after performing a movement outside of translator.
         """
-        request = main_pb2.TranslatorEmptyRequest()
-        request.translator_id = self.translator_id
+        request = dto.TranslatorEmptyRequest(
+            translator_id=self.translator_id,
+        )
         call("gcode/reset_position_from_stream", request)
 
     async def reset_position_async(
             self
     ) -> None:
         """
         Resets position of the translator from the underlying stream.
         Call this method after performing a movement outside of translator.
         """
-        request = main_pb2.TranslatorEmptyRequest()
-        request.translator_id = self.translator_id
+        request = dto.TranslatorEmptyRequest(
+            translator_id=self.translator_id,
+        )
         await call_async("gcode/reset_position_from_stream", request)
 
     def set_traverse_rate(
             self,
             traverse_rate: float,
             unit: VelocityUnits
     ) -> None:
         """
         Sets the speed at which the device moves when traversing (G0).
 
         Args:
             traverse_rate: The traverse rate.
             unit: Units of the traverse rate.
         """
-        request = main_pb2.TranslatorSetTraverseRateRequest()
-        request.translator_id = self.translator_id
-        request.traverse_rate = traverse_rate
-        request.unit = units_from_literals(unit).value
+        request = dto.TranslatorSetTraverseRateRequest(
+            translator_id=self.translator_id,
+            traverse_rate=traverse_rate,
+            unit=unit,
+        )
         call_sync("gcode/set_traverse_rate", request)
 
     def set_axis_position(
             self,
             axis: str,
             position: float,
             unit: LengthUnits
@@ -224,19 +245,20 @@
         This method does not cause any movement.
 
         Args:
             axis: Letter of the axis.
             position: The position.
             unit: Units of position.
         """
-        request = main_pb2.TranslatorSetAxisPositionRequest()
-        request.translator_id = self.translator_id
-        request.axis = axis
-        request.position = position
-        request.unit = units_from_literals(unit).value
+        request = dto.TranslatorSetAxisPositionRequest(
+            translator_id=self.translator_id,
+            axis=axis,
+            position=position,
+            unit=unit,
+        )
         call_sync("gcode/set_axis_position", request)
 
     def get_axis_position(
             self,
             axis: str,
             unit: LengthUnits
     ) -> float:
@@ -247,20 +269,23 @@
         Args:
             axis: Letter of the axis.
             unit: Units of position.
 
         Returns:
             Position of translator's axis.
         """
-        request = main_pb2.TranslatorGetAxisPositionRequest()
-        request.translator_id = self.translator_id
-        request.axis = axis
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("gcode/get_axis_position", request, response)
+        request = dto.TranslatorGetAxisPositionRequest(
+            translator_id=self.translator_id,
+            axis=axis,
+            unit=unit,
+        )
+        response = call_sync(
+            "gcode/get_axis_position",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set_axis_home_position(
             self,
             axis: str,
             position: float,
             unit: LengthUnits
@@ -270,19 +295,20 @@
         This position is used by G28.
 
         Args:
             axis: Letter of the axis.
             position: The home position.
             unit: Units of position.
         """
-        request = main_pb2.TranslatorSetAxisPositionRequest()
-        request.translator_id = self.translator_id
-        request.axis = axis
-        request.position = position
-        request.unit = units_from_literals(unit).value
+        request = dto.TranslatorSetAxisPositionRequest(
+            translator_id=self.translator_id,
+            axis=axis,
+            position=position,
+            unit=unit,
+        )
         call_sync("gcode/set_axis_home", request)
 
     def set_axis_secondary_home_position(
             self,
             axis: str,
             position: float,
             unit: LengthUnits
@@ -292,19 +318,20 @@
         This position is used by G30.
 
         Args:
             axis: Letter of the axis.
             position: The home position.
             unit: Units of position.
         """
-        request = main_pb2.TranslatorSetAxisPositionRequest()
-        request.translator_id = self.translator_id
-        request.axis = axis
-        request.position = position
-        request.unit = units_from_literals(unit).value
+        request = dto.TranslatorSetAxisPositionRequest(
+            translator_id=self.translator_id,
+            axis=axis,
+            position=position,
+            unit=unit,
+        )
         call_sync("gcode/set_axis_secondary_home", request)
 
     def get_axis_coordinate_system_offset(
             self,
             coordinate_system: str,
             axis: str,
             unit: LengthUnits
@@ -316,73 +343,82 @@
             coordinate_system: Coordinate system (e.g. G54).
             axis: Letter of the axis.
             unit: Units of position.
 
         Returns:
             Offset in translator units of the axis.
         """
-        request = main_pb2.TranslatorGetAxisOffsetRequest()
-        request.translator_id = self.translator_id
-        request.coordinate_system = coordinate_system
-        request.axis = axis
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call_sync("gcode/get_axis_offset", request, response)
+        request = dto.TranslatorGetAxisOffsetRequest(
+            translator_id=self.translator_id,
+            coordinate_system=coordinate_system,
+            axis=axis,
+            unit=unit,
+        )
+        response = call_sync(
+            "gcode/get_axis_offset",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def reset_after_stream_error(
             self
     ) -> None:
         """
         Resets internal state after device rejected generated command.
         Axis positions become uninitialized.
         """
-        request = main_pb2.TranslatorEmptyRequest()
-        request.translator_id = self.translator_id
+        request = dto.TranslatorEmptyRequest(
+            translator_id=self.translator_id,
+        )
         call_sync("gcode/reset_after_stream_error", request)
 
     def set_feed_rate_override(
             self,
             coefficient: float
     ) -> None:
         """
         Allows to scale feed rate of the translated code by a coefficient.
 
         Args:
             coefficient: Coefficient of the original feed rate.
         """
-        request = main_pb2.TranslatorSetFeedRateOverrideRequest()
-        request.translator_id = self.translator_id
-        request.coefficient = coefficient
+        request = dto.TranslatorSetFeedRateOverrideRequest(
+            translator_id=self.translator_id,
+            coefficient=coefficient,
+        )
         call_sync("gcode/set_feed_rate_override", request)
 
     @staticmethod
     def __free(
             translator_id: int
     ) -> None:
         """
         Releases native resources of a translator.
 
         Args:
             translator_id: The ID of the translator.
         """
-        request = main_pb2.TranslatorEmptyRequest()
-        request.translator_id = translator_id
+        request = dto.TranslatorEmptyRequest(
+            translator_id=translator_id,
+        )
         call_sync("gcode/free", request)
 
     def __get_current_coordinate_system(
             self
     ) -> str:
         """
         Gets current coordinate system (e.g. G54).
 
         Returns:
             Current coordinate system.
         """
-        request = main_pb2.TranslatorEmptyRequest()
-        request.translator_id = self.translator_id
-        response = main_pb2.StringResponse()
-        call_sync("gcode/get_current_coordinate_system", request, response)
+        request = dto.TranslatorEmptyRequest(
+            translator_id=self.translator_id,
+        )
+        response = call_sync(
+            "gcode/get_current_coordinate_system",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
 
     def __del__(self) -> None:
         Translator.__free(self.translator_id)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/gcode/translator_config.py` & `zaber_motion-6.0.0/zaber_motion/dto/gcode/translator_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,54 @@
-﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
-# ============== DO NOT EDIT DIRECTLY ============== #
-# pylint: disable=W0201
-
-from typing import List, Optional  # pylint: disable=unused-import
-from ..protobufs import main_pb2
+# This file is generated. Do not modify by hand.
+# pylint: disable=line-too-long, unused-argument, unused-import
+from dataclasses import dataclass, field
+from typing import List, Optional, Dict, Any, TYPE_CHECKING
+import bson
 from .axis_mapping import AxisMapping
 from .axis_transformation import AxisTransformation
 
 
+@dataclass
 class TranslatorConfig:
     """
     Configuration of a translator.
     """
 
-    def __init__(
-            self: 'TranslatorConfig',
-            axis_mappings: Optional[List[AxisMapping]] = None,
-            axis_transformations: Optional[List[AxisTransformation]] = None
-    ) -> None:
-        self._axis_mappings = axis_mappings
-        self._axis_transformations = axis_transformations
-
-    @property
-    def axis_mappings(self) -> Optional[List[AxisMapping]]:
-        """
-        Optional custom mapping of translator axes to stream axes.
-        """
-
-        return self._axis_mappings
-
-    @axis_mappings.setter
-    def axis_mappings(self, value: Optional[List[AxisMapping]]) -> None:
-        self._axis_mappings = value
-
-    @property
-    def axis_transformations(self) -> Optional[List[AxisTransformation]]:
-        """
-        Optional transformation of axes.
-        """
-
-        return self._axis_transformations
-
-    @axis_transformations.setter
-    def axis_transformations(self, value: Optional[List[AxisTransformation]]) -> None:
-        self._axis_transformations = value
+    axis_mappings: Optional[List[AxisMapping]] = None
+    """
+    Optional custom mapping of translator axes to stream axes.
+    """
 
-    def __repr__(self) -> str:
-        return str(self.__dict__)
+    axis_transformations: Optional[List[AxisTransformation]] = None
+    """
+    Optional transformation of axes.
+    """
 
     @staticmethod
-    def to_protobuf(source: 'Optional[TranslatorConfig]') -> main_pb2.TranslatorConfig:
-        pb_data = main_pb2.TranslatorConfig()
-
-        if source is None:
-            return pb_data
+    def zero_values() -> 'TranslatorConfig':
+        return TranslatorConfig(
+            axis_mappings=None,
+            axis_transformations=None,
+        )
 
-        if not isinstance(source, TranslatorConfig):
-            raise TypeError("Provided value is not TranslatorConfig.")
+    @staticmethod
+    def from_binary(data_bytes: bytes) -> 'TranslatorConfig':
+        """" Deserialize a binary representation of this class. """
+        data = bson.loads(data_bytes)  # type: Dict[str, Any]
+        return TranslatorConfig.from_dict(data)
+
+    def to_binary(self) -> bytes:
+        """" Serialize this class to a binary representation. """
+        return bson.dumps(self.to_dict())  # type: ignore
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            'axisMappings': [item.to_dict() for item in self.axis_mappings] if self.axis_mappings is not None else None,
+            'axisTransformations': [item.to_dict() for item in self.axis_transformations] if self.axis_transformations is not None else None,
+        }
 
-        if source.axis_mappings is not None:
-            pb_data.axis_mappings.extend(
-                [AxisMapping.to_protobuf(item) for item in source.axis_mappings])
-        if source.axis_transformations is not None:
-            pb_data.axis_transformations.extend(
-                [AxisTransformation.to_protobuf(item) for item in source.axis_transformations])
-        return pb_data
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> 'TranslatorConfig':
+        return TranslatorConfig(
+            axis_mappings=[AxisMapping.from_dict(item) for item in data.get('axisMappings')] if data.get('axisMappings') is not None else None,  # type: ignore
+            axis_transformations=[AxisTransformation.from_dict(item) for item in data.get('axisTransformations')] if data.get('axisTransformations') is not None else None,  # type: ignore
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zaber_motion-5.2.2/zaber_motion/library.py` & `zaber_motion-6.0.0/zaber_motion/library.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from .call import call_sync
-from .protobufs import main_pb2
-from .log_output_mode import LogOutputMode
-from .device_db_source_type import DeviceDbSourceType
+from .dto import requests as dto
+from .dto.log_output_mode import LogOutputMode
+from .dto.device_db_source_type import DeviceDbSourceType
 
 
 class Library:
     """
     Access class to general library information and configuration.
     """
 
@@ -20,17 +20,18 @@
         """
         Sets library logging output.
 
         Args:
             mode: Logging output mode.
             file_path: Path of the file to open.
         """
-        request = main_pb2.SetLogOutputRequest()
-        request.mode = mode.value
-        request.file_path = file_path
+        request = dto.SetLogOutputRequest(
+            mode=mode,
+            file_path=file_path,
+        )
         call_sync("logging/set_output", request)
 
     @staticmethod
     def set_device_db_source(
             source_type: DeviceDbSourceType,
             url_or_file_path: str = ""
     ) -> None:
@@ -38,17 +39,18 @@
         Sets source of Device DB data. Allows selection of a web service or a local file.
 
         Args:
             source_type: Source type.
             url_or_file_path: URL of the web service or path to the local file.
                 Leave empty for the default URL of Zaber web service.
         """
-        request = main_pb2.SetDeviceDbSourceRequest()
-        request.source_type = source_type.value
-        request.url_or_file_path = url_or_file_path
+        request = dto.SetDeviceDbSourceRequest(
+            source_type=source_type,
+            url_or_file_path=url_or_file_path,
+        )
         call_sync("device_db/set_source", request)
 
     @staticmethod
     def enable_device_db_store(
             store_location: str = ""
     ) -> None:
         """
@@ -57,49 +59,53 @@
         The stored data are later used instead of the Device DB.
 
         Args:
             store_location: Specifies relative or absolute path of the folder used by the store.
                 If left empty defaults to a folder in user home directory.
                 Must be accessible by the process.
         """
-        request = main_pb2.ToggleDeviceDbStoreRequest()
-        request.toggle_on = True
-        request.store_location = store_location
+        request = dto.ToggleDeviceDbStoreRequest(
+            toggle_on=True,
+            store_location=store_location,
+        )
         call_sync("device_db/toggle_store", request)
 
     @staticmethod
     def disable_device_db_store() -> None:
         """
         Disables Device DB store.
         """
-        request = main_pb2.ToggleDeviceDbStoreRequest()
+        request = dto.ToggleDeviceDbStoreRequest(
+        )
         call_sync("device_db/toggle_store", request)
 
     @staticmethod
     def set_internal_mode(
             mode: bool
     ) -> None:
         """
         Disables certain customer checks (like FF flag).
 
         Args:
             mode: Whether to turn internal mode on or off.
         """
-        request = main_pb2.SetInternalModeRequest()
-        request.mode = mode
+        request = dto.SetInternalModeRequest(
+            mode=mode,
+        )
         call_sync("library/set_internal_mode", request)
 
     @staticmethod
     def set_idle_polling_period(
             period: int
     ) -> None:
         """
         Sets the period between polling for IDLE during movements.
         Caution: Setting the period too low may cause performance issues.
 
         Args:
             period: Period in milliseconds.
                 Negative value restores the default period.
         """
-        request = main_pb2.IntRequest()
-        request.value = period
+        request = dto.IntRequest(
+            value=period,
+        )
         call_sync("library/set_idle_polling_period", request)
```

### Comparing `zaber_motion-5.2.2/zaber_motion/microscopy/filter_changer.py` & `zaber_motion-6.0.0/zaber_motion/microscopy/filter_changer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 # pylint: disable=W0622
 
 from ..call import call, call_async, call_sync
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from ..ascii import Device
 
 
 class FilterChanger:
     """
     A generic turret device.
     """
@@ -30,121 +30,138 @@
     ) -> int:
         """
         Gets number of filters of the changer.
 
         Returns:
             Number of positions.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = 1
-        response = main_pb2.IntResponse()
-        call("device/get_index_count", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=1,
+        )
+        response = call(
+            "device/get_index_count",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     async def get_number_of_filters_async(
             self
     ) -> int:
         """
         Gets number of filters of the changer.
 
         Returns:
             Number of positions.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = 1
-        response = main_pb2.IntResponse()
-        await call_async("device/get_index_count", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=1,
+        )
+        response = await call_async(
+            "device/get_index_count",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     def get_current_filter(
             self
     ) -> int:
         """
         Returns the current filter number starting from 1.
         The value of 0 indicates that the position is either unknown or between two filters.
 
         Returns:
             Filter number starting from 1 or 0 if the position cannot be determined.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = 1
-        response = main_pb2.IntResponse()
-        call("device/get_index_position", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=1,
+        )
+        response = call(
+            "device/get_index_position",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     async def get_current_filter_async(
             self
     ) -> int:
         """
         Returns the current filter number starting from 1.
         The value of 0 indicates that the position is either unknown or between two filters.
 
         Returns:
             Filter number starting from 1 or 0 if the position cannot be determined.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = 1
-        response = main_pb2.IntResponse()
-        await call_async("device/get_index_position", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=1,
+        )
+        response = await call_async(
+            "device/get_index_position",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     def change(
             self,
             filter: int
     ) -> None:
         """
         Changes to the specified filter.
 
         Args:
             filter: Filter number starting from 1.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = 1
-        request.type = main_pb2.DeviceMoveRequest.INDEX
-        request.wait_until_idle = True
-        request.arg_int = filter
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=1,
+            type=dto.AxisMoveType.INDEX,
+            wait_until_idle=True,
+            arg_int=filter,
+        )
         call("device/move", request)
 
     async def change_async(
             self,
             filter: int
     ) -> None:
         """
         Changes to the specified filter.
 
         Args:
             filter: Filter number starting from 1.
         """
-        request = main_pb2.DeviceMoveRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        request.axis = 1
-        request.type = main_pb2.DeviceMoveRequest.INDEX
-        request.wait_until_idle = True
-        request.arg_int = filter
+        request = dto.DeviceMoveRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+            axis=1,
+            type=dto.AxisMoveType.INDEX,
+            wait_until_idle=True,
+            arg_int=filter,
+        )
         await call_async("device/move", request)
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the device.
 
         Returns:
             A string that represents the device.
         """
-        request = main_pb2.AxisToStringRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        response = main_pb2.StringResponse()
-        call_sync("device/device_to_string", request, response)
+        request = dto.AxisToStringRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+        )
+        response = call_sync(
+            "device/device_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/microscopy/illuminator.py` & `zaber_motion-6.0.0/zaber_motion/microscopy/illuminator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from ..call import call, call_async, call_sync
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from ..ascii import DeviceIO, Connection, Device
 from .illuminator_channel import IlluminatorChannel
 
 
 class Illuminator:
     """
     Use to manage an LED controller.
-    It is subject to breaking changes without warning until further notice.
     Requires at least Firmware 7.09.
     """
 
     @property
     def device(self) -> Device:
         """
         The base device of this illuminator.
@@ -58,17 +57,18 @@
 
     def __verify_is_illuminator(
             self
     ) -> None:
         """
         Checks if this is an illuminator or some other type of device and throws an error if it is not.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+        )
         call_sync("illuminator/verify", request)
 
     @staticmethod
     def find(
             connection: Connection,
             device_address: int = 0
     ) -> 'Illuminator':
@@ -79,19 +79,22 @@
         Args:
             connection: Connection on which to detect the illuminator.
             device_address: Optional device address of the illuminator.
 
         Returns:
             New instance of illuminator.
         """
-        request = main_pb2.FindDeviceRequest()
-        request.interface_id = connection.interface_id
-        request.device_address = device_address
-        response = main_pb2.FindDeviceResponse()
-        call("illuminator/detect", request, response)
+        request = dto.FindDeviceRequest(
+            interface_id=connection.interface_id,
+            device_address=device_address,
+        )
+        response = call(
+            "illuminator/detect",
+            request,
+            dto.FindDeviceResponse.from_binary)
         return Illuminator(Device(connection, response.address))
 
     @staticmethod
     async def find_async(
             connection: Connection,
             device_address: int = 0
     ) -> 'Illuminator':
@@ -102,29 +105,35 @@
         Args:
             connection: Connection on which to detect the illuminator.
             device_address: Optional device address of the illuminator.
 
         Returns:
             New instance of illuminator.
         """
-        request = main_pb2.FindDeviceRequest()
-        request.interface_id = connection.interface_id
-        request.device_address = device_address
-        response = main_pb2.FindDeviceResponse()
-        await call_async("illuminator/detect", request, response)
+        request = dto.FindDeviceRequest(
+            interface_id=connection.interface_id,
+            device_address=device_address,
+        )
+        response = await call_async(
+            "illuminator/detect",
+            request,
+            dto.FindDeviceResponse.from_binary)
         return Illuminator(Device(connection, response.address))
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the device.
 
         Returns:
             A string that represents the device.
         """
-        request = main_pb2.AxisToStringRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        response = main_pb2.StringResponse()
-        call_sync("device/device_to_string", request, response)
+        request = dto.AxisToStringRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+        )
+        response = call_sync(
+            "device/device_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/microscopy/microscope.py` & `zaber_motion-6.0.0/zaber_motion/microscopy/microscope.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import Optional
 from ..call import call, call_async, call_sync
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from ..ascii import Connection, Device, Axis, AxisGroup
 from .illuminator import Illuminator
 from .filter_changer import FilterChanger
 from .objective_changer import ObjectiveChanger
-from .microscope_config import MicroscopeConfig
+from ..dto.microscopy.microscope_config import MicroscopeConfig
 
 
 class Microscope:
     """
     Represent a microscope.
-    It is subject to breaking changes without warning until further notice.
     Parts of the microscope may or may not be instantiated depending on the configuration.
     Requires at least Firmware 7.34.
     """
 
     @property
     def connection(self) -> Connection:
         """
@@ -77,15 +76,15 @@
 
     def __init__(self, connection: Connection, config: MicroscopeConfig):
         """
         Creates instance of `Microscope` from the given config.
         Parts are instantiated depending on device addresses in the config.
         """
         self._connection = connection
-        self._config = MicroscopeConfig.from_protobuf(MicroscopeConfig.to_protobuf(config))
+        self._config = MicroscopeConfig.from_binary(MicroscopeConfig.to_binary(config))
         self._illuminator = Illuminator(Device(connection, config.illuminator)) if config.illuminator else None
         self._focus_axis = Axis(Device(connection, config.focus_axis.device), config.focus_axis.axis)\
             if config.focus_axis and config.focus_axis.device else None
         self._x_axis = Axis(Device(connection, config.x_axis.device), config.x_axis.axis)\
             if config.x_axis and config.x_axis.device else None
         self._y_axis = Axis(Device(connection, config.y_axis.device), config.y_axis.axis)\
             if config.y_axis and config.y_axis.device else None
@@ -105,113 +104,130 @@
 
         Args:
             connection: Connection on which to detect the microscope.
 
         Returns:
             New instance of microscope.
         """
-        request = main_pb2.InterfaceEmptyRequest()
-        request.interface_id = connection.interface_id
-        response = main_pb2.MicroscopeConfig()
-        call("microscope/detect", request, response)
-        return Microscope(connection, MicroscopeConfig.from_protobuf(response))
+        request = dto.InterfaceEmptyRequest(
+            interface_id=connection.interface_id,
+        )
+        response = call(
+            "microscope/detect",
+            request,
+            dto.MicroscopeConfigResponse.from_binary)
+        return Microscope(connection, response.config)
 
     @staticmethod
     async def find_async(
             connection: Connection
     ) -> 'Microscope':
         """
         Finds a microscope on a connection.
 
         Args:
             connection: Connection on which to detect the microscope.
 
         Returns:
             New instance of microscope.
         """
-        request = main_pb2.InterfaceEmptyRequest()
-        request.interface_id = connection.interface_id
-        response = main_pb2.MicroscopeConfig()
-        await call_async("microscope/detect", request, response)
-        return Microscope(connection, MicroscopeConfig.from_protobuf(response))
+        request = dto.InterfaceEmptyRequest(
+            interface_id=connection.interface_id,
+        )
+        response = await call_async(
+            "microscope/detect",
+            request,
+            dto.MicroscopeConfigResponse.from_binary)
+        return Microscope(connection, response.config)
 
     def initialize(
             self,
             force: bool = False
     ) -> None:
         """
         Initializes the microscope.
         Homes all axes, filter changer, and objective changer if they require it.
 
         Args:
             force: Forces all devices to home even when not required.
         """
-        request = main_pb2.MicroscopeInitRequest()
-        request.interface_id = self.connection.interface_id
-        request.config.CopyFrom(MicroscopeConfig.to_protobuf(self._config))
-        request.force = force
+        request = dto.MicroscopeInitRequest(
+            interface_id=self.connection.interface_id,
+            config=self._config,
+            force=force,
+        )
         call("microscope/initialize", request)
 
     async def initialize_async(
             self,
             force: bool = False
     ) -> None:
         """
         Initializes the microscope.
         Homes all axes, filter changer, and objective changer if they require it.
 
         Args:
             force: Forces all devices to home even when not required.
         """
-        request = main_pb2.MicroscopeInitRequest()
-        request.interface_id = self.connection.interface_id
-        request.config.CopyFrom(MicroscopeConfig.to_protobuf(self._config))
-        request.force = force
+        request = dto.MicroscopeInitRequest(
+            interface_id=self.connection.interface_id,
+            config=self._config,
+            force=force,
+        )
         await call_async("microscope/initialize", request)
 
     def is_initialized(
             self
     ) -> bool:
         """
         Checks whether the microscope is initialized.
 
         Returns:
             True, when the microscope is initialized. False, otherwise.
         """
-        request = main_pb2.MicroscopeEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.config.CopyFrom(MicroscopeConfig.to_protobuf(self._config))
-        response = main_pb2.BoolResponse()
-        call("microscope/is_initialized", request, response)
+        request = dto.MicroscopeEmptyRequest(
+            interface_id=self.connection.interface_id,
+            config=self._config,
+        )
+        response = call(
+            "microscope/is_initialized",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     async def is_initialized_async(
             self
     ) -> bool:
         """
         Checks whether the microscope is initialized.
 
         Returns:
             True, when the microscope is initialized. False, otherwise.
         """
-        request = main_pb2.MicroscopeEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.config.CopyFrom(MicroscopeConfig.to_protobuf(self._config))
-        response = main_pb2.BoolResponse()
-        await call_async("microscope/is_initialized", request, response)
+        request = dto.MicroscopeEmptyRequest(
+            interface_id=self.connection.interface_id,
+            config=self._config,
+        )
+        response = await call_async(
+            "microscope/is_initialized",
+            request,
+            dto.BoolResponse.from_binary)
         return response.value
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the microscope.
 
         Returns:
             A string that represents the microscope.
         """
-        request = main_pb2.MicroscopeEmptyRequest()
-        request.interface_id = self.connection.interface_id
-        request.config.CopyFrom(MicroscopeConfig.to_protobuf(self._config))
-        response = main_pb2.StringResponse()
-        call_sync("microscope/to_string", request, response)
+        request = dto.MicroscopeEmptyRequest(
+            interface_id=self.connection.interface_id,
+            config=self._config,
+        )
+        response = call_sync(
+            "microscope/to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-6.0.0/zaber_motion/microscopy/objective_changer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
+from typing import Optional
 from ..call import call, call_async, call_sync
-from ..protobufs import main_pb2
-from ..measurement import Measurement
+from ..dto import requests as dto
+from ..dto.measurement import Measurement
 from ..ascii import Connection, Device, Axis
-from ..units import Units, units_from_literals, LengthUnits
+from ..units import Units, LengthUnits
 
 
 class ObjectiveChanger:
     """
     Represents an objective changer of a microscope.
     Unstable. Expect breaking changes in future releases.
     Requires at least Firmware 7.32.
@@ -53,20 +54,23 @@
             connection: Connection on which to detect the objective changer.
             turret_address: Optional device address of the turret device (X-MOR).
             focus_address: Optional device address of the focus device (X-LDA).
 
         Returns:
             New instance of objective changer.
         """
-        request = main_pb2.ObjectiveChangerRequest()
-        request.interface_id = connection.interface_id
-        request.turret_address = turret_address
-        request.focus_address = focus_address
-        response = main_pb2.ObjectiveChangerCreateResponse()
-        call("objective_changer/detect", request, response)
+        request = dto.ObjectiveChangerRequest(
+            interface_id=connection.interface_id,
+            turret_address=turret_address,
+            focus_address=focus_address,
+        )
+        response = call(
+            "objective_changer/detect",
+            request,
+            dto.ObjectiveChangerCreateResponse.from_binary)
         return ObjectiveChanger(
             Device(connection, response.turret),
             Axis(Device(connection, response.focus_address), response.focus_axis))
 
     @staticmethod
     async def find_async(
             connection: Connection,
@@ -82,164 +86,183 @@
             connection: Connection on which to detect the objective changer.
             turret_address: Optional device address of the turret device (X-MOR).
             focus_address: Optional device address of the focus device (X-LDA).
 
         Returns:
             New instance of objective changer.
         """
-        request = main_pb2.ObjectiveChangerRequest()
-        request.interface_id = connection.interface_id
-        request.turret_address = turret_address
-        request.focus_address = focus_address
-        response = main_pb2.ObjectiveChangerCreateResponse()
-        await call_async("objective_changer/detect", request, response)
+        request = dto.ObjectiveChangerRequest(
+            interface_id=connection.interface_id,
+            turret_address=turret_address,
+            focus_address=focus_address,
+        )
+        response = await call_async(
+            "objective_changer/detect",
+            request,
+            dto.ObjectiveChangerCreateResponse.from_binary)
         return ObjectiveChanger(
             Device(connection, response.turret),
             Axis(Device(connection, response.focus_address), response.focus_axis))
 
     def change(
             self,
             objective: int,
-            focus_offset: Measurement = Measurement(0)
+            focus_offset: Optional[Measurement] = None
     ) -> None:
         """
         Changes the objective.
         Runs a sequence of movements switching from the current objective to the new one.
         The focus stage moves to the focus datum after the objective change.
 
         Args:
             objective: Objective number starting from 1.
             focus_offset: Optional offset from the focus datum.
         """
-        request = main_pb2.ObjectiveChangerChangeRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
-        request.objective = objective
-        request.focus_offset.CopyFrom(Measurement.to_protobuf(focus_offset))
+        request = dto.ObjectiveChangerChangeRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+            objective=objective,
+            focus_offset=focus_offset,
+        )
         call("objective_changer/change", request)
 
     async def change_async(
             self,
             objective: int,
-            focus_offset: Measurement = Measurement(0)
+            focus_offset: Optional[Measurement] = None
     ) -> None:
         """
         Changes the objective.
         Runs a sequence of movements switching from the current objective to the new one.
         The focus stage moves to the focus datum after the objective change.
 
         Args:
             objective: Objective number starting from 1.
             focus_offset: Optional offset from the focus datum.
         """
-        request = main_pb2.ObjectiveChangerChangeRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
-        request.objective = objective
-        request.focus_offset.CopyFrom(Measurement.to_protobuf(focus_offset))
+        request = dto.ObjectiveChangerChangeRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+            objective=objective,
+            focus_offset=focus_offset,
+        )
         await call_async("objective_changer/change", request)
 
     def release(
             self
     ) -> None:
         """
         Moves the focus stage out of the turret releasing the current objective.
         """
-        request = main_pb2.ObjectiveChangerRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
+        request = dto.ObjectiveChangerRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+        )
         call("objective_changer/release", request)
 
     async def release_async(
             self
     ) -> None:
         """
         Moves the focus stage out of the turret releasing the current objective.
         """
-        request = main_pb2.ObjectiveChangerRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
+        request = dto.ObjectiveChangerRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+        )
         await call_async("objective_changer/release", request)
 
     def get_current_objective(
             self
     ) -> int:
         """
         Returns current objective number starting from 1.
         The value of 0 indicates that the position is either unknown or between two objectives.
 
         Returns:
             Current objective number starting from 1 or 0 if not applicable.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.device = self.turret.device_address
-        request.axis = 1
-        response = main_pb2.IntResponse()
-        call("device/get_index_position", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.turret.connection.interface_id,
+            device=self.turret.device_address,
+            axis=1,
+        )
+        response = call(
+            "device/get_index_position",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     async def get_current_objective_async(
             self
     ) -> int:
         """
         Returns current objective number starting from 1.
         The value of 0 indicates that the position is either unknown or between two objectives.
 
         Returns:
             Current objective number starting from 1 or 0 if not applicable.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.device = self.turret.device_address
-        request.axis = 1
-        response = main_pb2.IntResponse()
-        await call_async("device/get_index_position", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.turret.connection.interface_id,
+            device=self.turret.device_address,
+            axis=1,
+        )
+        response = await call_async(
+            "device/get_index_position",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     def get_number_of_objectives(
             self
     ) -> int:
         """
         Gets number of objectives that the turret can accommodate.
 
         Returns:
             Number of positions.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.device = self.turret.device_address
-        request.axis = 1
-        response = main_pb2.IntResponse()
-        call("device/get_index_count", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.turret.connection.interface_id,
+            device=self.turret.device_address,
+            axis=1,
+        )
+        response = call(
+            "device/get_index_count",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     async def get_number_of_objectives_async(
             self
     ) -> int:
         """
         Gets number of objectives that the turret can accommodate.
 
         Returns:
             Number of positions.
         """
-        request = main_pb2.AxisEmptyRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.device = self.turret.device_address
-        request.axis = 1
-        response = main_pb2.IntResponse()
-        await call_async("device/get_index_count", request, response)
+        request = dto.AxisEmptyRequest(
+            interface_id=self.turret.connection.interface_id,
+            device=self.turret.device_address,
+            axis=1,
+        )
+        response = await call_async(
+            "device/get_index_count",
+            request,
+            dto.IntResponse.from_binary)
         return response.value
 
     def get_focus_datum(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
@@ -249,22 +272,25 @@
 
         Args:
             unit: Units of datum.
 
         Returns:
             The datum.
         """
-        request = main_pb2.ObjectiveChangerSetRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        call("objective_changer/get_datum", request, response)
+        request = dto.ObjectiveChangerSetRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+            unit=unit,
+        )
+        response = call(
+            "objective_changer/get_datum",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     async def get_focus_datum_async(
             self,
             unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
@@ -274,22 +300,25 @@
 
         Args:
             unit: Units of datum.
 
         Returns:
             The datum.
         """
-        request = main_pb2.ObjectiveChangerSetRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.DoubleResponse()
-        await call_async("objective_changer/get_datum", request, response)
+        request = dto.ObjectiveChangerSetRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+            unit=unit,
+        )
+        response = await call_async(
+            "objective_changer/get_datum",
+            request,
+            dto.DoubleResponse.from_binary)
         return response.value
 
     def set_focus_datum(
             self,
             datum: float,
             unit: LengthUnits = Units.NATIVE
     ) -> None:
@@ -298,21 +327,22 @@
         The focus datum is the position that the focus stage moves to after an objective change.
         It is backed by the limit.home.offset setting.
 
         Args:
             datum: Value of datum.
             unit: Units of datum.
         """
-        request = main_pb2.ObjectiveChangerSetRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
-        request.value = datum
-        request.unit = units_from_literals(unit).value
+        request = dto.ObjectiveChangerSetRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+            value=datum,
+            unit=unit,
+        )
         call("objective_changer/set_datum", request)
 
     async def set_focus_datum_async(
             self,
             datum: float,
             unit: LengthUnits = Units.NATIVE
     ) -> None:
@@ -321,44 +351,49 @@
         The focus datum is the position that the focus stage moves to after an objective change.
         It is backed by the limit.home.offset setting.
 
         Args:
             datum: Value of datum.
             unit: Units of datum.
         """
-        request = main_pb2.ObjectiveChangerSetRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
-        request.value = datum
-        request.unit = units_from_literals(unit).value
+        request = dto.ObjectiveChangerSetRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+            value=datum,
+            unit=unit,
+        )
         await call_async("objective_changer/set_datum", request)
 
     def __verify_is_changer(
             self
     ) -> None:
         """
         Checks if this is a objective changer and throws an error if it is not.
         """
-        request = main_pb2.ObjectiveChangerRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.turret_address = self.turret.device_address
-        request.focus_address = self.focus_axis.device.device_address
-        request.focus_axis = self.focus_axis.axis_number
+        request = dto.ObjectiveChangerRequest(
+            interface_id=self.turret.connection.interface_id,
+            turret_address=self.turret.device_address,
+            focus_address=self.focus_axis.device.device_address,
+            focus_axis=self.focus_axis.axis_number,
+        )
         call_sync("objective_changer/verify", request)
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the device.
 
         Returns:
             A string that represents the device.
         """
-        request = main_pb2.AxisToStringRequest()
-        request.interface_id = self.turret.connection.interface_id
-        request.device = self.turret.device_address
-        response = main_pb2.StringResponse()
-        call_sync("device/device_to_string", request, response)
+        request = dto.AxisToStringRequest(
+            interface_id=self.turret.connection.interface_id,
+            device=self.turret.device_address,
+        )
+        response = call_sync(
+            "device/device_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/product/process_controller.py` & `zaber_motion-6.0.0/zaber_motion/product/process_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import List
 from ..call import call, call_sync, call_async
 
-from ..protobufs import main_pb2
+from ..dto import requests as dto
 from ..ascii.device import Device
 from .process import Process
 from ..ascii.connection import Connection
 
 
 class ProcessController:
     """
@@ -42,20 +42,23 @@
         Args:
             connection: The connection to detect process controllers on.
             identify: If the Process Controllers should be identified upon detection.
 
         Returns:
             A list of all `ProcessController`s on the connection.
         """
-        request = main_pb2.DeviceDetectRequest()
-        request.type = main_pb2.DeviceDetectRequest.PROCESS_CONTROLLER
-        request.interface_id = connection.interface_id
-        request.identify_devices = identify
-        response = main_pb2.DeviceDetectResponse()
-        call("device/detect", request, response)
+        request = dto.DeviceDetectRequest(
+            type=dto.DeviceType.PROCESS_CONTROLLER,
+            interface_id=connection.interface_id,
+            identify_devices=identify,
+        )
+        response = call(
+            "device/detect",
+            request,
+            dto.DeviceDetectResponse.from_binary)
         return [ProcessController(connection.get_device(device)) for device in response.devices]
 
     @staticmethod
     async def detect_async(
             connection: Connection,
             identify: bool = True
     ) -> List['ProcessController']:
@@ -65,20 +68,23 @@
         Args:
             connection: The connection to detect process controllers on.
             identify: If the Process Controllers should be identified upon detection.
 
         Returns:
             A list of all `ProcessController`s on the connection.
         """
-        request = main_pb2.DeviceDetectRequest()
-        request.type = main_pb2.DeviceDetectRequest.PROCESS_CONTROLLER
-        request.interface_id = connection.interface_id
-        request.identify_devices = identify
-        response = main_pb2.DeviceDetectResponse()
-        await call_async("device/detect", request, response)
+        request = dto.DeviceDetectRequest(
+            type=dto.DeviceType.PROCESS_CONTROLLER,
+            interface_id=connection.interface_id,
+            identify_devices=identify,
+        )
+        response = await call_async(
+            "device/detect",
+            request,
+            dto.DeviceDetectResponse.from_binary)
         return [ProcessController(connection.get_device(device)) for device in response.devices]
 
     def get_process(
             self,
             process_number: int
     ) -> Process:
         """
@@ -98,27 +104,31 @@
 
     def __verify_is_process_controller(
             self
     ) -> None:
         """
         Checks if this is a process controller or some other type of device and throws an error if it is not.
         """
-        request = main_pb2.DeviceEmptyRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
+        request = dto.DeviceEmptyRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+        )
         call_sync("process_controller/verify", request)
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string that represents the device.
 
         Returns:
             A string that represents the device.
         """
-        request = main_pb2.AxisToStringRequest()
-        request.interface_id = self.device.connection.interface_id
-        request.device = self.device.device_address
-        response = main_pb2.StringResponse()
-        call_sync("device/device_to_string", request, response)
+        request = dto.AxisToStringRequest(
+            interface_id=self.device.connection.interface_id,
+            device=self.device.device_address,
+        )
+        response = call_sync(
+            "device/device_to_string",
+            request,
+            dto.StringResponse.from_binary)
         return response.value
```

### Comparing `zaber_motion-5.2.2/zaber_motion/serialization.py` & `zaber_motion-6.0.0/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.2/zaber_motion/unit_table.py` & `zaber_motion-6.0.0/zaber_motion/unit_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from .call import call_sync
-from .protobufs import main_pb2
-from .units import Units, UnitsAndLiterals, units_from_literals
+from .dto import requests as dto
+from .units import UnitsAndLiterals
 
 
 class UnitTable:
     """
     Helper for working with units of measure.
     """
 
@@ -20,18 +20,21 @@
 
         Args:
             unit: Unit of measure.
 
         Returns:
             Symbols corresponding to the given unit. Throws NoValueForKey if no symbol is defined.
         """
-        request = main_pb2.UnitGetSymbolRequest()
-        request.unit = units_from_literals(unit).value
-        response = main_pb2.UnitGetSymbolResponse()
-        call_sync("units/get_symbol", request, response)
+        request = dto.UnitGetSymbolRequest(
+            unit=unit,
+        )
+        response = call_sync(
+            "units/get_symbol",
+            request,
+            dto.UnitGetSymbolResponse.from_binary)
         return response.symbol
 
     @staticmethod
     def get_unit(
             symbol: str
     ) -> UnitsAndLiterals:
         """
@@ -40,12 +43,15 @@
 
         Args:
             symbol: Symbol to look up.
 
         Returns:
             The unit enum value with the given symbols. Throws NoValueForKey if the symbol is not supported for lookup.
         """
-        request = main_pb2.UnitGetEnumRequest()
-        request.symbol = symbol
-        response = main_pb2.UnitGetEnumResponse()
-        call_sync("units/get_enum", request, response)
-        return Units(response.unit)
+        request = dto.UnitGetEnumRequest(
+            symbol=symbol,
+        )
+        response = call_sync(
+            "units/get_enum",
+            request,
+            dto.UnitGetEnumResponse.from_binary)
+        return response.unit
```

### Comparing `zaber_motion-5.2.2/zaber_motion/units.py` & `zaber_motion-6.0.0/zaber_motion/units.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-5.2.2/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-6.0.0/zaber_motion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 5.2.2
+Version: 6.0.0
 Summary: An official library for communicating with Zaber devices.
 Author-email: "Zaber Technologies Inc." <contact@zaber.com>
 License: The MIT License (MIT)
         
         Copyright 2018-2022 Zaber Technologies Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -2133,20 +2133,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: protobuf<4.22.0,>=3.20.0
-Requires-Dist: rx>=3.0.0
+Requires-Dist: reactivex~=4.0.0
+Requires-Dist: bson~=0.5
 Provides-Extra: dev
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mypy-protobuf; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pycodestyle; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
```

