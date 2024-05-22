# Comparing `tmp/sentry-kafka-schemas-0.1.87.tar.gz` & `tmp/sentry-kafka-schemas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-kafka-schemas-0.1.87.tar", last modified: Wed May 22 17:29:17 2024, max compression
+gzip compressed data, was "sentry-kafka-schemas-0.1.9.tar", last modified: Sat May 20 00:27:12 2023, max compression
```

## Comparing `sentry-kafka-schemas-0.1.87.tar` & `sentry-kafka-schemas-0.1.9.tar`

### file list

```diff
@@ -1,315 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.188406 sentry-kafka-schemas-0.1.87/
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 17:29:17.188406 sentry-kafka-schemas-0.1.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.156406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/codecs/msgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.156406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/any/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/any/garbage1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/buffered-segments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.156406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/buffered-segments/1/
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/buffered-segments/1/basic_buffered_segment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/end-merge.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
--rw-r--r--   0 runner    (1001) docker     (127)    61706 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/errors1.json
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/null-values.json
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/replace-group.json
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/start-merge.json
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/generic-events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/generic-events/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/generic-events/1/generic.json
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/generic-events/1/insert.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/group-attributes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/group-attributes/1/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/group-attributes/1/assignee_changed.json
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/group-attributes/1/group_created.json
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/group-attributes/1/group_deleted.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/group-attributes/1/owner_changed.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-events/1/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-events/1/dev-default-message.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-feedback-events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-feedback-events/1/
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-feedback-events/1/pokemart-widget-kcat.msgpack
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-feedback-events/1/relay-test_feedback_event_with_processing.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/1/base64-dist.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/1/base64-set.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/1/zstd-dist.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-metrics/1/zstd-set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-monitors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-monitors/1/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-monitors/1/checkin.msgpack
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-monitors/1/clock_pulse.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-events/1/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-events/1/archive.json
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-events/1/click-serialized.json
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-events/1/click.json
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-events/1/event-link.json
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-events/1/segment.json
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-events/1/viewed.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.160406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/monitors-clock-tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/monitors-clock-tasks/1/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/monitors-clock-tasks/1/mark_missing.json
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/monitors-clock-tasks/1/mark_timeout.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/monitors-clock-tick/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/monitors-clock-tick/1/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/monitors-clock-tick/1/example.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/outcomes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/outcomes/1/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/profile-functions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/profile-functions/1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/profile-functions/1/basic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/profile-metadata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/profile-metadata/1/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/profile-metadata/1/basic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.148406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/shared-resources-usage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/shared-resources-usage/1/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/shared-resources-usage/1/shared-resources-usage1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-commit-log/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-commit-log/1/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-commit-log/1/commit-log.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics-dist-base64.json
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics-dist-encoded-plain-array.json
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics-dist-zstd.json
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics-gauge.json
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics-set-encoded-plain-array.json
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics-sets-base64.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics-sets-zstd.json
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-metrics-summaries/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-metrics-summaries/1/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-metrics-summaries/1/metrics_summary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-profile-chunks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-profile-chunks/1/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-profile-chunks/1/valid.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.164406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries-empty-trace-id.json
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-spans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.168406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-spans/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-spans/1/basic_span.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-results/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.168406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-results/1/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-scheduled/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.168406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-scheduled/1/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-scheduled/1/example.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.152406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.168406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/transactions/1/
--rw-r--r--   0 runner    (1001) docker     (127)     8626 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.176406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:15.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:09.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/buffered_segments_dlq_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-22 17:29:11.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/buffered_segments_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:11.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/event_replacements_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 17:29:08.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-22 17:29:07.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/events_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    70487 2024-05-22 17:29:12.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/generic_events_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 17:29:13.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-22 17:29:05.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/group_attributes_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:03.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_attachments_dlq_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:11.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_events_dlq_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-22 17:29:05.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_events_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:07.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_feedback_events_dlq_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-22 17:29:11.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_feedback_events_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:14.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_generic_metrics_dlq_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:14.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_metrics_dlq_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-22 17:29:13.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-22 17:29:04.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_monitors_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-22 17:29:05.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_performance_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 17:29:14.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_replay_events_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-22 17:29:09.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:15.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_transactions_dlq_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 17:29:06.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-22 17:29:14.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/monitors_clock_tasks_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-22 17:29:09.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/monitors_clock_tick_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 17:29:15.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/outcomes_billing_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 17:29:08.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-22 17:29:09.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/processed_profiles_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-22 17:29:04.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/profiles_call_tree_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 17:29:12.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_events_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 17:29:06.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_generic_metrics_counters_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 17:29:07.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_generic_metrics_distributions_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 17:29:15.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_generic_metrics_gauges_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 17:29:09.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_generic_metrics_sets_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 17:29:15.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-22 17:29:04.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_transactions_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 17:29:06.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/shared_resources_usage_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:05.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_commit_log_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:06.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_dead_letter_generic_events_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:14.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_dead_letter_generic_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:08.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_dead_letter_group_attributes_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:04.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_dead_letter_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:07.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_dead_letter_querylog_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:08.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_dead_letter_replays_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:05.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_generic_events_commit_log_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:04.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_counters_commit_log_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:12.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_distributions_commit_log_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:10.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_gauges_commit_log_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:13.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_sets_commit_log_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-22 17:29:13.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:13.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_metrics_commit_log_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-22 17:29:07.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_metrics_summaries_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-22 17:29:11.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 17:29:08.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_profile_chunks_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-22 17:29:12.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-22 17:29:10.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_spans_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 17:29:06.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/snuba_transactions_commit_log_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 17:29:10.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    29235 2024-05-22 17:29:10.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/transactions_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.180406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/any.json
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/buffered-segments.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    19868 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    79416 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/generic-events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/group-attributes.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/ingest-events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/ingest-feedback-events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/ingest-monitors.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/ingest-replay-events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/monitors-clock-tasks.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/monitors-clock-tick.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/profile-functions.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/profile-metadata.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/shared-resources-usage.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/snuba-metrics-summaries.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/snuba-profile-chunks.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/snuba-spans.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/subscription-scheduled.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    38757 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/sentry_kafka_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.188406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/buffered-segments-dlq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/buffered-segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/event-replacements.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/generic-events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/group-attributes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-attachments-dlq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-events-dlq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-feedback-events-dlq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-feedback-events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-generic-metrics-dlq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-metrics-dlq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-monitors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-performance-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-replay-events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/ingest-transactions-dlq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/monitors-clock-tasks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/monitors-clock-tick.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/outcomes-billing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/outcomes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/processed-profiles.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/profiles-call-tree.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/scheduled-subscriptions-events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/scheduled-subscriptions-generic-metrics-counters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/scheduled-subscriptions-generic-metrics-distributions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/scheduled-subscriptions-generic-metrics-gauges.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/scheduled-subscriptions-generic-metrics-sets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/scheduled-subscriptions-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/scheduled-subscriptions-transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/shared-resources-usage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-commit-log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-dead-letter-generic-events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-dead-letter-generic-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-dead-letter-group-attributes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-dead-letter-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-dead-letter-querylog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-dead-letter-replays.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-generic-events-commit-log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-generic-metrics-counters-commit-log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-generic-metrics-distributions-commit-log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-generic-metrics-gauges-commit-log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-generic-metrics-sets-commit-log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-metrics-commit-log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-metrics-summaries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-profile-chunks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-spans.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/snuba-transactions-commit-log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/topics/transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.156406 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 17:29:17.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17006 2024-05-22 17:29:17.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:29:17.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:29:17.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 17:29:17.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 17:29:17.000000 sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:29:17.188406 sentry-kafka-schemas-0.1.87/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/tests/test_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/tests/test_codeowner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/tests/test_sentry_kafka_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/tests/test_valid_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/python/tests/test_valid_topic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:29:17.188406 sentry-kafka-schemas-0.1.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-22 17:28:58.000000 sentry-kafka-schemas-0.1.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.587360 sentry-kafka-schemas-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-20 00:27:12.587360 sentry-kafka-schemas-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.563357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/msgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.567358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/errors1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/replace-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/start-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.575358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.575358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.579359 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:10.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:09.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59601 2023-05-20 00:27:07.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/events_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:08.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-20 00:27:08.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-20 00:27:08.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:10.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-20 00:27:10.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:10.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-20 00:27:07.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-20 00:27:09.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-20 00:27:09.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:08.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25054 2023-05-20 00:27:09.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/transactions_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.579359 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    89040 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/events.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38689 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/sentry_kafka_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.583359 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/outcomes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/snuba-queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.563357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.587360 sentry-kafka-schemas-0.1.9/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_codeowner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_sentry_kafka_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_valid_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_valid_topic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:27:12.587360 sentry-kafka-schemas-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/setup.py
```

### Comparing `sentry-kafka-schemas-0.1.87/README.md` & `sentry-kafka-schemas-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 ## Defining schemas
 
 Currently only jsonschema is supported. The jsonschema should be placed directly in the `schemas` directory, and then referenced from the relevant topic via `resource` property.
 
 We use jsonschema for both JSON- and msgpack-based topics, as most msgpack types have a JSON-equivalent. For bytestrings, we type them using `{"description": "msgpack bytes"}`, which is currently just interpreted like `{}` (allow all types).
 
-If you don't want to hand-write it, for generating an initial json schema from a payload we like https://github.com/quicktype/quicktype
-
 ## How strict should my schema be?
 
 If in doubt, we recommend that schemas are only as strict as is minimally required by all consumers and downstream code required by Sentry. However it is ultimately up to the owners of the schema to decide whether a stricter schema is appropriate in particular scenarios.
 
 ## Adding example messages
 
 Example messages can be placed in the `examples` directory and referenced from the relevant topic/version.
