# Comparing `tmp/merlin-pyfunc-server-0.42.1.tar.gz` & `tmp/merlin-pyfunc-server-0.42.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-pyfunc-server-0.42.1.tar", last modified: Thu May 16 04:42:43 2024, max compression
+gzip compressed data, was "merlin-pyfunc-server-0.42.2.tar", last modified: Wed May 22 07:51:28 2024, max compression
```

## Comparing `merlin-pyfunc-server-0.42.1.tar` & `merlin-pyfunc-server-0.42.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.724781 merlin-pyfunc-server-0.42.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-16 04:42:43.724781 merlin-pyfunc-server-0.42.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.712782 merlin-pyfunc-server-0.42.1/benchmark/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/benchmark/benchmark.sh
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/benchmark/large.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    78669 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/benchmark/large.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/benchmark/medium.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/benchmark/medium.json
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/benchmark/small.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/benchmark/small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.712782 merlin-pyfunc-server-0.42.1/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/docker/base.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/docker/local.Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)     1277 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/docker/process_conda_env.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/docker/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.712782 merlin-pyfunc-server-0.42.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/examples/echo_http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/echo_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/echo_http/echo_http.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/echo_http/env.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/examples/echo_upi/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/echo_upi/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/echo_upi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/echo_upi/env.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/echo_upi/upi_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/echo_upi/upi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/examples/iris_http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/iris_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/iris_http/env.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/iris_http/iris_http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/examples/iris_http/models/
--rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/iris_http/models/model_1.bst
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/examples/iris_http/models/model_2.joblib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-16 04:42:43.000000 merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-16 04:42:43.000000 merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:42:43.000000 merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 04:42:43.000000 merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-16 04:42:43.000000 merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 04:42:43.000000 merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/prometheus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/prometheus/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/pyfuncserver/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/pyfuncserver/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/metrics/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/metrics/pusher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.716781 merlin-pyfunc-server-0.42.1/pyfuncserver/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/rest/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/rest/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/upi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/upi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/upi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/pyfuncserver/publisher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/publisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/publisher/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/publisher/publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/pyfuncserver/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/sampler/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/pyfuncserver/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/utils/contants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 04:42:42.000000 merlin-pyfunc-server-0.42.1/pyfuncserver/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:42:43.724781 merlin-pyfunc-server-0.42.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/test/local-artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/local-artifacts/MLmodel
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/local-artifacts/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.720781 merlin-pyfunc-server-0.42.1/test/local-artifacts/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/local-artifacts/artifacts/model_1.bst
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/local-artifacts/artifacts/model_2.joblib
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/local-artifacts/conda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/local-artifacts/python_env.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/local-artifacts/python_model.pkl
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/local-artifacts/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.724781 merlin-pyfunc-server-0.42.1/test/publisher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/publisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/publisher/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/publisher/test_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.724781 merlin-pyfunc-server-0.42.1/test/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/sampler/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/test_backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/test_upi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:43.724781 merlin-pyfunc-server-0.42.1/test/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/util/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 04:42:33.000000 merlin-pyfunc-server-0.42.1/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.382140 merlin-pyfunc-server-0.42.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-22 07:51:28.382140 merlin-pyfunc-server-0.42.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.370140 merlin-pyfunc-server-0.42.2/benchmark/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/benchmark/benchmark.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/benchmark/large.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    78669 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/benchmark/large.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/benchmark/medium.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/benchmark/medium.json
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/benchmark/small.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/benchmark/small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.370140 merlin-pyfunc-server-0.42.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/docker/base.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/docker/local.Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1277 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/docker/process_conda_env.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/docker/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.370140 merlin-pyfunc-server-0.42.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.370140 merlin-pyfunc-server-0.42.2/examples/echo_http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/echo_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/echo_http/echo_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/echo_http/env.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.374140 merlin-pyfunc-server-0.42.2/examples/echo_upi/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/echo_upi/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/echo_upi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/echo_upi/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/echo_upi/upi_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/echo_upi/upi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.374140 merlin-pyfunc-server-0.42.2/examples/iris_http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/iris_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/iris_http/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/iris_http/iris_http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.374140 merlin-pyfunc-server-0.42.2/examples/iris_http/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/iris_http/models/model_1.bst
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/examples/iris_http/models/model_2.joblib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.374140 merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-22 07:51:27.000000 merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-22 07:51:28.000000 merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:51:27.000000 merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-22 07:51:27.000000 merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-22 07:51:27.000000 merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 07:51:27.000000 merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.374140 merlin-pyfunc-server-0.42.2/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/prometheus/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.374140 merlin-pyfunc-server-0.42.2/pyfuncserver/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.374140 merlin-pyfunc-server-0.42.2/pyfuncserver/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/metrics/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/metrics/pusher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/pyfuncserver/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/rest/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/rest/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/upi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/upi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/upi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/pyfuncserver/publisher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/publisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/publisher/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/publisher/publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/pyfuncserver/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/sampler/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/pyfuncserver/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/utils/contants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 07:51:27.000000 merlin-pyfunc-server-0.42.2/pyfuncserver/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:51:28.382140 merlin-pyfunc-server-0.42.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.378140 merlin-pyfunc-server-0.42.2/test/local-artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/local-artifacts/MLmodel
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/local-artifacts/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.382140 merlin-pyfunc-server-0.42.2/test/local-artifacts/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/local-artifacts/artifacts/model_1.bst
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/local-artifacts/artifacts/model_2.joblib
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/local-artifacts/conda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/local-artifacts/python_env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/local-artifacts/python_model.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/local-artifacts/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.382140 merlin-pyfunc-server-0.42.2/test/publisher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/publisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/publisher/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/publisher/test_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.382140 merlin-pyfunc-server-0.42.2/test/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/sampler/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/test_backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/test_upi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:28.382140 merlin-pyfunc-server-0.42.2/test/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/util/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-22 07:51:19.000000 merlin-pyfunc-server-0.42.2/test/utils.py
```

### Comparing `merlin-pyfunc-server-0.42.1/.gitignore` & `merlin-pyfunc-server-0.42.2/.gitignore`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/PKG-INFO` & `merlin-pyfunc-server-0.42.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-pyfunc-server
-Version: 0.42.1
+Version: 0.42.2
 Summary: Model Server implementation for Merlin PyFunc model
 Home-page: UNKNOWN
 Author-email: merlin-dev@gojek.com
 License: UNKNOWN
 Description: # PyFunc Server
         
         PyFunc Server is Kserve extension for deploying user-defined python function model.
```

