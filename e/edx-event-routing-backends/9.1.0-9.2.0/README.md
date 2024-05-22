# Comparing `tmp/edx-event-routing-backends-9.1.0.tar.gz` & `tmp/edx-event-routing-backends-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-event-routing-backends-9.1.0.tar", last modified: Fri May 17 13:41:42 2024, max compression
+gzip compressed data, was "edx-event-routing-backends-9.2.0.tar", last modified: Wed May 22 15:17:47 2024, max compression
```

## Comparing `edx-event-routing-backends-9.1.0.tar` & `edx-event-routing-backends-9.2.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.588855 edx-event-routing-backends-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-17 13:41:42.588855 edx-event-routing-backends-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.588855 edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-17 13:41:42.000000 edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-17 13:41:42.000000 edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:41:42.000000 edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-17 13:41:42.000000 edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:41:42.000000 edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 13:41:42.000000 edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 13:41:42.000000 edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.572855 edx-event-routing-backends-9.1.0/event_routing_backends/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.572855 edx-event-routing-backends-9.1.0/event_routing_backends/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/backends/async_events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    13293 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/backends/events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/backends/sync_events_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.572855 edx-event-routing-backends-9.1.0/event_routing_backends/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44447 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/backends/tests/test_events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.572855 edx-event-routing-backends-9.1.0/event_routing_backends/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.572855 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.572855 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/helpers/event_log_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/helpers/queued_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/recover_failed_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.576855 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/tests/test_recover_failed_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15596 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/transform_tracking_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.576855 edx-event-routing-backends-9.1.0/event_routing_backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/migrations/0002_auto_20210503_0648.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/migrations/0003_auto_20210713_0344.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/migrations/0004_auto_20211025_1053.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.576855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.576855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/envelope_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.576855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.576855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/tests/test_caliper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.576855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/mixins/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/mixins/base_transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.580855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/openedx_filters/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/openedx_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/openedx_filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.580855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.580855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/tests/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/tests/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/tests/openedx_filters/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/tests/transformers_test_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.580855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.580855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.580855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.584855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/completion_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/exam_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/forum_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/grading_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.584855 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.584855 edx-event-routing-backends-9.1.0/event_routing_backends/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.568855 edx-event-routing-backends-9.1.0/event_routing_backends/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.568855 edx-event-routing-backends-9.1.0/event_routing_backends/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.584855 edx-event-routing-backends-9.1.0/event_routing_backends/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.568855 edx-event-routing-backends-9.1.0/event_routing_backends/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.584855 edx-event-routing-backends-9.1.0/event_routing_backends/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/templates/admin/router_conf_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.584855 edx-event-routing-backends-9.1.0/event_routing_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.588855 edx-event-routing-backends-9.1.0/event_routing_backends/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/event_routing_backends/utils/xapi_lrs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:41:42.588855 edx-event-routing-backends-9.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-17 13:41:42.588855 edx-event-routing-backends-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-17 13:41:34.000000 edx-event-routing-backends-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.029593 edx-event-routing-backends-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-22 15:17:47.029593 edx-event-routing-backends-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-22 15:17:46.000000 edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-22 15:17:47.000000 edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:17:46.000000 edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 15:17:46.000000 edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:17:46.000000 edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-22 15:17:46.000000 edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 15:17:46.000000 edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.013593 edx-event-routing-backends-9.2.0/event_routing_backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.013593 edx-event-routing-backends-9.2.0/event_routing_backends/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/backends/async_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13293 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/backends/events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/backends/sync_events_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.013593 edx-event-routing-backends-9.2.0/event_routing_backends/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44447 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/backends/tests/test_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.013593 edx-event-routing-backends-9.2.0/event_routing_backends/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.013593 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.013593 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/helpers/event_log_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/helpers/queued_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/recover_failed_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.013593 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/tests/test_recover_failed_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15596 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/transform_tracking_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.017593 edx-event-routing-backends-9.2.0/event_routing_backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/migrations/0002_auto_20210503_0648.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/migrations/0003_auto_20210713_0344.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/migrations/0004_auto_20211025_1053.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.017593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.017593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/envelope_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.017593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.017593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/tests/test_caliper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.017593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/mixins/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/mixins/base_transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.021593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/openedx_filters/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/openedx_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/openedx_filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.021593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.021593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/tests/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/tests/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/tests/openedx_filters/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/tests/transformers_test_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.021593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.021593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.021593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/completion_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/exam_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/forum_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/grading_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/event_routing_backends/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.009593 edx-event-routing-backends-9.2.0/event_routing_backends/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.009593 edx-event-routing-backends-9.2.0/event_routing_backends/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/event_routing_backends/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.009593 edx-event-routing-backends-9.2.0/event_routing_backends/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/event_routing_backends/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/templates/admin/router_conf_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/event_routing_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/event_routing_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/event_routing_backends/utils/xapi_lrs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:17:47.025593 edx-event-routing-backends-9.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-22 15:17:47.029593 edx-event-routing-backends-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-22 15:17:43.000000 edx-event-routing-backends-9.2.0/setup.py
```

### Comparing `edx-event-routing-backends-9.1.0/CHANGELOG.rst` & `edx-event-routing-backends-9.2.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[9.2.0]
+
+* Add discussion reference to comments and responses xAPI events
+
+[9.1.0]
+
+* Add python 3.11 and 3.12 support
+
 [9.0.1]
 
 * Fix an issue with the event routing backend async task to not find the event-tracking backend.
 
 [9.0.0]
 ~~~~~~~
