# Comparing `tmp/whylogs-1.4.1rc0.tar.gz` & `tmp/whylogs-1.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.4.1rc0.tar", max compression
+gzip compressed data, was "whylogs-1.4.1rc1.tar", max compression
```

## Comparing `whylogs-1.4.1rc0.tar` & `whylogs-1.4.1rc1.tar`

### file list

```diff
@@ -1,250 +1,250 @@
--rw-r--r--   0        0        0     3166 2024-05-13 20:41:30.719503 whylogs-1.4.1rc0/DESCRIPTION.md
--rw-r--r--   0        0        0     6650 2024-05-15 03:01:34.485133 whylogs-1.4.1rc0/pyproject.toml
--rw-r--r--   0        0        0     1801 2024-05-13 20:41:30.907000 whylogs-1.4.1rc0/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2024-05-13 20:41:30.907352 whylogs-1.4.1rc0/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2024-05-13 20:41:30.907525 whylogs-1.4.1rc0/whylogs/api/annotations.py
--rw-r--r--   0        0        0      168 2024-05-13 20:41:30.907751 whylogs-1.4.1rc0/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2024-05-13 20:41:30.907985 whylogs-1.4.1rc0/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2024-05-13 20:41:30.908136 whylogs-1.4.1rc0/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0    12819 2024-05-13 20:41:30.908467 whylogs-1.4.1rc0/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0      101 2024-05-13 20:41:30.908686 whylogs-1.4.1rc0/whylogs/api/logger/events/__init__.py
--rw-r--r--   0        0        0     5621 2024-05-13 20:41:30.908950 whylogs-1.4.1rc0/whylogs/api/logger/events/event.py
--rw-r--r--   0        0        0      750 2024-05-13 20:41:30.909958 whylogs-1.4.1rc0/whylogs/api/logger/events/file_name.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.910300 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/__init__.py
--rw-r--r--   0        0        0     7953 2024-05-13 20:41:30.910669 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/actor.py
--rw-r--r--   0        0        0     2614 2024-05-13 20:41:30.910850 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py
--rw-r--r--   0        0        0     1607 2024-05-13 20:41:30.911008 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
--rw-r--r--   0        0        0     1557 2024-05-13 20:41:30.911170 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/future_util.py
--rw-r--r--   0        0        0     1282 2024-05-13 20:41:30.911337 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/list_util.py
--rw-r--r--   0        0        0     1638 2024-05-13 20:41:30.911582 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
--rw-r--r--   0        0        0     5181 2024-05-13 20:41:30.911910 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py
--rw-r--r--   0        0        0      281 2024-05-13 20:41:30.912206 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
--rw-r--r--   0        0        0     5476 2024-05-13 20:41:30.912493 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py
--rw-r--r--   0        0        0    18881 2024-05-13 20:41:30.912846 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
--rw-r--r--   0        0        0     9034 2024-05-13 20:41:30.913261 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
--rw-r--r--   0        0        0      486 2024-05-13 20:41:30.913499 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/signal_util.py
--rw-r--r--   0        0        0      641 2024-05-13 20:41:30.913745 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/string_util.py
--rw-r--r--   0        0        0     3010 2024-05-13 20:41:30.913978 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
--rw-r--r--   0        0        0    18936 2024-05-13 20:41:30.914261 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
--rw-r--r--   0        0        0     4225 2024-05-13 20:41:30.914591 whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/time_util.py
--rw-r--r--   0        0        0     5777 2024-05-13 20:41:30.914912 whylogs-1.4.1rc0/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    22400 2024-05-15 02:30:21.369918 whylogs-1.4.1rc0/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9549 2024-05-13 20:41:30.915622 whylogs-1.4.1rc0/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2024-05-13 20:41:30.915893 whylogs-1.4.1rc0/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     7090 2024-05-13 20:41:30.916267 whylogs-1.4.1rc0/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2024-05-13 20:41:30.916520 whylogs-1.4.1rc0/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2024-05-13 20:41:30.917022 whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6178 2024-05-13 20:41:30.917370 whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7673 2024-05-13 20:41:30.917928 whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2024-05-13 20:41:30.918356 whylogs-1.4.1rc0/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2024-05-13 20:41:30.918577 whylogs-1.4.1rc0/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2024-05-13 20:41:30.918825 whylogs-1.4.1rc0/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2024-05-13 20:41:30.919109 whylogs-1.4.1rc0/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2024-05-13 20:41:30.919586 whylogs-1.4.1rc0/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2024-05-13 20:41:30.919946 whylogs-1.4.1rc0/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2024-05-13 20:41:30.920220 whylogs-1.4.1rc0/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2024-05-13 20:41:30.920477 whylogs-1.4.1rc0/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2024-05-13 20:41:30.920840 whylogs-1.4.1rc0/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2024-05-13 20:41:30.921341 whylogs-1.4.1rc0/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2024-05-13 20:41:30.921727 whylogs-1.4.1rc0/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0    18270 2024-05-13 20:41:30.922239 whylogs-1.4.1rc0/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      354 2024-05-13 20:41:30.922431 whylogs-1.4.1rc0/whylogs/api/whylabs/session/lazy.py
--rw-r--r--   0        0        0      442 2024-05-13 20:41:30.922716 whylogs-1.4.1rc0/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3893 2024-05-13 20:41:30.922952 whylogs-1.4.1rc0/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0     2823 2024-05-13 20:41:30.923189 whylogs-1.4.1rc0/whylogs/api/whylabs/session/prompts.py
--rw-r--r--   0        0        0    13613 2024-05-13 20:41:30.923686 whylogs-1.4.1rc0/whylogs/api/whylabs/session/session.py
--rw-r--r--   0        0        0     6940 2024-05-13 20:41:30.923985 whylogs-1.4.1rc0/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0     5142 2024-05-13 20:41:30.924237 whylogs-1.4.1rc0/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      278 2024-05-13 20:41:30.924455 whylogs-1.4.1rc0/whylogs/api/whylabs/session/why_init.py
--rw-r--r--   0        0        0     6581 2024-05-13 20:41:30.924726 whylogs-1.4.1rc0/whylogs/api/whylabs/session/whylabs_client_cache.py
--rw-r--r--   0        0        0      152 2024-05-13 20:41:30.925032 whylogs-1.4.1rc0/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     3498 2024-05-13 20:41:30.925288 whylogs-1.4.1rc0/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     2300 2024-05-13 20:41:30.925512 whylogs-1.4.1rc0/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2421 2024-05-13 20:41:30.925673 whylogs-1.4.1rc0/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     4021 2024-05-13 20:41:30.925836 whylogs-1.4.1rc0/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    11074 2024-05-13 20:41:30.926073 whylogs-1.4.1rc0/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0    10271 2024-05-13 20:41:30.926311 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_base.py
--rw-r--r--   0        0        0     6668 2024-05-13 20:41:30.926551 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_batch_writer.py
--rw-r--r--   0        0        0    39735 2024-05-13 20:41:30.926792 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_client.py
--rw-r--r--   0        0        0     4167 2024-05-13 20:41:30.927025 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_estimation_result_writer.py
--rw-r--r--   0        0        0     6713 2024-05-13 20:41:30.927310 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_reference_writer.py
--rw-r--r--   0        0        0     6789 2024-05-13 20:41:30.927510 whylogs-1.4.1rc0/whylogs/api/writer/whylabs_transaction_writer.py
--rw-r--r--   0        0        0     5433 2024-05-13 20:41:30.927736 whylogs-1.4.1rc0/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.927915 whylogs-1.4.1rc0/whylogs/context/__init__.py
--rw-r--r--   0        0        0      302 2024-05-13 20:41:30.928076 whylogs-1.4.1rc0/whylogs/context/environ.py
--rw-r--r--   0        0        0      516 2024-05-13 20:41:30.928216 whylogs-1.4.1rc0/whylogs/context/version.py
--rw-r--r--   0        0        0     1090 2024-05-13 20:41:30.928921 whylogs-1.4.1rc0/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3575 2024-05-13 20:41:30.929096 whylogs-1.4.1rc0/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2024-05-13 20:41:30.929270 whylogs-1.4.1rc0/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2024-05-13 20:41:30.929429 whylogs-1.4.1rc0/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2024-05-13 20:41:30.929662 whylogs-1.4.1rc0/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2024-05-13 20:41:30.929899 whylogs-1.4.1rc0/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2024-05-13 20:41:30.930056 whylogs-1.4.1rc0/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2024-05-13 20:41:30.930215 whylogs-1.4.1rc0/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2024-05-13 20:41:30.931005 whylogs-1.4.1rc0/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2024-05-13 20:41:30.931353 whylogs-1.4.1rc0/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2024-05-13 20:41:30.931575 whylogs-1.4.1rc0/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2024-05-13 20:41:30.931751 whylogs-1.4.1rc0/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2024-05-13 20:41:30.931922 whylogs-1.4.1rc0/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30661 2024-05-13 20:41:30.932293 whylogs-1.4.1rc0/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11321 2024-05-13 20:41:30.932713 whylogs-1.4.1rc0/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4230 2024-05-13 20:41:30.933105 whylogs-1.4.1rc0/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2024-05-13 20:41:30.933342 whylogs-1.4.1rc0/whylogs/core/errors.py
--rw-r--r--   0        0        0     1453 2024-05-15 02:30:21.370599 whylogs-1.4.1rc0/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2024-05-13 20:41:30.933808 whylogs-1.4.1rc0/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     2987 2024-05-13 20:41:30.934024 whylogs-1.4.1rc0/whylogs/core/metadata.py
--rw-r--r--   0        0        0     1740 2024-05-13 20:41:30.934222 whylogs-1.4.1rc0/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2024-05-13 20:41:30.934991 whylogs-1.4.1rc0/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2024-05-13 20:41:30.935290 whylogs-1.4.1rc0/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2024-05-13 20:41:30.935564 whylogs-1.4.1rc0/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2024-05-13 20:41:30.935923 whylogs-1.4.1rc0/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0    10678 2024-05-13 20:41:30.936222 whylogs-1.4.1rc0/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2024-05-13 20:41:30.936404 whylogs-1.4.1rc0/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2024-05-13 20:41:30.936738 whylogs-1.4.1rc0/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2024-05-13 20:41:30.936912 whylogs-1.4.1rc0/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2024-05-13 20:41:30.937166 whylogs-1.4.1rc0/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2024-05-13 20:41:30.937492 whylogs-1.4.1rc0/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2024-05-13 20:41:30.937745 whylogs-1.4.1rc0/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2024-05-13 20:41:30.938071 whylogs-1.4.1rc0/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2024-05-13 20:41:30.938345 whylogs-1.4.1rc0/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2024-05-13 20:41:30.938605 whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0    10663 2024-05-13 20:41:30.938862 whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2024-05-13 20:41:30.939106 whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2024-05-13 20:41:30.939268 whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2024-05-13 20:41:30.939524 whylogs-1.4.1rc0/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14608 2024-05-13 20:41:30.939849 whylogs-1.4.1rc0/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2024-05-13 20:41:30.940059 whylogs-1.4.1rc0/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2024-05-13 20:41:30.940367 whylogs-1.4.1rc0/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2024-05-13 20:41:30.940631 whylogs-1.4.1rc0/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2024-05-15 03:02:34.632043 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2024-05-15 03:02:33.305842 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2024-05-15 03:02:33.307701 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2024-05-15 03:02:33.310293 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2024-05-15 03:02:34.877348 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2024-05-15 03:02:33.315543 whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2024-05-15 03:02:33.030760 whylogs-1.4.1rc0/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2024-05-15 03:02:33.036140 whylogs-1.4.1rc0/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2024-05-13 20:41:30.940879 whylogs-1.4.1rc0/whylogs/core/relations.py
--rw-r--r--   0        0        0    11357 2024-05-13 20:41:30.941200 whylogs-1.4.1rc0/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10754 2024-05-13 20:41:30.941456 whylogs-1.4.1rc0/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2024-05-13 20:41:30.941607 whylogs-1.4.1rc0/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2024-05-13 20:41:30.941773 whylogs-1.4.1rc0/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2024-05-13 20:41:30.941963 whylogs-1.4.1rc0/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2118 2024-05-13 20:41:30.942176 whylogs-1.4.1rc0/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2024-05-13 20:41:30.942405 whylogs-1.4.1rc0/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2024-05-13 20:41:30.942560 whylogs-1.4.1rc0/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2024-05-13 20:41:30.942700 whylogs-1.4.1rc0/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2024-05-13 20:41:30.942853 whylogs-1.4.1rc0/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     2004 2024-05-13 20:41:30.943026 whylogs-1.4.1rc0/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      281 2024-05-13 20:41:30.943287 whylogs-1.4.1rc0/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4823 2024-05-13 20:41:30.943558 whylogs-1.4.1rc0/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1329 2024-05-13 20:41:30.943778 whylogs-1.4.1rc0/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2024-05-13 20:41:30.944297 whylogs-1.4.1rc0/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2024-05-13 20:41:30.944676 whylogs-1.4.1rc0/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    18600 2024-05-13 20:41:30.945021 whylogs-1.4.1rc0/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     9474 2024-05-13 20:41:30.945420 whylogs-1.4.1rc0/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2024-05-13 20:41:30.945789 whylogs-1.4.1rc0/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2024-05-13 20:41:30.946183 whylogs-1.4.1rc0/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2024-05-13 20:41:30.946534 whylogs-1.4.1rc0/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.946810 whylogs-1.4.1rc0/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2024-05-13 20:41:30.947195 whylogs-1.4.1rc0/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2024-05-13 20:41:30.947472 whylogs-1.4.1rc0/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2024-05-13 20:41:30.948164 whylogs-1.4.1rc0/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2024-05-13 20:41:30.949324 whylogs-1.4.1rc0/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2024-05-13 20:41:30.950641 whylogs-1.4.1rc0/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2024-05-13 20:41:30.950920 whylogs-1.4.1rc0/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2024-05-13 20:41:30.951685 whylogs-1.4.1rc0/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.952010 whylogs-1.4.1rc0/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.952250 whylogs-1.4.1rc0/whylogs/experimental/api/__init__.py
--rw-r--r--   0        0        0    16453 2024-05-13 20:41:30.952578 whylogs-1.4.1rc0/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2024-05-13 20:41:30.952889 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2024-05-13 20:41:30.953055 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2024-05-13 20:41:30.953221 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2024-05-13 20:41:30.953384 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2024-05-13 20:41:30.953622 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2024-05-13 20:41:30.954215 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2024-05-13 20:41:30.954467 whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2024-05-13 20:41:30.955051 whylogs-1.4.1rc0/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    19154 2024-05-13 20:41:30.955300 whylogs-1.4.1rc0/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0      299 2024-05-13 20:41:30.955597 whylogs-1.4.1rc0/whylogs/experimental/core/validators/__init__.py
--rw-r--r--   0        0        0     1218 2024-05-13 20:41:30.955843 whylogs-1.4.1rc0/whylogs/experimental/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1698 2024-05-13 20:41:30.956083 whylogs-1.4.1rc0/whylogs/experimental/core/validators/validator.py
--rw-r--r--   0        0        0     8861 2024-05-13 20:41:30.956579 whylogs-1.4.1rc0/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2024-05-13 20:41:30.956884 whylogs-1.4.1rc0/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2024-05-13 20:41:30.957168 whylogs-1.4.1rc0/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.957460 whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1369 2024-05-15 02:30:21.371374 whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2024-05-13 20:41:30.958548 whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2024-05-13 20:41:30.959073 whylogs-1.4.1rc0/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    11126 2024-05-13 20:41:30.959737 whylogs-1.4.1rc0/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2024-05-13 20:41:30.960137 whylogs-1.4.1rc0/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15564 2024-05-13 20:41:30.960577 whylogs-1.4.1rc0/whylogs/migration/converters.py
--rw-r--r--   0        0        0     7662 2024-05-13 20:41:30.960903 whylogs-1.4.1rc0/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2024-05-13 20:41:30.961302 whylogs-1.4.1rc0/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2024-05-13 20:41:30.961582 whylogs-1.4.1rc0/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.961990 whylogs-1.4.1rc0/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    22069 2024-05-13 20:41:30.962393 whylogs-1.4.1rc0/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2024-05-13 20:41:30.962713 whylogs-1.4.1rc0/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.962986 whylogs-1.4.1rc0/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2024-05-13 20:41:30.963500 whylogs-1.4.1rc0/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.963787 whylogs-1.4.1rc0/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2024-05-13 20:41:30.964141 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2024-05-13 20:41:30.964338 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2221 2024-05-15 02:30:21.372269 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2024-05-13 20:41:30.965593 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2024-05-13 20:41:30.965806 whylogs-1.4.1rc0/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2024-05-13 20:41:30.966035 whylogs-1.4.1rc0/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2024-05-13 20:41:30.966197 whylogs-1.4.1rc0/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2024-05-13 20:41:30.966896 whylogs-1.4.1rc0/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2024-05-13 20:41:30.967298 whylogs-1.4.1rc0/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2024-05-13 20:41:30.968459 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2024-05-13 20:41:30.969346 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2024-05-13 20:41:30.970143 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2024-05-13 20:41:30.971247 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2024-05-13 20:41:30.971901 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2024-05-13 20:41:30.972211 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2024-05-13 20:41:30.973349 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2024-05-13 20:41:30.973892 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2024-05-13 20:41:30.975202 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2024-05-13 20:41:30.976031 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2024-05-13 20:41:30.977239 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2024-05-13 20:41:30.977969 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2024-05-13 20:41:30.978839 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2024-05-13 20:41:30.979722 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2024-05-13 20:41:30.980137 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2024-05-13 20:41:30.980848 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2024-05-13 20:41:30.981667 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2024-05-13 20:41:30.981990 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2024-05-13 20:41:30.982756 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2024-05-13 20:41:30.983725 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2024-05-13 20:41:30.984109 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2024-05-13 20:41:30.984873 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2024-05-13 20:41:30.985612 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2024-05-13 20:41:30.985962 whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2024-05-13 20:41:30.986354 whylogs-1.4.1rc0/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2024-05-13 20:41:30.986744 whylogs-1.4.1rc0/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2024-05-13 20:41:30.988999 whylogs-1.4.1rc0/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2024-05-13 20:41:30.989496 whylogs-1.4.1rc0/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2024-05-13 20:41:30.990082 whylogs-1.4.1rc0/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2024-05-13 20:41:30.990502 whylogs-1.4.1rc0/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2024-05-13 20:41:30.991128 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2024-05-13 20:41:30.991614 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2024-05-13 20:41:30.992038 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2024-05-13 20:41:30.992470 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2024-05-13 20:41:30.992839 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2024-05-13 20:41:30.993104 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2024-05-13 20:41:30.993447 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2024-05-13 20:41:30.995992 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2024-05-13 20:41:30.997043 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2024-05-13 20:41:30.998284 whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2024-05-13 20:41:30.998658 whylogs-1.4.1rc0/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    22429 2024-05-13 20:41:30.998983 whylogs-1.4.1rc0/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2024-05-13 20:41:30.999513 whylogs-1.4.1rc0/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2024-05-13 20:41:30.999780 whylogs-1.4.1rc0/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2024-05-13 20:41:31.000214 whylogs-1.4.1rc0/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2024-05-13 20:41:31.000477 whylogs-1.4.1rc0/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2024-05-13 20:41:31.000760 whylogs-1.4.1rc0/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1128 2024-05-13 20:41:31.000999 whylogs-1.4.1rc0/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2024-05-13 20:41:31.001387 whylogs-1.4.1rc0/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2024-05-13 20:41:31.001651 whylogs-1.4.1rc0/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     7007 1970-01-01 00:00:00.000000 whylogs-1.4.1rc0/PKG-INFO
+-rw-r--r--   0        0        0     3166 2024-04-11 21:02:51.996289 whylogs-1.4.1rc1/DESCRIPTION.md
+-rw-r--r--   0        0        0     7119 2024-05-21 23:42:09.138510 whylogs-1.4.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     1801 2024-04-11 21:02:52.099792 whylogs-1.4.1rc1/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-11 21:02:52.100033 whylogs-1.4.1rc1/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-11 21:02:52.100189 whylogs-1.4.1rc1/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      168 2024-04-11 21:02:52.100496 whylogs-1.4.1rc1/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2024-04-11 21:02:52.100740 whylogs-1.4.1rc1/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2024-04-11 21:02:52.100900 whylogs-1.4.1rc1/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0    12819 2024-05-16 07:42:59.416851 whylogs-1.4.1rc1/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-11 21:02:52.101645 whylogs-1.4.1rc1/whylogs/api/logger/events/__init__.py
+-rw-r--r--   0        0        0     5621 2024-04-11 21:02:52.101826 whylogs-1.4.1rc1/whylogs/api/logger/events/event.py
+-rw-r--r--   0        0        0      750 2024-04-11 21:02:52.101977 whylogs-1.4.1rc1/whylogs/api/logger/events/file_name.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:02:52.102287 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/__init__.py
+-rw-r--r--   0        0        0     7953 2024-04-11 21:02:52.102648 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/actor.py
+-rw-r--r--   0        0        0     2614 2024-04-11 21:02:52.102874 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/data_logger.py
+-rw-r--r--   0        0        0     1607 2024-04-11 21:02:52.103165 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
+-rw-r--r--   0        0        0     1557 2024-04-11 21:02:52.103449 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/future_util.py
+-rw-r--r--   0        0        0     1282 2024-04-11 21:02:52.103722 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/list_util.py
+-rw-r--r--   0        0        0     1638 2024-04-11 21:02:52.103920 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
+-rw-r--r--   0        0        0     5181 2024-04-11 21:02:52.104087 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py
+-rw-r--r--   0        0        0      281 2024-04-11 21:02:52.104235 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
+-rw-r--r--   0        0        0     5476 2024-04-11 21:02:52.104409 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/process_actor.py
+-rw-r--r--   0        0        0    18881 2024-05-16 07:42:59.418493 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
+-rw-r--r--   0        0        0     9034 2024-05-21 23:21:54.647501 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
+-rw-r--r--   0        0        0      486 2024-04-11 21:02:52.105420 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/signal_util.py
+-rw-r--r--   0        0        0      641 2024-04-11 21:02:52.105565 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/string_util.py
+-rw-r--r--   0        0        0     3010 2024-04-11 21:02:52.105725 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/thread_actor.py
+-rw-r--r--   0        0        0    19662 2024-05-21 23:21:54.648625 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
+-rw-r--r--   0        0        0     4225 2024-04-11 21:02:52.106147 whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/time_util.py
+-rw-r--r--   0        0        0     5777 2024-04-11 21:02:52.106293 whylogs-1.4.1rc1/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    22400 2024-05-16 07:42:59.419284 whylogs-1.4.1rc1/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9549 2024-04-11 21:02:52.106723 whylogs-1.4.1rc1/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2024-04-11 21:02:52.107015 whylogs-1.4.1rc1/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     7090 2024-04-11 21:02:52.107701 whylogs-1.4.1rc1/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2024-04-11 21:02:52.107870 whylogs-1.4.1rc1/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2024-04-11 21:02:52.108209 whylogs-1.4.1rc1/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6178 2024-04-11 21:02:52.108485 whylogs-1.4.1rc1/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7673 2024-04-11 21:02:52.108678 whylogs-1.4.1rc1/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2024-04-11 21:02:52.108971 whylogs-1.4.1rc1/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2024-04-11 21:02:52.109260 whylogs-1.4.1rc1/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2024-04-11 21:02:52.110506 whylogs-1.4.1rc1/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2024-04-11 21:02:52.110752 whylogs-1.4.1rc1/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2024-04-11 21:02:52.111029 whylogs-1.4.1rc1/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2024-04-11 21:02:52.111287 whylogs-1.4.1rc1/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2024-04-11 21:02:52.111509 whylogs-1.4.1rc1/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2024-04-11 21:02:52.111682 whylogs-1.4.1rc1/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2024-04-11 21:02:52.111850 whylogs-1.4.1rc1/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2024-04-11 21:02:52.112362 whylogs-1.4.1rc1/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-11 21:02:52.112764 whylogs-1.4.1rc1/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0    18270 2024-04-11 21:02:52.113056 whylogs-1.4.1rc1/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      354 2024-04-11 21:02:52.113284 whylogs-1.4.1rc1/whylogs/api/whylabs/session/lazy.py
+-rw-r--r--   0        0        0      442 2024-04-11 21:02:52.113497 whylogs-1.4.1rc1/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3893 2024-04-11 21:02:52.113677 whylogs-1.4.1rc1/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0     2823 2024-04-11 21:02:52.114228 whylogs-1.4.1rc1/whylogs/api/whylabs/session/prompts.py
+-rw-r--r--   0        0        0    13613 2024-04-11 21:02:52.114530 whylogs-1.4.1rc1/whylogs/api/whylabs/session/session.py
+-rw-r--r--   0        0        0     6940 2024-04-11 21:02:52.114883 whylogs-1.4.1rc1/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0     5142 2024-04-11 21:02:52.115101 whylogs-1.4.1rc1/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      278 2024-04-11 21:02:52.115260 whylogs-1.4.1rc1/whylogs/api/whylabs/session/why_init.py
+-rw-r--r--   0        0        0     6581 2024-04-11 21:02:52.115444 whylogs-1.4.1rc1/whylogs/api/whylabs/session/whylabs_client_cache.py
+-rw-r--r--   0        0        0      152 2024-05-16 07:42:59.419998 whylogs-1.4.1rc1/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     3498 2024-05-16 07:42:59.420347 whylogs-1.4.1rc1/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     2300 2024-05-16 07:42:59.420658 whylogs-1.4.1rc1/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2421 2024-05-16 07:42:59.420988 whylogs-1.4.1rc1/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     4021 2024-05-16 07:42:59.421326 whylogs-1.4.1rc1/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    11074 2024-05-16 07:42:59.423042 whylogs-1.4.1rc1/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0    10271 2024-05-16 07:42:59.423507 whylogs-1.4.1rc1/whylogs/api/writer/whylabs_base.py
+-rw-r--r--   0        0        0     6668 2024-05-16 07:42:59.423922 whylogs-1.4.1rc1/whylogs/api/writer/whylabs_batch_writer.py
+-rw-r--r--   0        0        0    39735 2024-05-16 07:42:59.424668 whylogs-1.4.1rc1/whylogs/api/writer/whylabs_client.py
+-rw-r--r--   0        0        0     4167 2024-05-16 07:42:59.425199 whylogs-1.4.1rc1/whylogs/api/writer/whylabs_estimation_result_writer.py
+-rw-r--r--   0        0        0     6713 2024-05-16 07:42:59.425706 whylogs-1.4.1rc1/whylogs/api/writer/whylabs_reference_writer.py
+-rw-r--r--   0        0        0     6789 2024-05-16 07:42:59.426170 whylogs-1.4.1rc1/whylogs/api/writer/whylabs_transaction_writer.py
+-rw-r--r--   0        0        0     5420 2024-05-21 23:21:54.649477 whylogs-1.4.1rc1/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:02:52.117572 whylogs-1.4.1rc1/whylogs/context/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-11 21:02:52.117800 whylogs-1.4.1rc1/whylogs/context/environ.py
+-rw-r--r--   0        0        0      516 2024-04-11 21:02:52.118083 whylogs-1.4.1rc1/whylogs/context/version.py
+-rw-r--r--   0        0        0     1090 2024-04-11 21:02:52.118446 whylogs-1.4.1rc1/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3575 2024-04-11 21:02:52.118736 whylogs-1.4.1rc1/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2024-04-11 21:02:52.118979 whylogs-1.4.1rc1/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2024-04-11 21:02:52.119142 whylogs-1.4.1rc1/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2024-04-11 21:02:52.119440 whylogs-1.4.1rc1/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-11 21:02:52.119777 whylogs-1.4.1rc1/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2024-04-11 21:02:52.119935 whylogs-1.4.1rc1/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2024-04-11 21:02:52.120128 whylogs-1.4.1rc1/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2024-04-11 21:02:52.120301 whylogs-1.4.1rc1/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2024-04-11 21:02:52.121115 whylogs-1.4.1rc1/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2024-04-11 21:02:52.121340 whylogs-1.4.1rc1/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2024-04-11 21:02:52.121557 whylogs-1.4.1rc1/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2024-04-11 21:02:52.121785 whylogs-1.4.1rc1/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30661 2024-04-11 21:02:52.122160 whylogs-1.4.1rc1/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11229 2024-05-21 23:27:59.505123 whylogs-1.4.1rc1/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4230 2024-04-11 21:02:52.122660 whylogs-1.4.1rc1/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2024-04-11 21:02:52.123977 whylogs-1.4.1rc1/whylogs/core/errors.py
+-rw-r--r--   0        0        0     1453 2024-05-16 07:42:59.428606 whylogs-1.4.1rc1/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2024-04-11 21:02:52.125463 whylogs-1.4.1rc1/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     2987 2024-04-11 21:02:52.125665 whylogs-1.4.1rc1/whylogs/core/metadata.py
+-rw-r--r--   0        0        0     1740 2024-04-11 21:02:52.126366 whylogs-1.4.1rc1/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2024-04-11 21:02:52.127504 whylogs-1.4.1rc1/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2024-04-11 21:02:52.127717 whylogs-1.4.1rc1/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2024-04-11 21:02:52.127909 whylogs-1.4.1rc1/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2024-04-11 21:02:52.129091 whylogs-1.4.1rc1/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0    10678 2024-04-26 01:28:37.524869 whylogs-1.4.1rc1/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2024-04-11 21:02:52.129579 whylogs-1.4.1rc1/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2024-04-11 21:02:52.129866 whylogs-1.4.1rc1/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2024-04-11 21:02:52.130125 whylogs-1.4.1rc1/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2024-04-11 21:02:52.130379 whylogs-1.4.1rc1/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2024-04-11 21:02:52.130789 whylogs-1.4.1rc1/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2024-04-11 21:02:52.131027 whylogs-1.4.1rc1/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2024-04-11 21:02:52.131252 whylogs-1.4.1rc1/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2024-04-11 21:02:52.132284 whylogs-1.4.1rc1/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2024-04-11 21:02:52.132722 whylogs-1.4.1rc1/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0    10663 2024-04-11 21:02:52.133689 whylogs-1.4.1rc1/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2024-04-11 21:02:52.134251 whylogs-1.4.1rc1/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2024-04-11 21:02:52.135503 whylogs-1.4.1rc1/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2024-04-11 21:02:52.135812 whylogs-1.4.1rc1/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14608 2024-04-11 21:02:52.136251 whylogs-1.4.1rc1/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2024-04-11 21:02:52.136562 whylogs-1.4.1rc1/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2024-04-11 21:02:52.136960 whylogs-1.4.1rc1/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2024-04-11 21:02:52.137355 whylogs-1.4.1rc1/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2024-05-21 23:47:15.751542 whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2024-05-21 23:47:14.216585 whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2024-05-21 23:47:14.219097 whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2024-05-21 23:47:14.221990 whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2024-05-21 23:47:16.021869 whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2024-05-21 23:47:14.227994 whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2024-05-21 23:47:13.874034 whylogs-1.4.1rc1/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2024-05-21 23:47:13.878712 whylogs-1.4.1rc1/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2024-04-11 21:02:52.137664 whylogs-1.4.1rc1/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11357 2024-04-11 21:02:52.138004 whylogs-1.4.1rc1/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10754 2024-04-11 21:02:52.140974 whylogs-1.4.1rc1/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2024-04-11 21:02:52.141687 whylogs-1.4.1rc1/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2024-04-11 21:02:52.143908 whylogs-1.4.1rc1/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2024-04-11 21:02:52.144274 whylogs-1.4.1rc1/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2118 2024-04-11 21:02:52.144526 whylogs-1.4.1rc1/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2024-04-11 21:02:52.144959 whylogs-1.4.1rc1/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2024-04-11 21:02:52.145154 whylogs-1.4.1rc1/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2024-04-11 21:02:52.145361 whylogs-1.4.1rc1/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2024-04-11 21:02:52.145527 whylogs-1.4.1rc1/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     2004 2024-04-11 21:02:52.145770 whylogs-1.4.1rc1/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      281 2024-04-11 21:02:52.146156 whylogs-1.4.1rc1/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4823 2024-04-11 21:02:52.146373 whylogs-1.4.1rc1/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1329 2024-04-11 21:02:52.147148 whylogs-1.4.1rc1/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2024-04-11 21:02:52.147632 whylogs-1.4.1rc1/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2024-04-11 21:02:52.148350 whylogs-1.4.1rc1/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    18798 2024-05-21 23:27:59.507308 whylogs-1.4.1rc1/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     9474 2024-05-16 07:42:59.430700 whylogs-1.4.1rc1/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2024-04-11 21:02:52.149478 whylogs-1.4.1rc1/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2024-04-11 21:02:52.149719 whylogs-1.4.1rc1/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2024-04-11 21:02:52.149974 whylogs-1.4.1rc1/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:02:52.150210 whylogs-1.4.1rc1/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2024-04-11 21:02:52.150544 whylogs-1.4.1rc1/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2024-04-11 21:02:52.150872 whylogs-1.4.1rc1/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2024-04-11 21:02:52.151178 whylogs-1.4.1rc1/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2024-04-11 21:02:52.151905 whylogs-1.4.1rc1/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2024-04-11 21:02:52.152680 whylogs-1.4.1rc1/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2024-04-11 21:02:52.152944 whylogs-1.4.1rc1/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2024-04-11 21:02:52.153348 whylogs-1.4.1rc1/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:02:52.153646 whylogs-1.4.1rc1/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 01:28:37.524993 whylogs-1.4.1rc1/whylogs/experimental/api/__init__.py
+-rw-r--r--   0        0        0    16453 2024-05-07 23:42:41.683380 whylogs-1.4.1rc1/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2024-04-11 21:02:52.154570 whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-11 21:02:52.154816 whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2024-04-11 21:02:52.155022 whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2024-04-11 21:02:52.155229 whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2024-04-11 21:02:52.155470 whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2024-04-11 21:02:52.155723 whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2024-04-11 21:02:52.155908 whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2024-04-11 21:02:52.156922 whylogs-1.4.1rc1/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    19154 2024-04-11 21:02:52.157141 whylogs-1.4.1rc1/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0      299 2024-04-11 21:02:52.157369 whylogs-1.4.1rc1/whylogs/experimental/core/validators/__init__.py
+-rw-r--r--   0        0        0     1218 2024-04-11 21:02:52.157508 whylogs-1.4.1rc1/whylogs/experimental/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1698 2024-04-11 21:02:52.157648 whylogs-1.4.1rc1/whylogs/experimental/core/validators/validator.py
+-rw-r--r--   0        0        0     8861 2024-04-11 21:02:52.157896 whylogs-1.4.1rc1/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2024-04-11 21:02:52.158035 whylogs-1.4.1rc1/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2024-04-11 21:02:52.158226 whylogs-1.4.1rc1/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:02:52.158368 whylogs-1.4.1rc1/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1369 2024-05-16 07:42:59.431270 whylogs-1.4.1rc1/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2024-04-11 21:02:52.158722 whylogs-1.4.1rc1/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2024-04-11 21:02:52.159649 whylogs-1.4.1rc1/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    11126 2024-04-11 21:02:52.160469 whylogs-1.4.1rc1/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2024-04-11 21:02:52.160808 whylogs-1.4.1rc1/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15564 2024-04-11 21:02:52.161050 whylogs-1.4.1rc1/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     7662 2024-04-11 21:02:52.161208 whylogs-1.4.1rc1/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2024-04-11 21:02:52.161403 whylogs-1.4.1rc1/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-11 21:02:52.161540 whylogs-1.4.1rc1/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:02:52.161723 whylogs-1.4.1rc1/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    22069 2024-04-11 21:02:52.161960 whylogs-1.4.1rc1/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2024-04-11 21:02:52.162196 whylogs-1.4.1rc1/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:02:52.162396 whylogs-1.4.1rc1/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-11 21:02:52.162629 whylogs-1.4.1rc1/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:02:52.162802 whylogs-1.4.1rc1/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-11 21:02:52.163678 whylogs-1.4.1rc1/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2024-04-11 21:02:52.163933 whylogs-1.4.1rc1/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2221 2024-05-16 07:42:59.431737 whylogs-1.4.1rc1/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2024-04-11 21:02:52.164906 whylogs-1.4.1rc1/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2024-04-11 21:02:52.165085 whylogs-1.4.1rc1/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2024-04-11 21:02:52.165339 whylogs-1.4.1rc1/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2024-04-11 21:02:52.165478 whylogs-1.4.1rc1/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2024-04-11 21:02:52.165838 whylogs-1.4.1rc1/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2024-04-11 21:02:52.166593 whylogs-1.4.1rc1/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2024-04-11 21:02:52.168136 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2024-04-11 21:02:52.168490 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2024-04-11 21:02:52.168687 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2024-04-11 21:02:52.169624 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2024-04-11 21:02:52.169949 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2024-04-11 21:02:52.170134 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2024-04-11 21:02:52.170582 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2024-04-11 21:02:52.170953 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2024-04-11 21:02:52.171191 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2024-04-11 21:02:52.171626 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2024-04-11 21:02:52.171939 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2024-04-11 21:02:52.172133 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2024-04-11 21:02:52.172603 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2024-04-11 21:02:52.172910 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2024-04-11 21:02:52.173890 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2024-04-11 21:02:52.174468 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2024-04-11 21:02:52.176028 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2024-04-11 21:02:52.176280 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2024-04-11 21:02:52.176721 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2024-04-11 21:02:52.177078 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2024-04-11 21:02:52.177314 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2024-04-11 21:02:52.177836 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2024-04-11 21:02:52.178131 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2024-04-11 21:02:52.178353 whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2024-04-11 21:02:52.178688 whylogs-1.4.1rc1/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2024-04-11 21:02:52.178902 whylogs-1.4.1rc1/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2024-04-11 21:02:52.179771 whylogs-1.4.1rc1/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2024-04-11 21:02:52.180020 whylogs-1.4.1rc1/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2024-04-11 21:02:52.180379 whylogs-1.4.1rc1/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2024-04-11 21:02:52.181420 whylogs-1.4.1rc1/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2024-04-11 21:02:52.181808 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2024-04-11 21:02:52.182143 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2024-04-11 21:02:52.182536 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2024-04-11 21:02:52.182775 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2024-04-11 21:02:52.182984 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2024-04-11 21:02:52.183188 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2024-04-11 21:02:52.183395 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2024-04-11 21:02:52.185298 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2024-04-11 21:02:52.185999 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2024-04-11 21:02:52.186659 whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2024-04-11 21:02:52.186889 whylogs-1.4.1rc1/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    22429 2024-04-11 21:02:52.187060 whylogs-1.4.1rc1/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2024-04-11 21:02:52.187359 whylogs-1.4.1rc1/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2024-04-11 21:02:52.187524 whylogs-1.4.1rc1/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2024-04-11 21:02:52.188219 whylogs-1.4.1rc1/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2024-04-11 21:02:52.188363 whylogs-1.4.1rc1/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2024-04-11 21:02:52.188532 whylogs-1.4.1rc1/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1128 2024-04-11 21:02:52.188710 whylogs-1.4.1rc1/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2024-04-11 21:02:52.188935 whylogs-1.4.1rc1/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2024-04-11 21:02:52.189084 whylogs-1.4.1rc1/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     7007 1970-01-01 00:00:00.000000 whylogs-1.4.1rc1/PKG-INFO
```

### Comparing `whylogs-1.4.1rc0/DESCRIPTION.md` & `whylogs-1.4.1rc1/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/pyproject.toml` & `whylogs-1.4.1rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.4.1-rc0"
+version = "1.4.1-rc1"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
 