@@ -110,18 +108,14 @@
 
 ## Release process and development install
 
 For releasing a new stable version from main branch, go to
 [Actions](https://github.com/getsentry/sentry-kafka-schemas/actions) and
 trigger a new job for the `Release` workflow.
 
-We usually just increment the `patch` number for schema changes.
-e.g. If the last version was 0.1.11, the next version should be 0.1.12.
-Check https://github.com/getsentry/sentry-kafka-schemas/releases for the latest release numbers.
-
 After releasing a new version, you should immediately bump Sentry, Snuba and
 Relay to ensure that all services are synchronized onto the new schema as
 soon as possible.
 
 Most likely you are working on a PR to Snuba or Sentry where you already want
 to use those types. You can do that by running `make build` in this repo, then
 running `pip install -e ~/projects/sentry-kafka-schemas/`.
@@ -134,9 +128,7 @@
 working on, you can reinstall Python dependencies in that repo. Most likely the
 command is `make install-py-dev`.
 
 ## Schema ownership
 
 All topics definitions, schemas and examples should have a defined owner or multiple owners if shared.
 The CODEOWNERS file should be updated with this information whenever new schemas and topics are added.
-
-Review is only required from one team/owner, not from all of them.
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/codecs/__init__.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/codecs/json.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/json.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/codecs/msgpack.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/msgpack.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/errors1.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/errors1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/null-values.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/null-values.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries-empty-trace-id.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981060606060606%*

 * *Differences: {"'query_list'": "{0: {'trace_id': '8377f280e7eb4754a7f20df73ce2cf37'}}"}*

```diff
@@ -59,15 +59,15 @@
                 "result_cols": 5,
                 "result_rows": 22,
                 "sample": null,
                 "table_concurrent": 1,
                 "table_rate": 0.6
             },
             "status": "success",
-            "trace_id": ""
+            "trace_id": "8377f280e7eb4754a7f20df73ce2cf37"
         }
     ],
     "request": {
         "app_id": "legacy",
         "body": {
             "app_id": "legacy",
             "dataset": "events",
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {"'organization'": '1'}*

```diff
@@ -1,11 +1,12 @@
 {
     "dataset": "events",
     "end_timestamp": 1675919559,
     "entity": "events",
+    "organization": 1,
     "projects": [
         1
     ],
     "query_list": [
         {
             "end_timestamp": 1675919559,
             "profile": {
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Any, TypedDict, Literal
+from typing import List, Dict, TypedDict, Literal, Any
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """ payload_v3. """
 
     subscription_id: Required[str]
@@ -33,19 +33,15 @@
 class SubscriptionResult(TypedDict, total=False):
     """ subscription_result. """
 
     version: Required[Literal[3]]
     """ Required property """
 
     payload: Required["PayloadV3"]
-    """
-    payload_v3.
-
-    Required property
-    """
+    """ Required property """
 
 
 
 class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
     """ Required property """
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/generic_events_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/events_v1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,142 @@
-from typing import Literal, List, Tuple, TypedDict, Any, Union, Dict
+from typing import TypedDict, Any, Tuple, Dict, Union, Literal, List
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
  The SDK Interface describes the Sentry SDK and its configuration used to capture and transmit an event.
-
-Aggregation type: anyOf
 """
 
 
 
-GenericEvent = Union[Tuple[Literal[2], Literal['insert'], "InsertEvent", "_GroupInformation"]]
-"""
-generic_event.
+class EndDeleteGroupsMessageBody(TypedDict, total=False):
+    """ end_delete_groups_message_body. """
+
+    transaction_id: str
+    project_id: Required[int]
+    """ Required property """
+
+    group_ids: Required[List[int]]
+    """ Required property """
+
+    datetime: Required[str]
+    """ Required property """
+
+
+
+class EndDeleteTagMessageBody(TypedDict, total=False):
+    """ end_delete_tag_message_body. """
+
+    tag: Required[str]
+    """ Required property """
+
+    datetime: Required[str]
+    """ Required property """
+
+    project_id: Required[int]
+    """ Required property """
 
-Issue platform event
 
-Aggregation type: anyOf
+
+class EndMergeMessageBody(TypedDict, total=False):
+    """ end_merge_message_body. """
+
+    transaction_id: str
+    project_id: Required[int]
+    """ Required property """
+
+    previous_group_ids: Required[List[int]]
+    """ Required property """
+
+    new_group_id: Required[int]
+    """ Required property """
+
+    datetime: Required[str]
+    """ Required property """
+
+
+
+class EndUnmergeHierarchicalMessageBody(TypedDict, total=False):
+    """ end_unmerge_hierarchical_message_body. """
+
+    project_id: Required[int]
+    """ Required property """
+
+    previous_group_id: Required[int]
+    """ Required property """
+
+    new_group_id: Required[int]
+    """ Required property """
+
+    primary_hash: Required[str]
+    """ Required property """
+
+    hierarchical_hash: Required[str]
+    """ Required property """
+
+    datetime: Required[str]
+    """ Required property """
+
+
+
+class EndUnmergeMessageBody(TypedDict, total=False):
+    """ end_unmerge_message_body. """
+
+    transaction_id: str
+    project_id: Required[int]
+    """ Required property """
+
+    previous_group_id: Required[int]
+    """ Required property """
+
+    new_group_id: Required[int]
+    """ Required property """
+
+    hashes: Required[List[str]]
+    """ Required property """
+
+    datetime: Required[str]
+    """ Required property """
+
+
+
+EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_GroupInformation"], Tuple[Literal[2], Literal["start_delete_groups"], "_StartDeleteGroupsMessage2"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
 """
+event_stream_message.
+
+The snuba eventstream message.
+"""
+
+
+
+class ExcludeGroupsMessageBody(TypedDict, total=False):
+    """ exclude_groups_message_body. """
+
+    project_id: Required[int]
+    """ Required property """
+
+    group_ids: Required[List[int]]
+    """ Required property """
 
 
 
 class InsertEvent(TypedDict, total=False):
     """ insert_event. """
 
     data: Required["SentryEvent"]
-    """
-    sentry_event.
-
-    The sentry v7 event structure.
-
-    Required property
-    """
+    """ Required property """
 
     datetime: Required[str]
     """ Required property """
 
     event_id: Required["_EventId"]
-    """
-     Wrapper around a UUID with slightly different formatting.
-
-    Aggregation type: anyOf
-
-    Required property
-    """
+    """ Required property """
 
     group_id: Required[int]
     """ Required property """
 
     group_ids: List[int]
     message: Required[str]
     """ Required property """
@@ -62,30 +148,42 @@
     primary_hash: Required[str]
     """ Required property """
 
     project_id: Required[int]
     """ Required property """
 
     retention_days: Union[int, None]
-    occurrence_id: Required[str]
+
+
+class ReplaceGroupMessageBody(TypedDict, total=False):
+    """ replace_group_message_body. """
+
+    event_ids: Required[List[str]]
     """ Required property """
 
-    occurrence_data: Required["_InsertEventOccurrenceData"]
+    project_id: Required[int]
+    """ Required property """
+
+    from_timestamp: str
+    to_timestamp: str
+    transaction_id: str
+    datetime: str
+    new_group_id: Required[int]
     """ Required property """
 
 
 
 class SentryEvent(TypedDict, total=False):
     """
     sentry_event.
 
     The sentry v7 event structure.
     """
 
-    type: "_SentryEventType"
+    type: Union["_EventType", None]
     """
      Type of the event. Defaults to `default`.
 
      The event type determines how Sentry handles the event and has an impact on processing, rate
      limiting, and quotas. There are three fundamental classes of event types:
 
       - **Error monitoring events**: Processed and grouped into unique issues based on their
@@ -103,24 +201,18 @@
 
      ```json
      {
        "type": "transaction",
        "spans": []
      }
      ```
-
-    Aggregation type: anyOf
     """
 
-    contexts: "_SentryEventContexts"
-    """
-     Contexts describing the environment (e.g. device, os or browser).
-
-    Aggregation type: anyOf
-    """
+    contexts: Union["_Contexts", None]
+    """  Contexts describing the environment (e.g. device, os or browser). """
 
     culprit: Union[str, None]
     """
      Custom culprit of the event.
 
      This field is deprecated and shall not be set by client SDKs.
     """
@@ -141,30 +233,15 @@
      The environment name, such as `production` or `staging`.
 
      ```json
      { "environment": "production" }
      ```
     """
 
-    errors: Union[List["_SentryEventErrorsArrayItem"], None]
-    """
-     Errors encountered during processing. Intended to be phased out in favor of
-     annotation/metadata system.
-
-    default: None
-    items:
-      anyOf:
-      - $ref: '#/definitions/EventProcessingError'
-      - type: 'null'
-      used: !!set
-        $ref: null
-        anyOf: null
-    """
-
-    event_id: "_SentryEventEventId"
+    event_id: Union["_EventId", None]
     """
      Unique identifier of this event.
 
      Hexadecimal string representing a uuid4 value. The length is exactly 32 characters. Dashes
      are not allowed. Has to be lowercase.
 
      Even though this field is backfilled on the server with a new uuid4, it is strongly
@@ -175,74 +252,58 @@
      Example:
 
      ```json
      {
        "event_id": "fc6d8c0c43fc4630ad850ee518f1b9d0"
      }
      ```
-
-    Aggregation type: anyOf
     """
 
-    exception: "_SentryEventException"
-    """ Aggregation type: anyOf """
-
-    threads: "_SentryEventThreads"
-    """ Aggregation type: anyOf """
-
+    exception: Union["SentryExceptionChain", None]
+    threads: Union["SentryThreadChain", None]
     extra: Union[Dict[str, Any], None]
     """
      Arbitrary extra information set by the user.
 
      ```json
      {
          "extra": {
              "my_key": 1,
              "some_other_value": "foo bar"
          }
      }```
-
-    additionalProperties: True
     """
 
-    fingerprint: "_SentryEventFingerprint"
+    fingerprint: Union["_Fingerprint", None]
     """
      Manual fingerprint override.
 
      A list of strings used to dictate how this event is supposed to be grouped with other
      events into issues. For more information about overriding grouping see [Customize Grouping
      with Fingerprints](https://docs.sentry.io/data-management/event-grouping/).
 
      ```json
      {
          "fingerprint": ["myrpc", "POST", "/foo.bar"]
      }
-
-    Aggregation type: anyOf
     """
 
-    level: "_SentryEventLevel"
+    level: Union["_Level", None]
     """
      Severity level of the event. Defaults to `error`.
 
      Example:
 
      ```json
      {"level": "warning"}
      ```
-
-    Aggregation type: anyOf
     """
 
-    logentry: "_SentryEventLogentry"
-    """
-     Custom parameterized message for this event.
-
-    Aggregation type: anyOf
-    """
+    logentry: Union["_LogEntry", None]
+    """  Custom parameterized message for this event. """
 
     logger: Union[str, None]
     """  Logger that created the event. """
 
     modules: Union[Dict[str, Union[str, None]], None]
     """
      Name and versions of all installed modules/packages/dependencies in the current
@@ -254,19 +315,14 @@
 
      In Python this is a list of installed packages as reported by `pkg_resources` together with
      their reported version string.
 
      This is primarily used for suggesting to enable certain SDK integrations from within the UI
      and for making informed decisions on which frameworks to support in future development
      efforts.
-
-    additionalProperties:
-      type:
-      - string
-      - 'null'
     """
 
     platform: Union[str, None]
     """
      Platform identifier of this event (defaults to "other").
 
      A string representing the platform the SDK is submitting from. This will be used by the
@@ -275,79 +331,59 @@
 
      Acceptable values are: `as3`, `c`, `cfml`, `cocoa`, `csharp`, `elixir`, `haskell`, `go`,
      `groovy`, `java`, `javascript`, `native`, `node`, `objc`, `other`, `perl`, `php`, `python`,
      `ruby`
     """
 
     received: Required["_Timestamp"]
-    """
-    Can be a ISO-8601 formatted string or a unix timestamp in seconds (floating point values allowed).
-
-    Must be UTC.
-
-    Aggregation type: anyOf
-
-    Required property
-    """
+    """ Required property """
 
     release: Union[str, None]
     """
      The release version of the application.
 
      **Release versions must be unique across all projects in your organization.** This value
      can be the git SHA for the given project, or a product identifier with a semantic version.
     """
 
-    request: "_SentryEventRequest"
-    """
-     Information about a web request that occurred during the event.
+    request: Union["SentryRequest", None]
+    """  Information about a web request that occurred during the event. """
 
-    Aggregation type: anyOf
-    """
-
-    sdk: "_SentryEventSdk"
-    """
-     Information about the Sentry SDK that generated this event.
-
-    Aggregation type: anyOf
-    """
+    sdk: Union["ClientSdkInfo", None]
+    """  Information about the Sentry SDK that generated this event. """
 
     server_name: Union[str, None]
     """
      Server or device name the event was generated on.
 
      This is supposed to be a hostname.
     """
 
-    stacktrace: "_SentryEventStacktrace"
+    stacktrace: Union["_RawStacktrace", None]
     """
      Event stacktrace.
 
      DEPRECATED: Prefer `threads` or `exception` depending on which is more appropriate.
-
-    Aggregation type: anyOf
     """
 
-    tags: "_SentryEventTags"
+    tags: Union["_Tags", None]
     """
      Custom tags for this event.
 
      A map or list of tags for this event. Each tag must be less than 200 characters.
-
-    Aggregation type: anyOf
     """
 
     time_spent: Union[int, None]
     """
      Time since the start of the transaction until the error occurred.
 
     minimum: 0
     """
 
-    timestamp: "_SentryEventTimestamp"
+    timestamp: Union["_Timestamp", None]
     """
      Timestamp when the event was created.
 
      Indicates when the event was created in the Sentry SDK. The format is either a string as
      defined in [RFC 3339](https://tools.ietf.org/html/rfc3339) or a numeric (integer or float)
      value representing the number of seconds that have elapsed since the [Unix
      epoch](https://en.wikipedia.org/wiki/Unix_time).
@@ -366,64 +402,44 @@
 
      ```json
      { "timestamp": "2011-05-02T17:41:36Z" }
      { "timestamp": "2011-05-02T17:41:36" }
      { "timestamp": "2011-05-02T17:41:36.000" }
      { "timestamp": 1304358096.0 }
      ```
-
-    Aggregation type: anyOf
     """
 
     transaction: Union[str, None]
     """
      Transaction name of the event.
 
      For example, in a web app, this might be the route name (`"/users/<username>/"` or
      `UserView`), in a task queue it might be the function + module name.
     """
 
-    transaction_info: "_SentryEventTransactionInfo"
-    """
-     Additional information about the name of the transaction.
+    transaction_info: Union["_TransactionInfo", None]
+    """  Additional information about the name of the transaction. """
 
-    Aggregation type: anyOf
-    """
-
-    user: "_SentryEventUser"
-    """
-     Information about the user who triggered this event.
-
-    Aggregation type: anyOf
-    """
+    user: Union["SentryUser", None]
+    """  Information about the user who triggered this event. """
 
     version: Union[str, None]
     """  Version """
 
     hierarchical_hashes: List[str]
 
 
 class SentryExceptionChain(TypedDict, total=False):
     """
     sentry_exception_chain.
 
      One or multiple chained (nested) exceptions.
     """
 
-    values: Union[None, List["_SentryExceptionChainValuesArrayItem"]]
-    """
-    items:
-      anyOf:
-      - $ref: '#/definitions/Exception'
-      - type: 'null'
-      used: !!set
-        $ref: null
-        anyOf: null
-    """
-
+    values: Union[None, List[Union["_Exception", None]]]
 
 
 SentryRequest = Union["_SentryRequestAnyof0"]
 """
 sentry_request.
 
  Http request information.
@@ -480,39 +496,27 @@
      },
      "env": {
        "REMOTE_ADDR": "192.168.0.1"
      }
    }
  }
  ```
-
-Aggregation type: anyOf
 """
 
 
 
 class SentryThreadChain(TypedDict, total=False):
     """
     sentry_thread_chain.
 
      One or multiple threads.
     """
 
-    values: Required[Union[None, List["_SentryThreadChainValuesArrayItem"]]]
-    """
-    items:
-      anyOf:
-      - $ref: '#/definitions/Thread'
-      - type: 'null'
-      used: !!set
-        $ref: null
-        anyOf: null
-
-    Required property
-    """
+    values: Required[Union[None, List[Union["_Thread", None]]]]
+    """ Required property """
 
 
 
 SentryUser = Union["_SentryUserAnyof0"]
 """
 sentry_user.
 
@@ -525,28 +529,57 @@
      "username": "my_user",
      "email": "foo@example.com",
      "ip_address": "127.0.0.1",
      "subscription": "basic"
    }
  }
  ```
-
-Aggregation type: anyOf
 """
 
 
 
+class StartMergeMessageBody(TypedDict, total=False):
+    """ start_merge_message_body. """
+
+    transaction_id: str
+    project_id: Required[int]
+    """ Required property """
+
+    previous_group_ids: Required[List[int]]
+    """ Required property """
+
+    new_group_id: Required[int]
+    """ Required property """
+
+    datetime: Required[str]
+    """ Required property """
+
+
+
+class TombstoneEventsMessageBody(TypedDict, total=False):
+    """ tombstone_events_message_body. """
+
+    project_id: Required[int]
+    """ Required property """
+
+    event_ids: Required[List[str]]
+    """ Required property """
+
+    old_primary_hash: Union[str, None]
+    from_timestamp: str
+    to_timestamp: str
+    datetime: str
+
+
 _AppContext = Union["_AppContextAnyof0"]
 """
  Application information.
 
  App context describes the application. As opposed to the runtime, this is the actual
  application that was running and carries metadata about the current session.
-
-Aggregation type: anyOf
 """
 
 
 
 class _AppContextAnyof0(TypedDict, total=False):
     app_build: Union[str, None]
     """  Internal build ID as it appears on the platform. """
@@ -582,19 +615,15 @@
 
     in_foreground: Union[bool, None]
     """  A flag indicating whether the app is in foreground or not. An app is in foreground when it's visible to the user. """
 
 
 
 _BrowserContext = Union["_BrowserContextAnyof0"]
-"""
- Web browser information.
-
-Aggregation type: anyOf
-"""
+"""  Web browser information. """
 
 
 
 class _BrowserContextAnyof0(TypedDict, total=False):
     name: Union[str, None]
     """  Display name of the browser application. """
 
@@ -607,19 +636,14 @@
     integrations: Union[List[Union[str, None]], None]
     """
      List of integrations that are enabled in the SDK. _Optional._
 
      The list should have all enabled integrations, including default integrations. Default
      integrations are included because different SDK releases may contain different default
      integrations.
-
-    items:
-      type:
-      - string
-      - 'null'
     """
 
     name: Required[Union[str, None]]
     """
      Unique SDK name. _Required._
 
      The name of the SDK. The format is `entity.ecosystem[.flavor]` where entity identifies the
@@ -662,16 +686,14 @@
      "cloud.platform": "aws_ec2",
      "cloud.region": "us-east-1",
      "cloud.vavailability_zone": "us-east-1e",
      "host.id": "i-07d3301208fe0a55a",
      "host.type": "t2.large"
  }
  ```
-
-Aggregation type: anyOf
 """
 
 
 
 _CloudResourceContextAnyof0 = TypedDict('_CloudResourceContextAnyof0', {
     #  The cloud account ID the resource is assigned to.
     'cloud.account.id': Union[str, None],
@@ -688,85 +710,56 @@
     'host.id': Union[str, None],
     #  Machine type of the host.
     'host.type': Union[str, None],
 }, total=False)
 
 
 _Context = Union["_DeviceContext", "_OsContext", "_RuntimeContext", "_AppContext", "_BrowserContext", "_GpuContext", "_TraceContext", "_ProfileContext", "_MonitorContext", "_ResponseContext", "_OtelContext", "_CloudResourceContext", Dict[str, Any]]
-"""
- A context describes environment info (e.g. device, os or browser).
+"""  A context describes environment info (e.g. device, os or browser). """
 
-Aggregation type: anyOf
-"""
 
 
-
-_Contexts = Union[Dict[str, "_ContextsAnyof0Additionalproperties"]]
+_Contexts = Union[Dict[str, Union["_Context", None]]]
 """
  The Contexts Interface provides additional context data. Typically, this is data related to the
  current user and the environment. For example, the device or application version. Its canonical
  name is `contexts`.
 
  The `contexts` type can be used to define arbitrary contextual data on the event. It accepts an
  object of key/value pairs. The key is the “alias” of the context and can be freely chosen.
  However, as per policy, it should match the type of the context unless there are two values for
  a type. You can omit `type` if the key name is the type.
 
  Unknown data for the contexts is rendered as a key/value list.
 
  For more details about sending additional data with your event, see the [full documentation on
  Additional Data](https://docs.sentry.io/enriching-error-data/additional-data/).
-
-Aggregation type: anyOf
 """
 
 
 
-_ContextsAnyof0Additionalproperties = Union["_Context", None]
-""" Aggregation type: anyOf """
+_Cookies = Union[Union[Dict[str, Union[str, None]], List["_CookiesAnyof0Anyof1Item"]]]
+"""  A map holding cookies. """
 
 
 
-_Cookies = Union[str, Union[int, float], Dict[str, Any], List[Any], bool, None]
+_CookiesAnyof0Anyof1Item = Union[Tuple[Union[str, None], Union[str, None]], None]
 """
- A map holding cookies.
-
-anyOf:
-  - anyOf:
-    - additionalProperties:
-        type:
-        - string
-        - 'null'
-      type: object
-    - items:
-        items:
-        - type:
-          - string
-          - 'null'
-        - type:
-          - string
-          - 'null'
-        maxItems: 2
-        minItems: 2
-        type:
-        - array
-        - 'null'
-      type: array
+maxItems: 2
+minItems: 2
 """
 
 
 
 _DeviceContext = Union["_DeviceContextAnyof0"]
 """
  Device information.
 
  Device context describes the device that caused the event. This is most appropriate for mobile
  applications.
-
-Aggregation type: anyOf
 """
 
 
 
 class _DeviceContextAnyof0(TypedDict, total=False):
     arch: Union[str, None]
     """  Native cpu architecture of the device. """
@@ -957,93 +950,40 @@
      How much memory is usable for the app in bytes.
 
     minimum: 0
     """
 
 
 
-_EVENT_PROCESSING_ERROR_ANYOF0_NAME_DEFAULT = None
-""" Default value of the field path 'event processing error anyof0 name' """
-
-
-
-_EVENT_PROCESSING_ERROR_ANYOF0_VALUE_DEFAULT = None
-""" Default value of the field path 'event processing error anyof0 value' """
-
-
-
 _EventId = Union[str]
-"""
- Wrapper around a UUID with slightly different formatting.
-
-Aggregation type: anyOf
-"""
+"""  Wrapper around a UUID with slightly different formatting. """
 
 
 
-_EventProcessingError = Union["_EventProcessingErrorAnyof0"]
-"""
- An event processing error.
-
-Aggregation type: anyOf
-"""
-
-
-
-class _EventProcessingErrorAnyof0(TypedDict, total=False):
-    name: Union[str, None]
-    """
-     Affected key or deep path.
-
-    default: None
-    """
-
-    type: Required[Union[str, None]]
-    """
-     The error kind.
-
-    Required property
-    """
-
-    value: Union[str, Union[int, float], Dict[str, Any], List[Any], bool, None]
-    """
-     The original value causing this error.
-
-    default: None
-    """
-
-
-
-_EventType = Union[Literal['error'], Literal['csp'], Literal['hpkp'], Literal['expectct'], Literal['expectstaple'], Literal['transaction'], Literal['nel'], Literal['default'], Literal['generic'], Literal['feedback']]
+_EventType = Union[Literal["error"], Literal["csp"], Literal["hpkp"], Literal["expectct"], Literal["expectstaple"], Literal["transaction"], Literal["default"]]
 """
 The type of an event.
 
 The event type determines how Sentry handles the event and has an impact on processing, rate limiting, and quotas. There are three fundamental classes of event types:
 
-- **Error monitoring events** (`default`, `error`): Processed and grouped into unique issues based on their exception stack traces and error messages. - **Security events** (`csp`, `hpkp`, `expectct`, `expectstaple`): Derived from Browser security violation reports and grouped into unique issues based on the endpoint and violation. SDKs do not send such events. - **Transaction events** (`transaction`): Contain operation spans and collected into traces for performance monitoring. - **Feedback events** (`feedback`): Contains user feedback messages.
+- **Error monitoring events** (`default`, `error`): Processed and grouped into unique issues based on their exception stack traces and error messages. - **Security events** (`csp`, `hpkp`, `expectct`, `expectstaple`): Derived from Browser security violation reports and grouped into unique issues based on the endpoint and violation. SDKs do not send such events. - **Transaction events** (`transaction`): Contain operation spans and collected into traces for performance monitoring.
 """
-_EVENTTYPE_ERROR: Literal['error'] = "error"
-"""The values for the 'The type of an event' enum"""
-_EVENTTYPE_CSP: Literal['csp'] = "csp"
-"""The values for the 'The type of an event' enum"""
-_EVENTTYPE_HPKP: Literal['hpkp'] = "hpkp"
+_EVENTTYPE_ERROR: Literal["error"] = "error"
 """The values for the 'The type of an event' enum"""
-_EVENTTYPE_EXPECTCT: Literal['expectct'] = "expectct"
+_EVENTTYPE_CSP: Literal["csp"] = "csp"
 """The values for the 'The type of an event' enum"""
-_EVENTTYPE_EXPECTSTAPLE: Literal['expectstaple'] = "expectstaple"
+_EVENTTYPE_HPKP: Literal["hpkp"] = "hpkp"
 """The values for the 'The type of an event' enum"""
-_EVENTTYPE_TRANSACTION: Literal['transaction'] = "transaction"
+_EVENTTYPE_EXPECTCT: Literal["expectct"] = "expectct"
 """The values for the 'The type of an event' enum"""
-_EVENTTYPE_NEL: Literal['nel'] = "nel"
+_EVENTTYPE_EXPECTSTAPLE: Literal["expectstaple"] = "expectstaple"
 """The values for the 'The type of an event' enum"""
-_EVENTTYPE_DEFAULT: Literal['default'] = "default"
+_EVENTTYPE_TRANSACTION: Literal["transaction"] = "transaction"
 """The values for the 'The type of an event' enum"""
-_EVENTTYPE_GENERIC: Literal['generic'] = "generic"
-"""The values for the 'The type of an event' enum"""
-_EVENTTYPE_FEEDBACK: Literal['feedback'] = "feedback"
+_EVENTTYPE_DEFAULT: Literal["default"] = "default"
 """The values for the 'The type of an event' enum"""
 
 
 
 _Exception = Union["_ExceptionAnyof0"]
 """
  A single exception.
@@ -1065,145 +1005,68 @@
      "values": [
        {"type": "Exception": "value": "random boring invariant was not met!"},
        {"type": "ValueError", "value": "something went wrong, help!"},
      ]
    }
  }
  ```
-
-Aggregation type: anyOf
 """
 
 
 
 class _ExceptionAnyof0(TypedDict, total=False):
-    mechanism: "_ExceptionAnyof0Mechanism"
-    """
-     Mechanism by which this exception was generated and handled.
-
-    Aggregation type: anyOf
-    """
+    mechanism: Union["_Mechanism", None]
+    """  Mechanism by which this exception was generated and handled. """
 
     module: Union[str, None]
     """  The optional module, or package which the exception type lives in. """
 
-    stacktrace: "_ExceptionAnyof0Stacktrace"
-    """
-     Stack trace containing frames of this exception.
-
-    Aggregation type: anyOf
-    """
+    stacktrace: Union["_RawStacktrace", None]
+    """  Stack trace containing frames of this exception. """
 
-    raw_stacktrace: "_ExceptionAnyof0RawStacktrace"
-    """
-     Stack trace containing frames of this exception.
+    raw_stacktrace: Union["_RawStacktrace", None]
+    """  Stack trace containing frames of this exception. """
 
-    Aggregation type: anyOf
-    """
-
-    thread_id: "_ExceptionAnyof0ThreadId"
-    """
-     An optional value that refers to a [thread](#typedef-Thread).
-
-    Aggregation type: anyOf
-    """
+    thread_id: Union["_ThreadId", None]
+    """  An optional value that refers to a [thread](#typedef-Thread). """
 
     type: Union[str, None]
     """
      Exception type, e.g. `ValueError`.
 
      At least one of `type` or `value` is required, otherwise the exception is discarded.
     """
 
-    value: "_ExceptionAnyof0Value"
+    value: Union["_JsonLenientString", None]
     """
      Human readable display value.
 
      At least one of `type` or `value` is required, otherwise the exception is discarded.
-
-    Aggregation type: anyOf
     """
 
 
 
-_ExceptionAnyof0Mechanism = Union["_Mechanism", None]
-"""
- Mechanism by which this exception was generated and handled.
-
-Aggregation type: anyOf
-"""
-
-
-
-_ExceptionAnyof0RawStacktrace = Union["_RawStacktrace", None]
-"""
- Stack trace containing frames of this exception.
-
-Aggregation type: anyOf
-"""
-
-
-
-_ExceptionAnyof0Stacktrace = Union["_RawStacktrace", None]
-"""
- Stack trace containing frames of this exception.
-
-Aggregation type: anyOf
-"""
-
-
-
-_ExceptionAnyof0ThreadId = Union["_ThreadId", None]
-"""
- An optional value that refers to a [thread](#typedef-Thread).
-
-Aggregation type: anyOf
-"""
-
-
-
-_ExceptionAnyof0Value = Union["_JsonLenientString", None]
-"""
- Human readable display value.
-
- At least one of `type` or `value` is required, otherwise the exception is discarded.
-
-Aggregation type: anyOf
-"""
-
-
-
 _Fingerprint = Union[List[str]]
-"""
- A fingerprint value.
-
-Aggregation type: anyOf
-"""
+"""  A fingerprint value. """
 
 
 
 _Frame = Union["_FrameAnyof0"]
 """
  Holds information about a single stacktrace frame.
 
  Each object should contain **at least** a `filename`, `function` or `instruction_addr`
  attribute. All values are optional, but recommended.
-
-Aggregation type: anyOf
 """
 
 
 
 class _FrameAnyof0(TypedDict, total=False):
-    abs_path: "_FrameAnyof0AbsPath"
-    """
-     Absolute path to the source file.
-
-    Aggregation type: anyOf
-    """
+    abs_path: Union[str, None]
+    """  Absolute path to the source file. """
 
     addr_mode: Union[str, None]
     """
      Defines the addressing mode for addresses.
 
      This can be:
      - `"abs"` (the default): `instruction_addr` is absolute.
@@ -1220,64 +1083,52 @@
 
     minimum: 0
     """
 
     context_line: Union[str, None]
     """  Source code of the current line (`lineno`). """
 
-    filename: "_FrameAnyof0Filename"
-    """
-     The source file name (basename only).
-
-    Aggregation type: anyOf
-    """
+    filename: Union[str, None]
+    """  The source file name (basename only). """
 
     function: Union[str, None]
     """
      Name of the frame's function. This might include the name of a class.
 
      This function name may be shortened or demangled. If not, Sentry will demangle and shorten
      it for some platforms. The original function name will be stored in `raw_function`.
     """
 
-    function_id: "_FrameAnyof0FunctionId"
+    function_id: Union[str, None]
     """
      (.NET) The function id / index that uniquely identifies a function inside a module.
 
      This is the `MetadataToken` of a .NET `MethodBase`.
-
-    Aggregation type: anyOf
     """
 
-    image_addr: "_FrameAnyof0ImageAddr"
-    """
-     (C/C++/Native) Start address of the containing code module (image).
-
-    Aggregation type: anyOf
-    """
+    image_addr: Union[str, None]
+    """  (C/C++/Native) Start address of the containing code module (image). """
 
     in_app: Union[bool, None]
     """
      Override whether this frame should be considered part of application code, or part of
      libraries/frameworks/dependencies.
 
      Setting this attribute to `false` causes the frame to be hidden/collapsed by default and
      mostly ignored during issue grouping.
     """
 
-    instruction_addr: "_FrameAnyof0InstructionAddr"
+    instruction_addr: Union[str, None]
     """
      (C/C++/Native) An optional instruction address for symbolication.
 
      This should be a string with a hexadecimal number that includes a 0x prefix.
      If this is set and a known image is defined in the
      [Debug Meta Interface]({%- link _documentation/development/sdk-dev/event-payloads/debugmeta.md -%}),
      then symbolication can take place.
-
-    Aggregation type: anyOf
     """
 
     lineno: Union[int, None]
     """
      Line number within the source file, starting at 1.
 
     minimum: 0
@@ -1304,32 +1155,18 @@
      Which platform this frame is from.
 
      This can override the platform for a single frame. Otherwise, the platform of the event is
      assumed. This can be used for multi-platform stack traces, such as in React Native.
     """
 
     post_context: Union[List[Union[str, None]], None]
-    """
-     Source code of the lines after `lineno`.
-
-    items:
-      type:
-      - string
-      - 'null'
-    """
+    """  Source code of the lines after `lineno`. """
 
     pre_context: Union[List[Union[str, None]], None]
-    """
-     Source code leading up to `lineno`.
-
-    items:
-      type:
-      - string
-      - 'null'
-    """
+    """  Source code leading up to `lineno`. """
 
     raw_function: Union[str, None]
     """
      A raw (but potentially truncated) function value.
 
      The original function name, if the function name is shortened or demangled. Sentry shows the
      raw function when clicking on the shortened one in the UI.
@@ -1363,121 +1200,34 @@
      Potentially mangled name of the symbol as it appears in an executable.
 
      This is different from a function name by generally being the mangled
      name that appears natively in the binary.  This is relevant for languages
      like Swift, C++ or Rust.
     """
 
-    symbol_addr: "_FrameAnyof0SymbolAddr"
+    symbol_addr: Union[str, None]
     """
      (C/C++/Native) Start address of the frame's function.
 
      We use the instruction address for symbolication, but this can be used to calculate
      an instruction offset automatically.
-
-    Aggregation type: anyOf
-    """
-
-    vars: "_FrameAnyof0Vars"
-    """
-     Mapping of local variables and expression names that were available in this frame.
-
-    Aggregation type: anyOf
     """
 
-
-
-_FrameAnyof0AbsPath = Union[str, None]
-"""
- Absolute path to the source file.
-
-Aggregation type: anyOf
-"""
-
-
-
-_FrameAnyof0Filename = Union[str, None]
-"""
- The source file name (basename only).
-
-Aggregation type: anyOf
-"""
-
-
-
-_FrameAnyof0FunctionId = Union[str, None]
-"""
- (.NET) The function id / index that uniquely identifies a function inside a module.
-
- This is the `MetadataToken` of a .NET `MethodBase`.
-
-Aggregation type: anyOf
-"""
-
-
-
-_FrameAnyof0ImageAddr = Union[str, None]
-"""
- (C/C++/Native) Start address of the containing code module (image).
-
-Aggregation type: anyOf
-"""
-
-
-
-_FrameAnyof0InstructionAddr = Union[str, None]
-"""
- (C/C++/Native) An optional instruction address for symbolication.
-
- This should be a string with a hexadecimal number that includes a 0x prefix.
- If this is set and a known image is defined in the
- [Debug Meta Interface]({%- link _documentation/development/sdk-dev/event-payloads/debugmeta.md -%}),
- then symbolication can take place.
-
-Aggregation type: anyOf
-"""
-
-
-
-_FrameAnyof0SymbolAddr = Union[str, None]
-"""
- (C/C++/Native) Start address of the frame's function.
-
- We use the instruction address for symbolication, but this can be used to calculate
- an instruction offset automatically.
-
-Aggregation type: anyOf
-"""
-
-
-
-_FrameAnyof0Vars = Union["_FrameVars", None]
-"""
- Mapping of local variables and expression names that were available in this frame.
-
-Aggregation type: anyOf
-"""
+    vars: Union["_FrameVars", None]
+    """  Mapping of local variables and expression names that were available in this frame. """
 
 
 
 _FrameVars = Union[Dict[str, Any]]
-"""
- Frame local variables.
-
-Aggregation type: anyOf
-"""
+"""  Frame local variables. """
 
 
 
 _Geo = Union["_GeoAnyof0"]
-"""
- Geographical location of the end user or device.
-
-Aggregation type: anyOf
-"""
+"""  Geographical location of the end user or device. """
 
 
 
 class _GeoAnyof0(TypedDict, total=False):
     city: Union[str, None]
     """  Human readable city name. """
 
@@ -1505,16 +1255,14 @@
    "memory_size": 4096,
    "api_type": "Metal",
    "multi_threaded_rendering": true,
    "version": "Metal",
    "npot_support": "Full"
  }
  ```
-
-Aggregation type: anyOf
 """
 
 
 
 class _GpuContextAnyof0(TypedDict, total=False):
     api_type: Union[str, None]
     """
@@ -1595,104 +1343,72 @@
     """ $comment: yes, we have seen both types in prod, not sure where they come from """
 
     is_new: bool
     is_new_group_environment: bool
     is_regression: bool
 
 
-_Headers = Union[str, Union[int, float], Dict[str, Any], List[Any], bool, None]
-"""
- A map holding headers.
+_HeaderName = Union[str]
+"""  A "into-string" type that normalizes header names. """
 
-anyOf:
-  - anyOf:
-    - additionalProperties:
-        anyOf:
-        - $ref: '#/definitions/HeaderValue'
-        - type: 'null'
-      type: object
-    - items:
-        items:
-        - anyOf:
-          - $ref: '#/definitions/HeaderName'
-          - type: 'null'
-        - anyOf:
-          - $ref: '#/definitions/HeaderValue'
-          - type: 'null'
-        maxItems: 2
-        minItems: 2
-        type:
-        - array
-        - 'null'
-      type: array
-"""
 
 
+_HeaderValue = Union[str]
+"""  A "into-string" type that normalizes header values. """
 
-class _InsertEventOccurrenceData(TypedDict, total=False):
-    detection_time: Required[Union[int, float]]
-    """ Required property """
 
-    fingerprint: Required[List[str]]
-    """ Required property """
 
-    issue_title: Required[str]
-    """ Required property """
+_Headers = Union[Union[Dict[str, Union["_HeaderValue", None]], List["_HeadersAnyof0Anyof1Item"]]]
+"""  A map holding headers. """
 
-    subtitle: Union[str, None]
-    culprit: Union[str, None]
-    level: Union[str, None]
-    resource_id: Union[str, None]
-    id: Required[str]
-    """ Required property """
 
-    type: Required[int]
-    """ Required property """
+
+_HeadersAnyof0Anyof1Item = Union[Tuple[Union["_HeaderName", None], Union["_HeaderValue", None]], None]
+"""
+maxItems: 2
+minItems: 2
+"""
 
 
 
-_InstructionAddrAdjustment = Union[Literal['auto'], Literal['all_but_first'], Literal['all'], Literal['none']]
+_InstructionAddrAdjustment = Union[Literal["auto"], Literal["all_but_first"], Literal["all"], Literal["none"]]
 """
 Controls the mechanism by which the `instruction_addr` of a [`Stacktrace`] [`Frame`] is adjusted.
 
 The adjustment tries to transform *return addresses* to *call addresses* for symbolication. Typically, this adjustment needs to be done for all frames but the first, as the first frame is usually taken directly from the cpu context of a hardware exception or a suspended thread and the stack trace is created from that.
 
 When the stack walking implementation truncates frames from the top, `"all"` frames should be adjusted. In case the stack walking implementation already does the adjustment when producing stack frames, `"none"` should be used here.
 """
-_INSTRUCTIONADDRADJUSTMENT_AUTO: Literal['auto'] = "auto"
+_INSTRUCTIONADDRADJUSTMENT_AUTO: Literal["auto"] = "auto"
 """The values for the 'Controls the mechanism by which the `instruction_addr` of a [`Stacktrace`] [`Frame`] is adjusted' enum"""
-_INSTRUCTIONADDRADJUSTMENT_ALL_BUT_FIRST: Literal['all_but_first'] = "all_but_first"
+_INSTRUCTIONADDRADJUSTMENT_ALL_BUT_FIRST: Literal["all_but_first"] = "all_but_first"
 """The values for the 'Controls the mechanism by which the `instruction_addr` of a [`Stacktrace`] [`Frame`] is adjusted' enum"""
-_INSTRUCTIONADDRADJUSTMENT_ALL: Literal['all'] = "all"
+_INSTRUCTIONADDRADJUSTMENT_ALL: Literal["all"] = "all"
 """The values for the 'Controls the mechanism by which the `instruction_addr` of a [`Stacktrace`] [`Frame`] is adjusted' enum"""
-_INSTRUCTIONADDRADJUSTMENT_NONE: Literal['none'] = "none"
+_INSTRUCTIONADDRADJUSTMENT_NONE: Literal["none"] = "none"
 """The values for the 'Controls the mechanism by which the `instruction_addr` of a [`Stacktrace`] [`Frame`] is adjusted' enum"""
 
 
 
 _JsonLenientString = Union[str]
-"""
- A "into-string" type of value. All non-string values are serialized as JSON.
-
-Aggregation type: anyOf
-"""
+"""  A "into-string" type of value. All non-string values are serialized as JSON. """
 
 
 
-_Level = Union[Literal['debug'], Literal['info'], Literal['warning'], Literal['error'], Literal['fatal']]
+_Level = Union[Literal["debug"], Literal["info"], Literal["warning"], Literal["error"], Literal["fatal"]]
 """ Severity level of an event or breadcrumb. """
-_LEVEL_DEBUG: Literal['debug'] = "debug"
+_LEVEL_DEBUG: Literal["debug"] = "debug"
 """The values for the 'Severity level of an event or breadcrumb' enum"""
-_LEVEL_INFO: Literal['info'] = "info"
+_LEVEL_INFO: Literal["info"] = "info"
 """The values for the 'Severity level of an event or breadcrumb' enum"""
-_LEVEL_WARNING: Literal['warning'] = "warning"
+_LEVEL_WARNING: Literal["warning"] = "warning"
 """The values for the 'Severity level of an event or breadcrumb' enum"""
-_LEVEL_ERROR: Literal['error'] = "error"
+_LEVEL_ERROR: Literal["error"] = "error"
 """The values for the 'Severity level of an event or breadcrumb' enum"""
-_LEVEL_FATAL: Literal['fatal'] = "fatal"
+_LEVEL_FATAL: Literal["fatal"] = "fatal"
 """The values for the 'Severity level of an event or breadcrumb' enum"""
 
 
 
 _LogEntry = Union["_LogEntryAnyof0"]
 """
  A log entry message.
@@ -1713,89 +1429,54 @@
  {
    "message": {
      "message": "My raw message with interpreted strings like {foo}",
      "params": {"foo": "this"}
    }
  }
  ```
-
-Aggregation type: anyOf
 """
 
 
 
 class _LogEntryAnyof0(TypedDict, total=False):
-    formatted: "_LogEntryAnyof0Formatted"
+    formatted: Union[Union[str], None]
     """
      The formatted message. If `message` and `params` are given, Sentry
      will attempt to backfill `formatted` if empty.
 
      It must not exceed 8192 characters. Longer messages will be truncated.
-
-    Aggregation type: anyOf
     """
 
-    message: "_LogEntryAnyof0Message"
+    message: Union[Union[str], None]
     """
      The log message with parameter placeholders.
 
      This attribute is primarily used for grouping related events together into issues.
      Therefore this really should just be a string template, i.e. `Sending %d requests` instead
      of `Sending 9999 requests`. The latter is much better at home in `formatted`.
 
      It must not exceed 8192 characters. Longer messages will be truncated.
-
-    Aggregation type: anyOf
     """
 
-    params: Union[Dict[str, Any], List[Any], None]
+    params: Union[Dict[str, Any], None, None]
     """
      Parameters to be interpolated into the log message. This can be an array of positional
      parameters as well as a mapping of named arguments to their values.
     """
 
 
 
-_LogEntryAnyof0Formatted = Union["_Message", None]
-"""
- The formatted message. If `message` and `params` are given, Sentry
- will attempt to backfill `formatted` if empty.
-
- It must not exceed 8192 characters. Longer messages will be truncated.
-
-Aggregation type: anyOf
-"""
-
-
-
-_LogEntryAnyof0Message = Union["_Message", None]
-"""
- The log message with parameter placeholders.
-
- This attribute is primarily used for grouping related events together into issues.
- Therefore this really should just be a string template, i.e. `Sending %d requests` instead
- of `Sending 9999 requests`. The latter is much better at home in `formatted`.
-
- It must not exceed 8192 characters. Longer messages will be truncated.
-
-Aggregation type: anyOf
-"""
-
-
-
 _Mechanism = Union["_MechanismAnyof0"]
 """
  The mechanism by which an exception was generated and handled.
 
  The exception mechanism is an optional field residing in the [exception](#typedef-Exception).
  It carries additional information about the way the exception was created on the target system.
  This includes general exception values obtained from the operating system or runtime APIs, as
  well as mechanism-specific values.
-
-Aggregation type: anyOf
 """
 
 
 
 class _MechanismAnyof0(TypedDict, total=False):
     handled: Union[bool, None]
     """
@@ -1823,36 +1504,25 @@
      exception, while for native it is e.g. `"minidump"` or `"applecrashreport"`.
 
     Required property
     """
 
 
 
-_Message = Union[str]
-""" Aggregation type: anyOf """
-
-
-
 _MonitorContext = Union[Dict[str, Any]]
-"""
- Monitor information.
-
-Aggregation type: anyOf
-"""
+"""  Monitor information. """
 
 
 
 _OsContext = Union["_OsContextAnyof0"]
 """
  Operating system information.
 
  OS context describes the operating system on which the event was created. In web contexts, this
  is the operating system of the browser (generally pulled from the User-Agent string).
-
-Aggregation type: anyOf
 """
 
 
 
 class _OsContextAnyof0(TypedDict, total=False):
     build: Union[str, None]
     """  Internal build number of the operating system. """
@@ -1885,71 +1555,50 @@
 
 
 _OtelContext = Union["_OtelContextAnyof0"]
 """
  OpenTelemetry Context
 
  If an event has this context, it was generated from an OpenTelemetry signal (trace, metric, log).
-
-Aggregation type: anyOf
 """
 
 
 
 class _OtelContextAnyof0(TypedDict, total=False):
     attributes: Union[Dict[str, Any], None]
     """
      Attributes of the OpenTelemetry span that maps to a Sentry event.
 
      <https://github.com/open-telemetry/opentelemetry-proto/blob/724e427879e3d2bae2edc0218fff06e37b9eb46e/opentelemetry/proto/trace/v1/trace.proto#L174-L186>
-
-    additionalProperties: True
     """
 
     resource: Union[Dict[str, Any], None]
     """
      Information about an OpenTelemetry resource.
 
      <https://github.com/open-telemetry/opentelemetry-proto/blob/724e427879e3d2bae2edc0218fff06e37b9eb46e/opentelemetry/proto/resource/v1/resource.proto>
-
-    additionalProperties: True
     """
 
 
 
 _ProfileContext = Union["_ProfileContextAnyof0"]
-"""
- Profile context
-
-Aggregation type: anyOf
-"""
+"""  Profile context """
 
 
 
 class _ProfileContextAnyof0(TypedDict, total=False):
-    profile_id: Required["_ProfileContextAnyof0ProfileId"]
+    profile_id: Required[Union["_EventId", None]]
     """
      The profile ID.
 
-    Aggregation type: anyOf
-
     Required property
     """
 
 
 
-_ProfileContextAnyof0ProfileId = Union["_EventId", None]
-"""
- The profile ID.
-
-Aggregation type: anyOf
-"""
-
-
-
 class _RawStacktrace(TypedDict, total=False):
     """
      A stack trace of a single thread.
 
      A stack trace contains a list of frames, each with various bits (most optional) describing the
      context of that frame. Frames should be sorted from oldest to newest.
 
@@ -2014,55 +1663,37 @@
          "rip": "0x00007ff6eef54be2",
          "rsp": "0x0000003b710cd9e0"
        }
      }
      ```
     """
 
-    frames: Required[Union[List["_RawStacktraceFramesArrayItem"], None]]
+    frames: Required[Union[List[Union["_Frame", None]], None]]
     """
      Required. A non-empty list of stack frames. The list is ordered from caller to callee, or
      oldest to youngest. The last frame is the one creating the exception.
 
-    items:
-      anyOf:
-      - $ref: '#/definitions/Frame'
-      - type: 'null'
-      used: !!set
-        $ref: null
-        anyOf: null
-
     Required property
     """
 
-    instruction_addr_adjustment: "_RawStacktraceInstructionAddrAdjustment"
+    instruction_addr_adjustment: Union["_InstructionAddrAdjustment", None]
     """
      Optional. A flag that indicates if, and how, `instruction_addr` values need to be adjusted
      before they are symbolicated.
-
-    Aggregation type: anyOf
     """
 
     lang: Union[str, None]
     """  The language of the stacktrace. """
 
-    registers: Union[Dict[str, "_RawStacktraceRegistersObjectAdditionalproperties"], None]
+    registers: Union[Dict[str, Union[str, None]], None]
     """
      Register values of the thread (top frame).
 
      A map of register names and their values. The values should contain the actual register
      values of the thread, thus mapping to the last frame in the list.
-
-    additionalProperties:
-      anyOf:
-      - $ref: '#/definitions/RegVal'
-      - type: 'null'
-      used: !!set
-        $ref: null
-        anyOf: null
     """
 
     snapshot: Union[bool, None]
     """
      Indicates that this stack trace is a snapshot triggered by an external signal.
 
      If this field is `false`, then the stack trace points to the code that caused this stack
@@ -2072,111 +1703,58 @@
      If this field is `true`, then the stack trace was captured as part of creating an unrelated
      event. For example, a thread other than the crashing thread, or a stack trace computed as a
      result of an external kill signal.
     """
 
 
 
-_RawStacktraceFramesArrayItem = Union["_Frame", None]
-""" Aggregation type: anyOf """
-
-
-
-_RawStacktraceInstructionAddrAdjustment = Union["_InstructionAddrAdjustment", None]
-"""
- Optional. A flag that indicates if, and how, `instruction_addr` values need to be adjusted
- before they are symbolicated.
-
-Aggregation type: anyOf
-"""
-
-
-
-_RawStacktraceRegistersObjectAdditionalproperties = Union[str, None]
-""" Aggregation type: anyOf """
-
-
-
 _ResponseContext = Union["_ResponseContextAnyof0"]
-"""
- Response interface that contains information on a HTTP response related to the event.
-
-Aggregation type: anyOf
-"""
+"""  Response interface that contains information on a HTTP response related to the event. """
 
 
 
 class _ResponseContextAnyof0(TypedDict, total=False):
     body_size: Union[int, None]
     """
      HTTP response body size.
 
     minimum: 0
     """
 
-    cookies: "_ResponseContextAnyof0Cookies"
+    cookies: Union["_Cookies", None]
     """
      The cookie values.
 
      Can be given unparsed as string, as dictionary, or as a list of tuples.
-
-    Aggregation type: anyOf
     """
 
-    headers: "_ResponseContextAnyof0Headers"
+    headers: Union["_Headers", None]
     """
      A dictionary of submitted headers.
 
      If a header appears multiple times it, needs to be merged according to the HTTP standard
      for header merging. Header names are treated case-insensitively by Sentry.
-
-    Aggregation type: anyOf
     """
 
     status_code: Union[int, None]
     """
      HTTP status code.
 
     minimum: 0
     """
 
 
 
-_ResponseContextAnyof0Cookies = Union["_Cookies", None]
-"""
- The cookie values.
-
- Can be given unparsed as string, as dictionary, or as a list of tuples.
-
-Aggregation type: anyOf
-"""
-
-
-
-_ResponseContextAnyof0Headers = Union["_Headers", None]
-"""
- A dictionary of submitted headers.
-
- If a header appears multiple times it, needs to be merged according to the HTTP standard
- for header merging. Header names are treated case-insensitively by Sentry.
-
-Aggregation type: anyOf
-"""
-
-
-
 _RuntimeContext = Union["_RuntimeContextAnyof0"]
 """
  Runtime information.
 
  Runtime context describes a runtime in more detail. Typically, this context is present in
  `contexts` multiple times if multiple runtimes are involved (for instance, if you have a
  JavaScript application running on top of JVM).
-
-Aggregation type: anyOf
 """
 
 
 
 class _RuntimeContextAnyof0(TypedDict, total=False):
     build: Union[str, None]
     """  Application build string, if it is separate from the version. """
@@ -2194,475 +1772,239 @@
     """
 
     version: Union[str, None]
     """  Runtime version string. """
 
 
 
-_SENTRY_EVENT_ERRORS_DEFAULT = None
-""" Default value of the field path 'sentry_event errors' """
-
-
-
-_SentryEventContexts = Union["_Contexts", None]
-"""
- Contexts describing the environment (e.g. device, os or browser).
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventErrorsArrayItem = Union["_EventProcessingError", None]
-""" Aggregation type: anyOf """
-
-
-
-_SentryEventEventId = Union["_EventId", None]
-"""
- Unique identifier of this event.
-
- Hexadecimal string representing a uuid4 value. The length is exactly 32 characters. Dashes
- are not allowed. Has to be lowercase.
-
- Even though this field is backfilled on the server with a new uuid4, it is strongly
- recommended to generate that uuid4 clientside. There are some features like user feedback
- which are easier to implement that way, and debugging in case events get lost in your
- Sentry installation is also easier.
-
- Example:
-
- ```json
- {
-   "event_id": "fc6d8c0c43fc4630ad850ee518f1b9d0"
- }
- ```
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventException = Union["SentryExceptionChain", None]
-""" Aggregation type: anyOf """
-
-
-
-_SentryEventFingerprint = Union["_Fingerprint", None]
-"""
- Manual fingerprint override.
-
- A list of strings used to dictate how this event is supposed to be grouped with other
- events into issues. For more information about overriding grouping see [Customize Grouping
- with Fingerprints](https://docs.sentry.io/data-management/event-grouping/).
-
- ```json
- {
-     "fingerprint": ["myrpc", "POST", "/foo.bar"]
- }
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventLevel = Union["_Level", None]
-"""
- Severity level of the event. Defaults to `error`.
-
- Example:
-
- ```json
- {"level": "warning"}
- ```
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventLogentry = Union["_LogEntry", None]
-"""
- Custom parameterized message for this event.
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventRequest = Union["SentryRequest", None]
-"""
- Information about a web request that occurred during the event.
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventSdk = Union["ClientSdkInfo", None]
-"""
- Information about the Sentry SDK that generated this event.
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventStacktrace = Union["_RawStacktrace", None]
-"""
- Event stacktrace.
-
- DEPRECATED: Prefer `threads` or `exception` depending on which is more appropriate.
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventTags = Union["_Tags", None]
-"""
- Custom tags for this event.
-
- A map or list of tags for this event. Each tag must be less than 200 characters.
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventThreads = Union["SentryThreadChain", None]
-""" Aggregation type: anyOf """
-
-
-
-_SentryEventTimestamp = Union["_Timestamp", None]
-"""
- Timestamp when the event was created.
-
- Indicates when the event was created in the Sentry SDK. The format is either a string as
- defined in [RFC 3339](https://tools.ietf.org/html/rfc3339) or a numeric (integer or float)
- value representing the number of seconds that have elapsed since the [Unix
- epoch](https://en.wikipedia.org/wiki/Unix_time).
-
- Timezone is assumed to be UTC if missing.
-
- Sub-microsecond precision is not preserved with numeric values due to precision
- limitations with floats (at least in our systems). With that caveat in mind, just send
- whatever is easiest to produce.
-
- All timestamps in the event protocol are formatted this way.
-
- # Example
-
- All of these are the same date:
-
- ```json
- { "timestamp": "2011-05-02T17:41:36Z" }
- { "timestamp": "2011-05-02T17:41:36" }
- { "timestamp": "2011-05-02T17:41:36.000" }
- { "timestamp": 1304358096.0 }
- ```
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventTransactionInfo = Union["_TransactionInfo", None]
-"""
- Additional information about the name of the transaction.
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryEventType = Union["_EventType", None]
-"""
- Type of the event. Defaults to `default`.
-
- The event type determines how Sentry handles the event and has an impact on processing, rate
- limiting, and quotas. There are three fundamental classes of event types:
-
-  - **Error monitoring events**: Processed and grouped into unique issues based on their
-    exception stack traces and error messages.
-  - **Security events**: Derived from Browser security violation reports and grouped into
-    unique issues based on the endpoint and violation. SDKs do not send such events.
-  - **Transaction events** (`transaction`): Contain operation spans and collected into traces
-    for performance monitoring.
-
- Transactions must explicitly specify the `"transaction"` event type. In all other cases,
- Sentry infers the appropriate event type from the payload and overrides the stated type.
- SDKs should not send an event type other than for transactions.
-
- Example:
-
- ```json
- {
-   "type": "transaction",
-   "spans": []
- }
- ```
-
-Aggregation type: anyOf
-"""
+class _SentryRequestAnyof0(TypedDict, total=False):
+    body_size: Union[int, None]
+    """
+     HTTP request body size.
 
+    minimum: 0
+    """
 
+    cookies: Union["_Cookies", None]
+    """
+     The cookie values.
 
-_SentryEventUser = Union["SentryUser", None]
-"""
- Information about the user who triggered this event.
+     Can be given unparsed as string, as dictionary, or as a list of tuples.
+    """
 
-Aggregation type: anyOf
-"""
+    data: Union[None, Dict[str, Any], str, int, None, bool]
+    """
+     Request data in any format that makes sense.
 
+     SDKs should discard large and binary bodies by default. Can be given as string or
+     structural data of any format.
+    """
 
+    env: Union[Dict[str, Any], None]
+    """
+     Server environment data, such as CGI/WSGI.
 
-_SentryExceptionChainValuesArrayItem = Union["_Exception", None]
-""" Aggregation type: anyOf """
+     A dictionary containing environment information passed from the server. This is where
+     information such as CGI/WSGI/Rack keys go that are not HTTP headers.
 
+     Sentry will explicitly look for `REMOTE_ADDR` to extract an IP address.
+    """
 
+    fragment: Union[str, None]
+    """  The fragment of the request URL. """
 
-class _SentryRequestAnyof0(TypedDict, total=False):
-    headers: "_SentryRequestAnyof0Headers"
+    headers: Union["_Headers", None]
     """
      A dictionary of submitted headers.
 
      If a header appears multiple times it, needs to be merged according to the HTTP standard
      for header merging. Header names are treated case-insensitively by Sentry.
-
-    Aggregation type: anyOf
     """
 
+    inferred_content_type: Union[str, None]
+    """  The inferred content type of the request payload. """
+
     method: Union[str, None]
     """  HTTP request method. """
 
+    query_string: Union[Union[str, Union[Dict[str, Union[str, None]], List["_SentryRequestAnyof0QueryStringAnyof0Anyof1Anyof1Item"]]], None]
+    """
+     The query string component of the URL.
+
+     Can be given as unparsed string, dictionary, or list of tuples.
+
+     If the query string is not declared and part of the `url`, Sentry moves it to the
+     query string.
+    """
+
     url: Union[str, None]
     """
      The URL of the request if available.
 
     The query string can be declared either as part of the `url`, or separately in `query_string`.
     """
 
 
 
-_SentryRequestAnyof0Headers = Union["_Headers", None]
+_SentryRequestAnyof0QueryStringAnyof0Anyof1Anyof1Item = Union[Tuple[Union[str, None], Union[str, None]], None]
 """
- A dictionary of submitted headers.
-
- If a header appears multiple times it, needs to be merged according to the HTTP standard
- for header merging. Header names are treated case-insensitively by Sentry.
-
-Aggregation type: anyOf
+maxItems: 2
+minItems: 2
 """
 
 
 
-_SentryThreadChainValuesArrayItem = Union["_Thread", None]
-""" Aggregation type: anyOf """
-
-
-
 class _SentryUserAnyof0(TypedDict, total=False):
     data: Union[Dict[str, Any], None]
     """
      Additional arbitrary fields, as stored in the database (and sometimes as sent by clients).
      All data from `self.other` should end up here after store normalization.
-
-    additionalProperties: True
     """
 
     email: Union[str, None]
     """  Email address of the user. """
 
-    geo: "_SentryUserAnyof0Geo"
-    """
-     Approximate geographical location of the end user or device.
-
-    Aggregation type: anyOf
-    """
+    geo: Union["_Geo", None]
+    """  Approximate geographical location of the end user or device. """
 
     id: Union[str, None]
     """  Unique identifier of the user. """
 
-    ip_address: "_SentryUserAnyof0IpAddress"
-    """
-     Remote IP address of the user. Defaults to "{{auto}}".
-
-    Aggregation type: anyOf
-    """
+    ip_address: Union[str, None]
+    """  Remote IP address of the user. Defaults to "{{auto}}". """
 
     name: Union[str, None]
     """  Human readable name of the user. """
 
     segment: Union[str, None]
     """  The user segment, for apps that divide users in user segments. """
 
     username: Union[str, None]
     """  Username of the user. """
 
 
 
-_SentryUserAnyof0Geo = Union["_Geo", None]
-"""
- Approximate geographical location of the end user or device.
-
-Aggregation type: anyOf
-"""
-
-
-
-_SentryUserAnyof0IpAddress = Union[str, None]
-"""
- Remote IP address of the user. Defaults to "{{auto}}".
-
-Aggregation type: anyOf
-"""
-
-
-
 _SpanId = Union[str]
-"""
- A 16-character hex string as described in the W3C trace context spec.
-
-Aggregation type: anyOf
-"""
+"""  A 16-character hex string as described in the W3C trace context spec. """
 
 
 
-_SpanStatus = Union[Literal['ok'], Literal['cancelled'], Literal['unknown'], Literal['invalid_argument'], Literal['deadline_exceeded'], Literal['not_found'], Literal['already_exists'], Literal['permission_denied'], Literal['resource_exhausted'], Literal['failed_precondition'], Literal['aborted'], Literal['out_of_range'], Literal['unimplemented'], Literal['internal_error'], Literal['unavailable'], Literal['data_loss'], Literal['unauthenticated']]
+_SpanStatus = Union[Literal["ok"], Literal["cancelled"], Literal["unknown"], Literal["invalid_argument"], Literal["deadline_exceeded"], Literal["not_found"], Literal["already_exists"], Literal["permission_denied"], Literal["resource_exhausted"], Literal["failed_precondition"], Literal["aborted"], Literal["out_of_range"], Literal["unimplemented"], Literal["internal_error"], Literal["unavailable"], Literal["data_loss"], Literal["unauthenticated"]]
 """
 Trace status.
 
 Values from <https://github.com/open-telemetry/opentelemetry-specification/blob/8fb6c14e4709e75a9aaa64b0dbbdf02a6067682a/specification/api-tracing.md#status> Mapping to HTTP from <https://github.com/open-telemetry/opentelemetry-specification/blob/8fb6c14e4709e75a9aaa64b0dbbdf02a6067682a/specification/data-http.md#status>
 """
-_SPANSTATUS_OK: Literal['ok'] = "ok"
+_SPANSTATUS_OK: Literal["ok"] = "ok"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_CANCELLED: Literal['cancelled'] = "cancelled"
+_SPANSTATUS_CANCELLED: Literal["cancelled"] = "cancelled"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_UNKNOWN: Literal['unknown'] = "unknown"
+_SPANSTATUS_UNKNOWN: Literal["unknown"] = "unknown"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_INVALID_ARGUMENT: Literal['invalid_argument'] = "invalid_argument"
+_SPANSTATUS_INVALID_ARGUMENT: Literal["invalid_argument"] = "invalid_argument"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_DEADLINE_EXCEEDED: Literal['deadline_exceeded'] = "deadline_exceeded"
+_SPANSTATUS_DEADLINE_EXCEEDED: Literal["deadline_exceeded"] = "deadline_exceeded"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_NOT_FOUND: Literal['not_found'] = "not_found"
+_SPANSTATUS_NOT_FOUND: Literal["not_found"] = "not_found"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_ALREADY_EXISTS: Literal['already_exists'] = "already_exists"
+_SPANSTATUS_ALREADY_EXISTS: Literal["already_exists"] = "already_exists"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_PERMISSION_DENIED: Literal['permission_denied'] = "permission_denied"
+_SPANSTATUS_PERMISSION_DENIED: Literal["permission_denied"] = "permission_denied"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_RESOURCE_EXHAUSTED: Literal['resource_exhausted'] = "resource_exhausted"
+_SPANSTATUS_RESOURCE_EXHAUSTED: Literal["resource_exhausted"] = "resource_exhausted"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_FAILED_PRECONDITION: Literal['failed_precondition'] = "failed_precondition"
+_SPANSTATUS_FAILED_PRECONDITION: Literal["failed_precondition"] = "failed_precondition"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_ABORTED: Literal['aborted'] = "aborted"
+_SPANSTATUS_ABORTED: Literal["aborted"] = "aborted"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_OUT_OF_RANGE: Literal['out_of_range'] = "out_of_range"
+_SPANSTATUS_OUT_OF_RANGE: Literal["out_of_range"] = "out_of_range"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_UNIMPLEMENTED: Literal['unimplemented'] = "unimplemented"
+_SPANSTATUS_UNIMPLEMENTED: Literal["unimplemented"] = "unimplemented"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_INTERNAL_ERROR: Literal['internal_error'] = "internal_error"
+_SPANSTATUS_INTERNAL_ERROR: Literal["internal_error"] = "internal_error"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_UNAVAILABLE: Literal['unavailable'] = "unavailable"
+_SPANSTATUS_UNAVAILABLE: Literal["unavailable"] = "unavailable"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_DATA_LOSS: Literal['data_loss'] = "data_loss"
+_SPANSTATUS_DATA_LOSS: Literal["data_loss"] = "data_loss"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_UNAUTHENTICATED: Literal['unauthenticated'] = "unauthenticated"
+_SPANSTATUS_UNAUTHENTICATED: Literal["unauthenticated"] = "unauthenticated"
 """The values for the 'Trace status' enum"""
 
 
 
-_TagEntry = Union["_TagEntryAnyof0", None]
-""" Aggregation type: anyOf """
+class _StartDeleteGroupsMessage2(TypedDict, total=False):
+    transaction_id: str
+    project_id: Required[int]
+    """ Required property """
+
+    group_ids: Required[List[int]]
+    """ Required property """
+
+    datetime: Required[str]
+    """ Required property """
 
 
 
 _TagEntryAnyof0 = Tuple[Union[str, None], Union[str, None]]
 """
 maxItems: 2
 minItems: 2
 """
 
 
 
-_Tags = List["_TagEntry"]
+_Tags = List[Union["_TagEntryAnyof0", None]]
 """  Manual key/value tag pairs. """
 
 
 
 _Thread = Union["_ThreadAnyof0"]
 """
  A single thread.
 
  The Threads Interface specifies threads that were running at the time an event happened.
  These threads can also contain stack traces.
-
-Aggregation type: anyOf
 """
 
 
 
 class _ThreadAnyof0(TypedDict, total=False):
-    id: "_ThreadAnyof0Id"
-    """
-     An optional value that refers to a [thread](#typedef-Thread).
-
-    Aggregation type: anyOf
-    """
+    id: Union["_ThreadId", None]
+    """  An optional value that refers to a [thread](#typedef-Thread). """
 
     main: Union[bool, None]
     """
      If applicable, a flag indicating whether the thread was responsible for rendering the user interface.
 
      On mobile platforms this is oftentimes referred to as the `main thread` or `ui thread`.
     """
 
 
 
-_ThreadAnyof0Id = Union["_ThreadId", None]
-"""
- An optional value that refers to a [thread](#typedef-Thread).
-
-Aggregation type: anyOf
-"""
-
-
-
 _ThreadId = Union["_ThreadIdAnyof0", str]
-"""
- Represents a thread id.
-
-Aggregation type: anyOf
-"""
+"""  Represents a thread id. """
 
 
 
 _ThreadIdAnyof0 = int
 """ minimum: 0 """
 
 
 
 _Timestamp = Union[Union[int, float]]
 """
 Can be a ISO-8601 formatted string or a unix timestamp in seconds (floating point values allowed).
 
 Must be UTC.
-
-Aggregation type: anyOf
 """
 
 
 
 _TraceContext = Union["_TraceContextAnyof0"]
-"""
- Trace context
-
-Aggregation type: anyOf
-"""
+"""  Trace context """
 
 
 
 class _TraceContextAnyof0(TypedDict, total=False):
     client_sample_rate: Union[Union[int, float], None]
     """
      The client-side sample rate as reported in the envelope's `trace.sample_rate` header.
@@ -2676,104 +2018,46 @@
      The amount of time in milliseconds spent in this transaction span,
      excluding its immediate child spans.
     """
 
     op: Union[str, None]
     """  Span type (see `OperationType` docs). """
 
-    parent_span_id: "_TraceContextAnyof0ParentSpanId"
-    """
-     The ID of the span enclosing this span.
+    parent_span_id: Union["_SpanId", None]
+    """  The ID of the span enclosing this span. """
 
-    Aggregation type: anyOf
-    """
-
-    span_id: Required["_TraceContextAnyof0SpanId"]
+    span_id: Required[Union["_SpanId", None]]
     """
      The ID of the span.
 
-    Aggregation type: anyOf
-
     Required property
     """
 
-    status: "_TraceContextAnyof0Status"
+    status: Union["_SpanStatus", None]
     """
      Whether the trace failed or succeeded. Currently only used to indicate status of individual
      transactions.
-
-    Aggregation type: anyOf
     """
 
-    trace_id: Required["_TraceContextAnyof0TraceId"]
+    trace_id: Required[Union["_TraceId", None]]
     """
      The trace ID.
 
-    Aggregation type: anyOf
-
     Required property
     """
 
-    sampled: Union[bool, None]
-    """  Whether the trace connected to the event has been sampled as part of dynamic sampling """
-
-
-
-_TraceContextAnyof0ParentSpanId = Union["_SpanId", None]
-"""
- The ID of the span enclosing this span.
-
-Aggregation type: anyOf
-"""
-
-
-
-_TraceContextAnyof0SpanId = Union["_SpanId", None]
-"""
- The ID of the span.
-
-Aggregation type: anyOf
-"""
-
-
-
-_TraceContextAnyof0Status = Union["_SpanStatus", None]
-"""
- Whether the trace failed or succeeded. Currently only used to indicate status of individual
- transactions.
-
-Aggregation type: anyOf
-"""
-
-
-
-_TraceContextAnyof0TraceId = Union["_TraceId", None]
-"""
- The trace ID.
-
-Aggregation type: anyOf
-"""
-
 
 
 _TraceId = Union[str]
-"""
- A 32-character hex string as described in the W3C trace context spec.
-
-Aggregation type: anyOf
-"""
+"""  A 32-character hex string as described in the W3C trace context spec. """
 
 
 
 _TransactionInfo = Union["_TransactionInfoAnyof0"]
-"""
- Additional information about the name of the transaction.
-
-Aggregation type: anyOf
-"""
+"""  Additional information about the name of the transaction. """
 
 
 
 class _TransactionInfoAnyof0(TypedDict, total=False):
     source: Union[str, None]
     """
      Describes how the name of the transaction was determined.
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 class SubscriptionResult(TypedDict, total=False):
     """ subscription_result. """
 
     version: Required[Literal[3]]
     """ Required property """
 
     payload: Required["PayloadV3"]
-    """
-    payload_v3.
-
-    Required property
-    """
+    """ Required property """
 
 
 
 class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
     """ Required property """
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_events_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,51 @@
-from typing import Any, Dict, TypedDict, Union, List
+from typing import TypedDict, Any, Union, Literal
 from typing_extensions import Required
 
 
-class _Root(TypedDict, total=False):
-    """ Error message from Relay """
+class ReplayRecording(TypedDict, total=False):
+    """
+    replay_recording.
+
+    A replay recording, or a chunk thereof
+    """
 
-    type: Required[str]
+    type: Required[Literal["replay_recording_not_chunked"]]
     """ Required property """
 
-    payload: Required[Union[str, Union[int, float], Dict[str, Any], List[Any], bool, None]]
+    replay_id: Required[str]
+    """ Required property """
+
+    key_id: Union[None, int]
+    org_id: Required[int]
     """
-    bytes
+    minimum: 0
 
     Required property
     """
 
-    event_id: Required[str]
-    """ Required property """
-
     project_id: Required[int]
-    """ Required property """
+    """
+    minimum: 0
+
+    Required property
+    """
 
-    start_time: Required[int]
+    received: Required[int]
+    """
+    minimum: 0
+
+    Required property
+    """
+
+    retention_days: Required[int]
     """ Required property """
 
+    payload: Required[Any]
+    """
+    msgpack bytes
+
+    WARNING: we get an schema without any type
+
+    Required property
+    """
+
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/ingest_feedback_events_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,55 @@
-from typing import Dict, TypedDict, Union, Any, List
+from typing import Literal, Dict, Any, TypedDict, List
 from typing_extensions import Required
 
 
-class FeedbackEvent(TypedDict, total=False):
+class PayloadV3(TypedDict, total=False):
+    """ payload_v3. """
+
+    subscription_id: Required[str]
     """
-    feedback_event.
+    minLength: 1
 
-    User feedback event from Relay
+    Required property
     """
 
-    type: Required[str]
+    request: Required[Dict[str, Any]]
+    """ Required property """
+
+    result: Required["_PayloadV3Result"]
     """ Required property """
 
-    payload: Required[Union[str, Union[int, float], Dict[str, Any], List[Any], bool, None]]
+    timestamp: Required[str]
+    """ Required property """
+
+    entity: Required[str]
     """
-    bytes. JSON string of the wrapped feedback event
+    minLength: 1
 
     Required property
     """
 
-    event_id: Required[str]
+
+
+class SubscriptionResult(TypedDict, total=False):
+    """ subscription_result. """
+
+    version: Required[Literal[3]]
     """ Required property """
 
-    project_id: Required[int]
+    payload: Required["PayloadV3"]
     """ Required property """
 
-    start_time: Required[int]
+
+
+class _PayloadV3Result(TypedDict, total=False):
+    data: Required[List[Dict[str, Any]]]
     """ Required property """
 
+    meta: Required[List["_PayloadV3ResultMetaItem"]]
+    """ Required property """
+
+
+
+class _PayloadV3ResultMetaItem(TypedDict, total=False):
+    name: str
+    type: str
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Any, Literal, TypedDict, List
+from typing import TypedDict, Dict, Literal, Any, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """ payload_v3. """
 
     subscription_id: Required[str]
@@ -33,19 +33,15 @@
 class SubscriptionResult(TypedDict, total=False):
     """ subscription_result. """
 
     version: Required[Literal[3]]
     """ Required property """
 
     payload: Required["PayloadV3"]
-    """
-    payload_v3.
-
-    Required property
-    """
+    """ Required property """
 
 
 
 class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
     """ Required property """
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/monitors_clock_tasks_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,76 @@
-from typing import Literal, Union, TypedDict
+from typing import Literal, Any, TypedDict, List, Union, Dict
 from typing_extensions import Required
 
 
-class MarkMissing(TypedDict, total=False):
-    """
-    mark_missing.
+CounterMetricValue = Union[int, float]
+""" counter_metric_value. """
 
-    Indicates a monitor ID that should be marked as missed.
-    """
 
-    type: Required[Literal['mark_missing']]
-    """
-    Discriminant marker identifying the task.
 
-    Required property
-    """
+DistributionMetricValue = List[Union[int, float]]
+""" distribution_metric_value. """
 
-    ts: Required[Union[int, float]]
-    """
-    The timestamp the clock ticked at.
 
-    Required property
-    """
 
-    monitor_environment_id: Required[Union[int, float]]
-    """
-    The monitor environment ID to generate a missed check-in for.
+class Metric(TypedDict, total=False):
+    """ metric. """
 
-    Required property
-    """
+    version: Literal[1]
+    use_case_id: Required[str]
+    """ Required property """
 
+    org_id: Required[int]
+    """ Required property """
 
+    project_id: Required[int]
+    """ Required property """
 
-class MarkTimeout(TypedDict, total=False):
-    """
-    mark_timeout.
+    metric_id: Required[int]
+    """ Required property """
 
-    Indicates a check-in should be marked as having timed out.
-    """
+    type: Required[str]
+    """ Required property """
 
-    type: Required[Literal['mark_timeout']]
+    timestamp: Required[int]
     """
-    Discriminant marker identifying the task.
+    minimum: 0
 
     Required property
     """
 
-    ts: Required[Union[int, float]]
-    """
-    The timestamp the clock ticked at.
+    sentry_received_timestamp: Union[int, float]
+    tags: Required["_IntToInt"]
+    """ Required property """
 
-    Required property
-    """
+    value: Required[Union["CounterMetricValue", "SetMetricValue", "DistributionMetricValue"]]
+    """ Required property """
 
-    monitor_environment_id: Required[Union[int, float]]
-    """
-    The monitor environment ID the check-in is part of.
+    retention_days: Required[int]
+    """ Required property """
 
-    Required property
-    """
+    mapping_meta: Required["_MappingMeta"]
+    """ Required property """
 
-    checkin_id: Required[Union[int, float]]
-    """
-    The check-in ID to mark as timed out.
 
-    Required property
-    """
+
+SetMetricValue = List[int]
+""" set_metric_value. """
 
 
 
-MonitorsClockTasks = Union["MarkTimeout", "MarkMissing"]
+_IntToInt = Dict[str, Any]
+"""
+patternProperties:
+  ^[0-9]$:
+    type: integer
 """
-monitors_clock_tasks.
 
-Aggregation type: oneOf
+
+
+_MappingMeta = Dict[str, Any]
+"""
+patternProperties:
+  ^[chdfr]$:
+    $ref: '#/definitions/IntToString'
 """
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/profiles_call_tree_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,67 @@
-from typing import List, TypedDict
+from typing import List, TypedDict, Dict, Literal, Union, Any
 from typing_extensions import Required
 
 
-class _FunctionItem(TypedDict, total=False):
-    fingerprint: Required["_Uint"]
-    """
-    minimum: 0
+CounterMetricValue = Union[int, float]
+""" counter_metric_value. """
 
-    Required property
-    """
 
-    function: Required[str]
-    """ Required property """
 
-    in_app: Required[bool]
-    """ Required property """
+DistributionMetricValue = List[Union[int, float]]
+""" distribution_metric_value. """
 
-    package: Required[str]
-    """ Required property """
 
-    self_times_ns: Required[List["_Uint"]]
-    """ Required property """
 
+class GenericMetric(TypedDict, total=False):
+    """ generic_metric. """
+
+    version: Literal[2]
+    use_case_id: Required[str]
+    """ Required property """
 
+    org_id: Required[int]
+    """ Required property """
 
-class _Root(TypedDict, total=False):
-    functions: Required[List["_FunctionItem"]]
+    project_id: Required[int]
     """ Required property """
 
-    environment: str
-    profile_id: Required[str]
+    metric_id: Required[int]
     """ Required property """
 
-    platform: Required[str]
+    type: Required[str]
     """ Required property """
 
-    project_id: Required["_Uint"]
+    timestamp: Required[int]
     """
     minimum: 0
 
     Required property
     """
 
-    received: Required["_Uint"]
-    """
-    minimum: 0
+    sentry_received_timestamp: Union[int, float]
+    tags: Required[Dict[str, str]]
+    """ Required property """
 
-    Required property
-    """
+    value: Required[Union["CounterMetricValue", "SetMetricValue", "DistributionMetricValue"]]
+    """ Required property """
 
-    release: str
-    retention_days: Required["_Uint"]
-    """
-    minimum: 0
+    retention_days: Required[int]
+    """ Required property """
 
-    Required property
-    """
+    mapping_meta: Required["_MappingMeta"]
+    """ Required property """
 
-    timestamp: Required["_Uint"]
-    """
-    minimum: 0
 
-    Required property
-    """
 
-    transaction_name: Required[str]
-    """ Required property """
+SetMetricValue = List[int]
+""" set_metric_value. """
 
 
 
-_Uint = int
-""" minimum: 0 """
+_MappingMeta = Dict[str, Any]
+"""
+patternProperties:
+  ^[chdfr]$:
+    $ref: '#/definitions/IntToString'
+"""
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_events_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,139 @@
-from typing import TypedDict, Any, Dict, List
+from typing import List, TypedDict, Union, Any, Dict
 from typing_extensions import Required
 
 
-class _Root(TypedDict, total=False):
-    version: Required[int]
+class ClickhouseQueryProfile(TypedDict, total=False):
+    """ clickhouse_query_profile. """
+
+    time_range: Required[Union[int, None]]
+    """ Required property """
+
+    table: str
+    all_columns: List[str]
+    multi_level_condition: Required[bool]
+    """ Required property """
+
+    where_profile: Required["ClickhouseQueryProfileWhereProfile"]
+    """ Required property """
+
+    groupby_cols: Required[List[str]]
+    """ Required property """
+
+    array_join_cols: Required[List[str]]
+    """ Required property """
+
+
+
+class ClickhouseQueryProfileWhereProfile(TypedDict, total=False):
+    """ clickhouse_query_profile_where_profile. """
+
+    columns: Required[List[str]]
     """ Required property """
 
-    payload: Required["_RootPayload"]
+    mapping_cols: Required[List[str]]
     """ Required property """
 
 
 
-class _RootPayload(TypedDict, total=False):
-    subscription_id: Required[str]
+class QueryMetadata(TypedDict, total=False):
+    """ query_metadata. """
+
+    sql: Required[str]
+    """ Required property """
+
+    sql_anonymized: Required[str]
+    """ Required property """
+
+    start_timestamp: Required[Union[int, None]]
+    """ Required property """
+
+    end_timestamp: Required[Union[int, None]]
+    """ Required property """
+
+    stats: Required[Dict[str, Any]]
+    """ Required property """
+
+    status: Required[str]
+    """ Required property """
+
+    trace_id: Required[Union[str, None]]
     """ Required property """
 
-    request: Required[Dict[str, Any]]
+    profile: Required["ClickhouseQueryProfile"]
     """ Required property """
 
-    result: Required["_RootPayloadResult"]
+    result_profile: Required[Union[Dict[str, Any], None]]
     """ Required property """
 
-    timestamp: Required[str]
+    request_status: Required[str]
+    """ Required property """
+
+    slo: Required[str]
+    """ Required property """
+
+
+
+class Querylog(TypedDict, total=False):
+    """
+    querylog.
+
+    Querylog schema
+    """
+
+    request: Required["_QuerylogRequest"]
+    """ Required property """
+
+    dataset: Required[str]
     """ Required property """
 
     entity: Required[str]
     """ Required property """
 
+    start_timestamp: Required[Union[int, None]]
+    """ Required property """
+
+    end_timestamp: Required[Union[int, None]]
+    """ Required property """
+
+    status: Required[str]
+    """ Required property """
+
+    request_status: Required[str]
+    """ Required property """
 
+    slo: Required[str]
+    """ Required property """
+
+    projects: Required[List[int]]
+    """ Required property """
 
-class _RootPayloadResult(TypedDict, total=False):
-    data: Required[List[Dict[str, Any]]]
+    query_list: Required[List["QueryMetadata"]]
     """ Required property """
 
-    meta: Required[List[Any]]
+    timing: Required["_QuerylogTiming"]
     """ Required property """
 
+    snql_anonymized: str
+    organization: Union[int, None]
+
+
+class _QuerylogRequest(TypedDict, total=False):
+    id: Required[str]
+    """
+    pattern: [0-9a-fA-F]{32}
+
+    Required property
+    """
+
+    body: Dict[str, Any]
+    referrer: str
+    app_id: str
+    team: Union[str, None]
+    feature: Union[str, None]
+
+
+class _QuerylogTiming(TypedDict, total=False):
+    timestamp: int
+    duration_ms: int
+    marks_ms: Dict[str, int]
+    tags: Dict[str, str]
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/scheduled_subscriptions_generic_metrics_distributions_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,55 @@
-from typing import Any, TypedDict, List, Dict
+from typing import TypedDict, List, Dict, Any, Literal
 from typing_extensions import Required
 
 
-class _Root(TypedDict, total=False):
-    version: Required[int]
-    """ Required property """
-
-    payload: Required["_RootPayload"]
-    """ Required property """
-
+class PayloadV3(TypedDict, total=False):
+    """ payload_v3. """
 
-
-class _RootPayload(TypedDict, total=False):
     subscription_id: Required[str]
-    """ Required property """
+    """
+    minLength: 1
+
+    Required property
+    """
 
     request: Required[Dict[str, Any]]
     """ Required property """
 
-    result: Required["_RootPayloadResult"]
+    result: Required["_PayloadV3Result"]
     """ Required property """
 
     timestamp: Required[str]
     """ Required property """
 
     entity: Required[str]
+    """
+    minLength: 1
+
+    Required property
+    """
+
+
+
+class SubscriptionResult(TypedDict, total=False):
+    """ subscription_result. """
+
+    version: Required[Literal[3]]
+    """ Required property """
+
+    payload: Required["PayloadV3"]
     """ Required property """
 
 
 
-class _RootPayloadResult(TypedDict, total=False):
+class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
     """ Required property """
 
-    meta: Required[List[Any]]
+    meta: Required[List["_PayloadV3ResultMetaItem"]]
     """ Required property """
 
+
+
+class _PayloadV3ResultMetaItem(TypedDict, total=False):
+    name: str
+    type: str
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schema_types/transactions_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/transactions_v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from typing import Tuple, Union, Dict, List, TypedDict, Any, Literal
+from typing import Literal, Union, List, TypedDict, Dict, Any, Tuple
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
  The SDK Interface describes the Sentry SDK and its configuration used to capture and transmit an event.
-
-Aggregation type: anyOf
 """
 
 
 
 class TransactionEvent(TypedDict, total=False):
     """ transaction_event. """
 
@@ -43,16 +41,14 @@
 
 _AppContext = Union["_AppContextAnyof0"]
 """
  Application information.
 
  App context describes the application. As opposed to the runtime, this is the actual
  application that was running and carries metadata about the current session.
-
-Aggregation type: anyOf
 """
 
 
 
 class _AppContextAnyof0(TypedDict, total=False):
     app_build: Union[str, None]
     """  Internal build ID as it appears on the platform. """
@@ -94,19 +90,15 @@
 class _Breakdowns(TypedDict, total=False):
     span_ops: Required[Dict[str, "_NumOfSpans"]]
     """ Required property """
 
 
 
 _BrowserContext = Union["_BrowserContextAnyof0"]
-"""
- Web browser information.
-
-Aggregation type: anyOf
-"""
+"""  Web browser information. """
 
 
 
 class _BrowserContextAnyof0(TypedDict, total=False):
     name: Union[str, None]
     """  Display name of the browser application. """
 
@@ -119,19 +111,14 @@
     integrations: Union[List[Union[str, None]], None]
     """
      List of integrations that are enabled in the SDK. _Optional._
 
      The list should have all enabled integrations, including default integrations. Default
      integrations are included because different SDK releases may contain different default
      integrations.
-
-    items:
-      type:
-      - string
-      - 'null'
     """
 
     name: Required[Union[str, None]]
     """
      Unique SDK name. _Required._
 
      The name of the SDK. The format is `entity.ecosystem[.flavor]` where entity identifies the
@@ -174,16 +161,14 @@
      "cloud.platform": "aws_ec2",
      "cloud.region": "us-east-1",
      "cloud.vavailability_zone": "us-east-1e",
      "host.id": "i-07d3301208fe0a55a",
      "host.type": "t2.large"
  }
  ```
-
-Aggregation type: anyOf
 """
 
 
 
 _CloudResourceContextAnyof0 = TypedDict('_CloudResourceContextAnyof0', {
     #  The cloud account ID the resource is assigned to.
     'cloud.account.id': Union[str, None],
@@ -200,73 +185,46 @@
     'host.id': Union[str, None],
     #  Machine type of the host.
     'host.type': Union[str, None],
 }, total=False)
 
 
 _Context = Union["_DeviceContext", "_OsContext", "_RuntimeContext", "_AppContext", "_BrowserContext", "_GpuContext", "_TraceContext", "_ProfileContext", "_MonitorContext", "_ResponseContext", "_OtelContext", "_CloudResourceContext", Dict[str, Any]]
-"""
- A context describes environment info (e.g. device, os or browser).
-
-Aggregation type: anyOf
-"""
+"""  A context describes environment info (e.g. device, os or browser). """
 
 
 
-_Contexts = Union[Dict[str, "_ContextsAnyof0Additionalproperties"]]
+_Contexts = Union[Dict[str, Union["_Context", None]]]
 """
  The Contexts Interface provides additional context data. Typically, this is data related to the
  current user and the environment. For example, the device or application version. Its canonical
  name is `contexts`.
 
  The `contexts` type can be used to define arbitrary contextual data on the event. It accepts an
  object of key/value pairs. The key is the “alias” of the context and can be freely chosen.
  However, as per policy, it should match the type of the context unless there are two values for
  a type. You can omit `type` if the key name is the type.
 
  Unknown data for the contexts is rendered as a key/value list.
 
  For more details about sending additional data with your event, see the [full documentation on
  Additional Data](https://docs.sentry.io/enriching-error-data/additional-data/).
-
-Aggregation type: anyOf
 """
 
 
 
-_ContextsAnyof0Additionalproperties = Union["_Context", None]
-""" Aggregation type: anyOf """
+_Cookies = Union[Union[Dict[str, Union[str, None]], List["_CookiesAnyof0Anyof1Item"]]]
+"""  A map holding cookies. """
 
 
 
-_Cookies = Union[str, Union[int, float], Dict[str, Any], List[Any], bool, None]
+_CookiesAnyof0Anyof1Item = Union[Tuple[Union[str, None], Union[str, None]], None]
 """
- A map holding cookies.
-
-anyOf:
-  - anyOf:
-    - additionalProperties:
-        type:
-        - string
-        - 'null'
-      type: object
-    - items:
-        items:
-        - type:
-          - string
-          - 'null'
-        - type:
-          - string
-          - 'null'
-        maxItems: 2
-        minItems: 2
-        type:
-        - array
-        - 'null'
-      type: array
+maxItems: 2
+minItems: 2
 """
 
 
 
 class _Data(TypedDict, total=False):
     type: Required[str]
     """ Required property """
@@ -276,29 +234,21 @@
      Transaction name of the event.
 
      For example, in a web app, this might be the route name (`"/users/<username>/"` or
      `UserView`), in a task queue it might be the function + module name.
     """
 
     transaction_info: "_TransactionInfo"
-    """
-     Additional information about the name of the transaction.
-
-    Aggregation type: anyOf
-    """
-
     timestamp: Required[Union[int, float]]
     """ Required property """
 
     start_timestamp: Required[Union[int, float]]
     """ Required property """
 
-    received: Required[Union[int, float]]
-    """ Required property """
-
+    received: Union[int, float]
     release: Union[str, None]
     """
      The release version of the application.
 
      **Release versions must be unique across all projects in your organization.** This value
      can be the git SHA for the given project, or a product identifier with a semantic version.
     """
@@ -309,97 +259,42 @@
 
      ```json
      { "environment": "production" }
      ```
     """
 
     contexts: Required["_Contexts"]
-    """
-     The Contexts Interface provides additional context data. Typically, this is data related to the
-     current user and the environment. For example, the device or application version. Its canonical
-     name is `contexts`.
-
-     The `contexts` type can be used to define arbitrary contextual data on the event. It accepts an
-     object of key/value pairs. The key is the “alias” of the context and can be freely chosen.
-     However, as per policy, it should match the type of the context unless there are two values for
-     a type. You can omit `type` if the key name is the type.
-
-     Unknown data for the contexts is rendered as a key/value list.
-
-     For more details about sending additional data with your event, see the [full documentation on
-     Additional Data](https://docs.sentry.io/enriching-error-data/additional-data/).
-
-    Aggregation type: anyOf
-
-    Required property
-    """
+    """ Required property """
 
-    tags: "_DataTags"
+    tags: Union["_Tags", None]
     """
      Custom tags for this event.
 
      A map or list of tags for this event. Each tag must be less than 200 characters.
-
-    Aggregation type: anyOf
     """
 
     extra: "_Extra"
-    """
-     Arbitrary extra information set by the user.
-
-     ```json
-     {
-         "extra": {
-             "my_key": 1,
-             "some_other_value": "foo bar"
-         }
-     }```
-
-    additionalProperties: True
-    """
-
     sdk: "ClientSdkInfo"
-    """
-    client_sdk_info.
-
-     The SDK Interface describes the Sentry SDK and its configuration used to capture and transmit an event.
-
-    Aggregation type: anyOf
-    """
-
     project: int
     spans: Required[List["_Span"]]
     """ Required property """
 
     measurements: "_Measurements"
     breakdowns: "_Breakdowns"
     culprit: str
     title: str
     location: str
 
 
-_DataTags = Union["_Tags", None]
-"""
- Custom tags for this event.
-
- A map or list of tags for this event. Each tag must be less than 200 characters.
-
-Aggregation type: anyOf
-"""
-
-
-
 _DeviceContext = Union["_DeviceContextAnyof0"]
 """
  Device information.
 
  Device context describes the device that caused the event. This is most appropriate for mobile
  applications.
-
-Aggregation type: anyOf
 """
 
 
 
 class _DeviceContextAnyof0(TypedDict, total=False):
     arch: Union[str, None]
     """  Native cpu architecture of the device. """
@@ -591,35 +486,29 @@
 
     minimum: 0
     """
 
 
 
 _EventId = Union[str]
-"""
- Wrapper around a UUID with slightly different formatting.
-
-Aggregation type: anyOf
-"""
+"""  Wrapper around a UUID with slightly different formatting. """
 
 
 
 _Extra = Union[Dict[str, Any], None]
 """
  Arbitrary extra information set by the user.
 
  ```json
  {
      "extra": {
          "my_key": 1,
          "some_other_value": "foo bar"
      }
  }```
-
-additionalProperties: True
 """
 
 
 
 _GpuContext = Union["_GpuContextAnyof0"]
 """
  GPU information.
@@ -633,16 +522,14 @@
    "memory_size": 4096,
    "api_type": "Metal",
    "multi_threaded_rendering": true,
    "version": "Metal",
    "npot_support": "Full"
  }
  ```
-
-Aggregation type: anyOf
 """
 
 
 
 class _GpuContextAnyof0(TypedDict, total=False):
     api_type: Union[str, None]
     """
@@ -705,53 +592,43 @@
     """  The vendor name as reported by the graphics device. """
 
     version: Union[str, None]
     """  The Version of the graphics device. """
 
 
 
-_Headers = Union[str, Union[int, float], Dict[str, Any], List[Any], bool, None]
-"""
- A map holding headers.
+_HeaderName = Union[str]
+"""  A "into-string" type that normalizes header names. """
+
 
-anyOf:
-  - anyOf:
-    - additionalProperties:
-        anyOf:
-        - $ref: '#/definitions/HeaderValue'
-        - type: 'null'
-      type: object
-    - items:
-        items:
-        - anyOf:
-          - $ref: '#/definitions/HeaderName'
-          - type: 'null'
-        - anyOf:
-          - $ref: '#/definitions/HeaderValue'
-          - type: 'null'
-        maxItems: 2
-        minItems: 2
-        type:
-        - array
-        - 'null'
-      type: array
+
+_HeaderValue = Union[str]
+"""  A "into-string" type that normalizes header values. """
+
+
+
+_Headers = Union[Union[Dict[str, Union["_HeaderValue", None]], List["_HeadersAnyof0Anyof1Item"]]]
+"""  A map holding headers. """
+
+
+
+_HeadersAnyof0Anyof1Item = Union[Tuple[Union["_HeaderName", None], Union["_HeaderValue", None]], None]
+"""
+maxItems: 2
+minItems: 2
 """
 
 
 
 class _Measurements(TypedDict, total=False):
     num_of_spans: "_NumOfSpans"
 
 
 _MonitorContext = Union[Dict[str, Any]]
-"""
- Monitor information.
-
-Aggregation type: anyOf
-"""
+"""  Monitor information. """
 
 
 
 class _NumOfSpans(TypedDict, total=False):
     value: Required[Union[int, float]]
     """ Required property """
 
@@ -760,16 +637,14 @@
 
 _OsContext = Union["_OsContextAnyof0"]
 """
  Operating system information.
 
  OS context describes the operating system on which the event was created. In web contexts, this
  is the operating system of the browser (generally pulled from the User-Agent string).
-
-Aggregation type: anyOf
 """
 
 
 
 class _OsContextAnyof0(TypedDict, total=False):
     build: Union[str, None]
     """  Internal build number of the operating system. """
@@ -802,148 +677,94 @@
 
 
 _OtelContext = Union["_OtelContextAnyof0"]
 """
  OpenTelemetry Context
 
  If an event has this context, it was generated from an OpenTelemetry signal (trace, metric, log).
-
-Aggregation type: anyOf
 """
 
 
 
 class _OtelContextAnyof0(TypedDict, total=False):
     attributes: Union[Dict[str, Any], None]
     """
      Attributes of the OpenTelemetry span that maps to a Sentry event.
 
      <https://github.com/open-telemetry/opentelemetry-proto/blob/724e427879e3d2bae2edc0218fff06e37b9eb46e/opentelemetry/proto/trace/v1/trace.proto#L174-L186>
-
-    additionalProperties: True
     """
 
     resource: Union[Dict[str, Any], None]
     """
      Information about an OpenTelemetry resource.
 
      <https://github.com/open-telemetry/opentelemetry-proto/blob/724e427879e3d2bae2edc0218fff06e37b9eb46e/opentelemetry/proto/resource/v1/resource.proto>
-
-    additionalProperties: True
     """
 
 
 
 _ProfileContext = Union["_ProfileContextAnyof0"]
-"""
- Profile context
-
-Aggregation type: anyOf
-"""
+"""  Profile context """
 
 
 
 class _ProfileContextAnyof0(TypedDict, total=False):
-    profile_id: Required["_ProfileContextAnyof0ProfileId"]
+    profile_id: Required[Union["_EventId", None]]
     """
      The profile ID.
 
-    Aggregation type: anyOf
-
     Required property
     """
 
 
 
-_ProfileContextAnyof0ProfileId = Union["_EventId", None]
-"""
- The profile ID.
-
-Aggregation type: anyOf
-"""
-
-
-
 _ResponseContext = Union["_ResponseContextAnyof0"]
-"""
- Response interface that contains information on a HTTP response related to the event.
-
-Aggregation type: anyOf
-"""
+"""  Response interface that contains information on a HTTP response related to the event. """
 
 
 
 class _ResponseContextAnyof0(TypedDict, total=False):
     body_size: Union[int, None]
     """
      HTTP response body size.
 
     minimum: 0
     """
 
-    cookies: "_ResponseContextAnyof0Cookies"
+    cookies: Union["_Cookies", None]
     """
      The cookie values.
 
      Can be given unparsed as string, as dictionary, or as a list of tuples.
-
-    Aggregation type: anyOf
     """
 
-    headers: "_ResponseContextAnyof0Headers"
+    headers: Union["_Headers", None]
     """
      A dictionary of submitted headers.
 
      If a header appears multiple times it, needs to be merged according to the HTTP standard
      for header merging. Header names are treated case-insensitively by Sentry.
-
-    Aggregation type: anyOf
     """
 
     status_code: Union[int, None]
     """
      HTTP status code.
 
     minimum: 0
     """
 
 
 
-_ResponseContextAnyof0Cookies = Union["_Cookies", None]
-"""
- The cookie values.
-
- Can be given unparsed as string, as dictionary, or as a list of tuples.
-
-Aggregation type: anyOf
-"""
-
-
-
-_ResponseContextAnyof0Headers = Union["_Headers", None]
-"""
- A dictionary of submitted headers.
-
- If a header appears multiple times it, needs to be merged according to the HTTP standard
- for header merging. Header names are treated case-insensitively by Sentry.
-
-Aggregation type: anyOf
-"""
-
-
-
 _RuntimeContext = Union["_RuntimeContextAnyof0"]
 """
  Runtime information.
 
  Runtime context describes a runtime in more detail. Typically, this context is present in
  `contexts` multiple times if multiple runtimes are involved (for instance, if you have a
  JavaScript application running on top of JVM).
-
-Aggregation type: anyOf
 """
 
 
 
 class _RuntimeContextAnyof0(TypedDict, total=False):
     build: Union[str, None]
     """  Application build string, if it is separate from the version. """
@@ -989,89 +810,76 @@
     data: Required[Union[Dict[str, Any], None]]
     """ Required property """
 
     hash: str
 
 
 _SpanId = Union[str]
-"""
- A 16-character hex string as described in the W3C trace context spec.
+"""  A 16-character hex string as described in the W3C trace context spec. """
 
-Aggregation type: anyOf
-"""
 
 
-
-_SpanStatus = Union[Literal['ok'], Literal['cancelled'], Literal['unknown'], Literal['invalid_argument'], Literal['deadline_exceeded'], Literal['not_found'], Literal['already_exists'], Literal['permission_denied'], Literal['resource_exhausted'], Literal['failed_precondition'], Literal['aborted'], Literal['out_of_range'], Literal['unimplemented'], Literal['internal_error'], Literal['unavailable'], Literal['data_loss'], Literal['unauthenticated']]
+_SpanStatus = Union[Literal["ok"], Literal["cancelled"], Literal["unknown"], Literal["invalid_argument"], Literal["deadline_exceeded"], Literal["not_found"], Literal["already_exists"], Literal["permission_denied"], Literal["resource_exhausted"], Literal["failed_precondition"], Literal["aborted"], Literal["out_of_range"], Literal["unimplemented"], Literal["internal_error"], Literal["unavailable"], Literal["data_loss"], Literal["unauthenticated"]]
 """
 Trace status.
 
 Values from <https://github.com/open-telemetry/opentelemetry-specification/blob/8fb6c14e4709e75a9aaa64b0dbbdf02a6067682a/specification/api-tracing.md#status> Mapping to HTTP from <https://github.com/open-telemetry/opentelemetry-specification/blob/8fb6c14e4709e75a9aaa64b0dbbdf02a6067682a/specification/data-http.md#status>
 """
-_SPANSTATUS_OK: Literal['ok'] = "ok"
+_SPANSTATUS_OK: Literal["ok"] = "ok"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_CANCELLED: Literal['cancelled'] = "cancelled"
+_SPANSTATUS_CANCELLED: Literal["cancelled"] = "cancelled"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_UNKNOWN: Literal['unknown'] = "unknown"
+_SPANSTATUS_UNKNOWN: Literal["unknown"] = "unknown"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_INVALID_ARGUMENT: Literal['invalid_argument'] = "invalid_argument"
+_SPANSTATUS_INVALID_ARGUMENT: Literal["invalid_argument"] = "invalid_argument"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_DEADLINE_EXCEEDED: Literal['deadline_exceeded'] = "deadline_exceeded"
+_SPANSTATUS_DEADLINE_EXCEEDED: Literal["deadline_exceeded"] = "deadline_exceeded"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_NOT_FOUND: Literal['not_found'] = "not_found"
+_SPANSTATUS_NOT_FOUND: Literal["not_found"] = "not_found"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_ALREADY_EXISTS: Literal['already_exists'] = "already_exists"
+_SPANSTATUS_ALREADY_EXISTS: Literal["already_exists"] = "already_exists"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_PERMISSION_DENIED: Literal['permission_denied'] = "permission_denied"
+_SPANSTATUS_PERMISSION_DENIED: Literal["permission_denied"] = "permission_denied"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_RESOURCE_EXHAUSTED: Literal['resource_exhausted'] = "resource_exhausted"
+_SPANSTATUS_RESOURCE_EXHAUSTED: Literal["resource_exhausted"] = "resource_exhausted"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_FAILED_PRECONDITION: Literal['failed_precondition'] = "failed_precondition"
+_SPANSTATUS_FAILED_PRECONDITION: Literal["failed_precondition"] = "failed_precondition"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_ABORTED: Literal['aborted'] = "aborted"
+_SPANSTATUS_ABORTED: Literal["aborted"] = "aborted"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_OUT_OF_RANGE: Literal['out_of_range'] = "out_of_range"
+_SPANSTATUS_OUT_OF_RANGE: Literal["out_of_range"] = "out_of_range"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_UNIMPLEMENTED: Literal['unimplemented'] = "unimplemented"
+_SPANSTATUS_UNIMPLEMENTED: Literal["unimplemented"] = "unimplemented"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_INTERNAL_ERROR: Literal['internal_error'] = "internal_error"
+_SPANSTATUS_INTERNAL_ERROR: Literal["internal_error"] = "internal_error"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_UNAVAILABLE: Literal['unavailable'] = "unavailable"
+_SPANSTATUS_UNAVAILABLE: Literal["unavailable"] = "unavailable"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_DATA_LOSS: Literal['data_loss'] = "data_loss"
+_SPANSTATUS_DATA_LOSS: Literal["data_loss"] = "data_loss"
 """The values for the 'Trace status' enum"""
-_SPANSTATUS_UNAUTHENTICATED: Literal['unauthenticated'] = "unauthenticated"
+_SPANSTATUS_UNAUTHENTICATED: Literal["unauthenticated"] = "unauthenticated"
 """The values for the 'Trace status' enum"""
 
 
 
-_TagEntry = Union["_TagEntryAnyof0", None]
-""" Aggregation type: anyOf """
-
-
-
 _TagEntryAnyof0 = Tuple[Union[str, None], Union[str, None]]
 """
 maxItems: 2
 minItems: 2
 """
 
 
 
-_Tags = List["_TagEntry"]
+_Tags = List[Union["_TagEntryAnyof0", None]]
 """  Manual key/value tag pairs. """
 
 
 
 _TraceContext = Union["_TraceContextAnyof0"]
-"""
- Trace context
-
-Aggregation type: anyOf
-"""
+"""  Trace context """
 
 
 
 class _TraceContextAnyof0(TypedDict, total=False):
     client_sample_rate: Union[Union[int, float], None]
     """
      The client-side sample rate as reported in the envelope's `trace.sample_rate` header.
@@ -1085,101 +893,46 @@
      The amount of time in milliseconds spent in this transaction span,
      excluding its immediate child spans.
     """
 
     op: Union[str, None]
     """  Span type (see `OperationType` docs). """
 
-    parent_span_id: "_TraceContextAnyof0ParentSpanId"
-    """
-     The ID of the span enclosing this span.
+    parent_span_id: Union["_SpanId", None]
+    """  The ID of the span enclosing this span. """
 
-    Aggregation type: anyOf
-    """
-
-    span_id: Required["_TraceContextAnyof0SpanId"]
+    span_id: Required[Union["_SpanId", None]]
     """
      The ID of the span.
 
-    Aggregation type: anyOf
-
     Required property
     """
 
-    status: "_TraceContextAnyof0Status"
+    status: Union["_SpanStatus", None]
     """
      Whether the trace failed or succeeded. Currently only used to indicate status of individual
      transactions.
-
-    Aggregation type: anyOf
     """
 
-    trace_id: Required["_TraceContextAnyof0TraceId"]
+    trace_id: Required[Union["_TraceId", None]]
     """
      The trace ID.
 
-    Aggregation type: anyOf
-
     Required property
     """
 
 
 
-_TraceContextAnyof0ParentSpanId = Union["_SpanId", None]
-"""
- The ID of the span enclosing this span.
-
-Aggregation type: anyOf
-"""
-
-
-
-_TraceContextAnyof0SpanId = Union["_SpanId", None]
-"""
- The ID of the span.
-
-Aggregation type: anyOf
-"""
-
-
-
-_TraceContextAnyof0Status = Union["_SpanStatus", None]
-"""
- Whether the trace failed or succeeded. Currently only used to indicate status of individual
- transactions.
-
-Aggregation type: anyOf
-"""
-
-
-
-_TraceContextAnyof0TraceId = Union["_TraceId", None]
-"""
- The trace ID.
-
-Aggregation type: anyOf
-"""
-
-
-
 _TraceId = Union[str]
-"""
- A 32-character hex string as described in the W3C trace context spec.
-
-Aggregation type: anyOf
-"""
+"""  A 32-character hex string as described in the W3C trace context spec. """
 
 
 
 _TransactionInfo = Union["_TransactionInfoAnyof0"]
-"""
- Additional information about the name of the transaction.
-
-Aggregation type: anyOf
-"""
+"""  Additional information about the name of the transaction. """
 
 
 
 class _TransactionInfoAnyof0(TypedDict, total=False):
     source: Union[str, None]
     """
     Describes how the name of the transaction was determined.
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/generic-events.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/events.v1.schema.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6877681818633231%*

 * *Differences: {"'anyOf'": "{insert: [(1, OrderedDict([('$ref', '#/definitions/StartDeleteGroupsMessage')])), (2, "*

 * *            "OrderedDict([('$ref', '#/definitions/StartMergeMessage')])), (3, "*

 * *            "OrderedDict([('$ref', '#/definitions/StartUnmergeMessage')])), (4, "*

 * *            "OrderedDict([('$ref', '#/definitions/StartUnmergeHierarchicalMessage')])), (5, "*

 * *            "OrderedDict([('$ref', '#/definitions/StartDeleteTagMessage')])), (6, "*

 * *            "OrderedDict([('$ref', '#/definitions/EndDeleteGroupsMessag […]*

```diff
@@ -1,12 +1,51 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "anyOf": [
         {
             "$ref": "#/definitions/InsertEventMessage"
+        },
+        {
+            "$ref": "#/definitions/StartDeleteGroupsMessage"
+        },
+        {
+            "$ref": "#/definitions/StartMergeMessage"
+        },
+        {
+            "$ref": "#/definitions/StartUnmergeMessage"
+        },
+        {
+            "$ref": "#/definitions/StartUnmergeHierarchicalMessage"
+        },
+        {
+            "$ref": "#/definitions/StartDeleteTagMessage"
+        },
+        {
+            "$ref": "#/definitions/EndDeleteGroupsMessage"
+        },
+        {
+            "$ref": "#/definitions/EndMergeMessage"
+        },
+        {
+            "$ref": "#/definitions/EndUnmergeMessage"
+        },
+        {
+            "$ref": "#/definitions/EndUnmergeHierarchicalMessage"
+        },
+        {
+            "$ref": "#/definitions/EndDeleteTagMessage"
+        },
+        {
+            "$ref": "#/definitions/TombstoneEventsMessage"
+        },
+        {
+            "$ref": "#/definitions/ReplaceGroupMessage"
+        },
+        {
+            "$ref": "#/definitions/ExcludeGroupsMessage"
         }
     ],
     "definitions": {
         "Addr": {
             "type": "string"
         },
         "AppContext": {
@@ -590,14 +629,216 @@
                         }
                     },
                     "type": "object"
                 }
             ],
             "description": " Device information.\n\n Device context describes the device that caused the event. This is most appropriate for mobile\n applications."
         },
