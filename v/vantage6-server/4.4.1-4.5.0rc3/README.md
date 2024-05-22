# Comparing `tmp/vantage6-server-4.4.1.tar.gz` & `tmp/vantage6-server-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-4.4.1.tar", last modified: Wed May  8 12:54:35 2024, max compression
+gzip compressed data, was "vantage6-server-4.5.0rc3.tar", last modified: Wed May 22 15:04:59 2024, max compression
```

## Comparing `vantage6-server-4.4.1.tar` & `vantage6-server-4.5.0rc3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.460864 vantage6-server-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-08 12:54:35.460864 vantage6-server-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:54:35.460864 vantage6-server-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.444864 vantage6-server-4.4.1/tests_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)   174647 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.444864 vantage6-server-4.4.1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/algo_store_communication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.448864 vantage6-server-4.4.1/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.452864 vantage6-server-4.4.1/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.452864 vantage6-server-4.4.1/vantage6/server/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/study.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/task_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.456864 vantage6-server-4.4.1/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    31301 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.456864 vantage6-server-4.4.1/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/common/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/common/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/study.py
--rw-r--r--   0 runner    (1001) docker     (127)    40748 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.456864 vantage6-server-4.4.1/vantage6/server/resource/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/ui/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-08 12:54:22.000000 vantage6-server-4.4.1/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:54:35.456864 vantage6-server-4.4.1/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 12:54:35.000000 vantage6-server-4.4.1/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.541294 vantage6-server-4.5.0rc3/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174647 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.541294 vantage6-server-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    29923 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/algo_store_communication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.545294 vantage6-server-4.5.0rc3/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.549294 vantage6-server-4.5.0rc3/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.549294 vantage6-server-4.5.0rc3/vantage6/server/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/task_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32870 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/common/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/common/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40748 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/vantage6/server/resource/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/ui/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19467 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-22 15:04:46.000000 vantage6-server-4.5.0rc3/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:59.553294 vantage6-server-4.5.0rc3/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 15:04:59.000000 vantage6-server-4.5.0rc3/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-4.4.1/PKG-INFO` & `vantage6-server-4.5.0rc3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
@@ -12,47 +12,51 @@
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
 
 <h3 align=center> A Privacy Enhancing Technology (PET) Operations platform</h3>
 <h3 align="center">
 
 <!-- Badges go here-->
