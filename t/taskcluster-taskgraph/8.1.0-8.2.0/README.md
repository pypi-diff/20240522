# Comparing `tmp/taskcluster-taskgraph-8.1.0.tar.gz` & `tmp/taskcluster-taskgraph-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-8.1.0.tar", last modified: Thu May  9 00:03:30 2024, max compression
+gzip compressed data, was "taskcluster-taskgraph-8.2.0.tar", last modified: Wed May 22 15:46:21 2024, max compression
```

## Comparing `taskcluster-taskgraph-8.1.0.tar` & `taskcluster-taskgraph-8.2.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.164743 taskcluster-taskgraph-8.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-09 00:03:30.164743 taskcluster-taskgraph-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.148743 taskcluster-taskgraph-8.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:03:30.164743 taskcluster-taskgraph-8.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.144743 taskcluster-taskgraph-8.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.148743 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.148743 taskcluster-taskgraph-8.1.0/src/taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/filter_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/loader/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/loader/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    29171 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/morph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20107 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/
--rwxr-xr-x   0 runner    (1001) docker     (127)    29990 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/hgrc
--rw-r--r--   0 runner    (1001) docker     (127)    30813 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45753 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/run-task
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/target_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/from_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.156743 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/
--rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    52586 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/task_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.160743 taskcluster-taskgraph-8.1.0/src/taskgraph/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/set_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/treeherder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/workertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.164743 taskcluster-taskgraph-8.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_actions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_morph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15700 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_optimize_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_scripts_fetch_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_scripts_run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_target_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_taskgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transform_chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transform_docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transform_task_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_from_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_run_run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_run_toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_readonlydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_taskcluster.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_treeherder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_workertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.746732 taskcluster-taskgraph-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-22 15:46:21.746732 taskcluster-taskgraph-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.730732 taskcluster-taskgraph-8.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:46:21.746732 taskcluster-taskgraph-8.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.726732 taskcluster-taskgraph-8.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.730732 taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-22 15:46:21.000000 taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-22 15:46:21.000000 taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:46:21.000000 taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 15:46:21.000000 taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 15:46:21.000000 taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 15:46:21.000000 taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.730732 taskcluster-taskgraph-8.2.0/src/taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.734732 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.734732 taskcluster-taskgraph-8.2.0/src/taskgraph/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29171 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/morph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.734732 taskcluster-taskgraph-8.2.0/src/taskgraph/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20107 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.734732 taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29990 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 runner    (1001) docker     (127)    30813 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45753 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.734732 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/from_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.738732 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/
+-rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52586 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/task_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.738732 taskcluster-taskgraph-8.2.0/src/taskgraph/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/set_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:21.746732 taskcluster-taskgraph-8.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_actions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_morph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15700 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_optimize_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_scripts_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_target_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_taskgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transform_chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transform_docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transform_task_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_from_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_run_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_run_toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_transforms_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_readonlydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_treeherder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_workertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-22 15:46:17.000000 taskcluster-taskgraph-8.2.0/test/test_util_yaml.py
```

### Comparing `taskcluster-taskgraph-8.1.0/LICENSE` & `taskcluster-taskgraph-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/PKG-INFO` & `taskcluster-taskgraph-8.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 8.1.0
+Version: 8.2.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `taskcluster-taskgraph-8.1.0/README.rst` & `taskcluster-taskgraph-8.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/pyproject.toml` & `taskcluster-taskgraph-8.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/requirements/base.txt` & `taskcluster-taskgraph-8.2.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/requirements/dev.txt` & `taskcluster-taskgraph-8.2.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/requirements/test.txt` & `taskcluster-taskgraph-8.2.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/setup.py` & `taskcluster-taskgraph-8.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 8.1.0
+Version: 8.2.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-8.2.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/__init__.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "8.1.0"
+__version__ = "8.2.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/config.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/create.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/decision.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/docker.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 
 try:
     import zstandard as zstd
 except ImportError as e:
     zstd = e
 
 from taskgraph.util import docker
-from taskgraph.util.taskcluster import get_artifact_url, get_session
+from taskgraph.util.taskcluster import (
+    get_artifact_url,
+    get_session,
+)
 
 DEPLOY_WARNING = """
 *****************************************************************
 WARNING: Image is not suitable for deploying/pushing.
 
 To automatically tag the image the following files are required:
 - {image_dir}/REGISTRY
@@ -55,18 +58,17 @@
 
     params = Parameters(
         level=os.environ.get("MOZ_SCM_LEVEL", "3"),
         strict=False,
     )
     tasks = load_tasks_for_kind(params, "docker-image")
     task = tasks[f"build-docker-image-{image_name}"]
-    deadline = None
-    task_id = IndexSearch().should_replace_task(
-        task, {}, deadline, task.optimization.get("index-search", [])
-    )
+
+    indexes = task.optimization.get("index-search", [])
+    task_id = IndexSearch().should_replace_task(task, {}, None, indexes)
 
     if task_id in (True, False):
         print(
             "Could not find artifacts for a docker image "
             "named `{image_name}`. Local commits and other changes "
             "in your checkout may cause this error. Try "
             "updating to a fresh checkout of {project} "
```

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/generator.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/graph.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/main.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/morph.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/optimize/strategies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from datetime import datetime
 
 from taskgraph.optimize.base import OptimizationStrategy, register_strategy
 from taskgraph.util.path import match as match_path