@@ -175,14 +175,15 @@
 ipykernel = ">=6.11" # for developing in Jupyter notebook
 types-python-dateutil = "^2.8.12"
 moto = "^4.1.6"
 twine = "^4.0.1"
 gcp-storage-emulator = "^2022.6.11"
 types-urllib3 = "^1.26.25.5"
 pyright = "^1.1.338"
+ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
@@ -258,20 +259,40 @@
     | _build
     | buck-out
     | build
     | dist
     | tests
     | whylogs/core/proto
     | docs
+    | whylogs/api/logger/experimental/logger
   )/
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
 
 [tool.pyright]
 include = ["whylogs/api/logger/experimental/logger/**/*.py"]
 typeCheckingMode = "strict"
 
 reportMissingTypeStubs = false
 reportMissingParameterType = false
 reportMissingTypeArgumet = false
+
+[tool.ruff]
+line-length = 140
+indent-width = 4
+include = ["whylogs/api/logger/experimental/logger/**/*.py"]
+select = ["E", "F", "I", "W"]
+
+[tool.ruff.isort]
+known-first-party = ["whylogs"]
+
+[tool.ruff.lint]
+fixable = ["ALL"]
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+[tool.ruff.format]
+quote-style = "double"
+indent-style = "space"
+skip-magic-trailing-comma = false
+line-ending = "auto"
```

### Comparing `whylogs-1.4.1rc0/whylogs/__init__.py` & `whylogs-1.4.1rc1/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/annotations.py` & `whylogs-1.4.1rc1/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/fugue/profiler.py` & `whylogs-1.4.1rc1/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/fugue/registry.py` & `whylogs-1.4.1rc1/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/__init__.py` & `whylogs-1.4.1rc1/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/events/event.py` & `whylogs-1.4.1rc1/whylogs/api/logger/events/event.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/events/file_name.py` & `whylogs-1.4.1rc1/whylogs/api/logger/events/file_name.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/actor.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/data_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/future_util.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/future_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/list_util.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/list_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/process_actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 some issue deserializing or validating.
 """
 import sys
 
 if sys.version_info >= (3, 8):
     from typing import Protocol, TypedDict  # pylint: disable=no-name-in-module
 else:
-    from typing_extensions import TypedDict, Protocol
+    from typing_extensions import Protocol, TypedDict
 
 import base64
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 from whylogs.api.logger.experimental.logger.actor.thread_rolling_logger import (
     LoggerStatus,
```

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/string_util.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/string_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/thread_actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,19 +64,30 @@
     def _track_segments(self, data: TrackData) -> None:
         if self._schema is None:
             raise Exception("Schema missing in logger while using segments")
 
         if not isinstance(self._target, SegmentCache):
             raise Exception("Segment cache missing in logger while using segments")
 
-        if isinstance(data, List):
-            for row in data:
+        if self._schema:
+            if isinstance(data, List):
+                input_data = [self._schema._run_udfs(pandas=None, row=it)[1] for it in data]  # pyright: ignore[reportPrivateUsage, reportUnknownMemberType]
+            else:
+                df = data if isinstance(data, pd.DataFrame) else None
+                row = data if isinstance(data, dict) else None
+                df, row = self._schema._run_udfs(df, row)  # pyright: ignore[reportUnknownVariableType, reportUnknownMemberType, reportPrivateUsage]
+                input_data: TrackData = cast(TrackData, df if df is not None else row)
+        else:
+            input_data = data
+
+        if isinstance(input_data, List):
+            for row in input_data:
                 segment_processing(self._schema, row=row, segment_cache=self._target)
         else:
-            segment_processing(self._schema, data, segment_cache=self._target)
+            segment_processing(self._schema, input_data, segment_cache=self._target)
 
     def _track_profile(self, data: TrackData) -> None:
         if not isinstance(self._target, DatasetProfile):
             raise Exception("Dataset profile missing in logger")
 
         if isinstance(data, List):
             for row in data:
@@ -257,17 +268,15 @@
                 raise Exception("Minimum write schedule is five minutes.")
 
             if write_schedule.cadence == TimeGranularity.Minute and write_schedule.interval < 5:
                 raise Exception("Minimum write schedule is five minutes.")
 
             self._timer = FunctionTimer(write_schedule, self.flush)
         else:
-            self._logger.warning(
-                "No write schedule defined for logger. Profiles will only be written after calls to flush()."
-            )
+            self._logger.warning("No write schedule defined for logger. Profiles will only be written after calls to flush().")
 
         self._logger.debug(f"Created thread logger, pid {os.getpid()}")
 
     def process_batch(self, batch: List[LoggerMessage], batch_type: Type[LoggerMessage]) -> None:
         if batch_type == TrackMessage:
             self._process_track_messages(cast(List[TrackMessage], batch))
         elif batch_type == FlushMessage:
@@ -447,15 +456,21 @@
             sync: Whether or not to perform this action synchronously. By default, this is an asynchronous operation.
                 You can make this synchronous in order to react to errors. Mostly useful when initially setting up
                 logging since the only errors that can be responded to are data format related.
         """
         self._validate_data(data)
 
         result: Optional["Future[None]"] = Future() if sync else None