+
 [![Release](https://github.com/vantage6/vantage6/actions/workflows/release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/release.yml)
 [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://badge.fury.io/py/vantage6)
 [![Unittests](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/vantage6/vantage6/badge.svg?branch=main)](https://coveralls.io/github/vantage6/vantage6?branch=main)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://www.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vantage6/vantage6&amp;utm_campaign=Badge_Grade)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://app.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![DOI](https://zenodo.org/badge/492818831.svg)](https://zenodo.org/badge/latestdoi/492818831)
+
 </h3>
 
 <p align="center">
   <a href="#books-quickstart">Quickstart</a> •
   <a href="#project-structure">Project structure</a> •
   <a href="#gift_heart-join-the-community">Join the community</a> •
   <a href="#black_nib-references">References</a>
 </p>
 
+---
 
------------------------------------------------------------------------------------------------------
 This repository is contains all the **vantage6** infrastructure source code. The **vantage6** technology enables to manage and deploy privacy enhancing technologies like Federated Learning (FL) and Multi-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions, suggestions or just want to chat about federated learning: join our [Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel.
 
 ## Infrastructure overview
 
 ![Vantage6 architecture overview](docs/images/overview-infrastructure.png)
 
-*A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network.*
+_A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network._
 
 ## :books: Quickstart
 
 ### Requirements
+
 The **vantage6** infrastructure is delivered in Docker images. To run these images, you need to have [Docker](https://docs.docker.com/get-docker/) installed. To install the latest version of the vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we recommend using an environment manager like [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
 
 Install the latest version of the vantage6 CLI by using:
+
 ```bash
 pip install vantage6
 ```
 
 This install the `v6` commands, which allows you to manage your nodes and servers. To view all available options, run:
 
 ```bash
@@ -79,16 +83,16 @@
 
 # View server logs
 v6 server attach
 ```
 
 From here you can use the [vantage6-client](https://pypi.org/project/vantage6-client) to interact with the server. The demo network has a pre-configured organization with the following credentials:
 
-* Username: `org_1-admin`
-* Password: `password`
+- Username: `org_1-admin`
+- Password: `password`
 
 For example, you can create a new organization by running:
 
 ```python
 from vantage6.client import Client
 
 client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
@@ -106,69 +110,74 @@
 ```
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai)
 
 ## Project structure
 
 ### PYPI packages
+
 This repository is home to 6 PyPi packages:
 
-* [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
-* [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
-* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
-* [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
-* [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
-* [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
-* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
-* [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
+- [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
+- [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+- [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
+- [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
+- [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+- [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
+- [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
+- [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 This repository also hosts the code for the vantage6 user interface (UI). The UI
 is an Angular web application that can be used to interact with the vantage6 server
 easily.
 
 ### Docker images
+
 The vantage6 infrastructure is delivered in Docker images. All Docker images are stored in our private [Harbor](https://goharbor.io/) registry. The most important images are:
 
-* `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
-* `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
-* `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
-* `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
+- `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
+- `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
+- `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
+- `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
 
 with `VERSION` being the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or `4.1.0rc0`.
 
 Several other images are used to support the infrastructure:
 
-* `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
-* `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
-* `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
-* `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
-* `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
-* `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
+- `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
+- `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
+- `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
+- `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
+- `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
+- `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
 
 And finally there are some images released for algorithm development:
 
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
-* `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
 
 ## :gift_heart: Join the community!
+
 We hope to continue developing, improving, and supporting **vantage6** with the help of the federated learning community. If you are interested in contributing, first of all, thank you! Second, please take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/devops/contribute.html)
 
 <a href="https://github.com/vantage6/vantage6/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=vantage6/vantage6" />
 </a>
 
 ## :black_nib: References
+
 If you are using **vantage6**, please cite this repository as well as the accompanying papers as follows:
 
-> * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
-> * A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
-> * D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+> - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
+> - A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
+> - D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+
+---
 
------------------------------------------------------------------------------------------------------
 <p align="center">
   <a href="https://vantage6.ai">vantage6.ai</a> •
   <a href="https://discord.gg/yAyFf6Y">Discord</a> •
   <a href="https://vantage6.discourse.group/">Discourse</a> •
   <a href="https://docs.vantage6.ai">User documentation</a> •
 </p>
```

#### html2text {}

```diff
@@ -1,46 +1,45 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.4.1 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.5.0rc3 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
 bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66)) [[!![[UUnniitttteessttss]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//
    aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//
     vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll)) [[!![[CCoovveerraaggee SSttaattuuss]]((hhttttppss::////
  ccoovveerraallllss..iioo//rreeppooss//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66//bbaaddggee..ssvvgg??bbrraanncchh==mmaaiinn))]]((hhttttppss::////
  ccoovveerraallllss..iioo//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66??bbrraanncchh==mmaaiinn)) [[!![[CCooddaaccyy BBaaddggee]]((hhttttppss::////
 aapppp..ccooddaaccyy..ccoomm//pprroojjeecctt//bbaaddggee//GGrraaddee//22ee6600aacc33bb33ff228844662200880055ff77339999ccbbaa331177bbee))]]((hhttttppss::////
-                     wwwwww..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
-   ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==ggiitthhuubb..ccoomm&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==vvaannttaaggee66//
-   vvaannttaaggee66&&uuttmm__ccaammppaaiiggnn==BBaaddggee__GGrraaddee)) [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//DDOOII//
-   1100..55228811//zzeennooddoo..77338822660022..ssvvgg))]]((hhttttppss::////ddooii..oorrgg//1100..55228811//zzeennooddoo..77338822660022)) ********
+                     aapppp..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
+ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==gghh&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==&&uuttmm__ccaammppaaiiggnn==BBaaddggee__ggrraaddee))
+  [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//449922881188883311..ssvvgg))]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//
+                           llaatteessttddooii//449922881188883311)) ********
     _Q_u_i_c_k_s_t_a_r_t â¢ _P_r_o_j_e_c_t_ _s_t_r_u_c_t_u_r_e â¢ _J_o_i_n_ _t_h_e_ _c_o_m_m_u_n_i_t_y â¢ _R_e_f_e_r_e_n_c_e_s
--------------------------------------------------------------------------------
----------------------- This repository is contains all the **vantage6**
-infrastructure source code. The **vantage6** technology enables to manage and
-deploy privacy enhancing technologies like Federated Learning (FL) and Multi-
-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://
-vantage6.ai) to learn more! You can find more (user) documentation at
-[readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
-questions, suggestions or just want to chat about federated learning: join our
-[Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+--- This repository is contains all the **vantage6** infrastructure source
+code. The **vantage6** technology enables to manage and deploy privacy
+enhancing technologies like Federated Learning (FL) and Multi-Party Computation
+(MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn
+more! You can find more (user) documentation at [readthedocs
+(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
+suggestions or just want to chat about federated learning: join our [Discord
+(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
 Infrastructure overview ![Vantage6 architecture overview](docs/images/overview-
-infrastructure.png) *A High level overview of the vantage6 infrastructure.
+infrastructure.png) _A High level overview of the vantage6 infrastructure.
 Vantage6 has both a client-server and peer-to-peer architecture. The client is
 used by the researcher to create (PET) computation requests. It is also used to
 manage users, organizations and collaborations. The server contains users,
 organizations, collaborations, tasks and their results. It provides a central
 access point for both the clients and nodes. The nodes have access to privacy
 sensitive data and handle computation requests retrieved from the server.
 Computation request are executed as separate containers on the node. These
-containers are connected to containers at other nodes by a VPN network.* ## :
+containers are connected to containers at other nodes by a VPN network._ ## :
 books: Quickstart ### Requirements The **vantage6** infrastructure is delivered
 in Docker images. To run these images, you need to have [Docker](https://
 docs.docker.com/get-docker/) installed. To install the latest version of the
 vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we
 recommend using an environment manager like [mini-conda](https://docs.conda.io/
 en/latest/miniconda.html). Install the latest version of the vantage6 CLI by
 using: ```bash pip install vantage6 ``` This install the `v6` commands, which
@@ -49,75 +48,74 @@
 using: ```bash v6 dev create-demo-network ``` This creates a local network with
 a server and two nodes. You can start the network by running: ```bash v6 dev
 start-demo-network ``` This will start the server and nodes in the background.
 You can view the logs by running: ```bash # View node logs v6 node attach #
 View server logs v6 server attach ``` From here you can use the [vantage6-
 client](https://pypi.org/project/vantage6-client) to interact with the server.
 The demo network has a pre-configured organization with the following
-credentials: * Username: `org_1-admin` * Password: `password` For example, you
+credentials: - Username: `org_1-admin` - Password: `password` For example, you
 can create a new organization by running: ```python from vantage6.client import
 Client client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
 client.authenticate('org_1-admin', 'password') client.setup_encryption(None)
 client.organization.create( name='My organization', address1='My address',
 address2='My address', zipcode='1234AB', country='The Netherlands', domain='my-
 organization.com' ) ``` You can find more (user) documentation at [readthedocs
 (docs.vantage6.ai)](https://docs.vantage6.ai) ## Project structure ### PYPI
-packages This repository is home to 6 PyPi packages: * [vantage6](https://
-pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
+packages This repository is home to 6 PyPi packages: - [vantage6](https://
+pypi.org/project/vantage6) -> _CLI for managing node and server instances_ -
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+for interacting with the vantage6-server_ - [vantage6-algorithm-tools](https://
 pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
-algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
-node) -> _Node application package_ * [vantage6-server](https://pypi.org/
-project/vantage6-server) -> _Server application package_ * [vantage6-algorithm-
+algorithm development_ - [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ - [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ - [vantage6-algorithm-
 store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store
-application package_ * [vantage6-common](https://pypi.org/project/vantage6-
-common) -> _Package with common vantage6 functions_ * [vantage6-backend-common]
+application package_ - [vantage6-common](https://pypi.org/project/vantage6-
+common) -> _Package with common vantage6 functions_ - [vantage6-backend-common]
 (https://pypi.org/project/vantage6-backend-common) -> _Package with functions
 common to central server and algorithm store_ **Note that when using vantage6
 you do not install the _server_ and _node_ packages. These are delivered to you
 in Docker images.** This repository also hosts the code for the vantage6 user
 interface (UI). The UI is an Angular web application that can be used to
 interact with the vantage6 server easily. ### Docker images The vantage6
 infrastructure is delivered in Docker images. All Docker images are stored in
 our private [Harbor](https://goharbor.io/) registry. The most important images
-are: * `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
-Docker image_ * `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
-application Docker image_ * `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
-> _User interface Docker image_ * `harbor2.vantage6.ai/infrastructure/
+are: - `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
+Docker image_ - `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
+application Docker image_ - `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
+> _User interface Docker image_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-store:VERSION` -> _Algorithm store Docker image_ with `VERSION` being
 the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or
-`4.1.0rc0`. Several other images are used to support the infrastructure: *
+`4.1.0rc0`. Several other images are used to support the infrastructure: -
 `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image
-for the infrastructure_ * `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
-> _Squid proxy image used for the whitelisting service_ * `harbor2.vantage6.ai/
-infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ *
+for the infrastructure_ - `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
+> _Squid proxy image used for the whitelisting service_ - `harbor2.vantage6.ai/
+infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ -
 `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect
-to the VPN_ * `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
-image used for initialization_ * `harbor2.vantage6.ai/infrastructure/ssh-
+to the VPN_ - `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
+image used for initialization_ - `harbor2.vantage6.ai/infrastructure/ssh-
 tunnel` -> _SSH tunnel image used for connecting algorithms to external
 services_ And finally there are some images released for algorithm development:
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
-image for algorithm development_ * `harbor2.vantage6.ai/infrastructure/
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
+image for algorithm development_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI
 algorithm development_ ## :gift_heart: Join the community! We hope to continue
 developing, improving, and supporting **vantage6** with the help of the
 federated learning community. If you are interested in contributing, first of
 all, thank you! Second, please take a look at our [contributing guidelines]
 (https://docs.vantage6.ai/en/main/devops/contribute.html) _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_a_n_t_a_g_e_6_/_v_a_n_t_a_g_e_6_]## :black_nib: References If you are
 using **vantage6**, please cite this repository as well as the accompanying
-papers as follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
+papers as follows: > - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
 Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. >
-* A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
+- A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
 VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE
 for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-
 877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-
-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > * D. Smits\*,
+torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > - D. Smits\*,
 B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An
 Improved Infrastructure for Privacy-Preserving Analysis of Patient Data,
 Proceedings of the International Conference of Informatics, Management, and
 Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https:/
 /arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://
-ebooks.iospress.nl/volumearticle/60190)] --------------------------------------
----------------------------------------------------------------
+ebooks.iospress.nl/volumearticle/60190)] ---
        _v_a_n_t_a_g_e_6_._a_i â¢ _D_i_s_c_o_r_d â¢ _D_i_s_c_o_u_r_s_e â¢ _U_s_e_r_ _d_o_c_u_m_e_n_t_a_t_i_o_n â¢
```

### Comparing `vantage6-server-4.4.1/setup.py` & `vantage6-server-4.5.0rc3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     url="https://github.com/vantage6/vantage6",
     packages=find_namespace_packages(),
     python_requires=">=3.10",
     install_requires=[
         "bcrypt==4.0.1",
         "flasgger==0.9.5",
         "flask==2.2.5",
-        "Flask-Cors==3.0.10",
+        "Flask-Cors==4.0.1",
         "Flask-JWT-Extended==4.4.4",
         "Flask-Mail==0.9.1",
         "Flask-Principal==0.4.0",
         "Flask-RESTful==0.3.10",
         "flask-marshmallow==0.15.0",
         "Flask-SocketIO==5.3.6",
         "gevent==23.9.1",
```

### Comparing `vantage6-server-4.4.1/tests_server/test_models.py` & `vantage6-server-4.5.0rc3/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/tests_server/test_resources.py` & `vantage6-server-4.5.0rc3/tests_server/test_resources.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/__init__.py` & `vantage6-server-4.5.0rc3/vantage6/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
         # before request
         @self.app.before_request
         def do_before_request():
             """Before every flask request method."""
             # Add log message before each request
             log.debug(
-                f"Received request: {request.method} " f"{_get_request_path(request)}"
+                f"Received request: {request.method} {_get_request_path(request)}"
             )
 
             # This will obtain a (scoped) db session from the session factory
             # that is linked to the flask request global `g`. In every endpoint
             # we then can access the database by using this session. We ensure
             # that the session is removed (and uncommited changes are rolled
             # back) at the end of every request.
@@ -340,18 +340,18 @@
         def error_remove_db_session(error: HTTPException):
             """In case an HTTP-exception occurs during the request.
 
             It is important to close the db session to avoid having dangling
             sessions.
             """
             if error.code == 404:
-                log.debug(f"404 error for route '{_get_request_path(request)}'")
+                log.debug("404 error for route '%s'", _get_request_path(request))
             else:
-                log.warn("HTTP Exception occured during request")
-                log.debug(traceback.format_exc())
+                log.warning("HTTP Exception occured during request")
+                log.debug("Details exception: %s", traceback.format_exc())
             DatabaseSessionManager.clear_session()
             return error.get_response()
 
         @self.app.errorhandler(Exception)
         def error2_remove_db_session(error):
             """In case an exception occurs during the request.
 
@@ -608,15 +608,15 @@
                         RuleNeed(
                             name=rule.name, scope=rule.scope, operation=rule.operation
                         )
                     )
                 identity_changed.send(
                     current_app._get_current_object(), identity=auth_identity
                 )
-                log.debug(identity)
+                log.debug("identity %s", identity)
                 return identity
 
     def load_resources(self) -> None:
         """Import the modules containing API resources."""
 
         # make services available to the endpoints, this way each endpoint can
         # make use of 'em.
@@ -667,26 +667,26 @@
         # add default roles (if they don't exist yet)
         self._add_default_roles()
 
         # create root user if it is not in the DB yet
         try:
             db.User.get_by_username(SUPER_USER_INFO["username"])
         except Exception:
-            log.warn("No root user found! Is this the first run?")
+            log.warning("No root user found! Is this the first run?")
 
             log.debug("Creating organization for root user")
             org = db.Organization(name="root")
 
             # TODO use constant instead of 'Root' literal
             root = db.Role.get_by_name("Root")
 
-            log.warn(
-                f"Creating root user: "
-                f"username={SUPER_USER_INFO['username']}, "
-                f"password={SUPER_USER_INFO['password']}"
+            log.warning(
+                "Creating root user: username=%s, password=%s",
+                SUPER_USER_INFO["username"],
+                SUPER_USER_INFO["password"],
             )
 
             user = db.User(
                 username=SUPER_USER_INFO["username"],
                 roles=[root],
                 organization=org,
                 email="root@domain.ext",
```

### Comparing `vantage6-server-4.4.1/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/_data/dev/server.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-4.5.0rc3/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/_version.py` & `vantage6-server-4.5.0rc3/vantage6/server/_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 4, 1, "final", __build__, 0)
+version_info = (4, 5, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-server-4.4.1/vantage6/server/algo_store_communication.py` & `vantage6-server-4.5.0rc3/vantage6/server/algo_store_communication.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/cli/server.py` & `vantage6-server-4.5.0rc3/vantage6/server/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/context.py` & `vantage6-server-4.5.0rc3/vantage6/server/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/controller/fixture.py` & `vantage6-server-4.5.0rc3/vantage6/server/controller/fixture.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/db.py` & `vantage6-server-4.5.0rc3/vantage6/server/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,24 +54,23 @@
     Exception
         If the value is not an instance of db.Base or a list of db.Base
     """
     if isinstance(value, list):
         return [jsonable(i) for i in value]
 
     elif isinstance(value, Base):
-        log.debug(f"preparing={value}")
+        log.debug("preparing=%s", value)
         retval = dict()
         mapper = sql.inspect(value.__class__)
 
         columns = [
             c.key for c in mapper.columns if c.key not in value._hidden_attributes
         ]
 
         for column in columns:
-            # log.debug(f"processing column={column}")
             column_value = getattr(value, column)
 
             if isinstance(column_value, enum.Enum):
                 column_value = column_value.value
             elif isinstance(column_value, datetime.datetime):
                 column_value = column_value.isoformat()
             elif isinstance(column_value, bytes):
```

### Comparing `vantage6-server-4.4.1/vantage6/server/default_roles.py` & `vantage6-server-4.5.0rc3/vantage6/server/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/globals.py` & `vantage6-server-4.5.0rc3/vantage6/server/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/mail_service.py` & `vantage6-server-4.5.0rc3/vantage6/server/mail_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             Message to send in the email
         """
         with app.app_context():
             try:
                 self.mail.send(msg)
             except Exception as e:
                 log.error("Mailserver error!")
-                log.debug(e)
+                log.exception(e)
 
     def send_email(
         self,
         subject: str,
         sender: str,
         recipients: list[str],
         text_body: str,
```

### Comparing `vantage6-server-4.4.1/vantage6/server/model/__init__.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/algorithm_port.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/algorithm_store.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/authenticatable.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/base.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/collaboration.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/common/utils.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/member.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/node.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/node_config.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/organization.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/permission.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/role.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/rule.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/run.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/study.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/task.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import os
 
 from sqlalchemy import Column, String, ForeignKey, Integer, sql, DateTime
 from sqlalchemy.orm import relationship
 from sqlalchemy.ext.hybrid import hybrid_property
 
 from vantage6.common.task_status import TaskStatus, has_task_failed
 from vantage6.server.model.base import Base, DatabaseSessionManager
@@ -102,14 +103,19 @@
         the underlying algorithm runs.
 
         Returns
         -------
         str
             Status of task
         """
+        # The following is necessary because if readthedocs executes this code to
+        # generate function docs, it will fail with a sqlalchemy error (because there
+        # are no runs?).
+        if os.environ.get("READTHEDOCS"):
+            return ""
         # TODO what if there are no result ids? -> currently returns unknown
         run_statuses = [r.status for r in self.runs]
         if any([has_task_failed(status) for status in run_statuses]):
             return TaskStatus.FAILED.value
         elif TaskStatus.ACTIVE in run_statuses:
             return TaskStatus.ACTIVE.value
         elif TaskStatus.INITIALIZING in run_statuses:
```

### Comparing `vantage6-server-4.4.1/vantage6/server/model/task_database.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/task_database.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/model/user.py` & `vantage6-server-4.5.0rc3/vantage6/server/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/permission.py` & `vantage6-server-4.5.0rc3/vantage6/server/permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
         for res in RESOURCES:
             module = importlib.import_module("vantage6.server.resource." + res)
             try:
                 module.permissions(self)
             except Exception:
                 module_name = module.__name__.split(".")[-1]
                 log.debug(
-                    f"Resource '{module_name}' contains no or invalid permissions"
+                    "Resource '%s' contains no or invalid permissions", module_name
                 )
 
     def assign_rule_to_root(
         self, name: str, scope: Scope, operation: Operation
     ) -> None:
         """
         Assign a rule to the root role.
@@ -445,16 +445,18 @@
         rule = Rule.get_by_(resource, scope, operation)
         if not rule:
             rule = Rule(
                 name=resource, operation=operation, scope=scope, description=description
             )
             rule.save()
             log.debug(
-                f"New auth rule '{resource}' with scope={scope}"
-                f" and operation={operation} is stored in the DB"
+                "New auth rule '%s' with scope=%s and operation=%s is stored in the DB",
+                resource,
+                scope,
+                operation,
             )
 
         if assign_to_container:
             self.assign_rule_to_container(resource, scope, operation)
 
         if assign_to_node:
             self.assign_rule_to_node(resource, scope, operation)
```

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/__init__.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,14 @@
         def decorator(*args, **kwargs):
             # decode JWT-token
             identity = get_jwt_identity()
             claims = get_jwt()
 
             # check that identity has access to endpoint
             g.type = claims["client_type"]
-            # log.debug(f"Endpoint accessed as {g.type}")
 
             if g.type not in types:
                 # FIXME BvB 23-10-19: user gets a 500 error, would be better to
                 # get an error message with 400 code
                 msg = (
                     f"{g.type}s are not allowed to access {request.url} "
                     f"({request.method})"
```

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/algorithm_store.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/collaboration.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/collaboration.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,14 +189,19 @@
             description: Whether or not collaboration is encrypted
           - in: query
             name: organization_id
             schema:
               type: integer
             description: Organization id
           - in: query
+            name: algorithm_store_id
+            schema:
+              type: integer
+            description: Algorithm store ID that is available to the collaboration
+          - in: query
             name: include
             schema:
               type: array
               items:
                 type: string
             description: Include 'organizations' to include the organizations
               within the collaboration.
@@ -255,14 +260,28 @@
                     q.join(db.Member)
                     .join(db.Organization)
                     .filter(db.Organization.id == args["organization_id"])
                 )
             # else: no filter if user can only view collaborations of own
             # organization: the arg 'organization_id' is then superfluous
 
+        if "algorithm_store_id" in args:
+            # If this algorithm store is available for all collaborations, no filter is
+            # needed
+            store = db.AlgorithmStore.get(args["algorithm_store_id"])
+            if not store:
+                return {
+                    "msg": f"Algorithm store with id={args['algorithm_store_id']} not found"
+                }, HTTPStatus.NOT_FOUND
+            elif store.collaboration_id is not None:
+                # filter on collaborations that have access to this algorithm store
+                q = q.join(db.AlgorithmStore).filter(
+                    db.AlgorithmStore.collaboration_id == db.Collaboration.id,
+                )
+
         # filter based on permissions
         if not self.r.v_glo.can():
             if self.r.v_org.can():
                 q = q.join(db.Organization, db.Collaboration.organizations).filter(
                     db.Collaboration.organizations.any(id=auth_org_id)
                 )
             else:
@@ -520,14 +539,25 @@
             name = data["name"]
             if collaboration.name != name and db.Collaboration.exists("name", name):
                 return {
                     "msg": f"Collaboration name '{name}' already exists!"
                 }, HTTPStatus.BAD_REQUEST
             collaboration.name = name
         if "organization_ids" in data:
+            # Users with permission to edit a collaboration at collaboration scope are
+            # not allowed to change the organizations of the collaboration: that would
+            # be a permission escalation as doing so may allow them to also do other
+            # actions for newly added organizations. Therefore, only users with global
+            # permission can alter the organizations in a collaboration.
+            if not self.r.e_glo.can():
+                return {
+                    "msg": "You lack the permission to change the organizations of a "
+                    "collaboration!"
+                }, HTTPStatus.UNAUTHORIZED
+            # set new organizations
             collaboration.organizations = [
                 db.Organization.get(org_id)
                 for org_id in data["organization_ids"]
                 if db.Organization.get(org_id)
             ]
         if "encrypted" in data:
             collaboration.encrypted = data["encrypted"]
```

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/common/input_schema.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/common/input_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/common/output_schema.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/common/output_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,16 +341,20 @@
 
 
 class AlgorithmStoreSchema(HATEOASModelSchema):
     class Meta:
         model = db.AlgorithmStore
 
     collaborations = fields.Function(
-        lambda obj: create_one_to_many_link(
-            obj, link_to="collaboration", link_from="algorithm_store_id"
+        lambda obj: (
+            create_one_to_many_link(
+                obj, link_to="collaboration", link_from="algorithm_store_id"
+            )
+            if obj.collaboration_id
+            else None
         )
     )
 
 
 class UserSchema(HATEOASModelSchema):
     class Meta:
         model = db.User
```

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/event.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/event.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/health.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,10 +61,10 @@
         # test DB
         db_ok = False
         try:
             g.session.execute("SELECT 1")
             db_ok = True
         except Exception as e:
             log.error("DB not responding")
-            log.debug(e)
+            log.exception(e)
 
         return {"database": db_ok}, HTTPStatus.OK
```

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/node.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/organization.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/port.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/recover.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/recover.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         account_name = username or email
         log.info(
             "Someone requested password recovery for non-existing account '%s'",
             account_name,
         )
         return
 
-    log.debug("Password reset requested for '%s'", user.username)
+    log.info("Password reset requested for '%s'", user.username)
 
     # check that email has not already been sent recently
     email_sent_recently = user.last_email_recover_password_sent and (
         dt.datetime.now()
         < user.last_email_recover_password_sent
         + dt.timedelta(minutes=minutes_between_password_reset_emails)
     )
@@ -525,15 +525,15 @@
                 "errors": errors,
             }, HTTPStatus.BAD_REQUEST
 
         old_password = body.get("current_password")
         new_password = body.get("new_password")
 
         user = g.user
-        log.debug(f"Changing password for user {user.id}")
+        log.info(f"Changing password for user {user.id}")
 
         # check if the old password is correct
         pw_correct = user.check_password(old_password)
         if not pw_correct:
             return {
                 "msg": "Your current password is not correct!"
             }, HTTPStatus.UNAUTHORIZED
```

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/role.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/rule.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/run.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/stats.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/study.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/task.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/token.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/token.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/ui/column.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/ui/column.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/user.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/version.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/vpn.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/vpn.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                 )
             }, HTTPStatus.INTERNAL_SERVER_ERROR
         except requests.ConnectionError as e:
             log.critical(
                 f"Node <{g.node.id}> tries to obtain a vpn config. "
                 "However the VPN server is unreachable!"
             )
-            log.debug(e)
+            log.exception(e)
             return {
                 "msg": "VPN server unreachable. Please contact your server"
                 " administrator"
             }, HTTPStatus.SERVICE_UNAVAILABLE
 
         return {"ovpn_config": ovpn_config}, HTTPStatus.OK
 
@@ -214,23 +214,23 @@
                 )
             }, HTTPStatus.INTERNAL_SERVER_ERROR
         except requests.ConnectionError as e:
             log.critical(
                 f"Node <{g.node.id}> tries to obtain a VPN config. "
                 "However the VPN server is unreachable!"
             )
-            log.debug(e)
+            log.exception(e)
             return {"msg": "VPN server unreachable"}, HTTPStatus.SERVICE_UNAVAILABLE
 
         return {"ovpn_config": ovpn_config}, HTTPStatus.OK
 
     def _is_server_configured(self) -> bool:
         """Check if vpn server is available in configuration"""
         if "vpn_server" not in self.config:
-            log.debug(
+            log.warning(
                 f"Node <{g.node.id}> tries to obtain a vpn config but "
                 "this server has not configured a VPN server!"
             )
             return False
         return True
```

### Comparing `vantage6-server-4.4.1/vantage6/server/resource/websocket_test.py` & `vantage6-server-4.5.0rc3/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/utils.py` & `vantage6-server-4.5.0rc3/vantage6/server/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6/server/websockets.py` & `vantage6-server-4.5.0rc3/vantage6/server/websockets.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.4.1/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-4.5.0rc3/vantage6_server.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.4.1
+Version: 4.5.0rc3
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
@@ -12,47 +12,51 @@
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
 
 <h3 align=center> A Privacy Enhancing Technology (PET) Operations platform</h3>
 <h3 align="center">
 
 <!-- Badges go here-->
+
 [![Release](https://github.com/vantage6/vantage6/actions/workflows/release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/release.yml)
 [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://badge.fury.io/py/vantage6)
 [![Unittests](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/unit_tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/vantage6/vantage6/badge.svg?branch=main)](https://coveralls.io/github/vantage6/vantage6?branch=main)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://www.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vantage6/vantage6&amp;utm_campaign=Badge_Grade)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2e60ac3b3f284620805f7399cba317be)](https://app.codacy.com/gh/vantage6/vantage6/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![DOI](https://zenodo.org/badge/492818831.svg)](https://zenodo.org/badge/latestdoi/492818831)
+
 </h3>
 
 <p align="center">
   <a href="#books-quickstart">Quickstart</a> •
   <a href="#project-structure">Project structure</a> •
   <a href="#gift_heart-join-the-community">Join the community</a> •
   <a href="#black_nib-references">References</a>
 </p>
 
+---
 
------------------------------------------------------------------------------------------------------
 This repository is contains all the **vantage6** infrastructure source code. The **vantage6** technology enables to manage and deploy privacy enhancing technologies like Federated Learning (FL) and Multi-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions, suggestions or just want to chat about federated learning: join our [Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel.
 
 ## Infrastructure overview
 
 ![Vantage6 architecture overview](docs/images/overview-infrastructure.png)
 
-*A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network.*
+_A High level overview of the vantage6 infrastructure. Vantage6 has both a client-server and peer-to-peer architecture. The client is used by the researcher to create (PET) computation requests. It is also used to manage users, organizations and collaborations. The server contains users, organizations, collaborations, tasks and their results. It provides a central access point for both the clients and nodes. The nodes have access to privacy sensitive data and handle computation requests retrieved from the server. Computation request are executed as separate containers on the node. These containers are connected to containers at other nodes by a VPN network._
 
 ## :books: Quickstart
 
 ### Requirements
+
 The **vantage6** infrastructure is delivered in Docker images. To run these images, you need to have [Docker](https://docs.docker.com/get-docker/) installed. To install the latest version of the vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we recommend using an environment manager like [mini-conda](https://docs.conda.io/en/latest/miniconda.html).
 
 Install the latest version of the vantage6 CLI by using:
+
 ```bash
 pip install vantage6
 ```
 
 This install the `v6` commands, which allows you to manage your nodes and servers. To view all available options, run:
 
 ```bash
@@ -79,16 +83,16 @@
 
 # View server logs
 v6 server attach
 ```
 
 From here you can use the [vantage6-client](https://pypi.org/project/vantage6-client) to interact with the server. The demo network has a pre-configured organization with the following credentials:
 
-* Username: `org_1-admin`
-* Password: `password`
+- Username: `org_1-admin`
+- Password: `password`
 
 For example, you can create a new organization by running:
 
 ```python
 from vantage6.client import Client
 
 client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
@@ -106,69 +110,74 @@
 ```
 
 You can find more (user) documentation at [readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai)
 
 ## Project structure
 
 ### PYPI packages
+
 This repository is home to 6 PyPi packages:
 
-* [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
-* [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
-* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
-* [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
-* [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
-* [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
-* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
-* [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
+- [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
+- [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+- [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
+- [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
+- [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+- [vantage6-algorithm-store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store application package_
+- [vantage6-common](https://pypi.org/project/vantage6-common) -> _Package with common vantage6 functions_
+- [vantage6-backend-common](https://pypi.org/project/vantage6-backend-common) -> _Package with functions common to central server and algorithm store_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 This repository also hosts the code for the vantage6 user interface (UI). The UI
 is an Angular web application that can be used to interact with the vantage6 server
 easily.
 
 ### Docker images
+
 The vantage6 infrastructure is delivered in Docker images. All Docker images are stored in our private [Harbor](https://goharbor.io/) registry. The most important images are:
 
-* `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
-* `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
-* `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
-* `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
+- `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application Docker image_
+- `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server application Docker image_
+- `harbor2.vantage6.ai/infrastructure/ui:VERSION` -> _User interface Docker image_
+- `harbor2.vantage6.ai/infrastructure/algorithm-store:VERSION` -> _Algorithm store Docker image_
 
 with `VERSION` being the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or `4.1.0rc0`.
 
 Several other images are used to support the infrastructure:
 
-* `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
-* `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
-* `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
-* `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
-* `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
-* `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
+- `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image for the infrastructure_
+- `harbor2.vantage6.ai/infrastructure/squid:VERSION` -> _Squid proxy image used for the whitelisting service_
+- `harbor2.vantage6.ai/infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_
+- `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect to the VPN_
+- `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN image used for initialization_
+- `harbor2.vantage6.ai/infrastructure/ssh-tunnel` -> _SSH tunnel image used for connecting algorithms to external services_
 
 And finally there are some images released for algorithm development:
 
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
-* `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base image for algorithm development_
+- `harbor2.vantage6.ai/infrastructure/algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI algorithm development_
 
 ## :gift_heart: Join the community!
+
 We hope to continue developing, improving, and supporting **vantage6** with the help of the federated learning community. If you are interested in contributing, first of all, thank you! Second, please take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/devops/contribute.html)
 
 <a href="https://github.com/vantage6/vantage6/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=vantage6/vantage6" />
 </a>
 
 ## :black_nib: References
+
 If you are using **vantage6**, please cite this repository as well as the accompanying papers as follows:
 
-> * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
-> * A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
-> * D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+> - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX.
+> - A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse. VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)]
+> - D. Smits\*, B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An Improved Infrastructure for Privacy-Preserving Analysis of Patient Data, Proceedings of the International Conference of Informatics, Management, and Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https://arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://ebooks.iospress.nl/volumearticle/60190)]
+
+---
 
------------------------------------------------------------------------------------------------------
 <p align="center">
   <a href="https://vantage6.ai">vantage6.ai</a> •
   <a href="https://discord.gg/yAyFf6Y">Discord</a> •
   <a href="https://vantage6.discourse.group/">Discourse</a> •
   <a href="https://docs.vantage6.ai">User documentation</a> •
 </p>
```

#### html2text {}

```diff
@@ -1,46 +1,45 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.4.1 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.5.0rc3 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
 bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66)) [[!![[UUnniitttteessttss]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//
    aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//
     vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//uunniitt__tteessttss..yymmll)) [[!![[CCoovveerraaggee SSttaattuuss]]((hhttttppss::////
  ccoovveerraallllss..iioo//rreeppooss//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66//bbaaddggee..ssvvgg??bbrraanncchh==mmaaiinn))]]((hhttttppss::////
  ccoovveerraallllss..iioo//ggiitthhuubb//vvaannttaaggee66//vvaannttaaggee66??bbrraanncchh==mmaaiinn)) [[!![[CCooddaaccyy BBaaddggee]]((hhttttppss::////
 aapppp..ccooddaaccyy..ccoomm//pprroojjeecctt//bbaaddggee//GGrraaddee//22ee6600aacc33bb33ff228844662200880055ff77339999ccbbaa331177bbee))]]((hhttttppss::////
-                     wwwwww..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
-   ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==ggiitthhuubb..ccoomm&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==vvaannttaaggee66//
-   vvaannttaaggee66&&uuttmm__ccaammppaaiiggnn==BBaaddggee__GGrraaddee)) [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//DDOOII//
-   1100..55228811//zzeennooddoo..77338822660022..ssvvgg))]]((hhttttppss::////ddooii..oorrgg//1100..55228811//zzeennooddoo..77338822660022)) ********
+                     aapppp..ccooddaaccyy..ccoomm//gghh//vvaannttaaggee66//vvaannttaaggee66//
+ddaasshhbbooaarrdd??uuttmm__ssoouurrccee==gghh&&uuttmm__mmeeddiiuumm==rreeffeerrrraall&&uuttmm__ccoonntteenntt==&&uuttmm__ccaammppaaiiggnn==BBaaddggee__ggrraaddee))
+  [[!![[DDOOII]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//449922881188883311..ssvvgg))]]((hhttttppss::////zzeennooddoo..oorrgg//bbaaddggee//
+                           llaatteessttddooii//449922881188883311)) ********
     _Q_u_i_c_k_s_t_a_r_t â¢ _P_r_o_j_e_c_t_ _s_t_r_u_c_t_u_r_e â¢ _J_o_i_n_ _t_h_e_ _c_o_m_m_u_n_i_t_y â¢ _R_e_f_e_r_e_n_c_e_s
--------------------------------------------------------------------------------
----------------------- This repository is contains all the **vantage6**
-infrastructure source code. The **vantage6** technology enables to manage and
-deploy privacy enhancing technologies like Federated Learning (FL) and Multi-
-Party Computation (MPC). Please visit our [website (vantage6.ai)](https://
-vantage6.ai) to learn more! You can find more (user) documentation at
-[readthedocs (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
-questions, suggestions or just want to chat about federated learning: join our
-[Discord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+--- This repository is contains all the **vantage6** infrastructure source
+code. The **vantage6** technology enables to manage and deploy privacy
+enhancing technologies like Federated Learning (FL) and Multi-Party Computation
+(MPC). Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn
+more! You can find more (user) documentation at [readthedocs
+(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
+suggestions or just want to chat about federated learning: join our [Discord
+(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
 Infrastructure overview ![Vantage6 architecture overview](docs/images/overview-
-infrastructure.png) *A High level overview of the vantage6 infrastructure.
+infrastructure.png) _A High level overview of the vantage6 infrastructure.
 Vantage6 has both a client-server and peer-to-peer architecture. The client is
 used by the researcher to create (PET) computation requests. It is also used to
 manage users, organizations and collaborations. The server contains users,
 organizations, collaborations, tasks and their results. It provides a central
 access point for both the clients and nodes. The nodes have access to privacy
 sensitive data and handle computation requests retrieved from the server.
 Computation request are executed as separate containers on the node. These
-containers are connected to containers at other nodes by a VPN network.* ## :
+containers are connected to containers at other nodes by a VPN network._ ## :
 books: Quickstart ### Requirements The **vantage6** infrastructure is delivered
 in Docker images. To run these images, you need to have [Docker](https://
 docs.docker.com/get-docker/) installed. To install the latest version of the
 vantage6 CLI, you need to have [Python](https://www.python.org/downloads/), we
 recommend using an environment manager like [mini-conda](https://docs.conda.io/
 en/latest/miniconda.html). Install the latest version of the vantage6 CLI by
 using: ```bash pip install vantage6 ``` This install the `v6` commands, which
@@ -49,75 +48,74 @@
 using: ```bash v6 dev create-demo-network ``` This creates a local network with
 a server and two nodes. You can start the network by running: ```bash v6 dev
 start-demo-network ``` This will start the server and nodes in the background.
 You can view the logs by running: ```bash # View node logs v6 node attach #
 View server logs v6 server attach ``` From here you can use the [vantage6-
 client](https://pypi.org/project/vantage6-client) to interact with the server.
 The demo network has a pre-configured organization with the following
-credentials: * Username: `org_1-admin` * Password: `password` For example, you
+credentials: - Username: `org_1-admin` - Password: `password` For example, you
 can create a new organization by running: ```python from vantage6.client import
 Client client = Client('http://127.0.0.1', 5000, '/api', log_level='debug')
 client.authenticate('org_1-admin', 'password') client.setup_encryption(None)
 client.organization.create( name='My organization', address1='My address',
 address2='My address', zipcode='1234AB', country='The Netherlands', domain='my-
 organization.com' ) ``` You can find more (user) documentation at [readthedocs
 (docs.vantage6.ai)](https://docs.vantage6.ai) ## Project structure ### PYPI
-packages This repository is home to 6 PyPi packages: * [vantage6](https://
-pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
+packages This repository is home to 6 PyPi packages: - [vantage6](https://
+pypi.org/project/vantage6) -> _CLI for managing node and server instances_ -
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+for interacting with the vantage6-server_ - [vantage6-algorithm-tools](https://
 pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
-algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
-node) -> _Node application package_ * [vantage6-server](https://pypi.org/
-project/vantage6-server) -> _Server application package_ * [vantage6-algorithm-
+algorithm development_ - [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ - [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ - [vantage6-algorithm-
 store](https://pypi.org/project/vantage6-algorithm-store) -> _Algorithm store
-application package_ * [vantage6-common](https://pypi.org/project/vantage6-
-common) -> _Package with common vantage6 functions_ * [vantage6-backend-common]
+application package_ - [vantage6-common](https://pypi.org/project/vantage6-
+common) -> _Package with common vantage6 functions_ - [vantage6-backend-common]
 (https://pypi.org/project/vantage6-backend-common) -> _Package with functions
 common to central server and algorithm store_ **Note that when using vantage6
 you do not install the _server_ and _node_ packages. These are delivered to you
 in Docker images.** This repository also hosts the code for the vantage6 user
 interface (UI). The UI is an Angular web application that can be used to
 interact with the vantage6 server easily. ### Docker images The vantage6
 infrastructure is delivered in Docker images. All Docker images are stored in
 our private [Harbor](https://goharbor.io/) registry. The most important images
-are: * `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
-Docker image_ * `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
-application Docker image_ * `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
-> _User interface Docker image_ * `harbor2.vantage6.ai/infrastructure/
+are: - `harbor2.vantage6.ai/infrastructure/node:VERSION` -> _Node application
+Docker image_ - `harbor2.vantage6.ai/infrastructure/server:VERSION` -> _Server
+application Docker image_ - `harbor2.vantage6.ai/infrastructure/ui:VERSION` -
+> _User interface Docker image_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-store:VERSION` -> _Algorithm store Docker image_ with `VERSION` being
 the full semantic version of the vantage6 infrastructure, e.g. `4.0.0` or
-`4.1.0rc0`. Several other images are used to support the infrastructure: *
+`4.1.0rc0`. Several other images are used to support the infrastructure: -
 `harbor2.vantage6.ai/infrastructure/infrastructure-base:VERSION` -> _Base image
-for the infrastructure_ * `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
-> _Squid proxy image used for the whitelisting service_ * `harbor2.vantage6.ai/
-infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ *
+for the infrastructure_ - `harbor2.vantage6.ai/infrastructure/squid:VERSION` -
+> _Squid proxy image used for the whitelisting service_ - `harbor2.vantage6.ai/
+infrastructure/alpine` -> _Alpine image used for vpn traffic forwarding_ -
 `harbor2.vantage6.ai/infrastructure/vpn-client` -> _VPN image used to connect
-to the VPN_ * `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
-image used for initialization_ * `harbor2.vantage6.ai/infrastructure/ssh-
+to the VPN_ - `harbor2.vantage6.ai/infrastructure/vpn-configurator` -> _VPN
+image used for initialization_ - `harbor2.vantage6.ai/infrastructure/ssh-
 tunnel` -> _SSH tunnel image used for connecting algorithms to external
 services_ And finally there are some images released for algorithm development:
-* `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
-image for algorithm development_ * `harbor2.vantage6.ai/infrastructure/
+- `harbor2.vantage6.ai/infrastructure/algorithm-base:MAJOR.MINOR` -> _Base
+image for algorithm development_ - `harbor2.vantage6.ai/infrastructure/
 algorithm-ohdsi-base:MAJOR.MINOR` -> _Extended algorithm base image for OHDSI
 algorithm development_ ## :gift_heart: Join the community! We hope to continue
 developing, improving, and supporting **vantage6** with the help of the
 federated learning community. If you are interested in contributing, first of
 all, thank you! Second, please take a look at our [contributing guidelines]
 (https://docs.vantage6.ai/en/main/devops/contribute.html) _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_v_a_n_t_a_g_e_6_/_v_a_n_t_a_g_e_6_]## :black_nib: References If you are
 using **vantage6**, please cite this repository as well as the accompanying
-papers as follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
+papers as follows: > - F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6.
 Available at https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. >
-* A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
+- A. Moncada-Torres, F. Martin, M. Sieswerda, J. van Soest, G. Gelijnse.
 VANTAGE6: an open source priVAcy preserviNg federaTed leArninG infrastructurE
 for Secure Insight eXchange. AMIA Annual Symposium Proceedings, 2020, p. 870-
 877. [[BibTeX](https://arturomoncadatorres.com/bibtex/moncada-
-torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > * D. Smits\*,
+torres2020vantage6.txt), [PDF](https://vantage6.ai/vantage6/)] > - D. Smits\*,
 B. van Beusekom\*, F. Martin, L. Veen, G. Geleijnse, A. Moncada-Torres, An
 Improved Infrastructure for Privacy-Preserving Analysis of Patient Data,
 Proceedings of the International Conference of Informatics, Management, and
 Technology in Healthcare (ICIMTH), vol. 25, 2022, p. 144-147. [[BibTeX](https:/
 /arturomoncadatorres.com/bibtex/smits2022improved.txt), [PDF](https://
-ebooks.iospress.nl/volumearticle/60190)] --------------------------------------
----------------------------------------------------------------
+ebooks.iospress.nl/volumearticle/60190)] ---
        _v_a_n_t_a_g_e_6_._a_i â¢ _D_i_s_c_o_r_d â¢ _D_i_s_c_o_u_r_s_e â¢ _U_s_e_r_ _d_o_c_u_m_e_n_t_a_t_i_o_n â¢
```

### Comparing `vantage6-server-4.4.1/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-4.5.0rc3/vantage6_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