+        "EndDeleteGroupsMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "end_delete_groups"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "group_ids": {
+                            "items": {
+                                "type": "integer"
+                            },
+                            "type": "array"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        },
+                        "transaction_id": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "group_ids",
+                        "datetime"
+                    ],
+                    "title": "end_delete_groups_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
+        "EndDeleteTagMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "end_delete_tag"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        },
+                        "tag": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "tag",
+                        "datetime"
+                    ],
+                    "title": "end_delete_tag_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
+        "EndMergeMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "end_merge"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "new_group_id": {
+                            "type": "integer"
+                        },
+                        "previous_group_ids": {
+                            "items": {
+                                "type": "integer"
+                            },
+                            "type": "array"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        },
+                        "transaction_id": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "previous_group_ids",
+                        "new_group_id",
+                        "datetime"
+                    ],
+                    "title": "end_merge_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
+        "EndUnmergeHierarchicalMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "end_unmerge_hierarchical"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "hierarchical_hash": {
+                            "type": "string"
+                        },
+                        "new_group_id": {
+                            "type": "integer"
+                        },
+                        "previous_group_id": {
+                            "type": "integer"
+                        },
+                        "primary_hash": {
+                            "type": "string"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "previous_group_id",
+                        "new_group_id",
+                        "primary_hash",
+                        "hierarchical_hash",
+                        "datetime"
+                    ],
+                    "title": "end_unmerge_hierarchical_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
+        "EndUnmergeMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "end_unmerge"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "hashes": {
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": "array"
+                        },
+                        "new_group_id": {
+                            "type": "integer"
+                        },
+                        "previous_group_id": {
+                            "type": "integer"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        },
+                        "transaction_id": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "previous_group_id",
+                        "new_group_id",
+                        "hashes",
+                        "datetime"
+                    ],
+                    "title": "end_unmerge_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
         "Event": {
             "additionalProperties": true,
             "description": "The sentry v7 event structure.",
             "properties": {
                 "contexts": {
                     "anyOf": [
                         {
@@ -626,32 +867,14 @@
                 "environment": {
                     "description": " The environment name, such as `production` or `staging`.\n\n ```json\n { \"environment\": \"production\" }\n ```",
                     "type": [
                         "string",
                         "null"
                     ]
                 },
-                "errors": {
-                    "default": null,
-                    "description": " Errors encountered during processing. Intended to be phased out in favor of\n annotation/metadata system.",
-                    "items": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/definitions/EventProcessingError"
-                            },
-                            {
-                                "type": "null"
-                            }
-                        ]
-                    },
-                    "type": [
-                        "array",
-                        "null"
-                    ]
-                },
                 "event_id": {
                     "anyOf": [
                         {
                             "$ref": "#/definitions/EventId"
                         },
                         {
                             "type": "null"
@@ -892,59 +1115,24 @@
             "anyOf": [
                 {
                     "type": "string"
                 }
             ],
             "description": " Wrapper around a UUID with slightly different formatting."
         },
-        "EventProcessingError": {
-            "anyOf": [
-                {
-                    "properties": {
-                        "name": {
-                            "default": null,
-                            "description": " Affected key or deep path.",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "type": {
-                            "description": " The error kind.",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "value": {
-                            "default": null,
-                            "description": " The original value causing this error."
-                        }
-                    },
-                    "required": [
-                        "type"
-                    ],
-                    "type": "object"
-                }
-            ],
-            "description": " An event processing error."
-        },
         "EventType": {
-            "description": "The type of an event.\n\nThe event type determines how Sentry handles the event and has an impact on processing, rate limiting, and quotas. There are three fundamental classes of event types:\n\n- **Error monitoring events** (`default`, `error`): Processed and grouped into unique issues based on their exception stack traces and error messages. - **Security events** (`csp`, `hpkp`, `expectct`, `expectstaple`): Derived from Browser security violation reports and grouped into unique issues based on the endpoint and violation. SDKs do not send such events. - **Transaction events** (`transaction`): Contain operation spans and collected into traces for performance monitoring. - **Feedback events** (`feedback`): Contains user feedback messages.",
+            "description": "The type of an event.\n\nThe event type determines how Sentry handles the event and has an impact on processing, rate limiting, and quotas. There are three fundamental classes of event types:\n\n- **Error monitoring events** (`default`, `error`): Processed and grouped into unique issues based on their exception stack traces and error messages. - **Security events** (`csp`, `hpkp`, `expectct`, `expectstaple`): Derived from Browser security violation reports and grouped into unique issues based on the endpoint and violation. SDKs do not send such events. - **Transaction events** (`transaction`): Contain operation spans and collected into traces for performance monitoring.",
             "enum": [
                 "error",
                 "csp",
                 "hpkp",
                 "expectct",
                 "expectstaple",
                 "transaction",
-                "nel",
-                "default",
-                "generic",
-                "feedback"
+                "default"
             ],
             "type": "string"
         },
         "Exception": {
             "anyOf": [
                 {
                     "additionalProperties": true,
@@ -1043,14 +1231,45 @@
                         "array"
                     ]
                 }
             },
             "title": "sentry_exception_chain",
             "type": "object"
         },
+        "ExcludeGroupsMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "exclude_groups"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "group_ids": {
+                            "items": {
+                                "type": "integer"
+                            },
+                            "type": "array"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "group_ids"
+                    ],
+                    "title": "exclude_groups_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
         "Fingerprint": {
             "anyOf": [
                 {
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
@@ -1561,71 +1780,14 @@
                         "type": "integer"
                     },
                     "type": "array"
                 },
                 "message": {
                     "type": "string"
                 },
-                "occurrence_data": {
-                    "properties": {
-                        "culprit": {
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "detection_time": {
-                            "type": "number"
-                        },
-                        "fingerprint": {
-                            "items": {
-                                "type": "string"
-                            },
-                            "type": "array"
-                        },
-                        "id": {
-                            "type": "string"
-                        },
-                        "issue_title": {
-                            "type": "string"
-                        },
-                        "level": {
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "resource_id": {
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "subtitle": {
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "type": {
-                            "type": "integer"
-                        }
-                    },
-                    "required": [
-                        "detection_time",
-                        "fingerprint",
-                        "issue_title",
-                        "id",
-                        "type"
-                    ],
-                    "type": "object"
-                },
-                "occurrence_id": {
-                    "type": "string"
-                },
                 "organization_id": {
                     "type": "integer"
                 },
                 "platform": {
                     "type": "string"
                 },
                 "primary_hash": {
@@ -1645,17 +1807,15 @@
                 "data",
                 "project_id",
                 "datetime",
                 "event_id",
                 "message",
                 "primary_hash",
                 "platform",
-                "group_id",
-                "occurrence_id",
-                "occurrence_data"
+                "group_id"
             ],
             "title": "insert_event",
             "type": "object"
         },
         "InsertEventMessage": {
             "items": [
                 {
@@ -1960,37 +2120,189 @@
                 "frames"
             ],
             "type": "object"
         },
         "RegVal": {
             "type": "string"
         },
+        "ReplaceGroupMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "replace_group"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "event_ids": {
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": "array"
+                        },
+                        "from_timestamp": {
+                            "type": "string"
+                        },
+                        "new_group_id": {
+                            "type": "integer"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        },
+                        "to_timestamp": {
+                            "type": "string"
+                        },
+                        "transaction_id": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "event_ids",
+                        "project_id",
+                        "new_group_id"
+                    ],
+                    "title": "replace_group_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
         "Request": {
             "anyOf": [
                 {
                     "additionalProperties": true,
                     "properties": {
+                        "body_size": {
+                            "description": " HTTP request body size.",
+                            "minimum": 0,
+                            "type": [
+                                "integer",
+                                "null"
+                            ]
+                        },
+                        "cookies": {
+                            "anyOf": [
+                                {
+                                    "$ref": "#/definitions/Cookies"
+                                },
+                                {
+                                    "type": "null"
+                                }
+                            ],
+                            "description": " The cookie values.\n\n Can be given unparsed as string, as dictionary, or as a list of tuples."
+                        },
+                        "data": {
+                            "description": " Request data in any format that makes sense.\n\n SDKs should discard large and binary bodies by default. Can be given as string or\n structural data of any format.",
+                            "type": [
+                                "array",
+                                "object",
+                                "string",
+                                "integer",
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "env": {
+                            "additionalProperties": true,
+                            "description": " Server environment data, such as CGI/WSGI.\n\n A dictionary containing environment information passed from the server. This is where\n information such as CGI/WSGI/Rack keys go that are not HTTP headers.\n\n Sentry will explicitly look for `REMOTE_ADDR` to extract an IP address.",
+                            "type": [
+                                "object",
+                                "null"
+                            ]
+                        },
+                        "fragment": {
+                            "description": " The fragment of the request URL.",
+                            "type": [
+                                "string",
+                                "null"
+                            ]
+                        },
                         "headers": {
                             "anyOf": [
                                 {
                                     "$ref": "#/definitions/Headers"
                                 },
                                 {
                                     "type": "null"
                                 }
                             ],
                             "description": " A dictionary of submitted headers.\n\n If a header appears multiple times it, needs to be merged according to the HTTP standard\n for header merging. Header names are treated case-insensitively by Sentry."
                         },
+                        "inferred_content_type": {
+                            "description": " The inferred content type of the request payload.",
+                            "type": [
+                                "string",
+                                "null"
+                            ]
+                        },
                         "method": {
                             "description": " HTTP request method.",
                             "type": [
                                 "string",
                                 "null"
                             ]
                         },
+                        "query_string": {
+                            "anyOf": [
+                                {
+                                    "anyOf": [
+                                        {
+                                            "type": "string"
+                                        },
+                                        {
+                                            "anyOf": [
+                                                {
+                                                    "additionalProperties": {
+                                                        "type": [
+                                                            "string",
+                                                            "null"
+                                                        ]
+                                                    },
+                                                    "type": "object"
+                                                },
+                                                {
+                                                    "items": {
+                                                        "items": [
+                                                            {
+                                                                "type": [
+                                                                    "string",
+                                                                    "null"
+                                                                ]
+                                                            },
+                                                            {
+                                                                "type": [
+                                                                    "string",
+                                                                    "null"
+                                                                ]
+                                                            }
+                                                        ],
+                                                        "maxItems": 2,
+                                                        "minItems": 2,
+                                                        "type": [
+                                                            "array",
+                                                            "null"
+                                                        ]
+                                                    },
+                                                    "type": "array"
+                                                }
+                                            ]
+                                        }
+                                    ]
+                                },
+                                {
+                                    "type": "null"
+                                }
+                            ],
+                            "description": " The query string component of the URL.\n\n Can be given as unparsed string, dictionary, or list of tuples.\n\n If the query string is not declared and part of the `url`, Sentry moves it to the\n query string."
+                        },
                         "url": {
                             "description": " The URL of the request if available.\n\nThe query string can be declared either as part of the `url`, or separately in `query_string`.",
                             "type": [
                                 "string",
                                 "null"
                             ]
                         }
@@ -2122,14 +2434,135 @@
                 "unauthenticated"
             ],
             "type": "string"
         },
         "Stacktrace": {
             "$ref": "#/definitions/RawStacktrace"
         },
+        "StartDeleteGroupsMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "start_delete_groups"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "group_ids": {
+                            "items": {
+                                "type": "integer"
+                            },
+                            "type": "array"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        },
+                        "transaction_id": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "group_ids",
+                        "datetime"
+                    ],
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
+        "StartDeleteTagMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "start_delete_tag"
+                },
+                {
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
+        "StartMergeMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "start_merge"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "new_group_id": {
+                            "type": "integer"
+                        },
+                        "previous_group_ids": {
+                            "items": {
+                                "type": "integer"
+                            },
+                            "type": "array"
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        },
+                        "transaction_id": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "previous_group_ids",
+                        "new_group_id",
+                        "datetime"
+                    ],
+                    "title": "start_merge_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
+        "StartUnmergeHierarchicalMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "start_unmerge_hierarchical"
+                },
+                {
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
+        "StartUnmergeMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "start_unmerge"
+                },
+                {
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
         "String": {
             "type": "string"
         },
         "SystemSdkInfo": {
             "anyOf": [
                 {
                     "additionalProperties": true,
@@ -2275,14 +2708,60 @@
             "anyOf": [
                 {
                     "type": "number"
                 }
             ],
             "description": "Can be a ISO-8601 formatted string or a unix timestamp in seconds (floating point values allowed).\n\nMust be UTC."
         },
+        "TombstoneEventsMessage": {
+            "items": [
+                {
+                    "const": 2
+                },
+                {
+                    "const": "tombstone_events"
+                },
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "datetime": {
+                            "$ref": "#/definitions/SnubaDatetime"
+                        },
+                        "event_ids": {
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": "array"
+                        },
+                        "from_timestamp": {
+                            "type": "string"
+                        },
+                        "old_primary_hash": {
+                            "type": [
+                                "string",
+                                "null"
+                            ]
+                        },
+                        "project_id": {
+                            "type": "integer"
+                        },
+                        "to_timestamp": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "project_id",
+                        "event_ids"
+                    ],
+                    "title": "tombstone_events_message_body",
+                    "type": "object"
+                }
+            ],
+            "type": "array"
+        },
         "TraceContext": {
             "anyOf": [
                 {
                     "additionalProperties": true,
                     "properties": {
                         "client_sample_rate": {
                             "description": " The client-side sample rate as reported in the envelope's `trace.sample_rate` header.\n\n The server takes this field from envelope headers and writes it back into the event. Clients\n should not ever send this value.",
@@ -2312,21 +2791,14 @@
                                 },
                                 {
                                     "type": "null"
                                 }
                             ],
                             "description": " The ID of the span enclosing this span."
                         },
-                        "sampled": {
-                            "description": " Whether the trace connected to the event has been sampled as part of dynamic sampling",
-                            "type": [
-                                "boolean",
-                                "null"
-                            ]
-                        },
                         "span_id": {
                             "anyOf": [
                                 {
                                     "$ref": "#/definitions/SpanId"
                                 },
                                 {
                                     "type": "null"
@@ -2470,10 +2942,10 @@
                     "type": "object"
                 }
             ],
             "description": " Information about the user who triggered an event.\n\n ```json\n {\n   \"user\": {\n     \"id\": \"unique_id\",\n     \"username\": \"my_user\",\n     \"email\": \"foo@example.com\",\n     \"ip_address\": \"127.0.0.1\",\n     \"subscription\": \"basic\"\n   }\n }\n ```",
             "title": "sentry_user"
         }
     },
-    "description": "Issue platform event",
-    "title": "generic_event"
+    "description": "The snuba eventstream message.",
+    "title": "event_stream_message"
 }
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/group-attributes.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'$ref'": "'#/definitions/Main'",*

 * * "'definitions'": "{replace: OrderedDict([('Main', OrderedDict([('title', 'metric'), ('type', "*

 * *                  "'object'), ('additionalProperties', True), ('properties', "*

 * *                  "OrderedDict([('version', OrderedDict([('const', 1)])), ('use_case_id', "*

 * *                  "OrderedDict([('type', 'string')])), ('org_id', OrderedDict([('type', "*

 * *                  "'integer')])), ('project_id', OrderedDict([('type', 'integer')])), "*

 * *                  "('metric_id', […]*

```diff
@@ -1,104 +1,106 @@
 {
-    "$ref": "#/definitions/GroupAttributesSnapshot",
+    "$ref": "#/definitions/Main",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
-        "GroupAttributesSnapshot": {
-            "properties": {
-                "assignee_team_id": {
-                    "type": [
-                        "integer",
-                        "null"
-                    ]
-                },
-                "assignee_user_id": {
-                    "type": [
-                        "integer",
-                        "null"
-                    ]
-                },
-                "first_seen": {
+        "IntToInt": {
+            "patternProperties": {
+                "^[0-9]$": {
+                    "type": "integer"
+                }
+            },
+            "type": "object"
+        },
+        "IntToString": {
+            "patternProperties": {
+                "^[0-9]$": {
                     "type": "string"
+                }
+            },
+            "type": "object"
+        },
+        "Main": {
+            "additionalProperties": true,
+            "properties": {
+                "mapping_meta": {
+                    "$ref": "#/definitions/MappingMeta"
                 },
-                "group_deleted": {
-                    "type": "boolean"
-                },
-                "group_id": {
+                "metric_id": {
                     "type": "integer"
                 },
-                "num_comments": {
+                "org_id": {
                     "type": "integer"
                 },
-                "owner_codeowners_team_id": {
-                    "type": [
-                        "integer",
-                        "null"
-                    ]
-                },
-                "owner_codeowners_user_id": {
-                    "type": [
-                        "integer",
-                        "null"
-                    ]
-                },
-                "owner_ownership_rule_team_id": {
-                    "type": [
-                        "integer",
-                        "null"
-                    ]
+                "project_id": {
+                    "type": "integer"
                 },
-                "owner_ownership_rule_user_id": {
-                    "type": [
-                        "integer",
-                        "null"
-                    ]
+                "retention_days": {
+                    "type": "integer"
                 },
-                "owner_suspect_commit_user_id": {
-                    "type": [
-                        "integer",
-                        "null"
-                    ]
+                "sentry_received_timestamp": {
+                    "type": "number"
                 },
-                "priority": {
-                    "type": [
-                        "integer",
-                        "null"
-                    ]
+                "tags": {
+                    "$ref": "#/definitions/IntToInt"
                 },
-                "project_id": {
+                "timestamp": {
+                    "minimum": 0,
                     "type": "integer"
                 },
-                "status": {
-                    "type": "integer"
+                "type": {
+                    "type": "string"
                 },
-                "substatus": {
-                    "type": [
-                        "integer",
-                        "null"
+                "use_case_id": {
+                    "type": "string"
+                },
+                "value": {
+                    "anyOf": [
+                        {
+                            "title": "counter_metric_value",
+                            "type": "number"
+                        },
+                        {
+                            "items": {
+                                "type": "integer"
+                            },
+                            "title": "set_metric_value",
+                            "type": "array"
+                        },
+                        {
+                            "items": {
+                                "type": "number"
+                            },
+                            "title": "distribution_metric_value",
+                            "type": "array"
+                        }
                     ]
                 },
-                "timestamp": {
-                    "type": "string"
+                "version": {
+                    "const": 1
                 }
             },
             "required": [
-                "group_deleted",
+                "mapping_meta",
+                "metric_id",
+                "org_id",
                 "project_id",
-                "group_id",
-                "status",
-                "substatus",
-                "first_seen",
-                "num_comments",
-                "assignee_user_id",
-                "assignee_team_id",
-                "owner_suspect_commit_user_id",
-                "owner_ownership_rule_user_id",
-                "owner_ownership_rule_team_id",
-                "owner_codeowners_user_id",
-                "owner_codeowners_team_id",
-                "timestamp"
+                "retention_days",
+                "tags",
+                "timestamp",
+                "type",
+                "use_case_id",
+                "value"
             ],
-            "title": "group_attributes_snapshot",
+            "title": "metric",
+            "type": "object"
+        },
+        "MappingMeta": {
+            "additionalProperties": true,
+            "patternProperties": {
+                "^[chdfr]$": {
+                    "$ref": "#/definitions/IntToString"
+                }
+            },
             "type": "object"
         }
     }
 }
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/ingest-monitors.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3%*

 * *Differences: {"'$ref'": "'#/definitions/Main'",*

 * * "'definitions'": "{replace: OrderedDict([('Main', OrderedDict([('title', 'subscription_result'), "*

 * *                  "('type', 'object'), ('additionalProperties', True), ('properties', "*

 * *                  "OrderedDict([('version', OrderedDict([('const', 3)])), ('payload', "*

 * *                  "OrderedDict([('type', 'object'), ('title', 'payload_v3'), "*

 * *                  "('additionalProperties', True), ('properties', OrderedDict([('subscription_id', "*

 * *                  "Or […]*

```diff
@@ -1,73 +1,79 @@
 {
+    "$ref": "#/definitions/Main",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
-        "ClockPulseMessage": {
-            "additionalProperties": false,
-            "description": "A message that is only used as a marker for minute boundaries.",
-            "properties": {
-                "message_type": {
-                    "const": "clock_pulse",
-                    "description": "Discriminant marker identifying this as a clock-pulse message."
-                }
-            },
-            "required": [
-                "message_type"
-            ],
-            "title": "clock_pulse",
-            "type": "object"
-        },
-        "MonitorCheckIn": {
+        "Main": {
             "additionalProperties": true,
-            "description": "A message that contains a monitor check-in payload.",
             "properties": {
-                "message_type": {
-                    "const": "check_in",
-                    "description": "Discriminant marker identifying this as a check-in message."
-                },
                 "payload": {
-                    "description": "bytes. JSON string of the wrapped monitor check-in event."
-                },
-                "project_id": {
-                    "description": "The project for which this check-in is being sent.",
-                    "maximum": 18446744073709551615,
-                    "minimum": 0,
-                    "type": "integer"
-                },
-                "retention_days": {
-                    "maximum": 65535,
-                    "minimum": 0,
-                    "type": "integer"
+                    "additionalProperties": true,
+                    "properties": {
+                        "entity": {
+                            "minLength": 1,
+                            "type": "string"
+                        },
+                        "request": {
+                            "type": "object"
+                        },
+                        "result": {
+                            "additionalProperties": true,
+                            "properties": {
+                                "data": {
+                                    "items": {
+                                        "type": "object"
+                                    },
+                                    "type": "array"
+                                },
+                                "meta": {
+                                    "items": {
+                                        "additionalProperties": true,
+                                        "properties": {
+                                            "name": {
+                                                "type": "string"
+                                            },
+                                            "type": {
+                                                "type": "string"
+                                            }
+                                        },
+                                        "type": "object"
+                                    },
+                                    "type": "array"
+                                }
+                            },
+                            "required": [
+                                "data",
+                                "meta"
+                            ],
+                            "type": "object"
+                        },
+                        "subscription_id": {
+                            "minLength": 1,
+                            "type": "string"
+                        },
+                        "timestamp": {
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "subscription_id",
+                        "request",
+                        "result",
+                        "timestamp",
+                        "entity"
+                    ],
+                    "title": "payload_v3",
+                    "type": "object"
                 },
-                "sdk": {
-                    "description": "The originating SDK client identifier string.",
-                    "type": [
-                        "string",
-                        "null"
-                    ]
-                },
-                "start_time": {
-                    "description": "The time relay produced the check-in to kafka. In seconds with floating precision.",
-                    "type": "number"
+                "version": {
+                    "const": 3
                 }
             },
             "required": [
-                "message_type",
-                "payload",
-                "start_time",
-                "project_id",
-                "retention_days"
+                "version",
+                "payload"
             ],
-            "title": "check_in",
+            "title": "subscription_result",
             "type": "object"
         }
-    },
-    "oneOf": [
-        {
-            "$ref": "#/definitions/ClockPulseMessage"
-        },
-        {
-            "$ref": "#/definitions/MonitorCheckIn"
-        }
-    ],
-    "title": "ingest_monitor_message"
+    }
 }
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/profile-functions.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'$ref'": "'#/definitions/Main'",*

 * * "'definitions'": "{replace: OrderedDict([('Main', OrderedDict([('type', 'object'), ('title', "*

 * *                  "'generic_metric'), ('additionalProperties', True), ('properties', "*

 * *                  "OrderedDict([('version', OrderedDict([('const', 2)])), ('use_case_id', "*

 * *                  "OrderedDict([('type', 'string')])), ('org_id', OrderedDict([('type', "*

 * *                  "'integer')])), ('project_id', OrderedDict([('type', 'integer')])), "*

 * *                  "('met […]*

```diff
@@ -1,89 +1,105 @@
 {
-    "$ref": "#/definitions/ProfileFunctions",
+    "$ref": "#/definitions/Main",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
-        "Function": {
-            "items": {
-                "properties": {
-                    "fingerprint": {
-                        "$ref": "#/definitions/UInt"
-                    },
-                    "function": {
-                        "type": "string"
-                    },
-                    "in_app": {
-                        "type": "boolean"
-                    },
-                    "package": {
-                        "type": "string"
-                    },
-                    "self_times_ns": {
-                        "items": {
-                            "$ref": "#/definitions/UInt"
-                        },
-                        "type": "array"
-                    }
-                },
-                "required": [
-                    "fingerprint",
-                    "function",
-                    "in_app",
-                    "package",
-                    "self_times_ns"
-                ],
-                "type": "object"
+        "IntToString": {
+            "additionalProperties": true,
+            "patternProperties": {
+                "^[0-9]$": {
+                    "type": "string"
+                }
             },
-            "type": "array"
+            "type": "object"
         },
-        "ProfileFunctions": {
+        "Main": {
+            "additionalProperties": true,
             "properties": {
-                "environment": {
-                    "type": "string"
+                "mapping_meta": {
+                    "$ref": "#/definitions/MappingMeta"
                 },
-                "functions": {
-                    "$ref": "#/definitions/Function"
+                "metric_id": {
+                    "type": "integer"
                 },
-                "platform": {
-                    "type": "string"
-                },
-                "profile_id": {
-                    "type": "string"
+                "org_id": {
+                    "type": "integer"
                 },
                 "project_id": {
-                    "$ref": "#/definitions/UInt"
+                    "type": "integer"
                 },
-                "received": {
-                    "$ref": "#/definitions/UInt"
+                "retention_days": {
+                    "type": "integer"
                 },
-                "release": {
-                    "type": "string"
+                "sentry_received_timestamp": {
+                    "type": "number"
                 },
-                "retention_days": {
-                    "$ref": "#/definitions/UInt"
+                "tags": {
+                    "$ref": "#/definitions/StringToString"
                 },
                 "timestamp": {
-                    "$ref": "#/definitions/UInt"
+                    "minimum": 0,
+                    "type": "integer"
                 },
-                "transaction_name": {
+                "type": {
                     "type": "string"
+                },
+                "use_case_id": {
+                    "type": "string"
+                },
+                "value": {
+                    "anyOf": [
+                        {
+                            "title": "counter_metric_value",
+                            "type": "number"
+                        },
+                        {
+                            "items": {
+                                "type": "integer"
+                            },
+                            "title": "set_metric_value",
+                            "type": "array"
+                        },
+                        {
+                            "items": {
+                                "type": "number"
+                            },
+                            "title": "distribution_metric_value",
+                            "type": "array"
+                        }
+                    ]
+                },
+                "version": {
+                    "const": 2
                 }
             },
             "required": [
-                "functions",
-                "profile_id",
-                "platform",
+                "mapping_meta",
+                "metric_id",
+                "org_id",
                 "project_id",
-                "received",
                 "retention_days",
+                "tags",
                 "timestamp",
-                "transaction_name"
+                "type",
+                "use_case_id",
+                "value"
             ],
+            "title": "generic_metric",
             "type": "object"
         },
-        "UInt": {
-            "minimum": 0,
-            "type": "integer"
+        "MappingMeta": {
+            "additionalProperties": true,
+            "patternProperties": {
+                "^[chdfr]$": {
+                    "$ref": "#/definitions/IntToString"
+                }
+            },
+            "type": "object"
+        },
+        "StringToString": {
+            "additionalProperties": {
+                "type": "string"
+            },
+            "type": "object"
         }
-    },
-    "title": "profile_functions"
+    }
 }
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'additionalProperties'": 'True',*

 * * "'definitions'": "{replace: OrderedDict([('QueryMetadata', OrderedDict([('type', 'object'), "*

 * *                  "('title', 'query_metadata'), ('properties', OrderedDict([('sql', "*

 * *                  "OrderedDict([('type', 'string')])), ('sql_anonymized', OrderedDict([('type', "*

 * *                  "'string')])), ('start_timestamp', OrderedDict([('type', ['integer', "*

 * *                  "'null'])])), ('end_timestamp', OrderedDict([('type', ['integer', 'null'])])), "*

 * *           […]*

```diff
@@ -1,198 +1,251 @@
 {
-    "$ref": "#/definitions/Main",
     "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": true,
     "definitions": {
-        "IntToString": {
-            "additionalProperties": true,
-            "patternProperties": {
-                "^[0-9]$": {
+        "ClickhouseQueryProfile": {
+            "properties": {
+                "all_columns": {
+                    "$ref": "#/definitions/ColumnList"
+                },
+                "array_join_cols": {
+                    "$ref": "#/definitions/ColumnList"
+                },
+                "groupby_cols": {
+                    "$ref": "#/definitions/ColumnList"
+                },
+                "multi_level_condition": {
+                    "type": "boolean"
+                },
+                "table": {
                     "type": "string"
+                },
+                "time_range": {
+                    "type": [
+                        "integer",
+                        "null"
+                    ]
+                },
+                "where_profile": {
+                    "additionalProperties": true,
+                    "properties": {
+                        "columns": {
+                            "$ref": "#/definitions/ColumnList"
+                        },
+                        "mapping_cols": {
+                            "$ref": "#/definitions/ColumnList"
+                        }
+                    },
+                    "required": [
+                        "columns",
+                        "mapping_cols"
+                    ],
+                    "title": "clickhouse_query_profile_where_profile",
+                    "type": "object"
                 }
             },
+            "required": [
+                "time_range",
+                "multi_level_condition",
+                "where_profile",
+                "groupby_cols",
+                "array_join_cols"
+            ],
+            "title": "clickhouse_query_profile",
             "type": "object"
         },
-        "Main": {
+        "ColumnList": {
+            "items": {
+                "type": "string"
+            },
+            "type": "array"
+        },
+        "QueryMetadata": {
             "additionalProperties": true,
             "properties": {
-                "aggregation_option": {
-                    "type": "string"
+                "end_timestamp": {
+                    "type": [
+                        "integer",
+                        "null"
+                    ]
                 },
-                "mapping_meta": {
-                    "$ref": "#/definitions/MappingMeta"
+                "profile": {
+                    "$ref": "#/definitions/ClickhouseQueryProfile"
                 },
-                "metric_id": {
-                    "type": "integer"
+                "request_status": {
+                    "type": "string"
                 },
-                "org_id": {
-                    "type": "integer"
+                "result_profile": {
+                    "type": [
+                        "object",
+                        "null"
+                    ]
                 },
-                "project_id": {
-                    "type": "integer"
+                "slo": {
+                    "type": "string"
                 },
-                "retention_days": {
-                    "type": "integer"
+                "sql": {
+                    "type": "string"
                 },
-                "sentry_received_timestamp": {
-                    "type": "number"
+                "sql_anonymized": {
+                    "type": "string"
                 },
-                "tags": {
-                    "$ref": "#/definitions/StringToString"
+                "start_timestamp": {
+                    "type": [
+                        "integer",
+                        "null"
+                    ]
                 },
-                "timestamp": {
-                    "minimum": 0,
-                    "type": "integer"
+                "stats": {
+                    "type": "object"
                 },
-                "type": {
+                "status": {
                     "type": "string"
                 },
-                "use_case_id": {
+                "trace_id": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                }
+            },
+            "required": [
+                "sql",
+                "sql_anonymized",
+                "start_timestamp",
+                "end_timestamp",
+                "stats",
+                "status",
+                "trace_id",
+                "profile",
+                "result_profile",
+                "request_status",
+                "slo"
+            ],
+            "title": "query_metadata",
+            "type": "object"
+        }
+    },
+    "description": "Querylog schema",
+    "properties": {
+        "dataset": {
+            "type": "string"
+        },
+        "end_timestamp": {
+            "type": [
+                "integer",
+                "null"
+            ]
+        },
+        "entity": {
+            "type": "string"
+        },
+        "organization": {
+            "type": [
+                "integer",
+                "null"
+            ]
+        },
+        "projects": {
+            "items": {
+                "type": "integer"
+            },
+            "type": "array"
+        },
+        "query_list": {
+            "items": {
+                "$ref": "#/definitions/QueryMetadata"
+            },
+            "type": "array"
+        },
+        "request": {
+            "properties": {
+                "app_id": {
                     "type": "string"
                 },
-                "value": {
-                    "anyOf": [
-                        {
-                            "properties": {
-                                "data": {
-                                    "anyOf": [
-                                        {
-                                            "items": {
-                                                "type": "number"
-                                            },
-                                            "type": "array"
-                                        },
-                                        {
-                                            "items": {
-                                                "type": "integer"
-                                            },
-                                            "type": "array"
-                                        }
-                                    ]
-                                },
-                                "format": {
-                                    "const": "array"
-                                }
-                            },
-                            "required": [
-                                "format",
-                                "data"
-                            ],
-                            "title": "encoded_series_array_metric_value",
-                            "type": "object"
-                        },
-                        {
-                            "properties": {
-                                "data": {
-                                    "type": "string"
-                                },
-                                "format": {
-                                    "const": "base64"
-                                }
-                            },
-                            "required": [
-                                "format",
-                                "data"
-                            ],
-                            "title": "encoded_series_base64_metric_value",
-                            "type": "object"
-                        },
-                        {
-                            "properties": {
-                                "data": {
-                                    "type": "string"
-                                },
-                                "format": {
-                                    "const": "zstd"
-                                }
-                            },
-                            "required": [
-                                "format",
-                                "data"
-                            ],
-                            "title": "encoded_series_zstd_metric_value",
-                            "type": "object"
-                        },
-                        {
-                            "title": "counter_metric_value",
-                            "type": "number"
-                        },
-                        {
-                            "items": {
-                                "type": "integer"
-                            },
-                            "title": "set_metric_value",
-                            "type": "array"
-                        },
-                        {
-                            "items": {
-                                "type": "number"
-                            },
-                            "title": "distribution_metric_value",
-                            "type": "array"
-                        },
-                        {
-                            "additionalProperties": false,
-                            "properties": {
-                                "count": {
-                                    "type": "integer"
-                                },
-                                "last": {
-                                    "type": "number"
-                                },
-                                "max": {
-                                    "type": "number"
-                                },
-                                "min": {
-                                    "type": "number"
-                                },
-                                "sum": {
-                                    "type": "number"
-                                }
-                            },
-                            "required": [
-                                "min",
-                                "max",
-                                "sum",
-                                "count",
-                                "last"
-                            ],
-                            "title": "gauge_metric_value",
-                            "type": "object"
-                        }
+                "body": {
+                    "type": "object"
+                },
+                "feature": {
+                    "type": [
+                        "string",
+                        "null"
                     ]
                 },
-                "version": {
-                    "const": 2
+                "id": {
+                    "pattern": "[0-9a-fA-F]{32}",
+                    "type": "string"
+                },
+                "referrer": {
+                    "type": "string"
+                },
+                "team": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 }
             },
             "required": [
-                "mapping_meta",
-                "metric_id",
-                "org_id",
-                "project_id",
-                "retention_days",
-                "tags",
-                "timestamp",
-                "type",
-                "use_case_id",
-                "value"
+                "id"
             ],
-            "title": "generic_metric",
             "type": "object"
         },
-        "MappingMeta": {
+        "request_status": {
+            "type": "string"
+        },
+        "slo": {
+            "type": "string"
+        },
+        "snql_anonymized": {
+            "type": "string"
+        },
+        "start_timestamp": {
+            "type": [
+                "integer",
+                "null"
+            ]
+        },
+        "status": {
+            "type": "string"
+        },
+        "timing": {
             "additionalProperties": true,
-            "patternProperties": {
-                "^[chdfr]$": {
-                    "$ref": "#/definitions/IntToString"
+            "properties": {
+                "duration_ms": {
+                    "type": "integer"
+                },
+                "marks_ms": {
+                    "additionalProperties": {
+                        "type": "integer"
+                    },
+                    "type": "object"
+                },
+                "tags": {
+                    "additionalProperties": {
+                        "type": "string"
+                    },
+                    "type": "object"
+                },
+                "timestamp": {
+                    "type": "integer"
                 }
             },
             "type": "object"
-        },
-        "StringToString": {
-            "additionalProperties": {
-                "type": "string"
-            },
-            "type": "object"
         }
-    }
+    },
+    "required": [
+        "request",
+        "dataset",
+        "entity",
+        "start_timestamp",
+        "end_timestamp",
+        "status",
+        "request_status",
+        "slo",
+        "projects",
+        "query_list",
+        "timing"
+    ],
+    "title": "querylog",
+    "type": "object"
 }
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'$ref'": "'#/definitions/IngestMetric'",*

 * * "'definitions'": "{replace: OrderedDict([('IngestMetric', OrderedDict([('type', 'object'), "*

 * *                  "('title', 'ingest_metric'), ('additionalProperties', True), ('properties', "*

 * *                  "OrderedDict([('org_id', OrderedDict([('description', 'The organization for "*

 * *                  "which this metric is being sent.'), ('type', 'integer'), ('minimum', 0), "*

 * *                  "('maximum', 18446744073709551615)])), ('project_id', "*

 * *                […]*

```diff
@@ -1,106 +1,89 @@
 {
-    "$ref": "#/definitions/Main",
+    "$ref": "#/definitions/IngestMetric",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
-        "IntToInt": {
-            "patternProperties": {
-                "^[0-9]$": {
-                    "type": "integer"
-                }
-            },
-            "type": "object"
-        },
-        "IntToString": {
-            "patternProperties": {
-                "^[0-9]$": {
-                    "type": "string"
-                }
-            },
-            "type": "object"
-        },
-        "Main": {
+        "IngestMetric": {
             "additionalProperties": true,
             "properties": {
-                "mapping_meta": {
-                    "$ref": "#/definitions/MappingMeta"
-                },
-                "metric_id": {
-                    "type": "integer"
+                "name": {
+                    "description": "The metric name. Relay sometimes calls this an MRI and makes assumptions about its string shape, and those assumptions also exist in certain queries. The rest of the ingestion pipeline treats it as an opaque string.",
+                    "type": "string"
                 },
                 "org_id": {
+                    "description": "The organization for which this metric is being sent.",
+                    "maximum": 18446744073709551615,
+                    "minimum": 0,
                     "type": "integer"
                 },
                 "project_id": {
+                    "description": "The project for which this metric is being sent.",
+                    "maximum": 18446744073709551615,
+                    "minimum": 0,
                     "type": "integer"
                 },
                 "retention_days": {
+                    "maximum": 65535,
+                    "minimum": 0,
                     "type": "integer"
                 },
-                "sentry_received_timestamp": {
-                    "type": "number"
-                },
                 "tags": {
-                    "$ref": "#/definitions/IntToInt"
+                    "additionalProperties": {
+                        "type": "string"
+                    },
+                    "type": "object"
                 },
                 "timestamp": {
+                    "description": "The timestamp at which this metric was being sent. Relay will round this down to the next 10-second interval.",
+                    "maximum": 18446744073709551615,
                     "minimum": 0,
                     "type": "integer"
                 },
                 "type": {
-                    "type": "string"
-                },
-                "use_case_id": {
+                    "description": "The metric type. [c]ounter, [d]istribution, [s]et. Relay additionally defines Gauge, but that metric type is completely unsupported downstream.",
+                    "enum": [
+                        "c",
+                        "d",
+                        "s"
+                    ],
                     "type": "string"
                 },
                 "value": {
                     "anyOf": [
                         {
                             "title": "counter_metric_value",
                             "type": "number"
                         },
                         {
                             "items": {
+                                "maximum": 4294967295,
+                                "minimum": 0,
                                 "type": "integer"
                             },
                             "title": "set_metric_value",
                             "type": "array"
                         },
                         {
                             "items": {
                                 "type": "number"
                             },
                             "title": "distribution_metric_value",
                             "type": "array"
                         }
                     ]
-                },
-                "version": {
-                    "const": 1
                 }
             },
             "required": [
-                "mapping_meta",
-                "metric_id",
+                "name",
                 "org_id",
                 "project_id",
                 "retention_days",
                 "tags",
                 "timestamp",
                 "type",
-                "use_case_id",
                 "value"
             ],
-            "title": "metric",
-            "type": "object"
-        },
-        "MappingMeta": {
-            "additionalProperties": true,
-            "patternProperties": {
-                "^[chdfr]$": {
-                    "$ref": "#/definitions/IntToString"
-                }
-            },
+            "title": "ingest_metric",
             "type": "object"
         }
     }
 }
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999627976190476%*

 * *Differences: {"'definitions'": "{'Data': {'required': {delete: [5]}}}"}*

```diff
@@ -410,16 +410,15 @@
                 }
             },
             "required": [
                 "contexts",
                 "spans",
                 "start_timestamp",
                 "timestamp",
-                "type",
-                "received"
+                "type"
             ],
             "type": "object"
         },
         "DeviceContext": {
             "anyOf": [
                 {
                     "additionalProperties": true,
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/sentry_kafka_schemas.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/sentry_kafka_schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,15 @@
     Optional,
     MutableMapping,
     Sequence,
     Tuple,
     TypedDict,
     cast,
     Literal,
-    Mapping,
 )
-from typing_extensions import NotRequired
-
 from sentry_kafka_schemas.types import Schema, Example
 from sentry_kafka_schemas.codecs import Codec
 from sentry_kafka_schemas.codecs.json import JsonCodec
 from sentry_kafka_schemas.codecs.msgpack import MsgpackCodec
 from pathlib import Path
 from yaml import safe_load
 
@@ -45,65 +42,59 @@
 
 
 class TopicData(TypedDict):
     topic: str
     description: str
     services: ServicesData
     schemas: Sequence[TopicSchema]
-    pipeline: NotRequired[str]
-    topic_creation_config: Mapping[str, str]
-    partitions: Optional[int]
 
 
 _TOPICS_PATH = Path.joinpath(Path(__file__).parent, "topics")
 _SCHEMAS_PATH = Path.joinpath(Path(__file__).parent, "schemas")
 _EXAMPLES_PATH = Path.joinpath(Path(__file__).parent, "examples")
 
 
-def list_topics() -> Iterable[str]:
+def _list_topics() -> Iterable[str]:
     """
     List all defined topic names.
+
+    This is not yet stable API, just internally used by code generation.
     """
     for file in os.listdir(_TOPICS_PATH):
         assert file.endswith(".yaml")
         yield file[: -len(".yaml")]
 
 
-def get_topic(topic: str) -> TopicData:
+def _get_topic(topic: str) -> TopicData:
     """
     Get metadata for a specific topic name.
 
     This is not yet stable API, just internally used by code generation.
     """
     topic_path = Path.joinpath(_TOPICS_PATH, f"{topic}.yaml")
 
     try:
         with open(topic_path) as f:
             topic_data = cast(TopicData, safe_load(f))
     except FileNotFoundError:
         raise SchemaNotFound
-    if "topic_creation_config" not in topic_data:
-        topic_data["topic_creation_config"] = {}
-
-    if "partitions" not in topic_data:
-        topic_data["partitions"] = None
 
     return topic_data
 
 
 def _get_schema(topic: str, version: Optional[int] = None) -> Schema:
     """
     Returns the schema for a topic. If version is passed, return the schema for
     the specified version, otherwise the latest version is returned.
 
     If a matching schema can't be found, raise SchemaNotFound.
 
     Only JSON schemas are currently supported.
     """
-    topic_data = get_topic(topic)
+    topic_data = _get_topic(topic)
 
     topic_schemas = sorted(topic_data["schemas"], key=lambda x: x["version"])
 
     schema_metadata = None
     if version is None:
         schema_metadata = topic_schemas[-1]
     else:
```

### Comparing `sentry-kafka-schemas-0.1.87/python/sentry_kafka_schemas/types.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/types.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/tests/test_codecs.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/tests/test_codeowner.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_codeowner.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.87/python/tests/test_examples.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Iterator, Tuple
 import pytest
 import fastjsonschema
 import rapidjson
 import jsonschema
 
 from sentry_kafka_schemas.sentry_kafka_schemas import (
-    list_topics,
-    get_topic,
+    _list_topics,
+    _get_topic,
     _get_schema,
 )
 from sentry_kafka_schemas.types import Example
 from sentry_kafka_schemas import iter_examples
 
 
 def get_all_examples() -> Iterator[Tuple[str, int, Example]]:
-    for topic in list_topics():
-        for schema_raw in get_topic(topic)["schemas"]:
+    for topic in _list_topics():
+        for schema_raw in _get_topic(topic)["schemas"]:
             version = schema_raw["version"]
             for x in iter_examples(topic, version=version):
                 yield topic, version, x
 
 
 def _get_most_specific_jsonschema_error(e: jsonschema.ValidationError) -> None:
     """
```

### Comparing `sentry-kafka-schemas-0.1.87/python/tests/test_valid_schemas.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_valid_schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import re
 from typing import Any, Iterator, Tuple
 import pytest
 
 from sentry_kafka_schemas.sentry_kafka_schemas import (
-    list_topics,
-    get_topic,
+    _list_topics,
+    _get_topic,
     _get_schema,
 )
 
 
 def get_all_schemas() -> Iterator[Tuple[str, int]]:
-    for topic in list_topics():
-        for schema_raw in get_topic(topic)["schemas"]:
+    for topic in _list_topics():
+        for schema_raw in _get_topic(topic)["schemas"]:
             version = schema_raw["version"]
             yield topic, version
 
 
 _VALID_DEFINITION_NAMES = re.compile(r"^[A-Z]([a-zA-Z0-9]+)$")
 _VALID_TITLE_NAMES = re.compile(r"^[a-z][a-z0-9_]+$")
 
@@ -42,15 +42,15 @@
             used_titles.add(title)
 
         if (
             "properties" in obj
             or "additionalProperites" in obj
             or "patternProperties" in obj
             or "required" in obj
-        ) and "object" not in obj.get("type", ()):
+        ) and obj.get("type") != "object":
             # Impose restriction so that types will be good:
             # https://github.com/sbrunner/jsonschema-gentypes/issues/469
             raise AssertionError(
                 "type=object needs to be specified explicitly on all schemas, if properties are defined"
             )
 
         for value in obj.get("properties", {}).values():
```

### Comparing `sentry-kafka-schemas-0.1.87/python/tests/test_valid_topic_data.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_valid_topic_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from pathlib import Path
 
-from sentry_kafka_schemas import get_codec, list_topics, get_topic
+from sentry_kafka_schemas import get_codec
 import fastjsonschema
 from yaml import safe_load
 import re
 
 _SCHEMAS = Path(__file__).parents[2].joinpath("schemas/")
 _EXAMPLES = Path(__file__).parents[2].joinpath("examples/")
 _TOPICS = Path(__file__).parents[2].joinpath("topics/")
 
 _TOPIC_SCHEMA = fastjsonschema.compile(
     {
         "properties": {
             "topic": {"type": "string"},
             "description": {"type": "string"},
-            "pipeline": {"type": "string"},
             "services": {
                 "properties": {
                     "consumers": {
                         "type": "array",
                         "items": {"$ref": "#/definitions/Repo"},
                     },
                     "producers": {
@@ -44,30 +43,24 @@
                         "type",
                         "compatibility_mode",
                         "resource",
                         "examples",
                     ],
                 },
             },
-            "topic_creation_config": {
-                "type": "object",
-                "additionalProperties": {"type": "string"},
-            },
         },
         "aditionalProperties": False,
         "required": ["topic", "description", "services"],
         "definitions": {
             "Repo": {
                 "enum": [
                     # enumerate all repos here to avoid typos
+                    "getsentry/snuba",
                     "getsentry/relay",
                     "getsentry/sentry",
-                    "getsentry/snuba",
-                    "getsentry/vroom",
-                    "getsentry/super-big-consumers",
                 ]
             }
         },
     }
 )
 
 
@@ -94,21 +87,14 @@
             assert topic_name == filename.stem
             assert valid_chars.match(topic_name)
             assert len(topic_name) <= 255
 
             # Check description provided for topic
             assert topic_data["description"]
 
-            # Check every topic has an explicit, valid compression type
-            # Today we use lz4 everywhere, this list can be extended if needed
-            valid_types = ["lz4"]
-            assert (
-                topic_data["topic_creation_config"]["compression.type"] in valid_types
-            )
-
             # Check valid schema versions
             topic_schemas = topic_data["schemas"]
             for i, schema_raw in enumerate(topic_schemas):
                 used_schema_filepaths.add(_SCHEMAS.joinpath(schema_raw["resource"]))
                 for example_path in schema_raw["examples"]:
                     for entry in _EXAMPLES.joinpath(example_path).rglob("*"):
                         if entry.is_file():
@@ -133,16 +119,7 @@
     for entry in _EXAMPLES.rglob("*"):
         if entry.is_file():
             existing_examples.add(entry)
 
     # Assert that every example file in examples/ is referenced by a topic.
     unused_examples = existing_examples - used_examples
     assert not unused_examples
-
-
-def test_retention() -> None:
-    # All topics at sentry have either 1 day or 7 day retention and this property is mandatory
-    allowed_values = (str(1 * 1000 * 60 * 60 * 24), str(7 * 1000 * 60 * 60 * 24))
-
-    for topic_name in list_topics():
-        topic = get_topic(topic_name)
-        assert topic["topic_creation_config"]["retention.ms"] in allowed_values
```

### Comparing `sentry-kafka-schemas-0.1.87/setup.py` & `sentry-kafka-schemas-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def get_requirements() -> Sequence[str]:
     with open("python/requirements.txt") as fp:
         return [x.strip() for x in fp if not x.startswith("#")]
 
 setup(
     name="sentry-kafka-schemas",
-    version="0.1.87",
+    version="0.1.9",
     author="Sentry",
     author_email="oss@sentry.io",
     url="https://github.com/getsentry/sentry-kafka-schemas",
     description="Kafka topics and schemas for Sentry",
     zip_safe=False,
     install_requires=get_requirements(),
     packages=find_packages(where="python/", exclude=["generate_python_types.py", "tests/"]),
```

