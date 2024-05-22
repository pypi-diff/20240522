# Comparing `tmp/nextline-0.7.5.tar.gz` & `tmp/nextline-0.7.6.tar.gz`

## Comparing `nextline-0.7.5.tar` & `nextline-0.7.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/__about__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/__init__.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/continuous.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/count.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/disable.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/events.py
--rw-r--r--   0        0        0     9959 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/py.typed
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/types.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/fsm/__init__.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/fsm/factory.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/fsm/state.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/__init__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/hook.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/spec.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/argument.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/__init__.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/prompt_info.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/prompt_notice.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/run_info.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/run_no.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/script.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/state_name.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/stdout.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/trace_info.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/registrars/trace_nos.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/session/__init__.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/session/monitor.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/plugin/plugins/session/session.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/__init__.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/call.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/commands.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/exc.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/path.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/runner.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/types.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/utils.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/hook.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/skip.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/spec.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/__init__.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/_script.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/compose.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/concurrency.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/filter.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/global_.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/local_.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/peek.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/repeat.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/__init__.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/custom.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/factory.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/prompt.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/stream.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/__init__.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/func.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/multiprocessing_logging.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/path.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/peek.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/profile.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/queue.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/run.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/thread_exception.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/thread_task_id.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/timer.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/done_callback/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/done_callback/task.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/done_callback/thread.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/done_callback/union.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/pubsub/__init__.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/pubsub/broker.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 nextline-0.7.5/nextline/utils/pubsub/item.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 nextline-0.7.5/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline-0.7.5/LICENSE
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 nextline-0.7.5/README.md
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 nextline-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 nextline-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/__about__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/__init__.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/continuous.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/count.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/disable.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/events.py
+-rw-r--r--   0        0        0     9959 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/py.typed
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/types.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/fsm/__init__.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/fsm/factory.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/fsm/state.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/__init__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/hook.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/spec.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/argument.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/__init__.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/prompt_info.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/prompt_notice.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/run_info.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/run_no.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/script.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/state_name.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/stdout.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/trace_info.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/registrars/trace_nos.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/session/__init__.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/session/monitor.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/plugin/plugins/session/session.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/__init__.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/call.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/commands.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/exc.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/path.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/runner.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/types.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/utils.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/hook.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/skip.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/spec.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/__init__.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/_script.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/compose.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/concurrency.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/filter.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/global_.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/local_.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/peek.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/repeat.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/__init__.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/custom.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/factory.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/prompt.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/stream.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/__init__.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/func.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/multiprocessing_logging.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/path.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/peek.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/profile.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/queue.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/run.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/thread_exception.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/thread_task_id.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/timer.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/done_callback/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/done_callback/task.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/done_callback/thread.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/done_callback/union.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/pubsub/__init__.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/pubsub/broker.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 nextline-0.7.6/nextline/utils/pubsub/item.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 nextline-0.7.6/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline-0.7.6/LICENSE
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 nextline-0.7.6/README.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 nextline-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 nextline-0.7.6/PKG-INFO
```

### Comparing `nextline-0.7.5/nextline/continuous.py` & `nextline-0.7.6/nextline/continuous.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/count.py` & `nextline-0.7.6/nextline/count.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/events.py` & `nextline-0.7.6/nextline/events.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/main.py` & `nextline-0.7.6/nextline/main.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/types.py` & `nextline-0.7.6/nextline/types.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/fsm/factory.py` & `nextline-0.7.6/nextline/fsm/factory.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/fsm/state.py` & `nextline-0.7.6/nextline/fsm/state.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/hook.py` & `nextline-0.7.6/nextline/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/spec.py` & `nextline-0.7.6/nextline/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/__init__.py` & `nextline-0.7.6/nextline/plugin/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/argument.py` & `nextline-0.7.6/nextline/plugin/plugins/argument.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/registrars/__init__.py` & `nextline-0.7.6/nextline/plugin/plugins/registrars/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/registrars/prompt_info.py` & `nextline-0.7.6/nextline/plugin/plugins/registrars/prompt_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/registrars/prompt_notice.py` & `nextline-0.7.6/nextline/plugin/plugins/registrars/prompt_notice.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/registrars/run_info.py` & `nextline-0.7.6/nextline/plugin/plugins/registrars/run_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/registrars/stdout.py` & `nextline-0.7.6/nextline/plugin/plugins/registrars/stdout.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/registrars/trace_info.py` & `nextline-0.7.6/nextline/plugin/plugins/registrars/trace_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/registrars/trace_nos.py` & `nextline-0.7.6/nextline/plugin/plugins/registrars/trace_nos.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/session/monitor.py` & `nextline-0.7.6/nextline/plugin/plugins/session/monitor.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/plugin/plugins/session/session.py` & `nextline-0.7.6/nextline/plugin/plugins/session/session.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/__init__.py` & `nextline-0.7.6/nextline/spawned/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/call.py` & `nextline-0.7.6/nextline/spawned/call.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/path.py` & `nextline-0.7.6/nextline/spawned/path.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/runner.py` & `nextline-0.7.6/nextline/spawned/runner.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/types.py` & `nextline-0.7.6/nextline/spawned/types.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/utils.py` & `nextline-0.7.6/nextline/spawned/utils.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/hook.py` & `nextline-0.7.6/nextline/spawned/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/skip.py` & `nextline-0.7.6/nextline/spawned/plugin/skip.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/spec.py` & `nextline-0.7.6/nextline/spawned/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/__init__.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/_script.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/_script.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/compose.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/compose.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/concurrency.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/concurrency.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/filter.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/filter.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/global_.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/global_.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/local_.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/local_.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/peek.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/peek.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/repeat.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/repeat.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/custom.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/custom.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/factory.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/factory.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/prompt.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/prompt.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/spawned/plugin/plugins/pdb_/stream.py` & `nextline-0.7.6/nextline/spawned/plugin/plugins/pdb_/stream.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/__init__.py` & `nextline-0.7.6/nextline/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/func.py` & `nextline-0.7.6/nextline/utils/func.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/multiprocessing_logging.py` & `nextline-0.7.6/nextline/utils/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/peek.py` & `nextline-0.7.6/nextline/utils/peek.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/queue.py` & `nextline-0.7.6/nextline/utils/queue.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/run.py` & `nextline-0.7.6/nextline/utils/run.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/thread_exception.py` & `nextline-0.7.6/nextline/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/thread_task_id.py` & `nextline-0.7.6/nextline/utils/thread_task_id.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/timer.py` & `nextline-0.7.6/nextline/utils/timer.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/done_callback/task.py` & `nextline-0.7.6/nextline/utils/done_callback/task.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/done_callback/thread.py` & `nextline-0.7.6/nextline/utils/done_callback/thread.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/done_callback/union.py` & `nextline-0.7.6/nextline/utils/done_callback/union.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/pubsub/broker.py` & `nextline-0.7.6/nextline/utils/pubsub/broker.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/nextline/utils/pubsub/item.py` & `nextline-0.7.6/nextline/utils/pubsub/item.py`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/.gitignore` & `nextline-0.7.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/LICENSE` & `nextline-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nextline-0.7.5/README.md` & `nextline-0.7.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,19 @@
+# Nextline
+
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline.svg)](https://pypi.org/project/nextline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline.svg)](https://pypi.org/project/nextline)
+
 [![Test Status](https://github.com/simonsobs/nextline/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/nextline/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline)
 
-# Nextline
+---
 
 _Nextline_ is a DAQ sequencer of the [Observatory Control System
 (OCS)](https://github.com/simonsobs/ocs/). Nextline allows line-by-line
 execution of concurrent Python scripts, which control telescopes, by multiple
 users simultaneously from web browsers.
 
 This package provides the core functionality of Nextline. It is used in
 [_nextline-graphql_](https://github.com/simonsobs/nextline-graphql), the
 plugin-based framework of the backend API server of Nextline.
-
-## License
-
-- _Nextline_ is licensed under the MIT license.
-
----
-
-## Contact
-
-- [Tai Sakuma](https://github.com/TaiSakuma) <span itemscope itemtype="https://schema.org/Person"><a itemprop="sameAs" content="https://orcid.org/0000-0003-3225-9861" href="https://orcid.org/0000-0003-3225-9861" target="orcid.widget" rel="me noopener noreferrer" style="vertical-align:text-top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a></span>
```