+from taskgraph.util.taskcluster import find_task_id, status_task
 
 logger = logging.getLogger(__name__)
 
 
 @register_strategy("index-search")
 class IndexSearch(OptimizationStrategy):
     # A task with no dependencies remaining after optimization will be replaced
@@ -19,20 +20,36 @@
     # In every of those cases, we need to run the task to create or refresh
     # artifacts.
 
     fmt = "%Y-%m-%dT%H:%M:%S.%fZ"
 
     def should_replace_task(self, task, params, deadline, arg):
         "Look for a task with one of the given index paths"
-        index_paths, label_to_taskid, taskid_to_status = arg
+        batched = False
+        # Appease static checker that doesn't understand that this is not needed
+        label_to_taskid = {}
+        taskid_to_status = {}
+
+        if isinstance(arg, tuple) and len(arg) == 3:
+            # allow for a batched call optimization instead of two queries
+            # per index path
+            index_paths, label_to_taskid, taskid_to_status = arg
+            batched = True
+        else:
+            index_paths = arg
 
         for index_path in index_paths:
             try:
-                task_id = label_to_taskid[index_path]
-                status = taskid_to_status[task_id]
+                if batched:
+                    task_id = label_to_taskid[index_path]
+                    status = taskid_to_status[task_id]
+                else:
+                    # 404 is raised as `KeyError` also end up here
+                    task_id = find_task_id(index_path)
+                    status = status_task(task_id)
                 # status can be `None` if we're in `testing` mode
                 # (e.g. test-action-callback)
                 if not status or status.get("state") in ("exception", "failed"):
                     continue
 
                 if deadline and datetime.strptime(
                     status["expires"], self.fmt
```

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/parameters.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-8.2.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/task.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/chunking.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/chunking.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/__init__.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/common.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/index_search.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/run_task.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/toolchain.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/run/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/task_context.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/transforms/task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/path.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/set_name.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/set_name.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/time.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-8.2.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-8.2.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_actions_registry.py` & `taskcluster-taskgraph-8.2.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_create.py` & `taskcluster-taskgraph-8.2.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_decision.py` & `taskcluster-taskgraph-8.2.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_docker.py` & `taskcluster-taskgraph-8.2.0/test/test_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_generator.py` & `taskcluster-taskgraph-8.2.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_graph.py` & `taskcluster-taskgraph-8.2.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_main.py` & `taskcluster-taskgraph-8.2.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_morph.py` & `taskcluster-taskgraph-8.2.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_optimize.py` & `taskcluster-taskgraph-8.2.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_parameters.py` & `taskcluster-taskgraph-8.2.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-8.2.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_scripts_run_task.py` & `taskcluster-taskgraph-8.2.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_target_tasks.py` & `taskcluster-taskgraph-8.2.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_taskgraph.py` & `taskcluster-taskgraph-8.2.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transform_chunking.py` & `taskcluster-taskgraph-8.2.0/test/test_transform_chunking.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transform_docker_image.py` & `taskcluster-taskgraph-8.2.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transform_task_context.py` & `taskcluster-taskgraph-8.2.0/test/test_transform_task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_base.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_cached_tasks.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_fetch.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_notify.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_run.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_run.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_run_run_task.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_run_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_run_toolchain.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_run_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_transforms_task.py` & `taskcluster-taskgraph-8.2.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_archive.py` & `taskcluster-taskgraph-8.2.0/test/test_util_archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_attributes.py` & `taskcluster-taskgraph-8.2.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_cached_tasks.py` & `taskcluster-taskgraph-8.2.0/test/test_util_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_dependencies.py` & `taskcluster-taskgraph-8.2.0/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_docker.py` & `taskcluster-taskgraph-8.2.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_parameterization.py` & `taskcluster-taskgraph-8.2.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_path.py` & `taskcluster-taskgraph-8.2.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_python_path.py` & `taskcluster-taskgraph-8.2.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_readonlydict.py` & `taskcluster-taskgraph-8.2.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_schema.py` & `taskcluster-taskgraph-8.2.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_taskcluster.py` & `taskcluster-taskgraph-8.2.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_templates.py` & `taskcluster-taskgraph-8.2.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_time.py` & `taskcluster-taskgraph-8.2.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_treeherder.py` & `taskcluster-taskgraph-8.2.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_vcs.py` & `taskcluster-taskgraph-8.2.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_verify.py` & `taskcluster-taskgraph-8.2.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_workertypes.py` & `taskcluster-taskgraph-8.2.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.1.0/test/test_util_yaml.py` & `taskcluster-taskgraph-8.2.0/test/test_util_yaml.py`

 * *Files identical despite different names*