-        self.send(TrackMessage(data=data, timestamp_ms=timestamp_ms or self.current_time_ms(), result=result))
+        self.send(
+            TrackMessage(
+                data=data,
+                timestamp_ms=timestamp_ms or self.current_time_ms(),
+                result=result,
+            )
+        )
         if result is not None:
             self._logger.debug("Waiting for track to complete")
             wait_result(result)
 
     def flush(self) -> None:
         """
         Flush the internal state, causing everything to be written using the configured writers.
```

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/experimental/logger/actor/time_util.py` & `whylogs-1.4.1rc1/whylogs/api/logger/experimental/logger/actor/time_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/logger.py` & `whylogs-1.4.1rc1/whylogs/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/result_set.py` & `whylogs-1.4.1rc1/whylogs/api/logger/result_set.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/rolling.py` & `whylogs-1.4.1rc1/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/segment_cache.py` & `whylogs-1.4.1rc1/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/segment_processing.py` & `whylogs-1.4.1rc1/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/logger/transient.py` & `whylogs-1.4.1rc1/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.4.1rc1/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.4.1rc1/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/reader/local.py` & `whylogs-1.4.1rc1/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/reader/reader.py` & `whylogs-1.4.1rc1/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/reader/s3.py` & `whylogs-1.4.1rc1/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/store/local_store.py` & `whylogs-1.4.1rc1/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/store/profile_store.py` & `whylogs-1.4.1rc1/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/store/query.py` & `whylogs-1.4.1rc1/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/store/sqlite_store.py` & `whylogs-1.4.1rc1/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/usage_stats/__init__.py` & `whylogs-1.4.1rc1/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/whylabs/session/config.py` & `whylogs-1.4.1rc1/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.4.1rc1/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/whylabs/session/prompts.py` & `whylogs-1.4.1rc1/whylogs/api/whylabs/session/prompts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/whylabs/session/session.py` & `whylogs-1.4.1rc1/whylogs/api/whylabs/session/session.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.4.1rc1/whylogs/api/whylabs/session/session_manager.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.4.1rc1/whylogs/api/whylabs/session/session_types.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/whylabs/session/whylabs_client_cache.py` & `whylogs-1.4.1rc1/whylogs/api/whylabs/session/whylabs_client_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/gcs.py` & `whylogs-1.4.1rc1/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/local.py` & `whylogs-1.4.1rc1/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/mlflow.py` & `whylogs-1.4.1rc1/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/s3.py` & `whylogs-1.4.1rc1/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/whylabs.py` & `whylogs-1.4.1rc1/whylogs/api/writer/whylabs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_base.py` & `whylogs-1.4.1rc1/whylogs/api/writer/whylabs_base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_batch_writer.py` & `whylogs-1.4.1rc1/whylogs/api/writer/whylabs_batch_writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_client.py` & `whylogs-1.4.1rc1/whylogs/api/writer/whylabs_client.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_estimation_result_writer.py` & `whylogs-1.4.1rc1/whylogs/api/writer/whylabs_estimation_result_writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_reference_writer.py` & `whylogs-1.4.1rc1/whylogs/api/writer/whylabs_reference_writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/whylabs_transaction_writer.py` & `whylogs-1.4.1rc1/whylogs/api/writer/whylabs_transaction_writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/api/writer/writer.py` & `whylogs-1.4.1rc1/whylogs/api/writer/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         except FileExistsError:
             pass
         return open(path, f"w{mode}")
 
     @abstractmethod
     def _get_default_filename(self) -> str:
         """Returns filename to write if None passed to Writable::write()"""
-        pass
 
     def _get_default_path(self) -> Optional[str]:
         """
         Returns the default path to write to, excluding filename(s). None = use CWD
         """
         return os.getcwd()
```

### Comparing `whylogs-1.4.1rc0/whylogs/context/version.py` & `whylogs-1.4.1rc1/whylogs/context/version.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/__init__.py` & `whylogs-1.4.1rc1/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/column_profile.py` & `whylogs-1.4.1rc1/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/configs.py` & `whylogs-1.4.1rc1/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.4.1rc1/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/dataset_profile.py` & `whylogs-1.4.1rc1/whylogs/core/dataset_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from whylogs.api.writer.writer import Writable
 from whylogs.core.metrics import Metric
 from whylogs.core.model_performance_metrics.model_performance_metrics import (
     ModelPerformanceMetrics,
 )
 from whylogs.core.preprocessing import ColumnProperties
-from whylogs.core.utils.utils import deprecated_alias
+from whylogs.core.utils.utils import deprecated_alias, ensure_timezone
 
 from .column_profile import ColumnProfile
 from .input_resolver import _pandas_or_dict
 from .schema import DatasetSchema
 from .stubs import pd
 from .view import DatasetProfileView
 
@@ -80,17 +80,15 @@
         return self._track_count == 0
 
     @property
     def metadata(self) -> Dict[str, str]:
         return self._metadata
 
     def set_dataset_timestamp(self, dataset_timestamp: datetime) -> None:
-        if dataset_timestamp.tzinfo is None:
-            logger.warning("No timezone set in the datetime_timestamp object. Default to local timezone")
-
+        ensure_timezone(dataset_timestamp)
         self._dataset_timestamp = dataset_timestamp.astimezone(tz=timezone.utc)
 
     def add_metric(self, col_name: str, metric: Metric) -> None:
         if col_name not in self._columns:
             raise ValueError(f"{col_name} is not a column in the dataset profile")
         self._columns[col_name].add_metric(metric)
```

### Comparing `whylogs-1.4.1rc0/whylogs/core/datatypes.py` & `whylogs-1.4.1rc1/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/errors.py` & `whylogs-1.4.1rc1/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/feature_weights.py` & `whylogs-1.4.1rc1/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/input_resolver.py` & `whylogs-1.4.1rc1/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metadata.py` & `whylogs-1.4.1rc1/whylogs/core/metadata.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metric_getters.py` & `whylogs-1.4.1rc1/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/__init__.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/aggregators.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/column_metrics.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/compound_metric.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/decorators.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/deserializers.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/maths.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/metric_components.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/metrics.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/multimetric.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/serializers.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/metrics/unicode_range.py` & `whylogs-1.4.1rc1/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.4.1rc1/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.4.1rc1/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.4.1rc1/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/predicate_parser.py` & `whylogs-1.4.1rc1/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/preprocessing.py` & `whylogs-1.4.1rc1/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.4.1rc1/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.4.1rc1/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.4.1rc1/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/relations.py` & `whylogs-1.4.1rc1/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/resolvers.py` & `whylogs-1.4.1rc1/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/schema.py` & `whylogs-1.4.1rc1/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/segmentation_partition.py` & `whylogs-1.4.1rc1/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/specialized_resolvers.py` & `whylogs-1.4.1rc1/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/stubs.py` & `whylogs-1.4.1rc1/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.4.1rc1/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/utils/stats_calculations.py` & `whylogs-1.4.1rc1/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/utils/utils.py` & `whylogs-1.4.1rc1/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/validators/condition_validator.py` & `whylogs-1.4.1rc1/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/validators/validator.py` & `whylogs-1.4.1rc1/whylogs/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/view/column_profile_view.py` & `whylogs-1.4.1rc1/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.4.1rc1/whylogs/core/view/dataset_profile_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,18 @@
         return self._dataset_timestamp
 
     @dataset_timestamp.setter
     def dataset_timestamp(self, date: datetime) -> "DatasetProfileView":
         self._dataset_timestamp = date
         return self
 
+    def set_dataset_timestamp(self, dataset_timestamp: datetime) -> None:
+        ensure_timezone(dataset_timestamp)
+        self._dataset_timestamp = dataset_timestamp.astimezone(tz=timezone.utc)
+
     @property
     def creation_timestamp(self) -> Optional[datetime]:
         return self._creation_timestamp
 
     @property
     def metadata(self) -> Dict[str, str]:
         return self._metadata
```

### Comparing `whylogs-1.4.1rc0/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.4.1rc1/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/base.py` & `whylogs-1.4.1rc1/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/configs.py` & `whylogs-1.4.1rc1/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.4.1rc1/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/descr/employee.rst` & `whylogs-1.4.1rc1/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/descr/weather.rst` & `whylogs-1.4.1rc1/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/ecommerce.py` & `whylogs-1.4.1rc1/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/employee.py` & `whylogs-1.4.1rc1/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/utils.py` & `whylogs-1.4.1rc1/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/datasets/weather.py` & `whylogs-1.4.1rc1/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/api/logger/__init__.py` & `whylogs-1.4.1rc1/whylogs/experimental/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.4.1rc1/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.4.1rc1/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/core/udf_schema.py` & `whylogs-1.4.1rc1/whylogs/experimental/core/udf_schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/core/validators/condition_validator.py` & `whylogs-1.4.1rc1/whylogs/experimental/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/core/validators/validator.py` & `whylogs-1.4.1rc1/whylogs/experimental/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.4.1rc1/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.4.1rc1/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.4.1rc1/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.4.1rc1/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.4.1rc1/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.4.1rc1/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/extras/image_metric.py` & `whylogs-1.4.1rc1/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/migration/converters.py` & `whylogs-1.4.1rc1/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/migration/uncompound.py` & `whylogs-1.4.1rc1/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.4.1rc1/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/drift/configs.py` & `whylogs-1.4.1rc1/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/enums/enums.py` & `whylogs-1.4.1rc1/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.4.1rc1/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.4.1rc1/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.4.1rc1/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.4.1rc1/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.4.1rc1/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.4.1rc1/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.4.1rc1/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.4.1rc1/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/js/d3.min.js` & `whylogs-1.4.1rc1/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/js/handlebars.js` & `whylogs-1.4.1rc1/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.4.1rc1/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.4.1rc1/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/html/templates/index.html` & `whylogs-1.4.1rc1/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.4.1rc1/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.4.1rc1/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.4.1rc1/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.4.1rc1/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.4.1rc1/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.4.1rc1/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.4.1rc1/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.4.1rc1/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.1rc0/PKG-INFO` & `whylogs-1.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.4.1rc0
+Version: 1.4.1rc1
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