### Comparing `merlin-pyfunc-server-0.42.1/README.md` & `merlin-pyfunc-server-0.42.2/README.md`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/benchmark/benchmark.sh` & `merlin-pyfunc-server-0.42.2/benchmark/benchmark.sh`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/benchmark/large.json` & `merlin-pyfunc-server-0.42.2/benchmark/large.json`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/benchmark/medium.json` & `merlin-pyfunc-server-0.42.2/benchmark/medium.json`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/docker/Dockerfile` & `merlin-pyfunc-server-0.42.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/docker/base.Dockerfile` & `merlin-pyfunc-server-0.42.2/docker/base.Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/docker/local.Dockerfile` & `merlin-pyfunc-server-0.42.2/docker/local.Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/docker/process_conda_env.sh` & `merlin-pyfunc-server-0.42.2/docker/process_conda_env.sh`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/docker/run.sh` & `merlin-pyfunc-server-0.42.2/docker/run.sh`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/examples/echo_upi/upi_client.py` & `merlin-pyfunc-server-0.42.2/examples/echo_upi/upi_client.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/examples/echo_upi/upi_server.py` & `merlin-pyfunc-server-0.42.2/examples/echo_upi/upi_server.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/examples/iris_http/iris_http.py` & `merlin-pyfunc-server-0.42.2/examples/iris_http/iris_http.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/examples/iris_http/models/model_1.bst` & `merlin-pyfunc-server-0.42.2/examples/iris_http/models/model_1.bst`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/examples/iris_http/models/model_2.joblib` & `merlin-pyfunc-server-0.42.2/examples/iris_http/models/model_2.joblib`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/PKG-INFO` & `merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-pyfunc-server
-Version: 0.42.1
+Version: 0.42.2
 Summary: Model Server implementation for Merlin PyFunc model
 Home-page: UNKNOWN
 Author-email: merlin-dev@gojek.com
 License: UNKNOWN
 Description: # PyFunc Server
         
         PyFunc Server is Kserve extension for deploying user-defined python function model.
```

### Comparing `merlin-pyfunc-server-0.42.1/merlin_pyfunc_server.egg-info/SOURCES.txt` & `merlin-pyfunc-server-0.42.2/merlin_pyfunc_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/__init__.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/__main__.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/__main__.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/config.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/config.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/metrics/handler.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/metrics/handler.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/metrics/pusher.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/metrics/pusher.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/model/model.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/model/model.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/rest/handler.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/rest/handler.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/rest/server.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/rest/server.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/protocol/upi/server.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/protocol/upi/server.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/publisher/kafka.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/publisher/kafka.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/publisher/publisher.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/publisher/publisher.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/sampler/sampler.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/server.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/server.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/utils/contants.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/utils/contants.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/pyfuncserver/utils/converter.py` & `merlin-pyfunc-server-0.42.2/pyfuncserver/utils/converter.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/setup.py` & `merlin-pyfunc-server-0.42.2/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/local-artifacts/MLmodel` & `merlin-pyfunc-server-0.42.2/test/local-artifacts/MLmodel`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/local-artifacts/artifacts/model_1.bst` & `merlin-pyfunc-server-0.42.2/test/local-artifacts/artifacts/model_1.bst`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/local-artifacts/artifacts/model_2.joblib` & `merlin-pyfunc-server-0.42.2/test/local-artifacts/artifacts/model_2.joblib`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/local-artifacts/python_model.pkl` & `merlin-pyfunc-server-0.42.2/test/local-artifacts/python_model.pkl`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/publisher/test_kafka.py` & `merlin-pyfunc-server-0.42.2/test/publisher/test_kafka.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/publisher/test_publisher.py` & `merlin-pyfunc-server-0.42.2/test/publisher/test_publisher.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/sampler/test_sampler.py` & `merlin-pyfunc-server-0.42.2/test/sampler/test_sampler.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/test_backward_compatibility.py` & `merlin-pyfunc-server-0.42.2/test/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/test_examples.py` & `merlin-pyfunc-server-0.42.2/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/test_http.py` & `merlin-pyfunc-server-0.42.2/test/test_http.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/test_upi.py` & `merlin-pyfunc-server-0.42.2/test/test_upi.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/util/test_converter.py` & `merlin-pyfunc-server-0.42.2/test/util/test_converter.py`

 * *Files identical despite different names*

### Comparing `merlin-pyfunc-server-0.42.1/test/utils.py` & `merlin-pyfunc-server-0.42.2/test/utils.py`

 * *Files identical despite different names*