### Comparing `nextline-0.7.5/pyproject.toml` & `nextline-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "apluggy>=0.9",
+    "apluggy>=1.0",
     "exceptiongroup>=1.2",
     "transitions>=0.9",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "isort", "flake8", "mypy", "tox", "twine"]
```

### Comparing `nextline-0.7.5/PKG-INFO` & `nextline-0.7.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextline
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Python library for controlling Python scripts execution
 Project-URL: Homepage, https://github.com/simonsobs/nextline#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline/issues
 Project-URL: Source, https://github.com/simonsobs/nextline
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
-Requires-Dist: apluggy>=0.9
+Requires-Dist: apluggy>=1.0
 Requires-Dist: exceptiongroup>=1.2
 Requires-Dist: transitions>=0.9
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
@@ -30,33 +30,26 @@
 Requires-Dist: hypothesis>=6.65; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.18; extra == 'tests'
 Requires-Dist: pytest-cov>=3.0; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.1; extra == 'tests'
 Requires-Dist: pytest>=7.0; extra == 'tests'
 Description-Content-Type: text/markdown
 
+# Nextline
+
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline.svg)](https://pypi.org/project/nextline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline.svg)](https://pypi.org/project/nextline)
+
 [![Test Status](https://github.com/simonsobs/nextline/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/nextline/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline)
 
-# Nextline
+---
 
 _Nextline_ is a DAQ sequencer of the [Observatory Control System
 (OCS)](https://github.com/simonsobs/ocs/). Nextline allows line-by-line
 execution of concurrent Python scripts, which control telescopes, by multiple
 users simultaneously from web browsers.
 
 This package provides the core functionality of Nextline. It is used in
 [_nextline-graphql_](https://github.com/simonsobs/nextline-graphql), the
 plugin-based framework of the backend API server of Nextline.
-
-## License
-
-- _Nextline_ is licensed under the MIT license.
-
----
-
-## Contact
-
-- [Tai Sakuma](https://github.com/TaiSakuma) <span itemscope itemtype="https://schema.org/Person"><a itemprop="sameAs" content="https://orcid.org/0000-0003-3225-9861" href="https://orcid.org/0000-0003-3225-9861" target="orcid.widget" rel="me noopener noreferrer" style="vertical-align:text-top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a></span>
```