```

### Comparing `edx-event-routing-backends-9.1.0/LICENSE.txt` & `edx-event-routing-backends-9.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/PKG-INFO` & `edx-event-routing-backends-9.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 9.1.0
+Version: 9.2.0
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -138,14 +138,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[9.2.0]
+
+* Add discussion reference to comments and responses xAPI events
+
+[9.1.0]
+
+* Add python 3.11 and 3.12 support
+
 [9.0.1]
 
 * Fix an issue with the event routing backend async task to not find the event-tracking backend.
 
 [9.0.0]
 ~~~~~~~
```

### Comparing `edx-event-routing-backends-9.1.0/README.rst` & `edx-event-routing-backends-9.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/PKG-INFO` & `edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 9.1.0
+Version: 9.2.0
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -138,14 +138,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[9.2.0]
+
+* Add discussion reference to comments and responses xAPI events
+
+[9.1.0]
+
+* Add python 3.11 and 3.12 support
+
 [9.0.1]
 
 * Fix an issue with the event routing backend async task to not find the event-tracking backend.
 
 [9.0.0]
 ~~~~~~~
```

### Comparing `edx-event-routing-backends-9.1.0/edx_event_routing_backends.egg-info/SOURCES.txt` & `edx-event-routing-backends-9.2.0/edx_event_routing_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/admin.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/admin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/apps.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/apps.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/backends/async_events_router.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/backends/async_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/backends/events_router.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/backends/events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/backends/sync_events_router.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/backends/sync_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/backends/tests/test_events_router.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/backends/tests/test_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/helpers.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/helpers/event_log_parser.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/helpers/event_log_parser.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/helpers/queued_sender.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/helpers/queued_sender.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/recover_failed_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/recover_failed_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/tests/test_recover_failed_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/tests/test_recover_failed_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/management/commands/transform_tracking_logs.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/management/commands/transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/migrations/0001_initial.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/migrations/0002_auto_20210503_0648.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/migrations/0002_auto_20210503_0648.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/migrations/0004_auto_20211025_1053.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/migrations/0004_auto_20211025_1053.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/models.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/__init__.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/envelope_processor.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/__init__.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/event_transformers/video_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/tests/test_caliper.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/tests/test_caliper.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/tests/test_transformers.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/transformer.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/caliper/transformer_processor.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/caliper/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/mixins/base_transformer.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/mixins/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/mixins/base_transformer_processor.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/mixins/base_transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/openedx_filters/decorators.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/openedx_filters/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/openedx_filters/filters.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/openedx_filters/filters.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/tests/openedx_filters/test_filters.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/tests/openedx_filters/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/tests/transformers_test_mixin.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/tests/transformers_test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/registry.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/__init__.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/constants.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/constants.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/__init__.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/completion_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/completion_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/exam_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/exam_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/forum_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/forum_events.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,25 +23,52 @@
         Returns:
             `Activity`
         """
 
         object_id = self.get_data('data.id', True)
         object_path = self.get_data('context.path', True).rstrip('/').replace(object_id, '').rstrip('/')
 
+        kwargs = {}
+
+        if self.get_data('data.title'):
+            kwargs['name'] = LanguageMap({constants.EN: self.get_data('data.title')})
+
         return Activity(
             id='{lms_root_url}{object_path}/{object_id}'.format(
                     lms_root_url=settings.LMS_ROOT_URL,
                     object_path=object_path,
                     object_id=object_id
                 ),
             definition=ActivityDefinition(
                 type=constants.XAPI_ACTIVITY_DISCUSSION,
+                **kwargs
             )
         )
 
+    def get_context_activities(self):
+        context_activities = super().get_context_activities()
+
+        discussion = self.get_data('data.discussion.id')
+        if not discussion:
+            return context_activities
+
+        context_activities.grouping = [
+            Activity(
+                id='{lms_root_url}/api/discussion/v1/threads/{discussion_id}'.format(
+                    lms_root_url=settings.LMS_ROOT_URL,
+                    discussion_id=discussion
+                ),
+                definition=ActivityDefinition(
+                    type=constants.XAPI_ACTIVITY_DISCUSSION,
+                )
+            )
+        ]
+
+        return context_activities
+
 
 @XApiTransformersRegistry.register('edx.forum.thread.created')
 class ThreadCreatedTransformer(BaseForumThreadTransformer):
     """
     Transformers for event generated when learner creates a thread in discussion forum.
     """
     _verb = Verb(
```

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/grading_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/grading_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/event_transformers/video_events.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/tests/test_transformers.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/tests/test_xapi.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/transformer.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/processors/xapi/transformer_processor.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/processors/xapi/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/settings/common.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/settings/common.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/settings/production.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/settings/production.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js` & `edx-event-routing-backends-9.2.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/tasks.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/tests/factories.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/tests/test_helpers.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/tests/test_mixin.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/tests/test_models.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/tests/test_settings.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/utils/http_client.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/event_routing_backends/utils/xapi_lrs_client.py` & `edx-event-routing-backends-9.2.0/event_routing_backends/utils/xapi_lrs_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/requirements/base.in` & `edx-event-routing-backends-9.2.0/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/requirements/constraints.txt` & `edx-event-routing-backends-9.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-9.1.0/setup.py` & `edx-event-routing-backends-9.2.0/setup.py`

 * *Files identical despite different names*

