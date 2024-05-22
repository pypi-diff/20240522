# Comparing `tmp/firexapp-5.4.7.tar.gz` & `tmp/firexapp-5.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firexapp-5.4.7.tar", last modified: Thu Sep 21 21:13:52 2023, max compression
+gzip compressed data, was "firexapp-5.4.9.tar", last modified: Tue Nov 14 20:38:33 2023, max compression
```

## Comparing `firexapp-5.4.7.tar` & `firexapp-5.4.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.259469 firexapp-5.4.7/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2023-09-21 21:13:36.000000 firexapp-5.4.7/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2023-09-21 21:13:36.000000 firexapp-5.4.7/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      894 2023-09-21 21:13:52.259469 firexapp-5.4.7/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2023-09-21 21:13:36.000000 firexapp-5.4.7/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2023-09-21 21:13:36.000000 firexapp-5.4.7/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.260469 firexapp-5.4.7/firexapp/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-09-21 21:13:52.260469 firexapp-5.4.7/firexapp/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7425 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/application.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.250469 firexapp-5.4.7/firexapp/broker_manager/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      699 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/broker_manager/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/broker_manager/broker_factory.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13693 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/broker_manager/redis_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13246 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/celery_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6680 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/common.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/discovery.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.251469 firexapp-5.4.7/firexapp/engine/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/engine/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/engine/celery.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4667 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/engine/default_celery_config.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7194 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/engine/logging.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.252469 firexapp-5.4.7/firexapp/events/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/events/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4726 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/events/broker_event_consumer.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    14847 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/events/event_aggregator.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3571 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/events/model.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/fileregistry.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    21959 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/firex_subprocess.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/info.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11513 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/plugins.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.252469 firexapp-5.4.7/firexapp/reporters/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/reporters/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6049 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/reporters/json_reporter.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.255469 firexapp-5.4.7/firexapp/submit/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    10102 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/arguments.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5627 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/console.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/install_configs.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/report_trigger.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5423 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/reporting.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9662 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/shutdown.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    32721 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/submit.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1576 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/tracking_service.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4612 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/submit/uid.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.256469 firexapp-5.4.7/firexapp/tasks/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/tasks/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/tasks/core_tasks.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/tasks/example.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3687 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/tasks/root_tasks.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.258469 firexapp-5.4.7/firexapp/testing/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/testing/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4360 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/testing/config_base.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    12671 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/testing/config_interpreter.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/testing/coverage_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3365 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/testing/pydev_debug_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7258 2023-09-21 21:13:36.000000 firexapp-5.4.7/firexapp/testing/test_infra.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-09-21 21:13:52.249469 firexapp-5.4.7/firexapp.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      894 2023-09-21 21:13:52.000000 firexapp-5.4.7/firexapp.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2023-09-21 21:13:52.000000 firexapp-5.4.7/firexapp.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-09-21 21:13:52.000000 firexapp-5.4.7/firexapp.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      190 2023-09-21 21:13:52.000000 firexapp-5.4.7/firexapp.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      201 2023-09-21 21:13:52.000000 firexapp-5.4.7/firexapp.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        9 2023-09-21 21:13:52.000000 firexapp-5.4.7/firexapp.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-09-21 21:13:52.000000 firexapp-5.4.7/firexapp.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2023-09-21 21:13:52.260469 firexapp-5.4.7/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1731 2023-09-21 21:13:36.000000 firexapp-5.4.7/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-09-21 21:13:36.000000 firexapp-5.4.7/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.102075 firexapp-5.4.9/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2023-11-14 20:38:17.000000 firexapp-5.4.9/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2023-11-14 20:38:17.000000 firexapp-5.4.9/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      894 2023-11-14 20:38:33.102075 firexapp-5.4.9/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2023-11-14 20:38:17.000000 firexapp-5.4.9/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2023-11-14 20:38:17.000000 firexapp-5.4.9/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.103075 firexapp-5.4.9/firexapp/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-11-14 20:38:33.103075 firexapp-5.4.9/firexapp/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7425 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/application.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.093075 firexapp-5.4.9/firexapp/broker_manager/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      699 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/broker_manager/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/broker_manager/broker_factory.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13693 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/broker_manager/redis_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13246 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/celery_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6680 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/common.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/discovery.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.094075 firexapp-5.4.9/firexapp/engine/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/engine/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/engine/celery.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4667 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/engine/default_celery_config.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7194 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/engine/logging.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.095075 firexapp-5.4.9/firexapp/events/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/events/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4726 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/events/broker_event_consumer.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    14847 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/events/event_aggregator.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3968 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/events/model.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/fileregistry.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    21959 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/firex_subprocess.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/info.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11513 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/plugins.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.096075 firexapp-5.4.9/firexapp/reporters/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/reporters/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6091 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/reporters/json_reporter.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.099075 firexapp-5.4.9/firexapp/submit/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    10102 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/arguments.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5627 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/console.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7703 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/install_configs.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/report_trigger.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5423 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/reporting.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9694 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/shutdown.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    32721 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/submit.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1576 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/tracking_service.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4804 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/submit/uid.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.100075 firexapp-5.4.9/firexapp/tasks/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/tasks/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/tasks/core_tasks.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6727 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/tasks/example.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3687 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/tasks/root_tasks.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.101075 firexapp-5.4.9/firexapp/testing/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/testing/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4360 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/testing/config_base.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    12671 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/testing/config_interpreter.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/testing/coverage_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3365 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/testing/pydev_debug_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7258 2023-11-14 20:38:17.000000 firexapp-5.4.9/firexapp/testing/test_infra.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-11-14 20:38:33.092074 firexapp-5.4.9/firexapp.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      894 2023-11-14 20:38:33.000000 firexapp-5.4.9/firexapp.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2023-11-14 20:38:33.000000 firexapp-5.4.9/firexapp.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-11-14 20:38:33.000000 firexapp-5.4.9/firexapp.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      190 2023-11-14 20:38:33.000000 firexapp-5.4.9/firexapp.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      201 2023-11-14 20:38:33.000000 firexapp-5.4.9/firexapp.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        9 2023-11-14 20:38:33.000000 firexapp-5.4.9/firexapp.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-11-14 20:38:33.000000 firexapp-5.4.9/firexapp.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2023-11-14 20:38:33.103075 firexapp-5.4.9/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1731 2023-11-14 20:38:17.000000 firexapp-5.4.9/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-11-14 20:38:17.000000 firexapp-5.4.9/versioneer.py
```

### Comparing `firexapp-5.4.7/LICENSE` & `firexapp-5.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/PKG-INFO` & `firexapp-5.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firexapp
-Version: 5.4.7
+Version: 5.4.9
 Summary: Core firex application libraries
 Home-page: https://github.com/FireXStuff/firexapp
 Author: Core FireX Team
 Author-email: firex-dev@gmail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `firexapp-5.4.7/fastentrypoints.py` & `firexapp-5.4.9/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/application.py` & `firexapp-5.4.9/firexapp/application.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/broker_manager/__init__.py` & `firexapp-5.4.9/firexapp/broker_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/broker_manager/broker_factory.py` & `firexapp-5.4.9/firexapp/broker_manager/broker_factory.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/broker_manager/redis_manager.py` & `firexapp-5.4.9/firexapp/broker_manager/redis_manager.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/celery_manager.py` & `firexapp-5.4.9/firexapp/celery_manager.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/common.py` & `firexapp-5.4.9/firexapp/common.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/discovery.py` & `firexapp-5.4.9/firexapp/discovery.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/engine/celery.py` & `firexapp-5.4.9/firexapp/engine/celery.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/engine/default_celery_config.py` & `firexapp-5.4.9/firexapp/engine/default_celery_config.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/engine/logging.py` & `firexapp-5.4.9/firexapp/engine/logging.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/events/broker_event_consumer.py` & `firexapp-5.4.9/firexapp/events/broker_event_consumer.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/events/event_aggregator.py` & `firexapp-5.4.9/firexapp/events/event_aggregator.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/events/model.py` & `firexapp-5.4.9/firexapp/events/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,15 +83,38 @@
 TASK_COLUMN_NAMES = [tc.value for tc in TaskColumn]
 
 
 def get_task_data(input_dict):
     return {k: v for k, v in input_dict.items() if k in TASK_COLUMN_NAMES}
 
 
-FireXTask = namedtuple('FireXTask', [tc.value for tc in TaskColumn])
+FireXTask = namedtuple('FireXTask', [
+    # MUST BE SAME ORDER AS TaskColumn
+    "uuid",
+    "firex_id",
+    "chain_depth",
+    "firex_bound_args",
+    "firex_result",
+    "firex_default_bound_args",
+    "from_plugin",
+    "hostname",
+    "logs_url",
+    "long_name",
+    "name",
+    "actual_runtime",
+    "first_started",
+    "parent_id",
+    "retries",
+    "state",
+    "task_num",
+    "utcoffset",
+    "exception",
+    "traceback",
+    'exception_cause_uuid',
+])
 
 
 def is_chain_exception(task):
     return task.exception and task.exception.strip().startswith(ChainInterruptedException.__name__)
 
 
 def get_chain_exception_child_uuid(task):
```

### Comparing `firexapp-5.4.7/firexapp/fileregistry.py` & `firexapp-5.4.9/firexapp/fileregistry.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/firex_subprocess.py` & `firexapp-5.4.9/firexapp/firex_subprocess.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/info.py` & `firexapp-5.4.9/firexapp/info.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/plugins.py` & `firexapp-5.4.9/firexapp/plugins.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/reporters/json_reporter.py` & `firexapp-5.4.9/firexapp/reporters/json_reporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import getpass
 from socket import gethostname
 from dataclasses import dataclass, fields
-from typing import List, Dict, Optional
+from typing import List, Dict, Optional, Any
 
 from firexapp.application import get_app_tasks
 from firexapp.common import silent_mkdir, create_link
 from firexkit.result import get_results
 from firexkit.task import convert_to_serializable
 from celery.utils.log import get_task_logger
 from firexapp.engine.celery import app
@@ -19,16 +19,17 @@
     completed: bool
     chain: List[str]
     firex_id: str
     logs_path: str
     submission_host: str
     submission_dir: str
     submission_cmd: List[str]
-    viewers: Dict[str, str]
-    results: Optional[Dict] = None
+    viewers: dict[str, str]
+    inputs: dict[str, Any]
+    results: Optional[dict[str, Any]] = None
     revoked: bool = False
 
 
 class FireXJsonReportGenerator:
     formatters = ('json',)
 
     reporter_dirname = 'json_reporter'
```

### Comparing `firexapp-5.4.7/firexapp/submit/arguments.py` & `firexapp-5.4.9/firexapp/submit/arguments.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/submit/console.py` & `firexapp-5.4.9/firexapp/submit/console.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/submit/install_configs.py` & `firexapp-5.4.9/firexapp/submit/install_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from firexkit.resources import get_packaged_install_config_path
 from firexapp.submit.uid import Uid
 from firexapp.common import render_template
 
 INSTALL_CONFIGS_ENV_NAME = 'firex_install_config'
 INSTALL_CONFIGS_RUN_BASENAME = 'install-configs.json'
 
+
 class FireXViewerTemplates(NamedTuple):
-    viewer_base: str = ""
+    viewer_base: Optional[str] = ""
     run_path_template: str = ""
     task_path_template: str = ""
     run_logs_root_path_template: str = ""
     run_logs_entry_path_template: str = ""
 
 
 # Data-only representation of the config. This is expected to EXACTLY reflect the contents of the config file.
```

### Comparing `firexapp-5.4.7/firexapp/submit/report_trigger.py` & `firexapp-5.4.9/firexapp/submit/report_trigger.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/submit/reporting.py` & `firexapp-5.4.9/firexapp/submit/reporting.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/submit/shutdown.py` & `firexapp-5.4.9/firexapp/submit/shutdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from celery import Celery
 import redis.exceptions
 import kombu.exceptions
 
 from firexapp.celery_manager import CeleryManager
 from firexapp.submit.uid import Uid
 from firexapp.broker_manager.broker_factory import BrokerFactory, REDIS_BIN_ENV
-from firexkit.inspect import get_active, get_revoked, get_active_queues
 from firexapp.common import qualify_firex_bin, select_env_vars
+from firexkit.inspect import get_active, get_revoked, get_active_queues
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_CELERY_SHUTDOWN_TIMEOUT = 5 * 60
 MaybeCeleryActiveTasks = namedtuple('MaybeCeleryActiveTasks', ['celery_read_success', 'active_tasks'])
 
 
 def _launch_shutdown_subprocess(shutdown_cmd: list[str]) -> int:
     shutdown_subprocess_env = select_env_vars([REDIS_BIN_ENV, 'PATH'])
     try:
-        import detach
+        import detach # noqa
     except ModuleNotFoundError:
         # don't break old installs that don't have detach
         return subprocess.Popen(
             shutdown_cmd,
             close_fds=True,
             env=shutdown_subprocess_env,
             preexec_fn=os.setpgrp,
@@ -87,16 +87,16 @@
     # Note: get_active can hang in celery/kombu library if broker is down.
     # Checking for broker.is_alive() is an attempt to prevent that, but note
     # the broker can theoretically die between that call and the get_active() call.
     if not broker.is_alive():
         return None
     try:
         return inspect_fn(inspect_retry_timeout=4, celery_app=celery_app, **kwargs)
-    except (redis.exceptions.ConnectionError, kombu.exceptions.DecodeError) as e:
-        logger.warning(e)
+    except (redis.exceptions.ConnectionError, kombu.exceptions.DecodeError) as ex:
+        logger.warning(ex)
         return None
 
 
 def get_active_broker_safe(broker, celery_app):
     return _inspect_broker_safe(get_active, broker, celery_app,
                                 # shutdown can't deserialize task args because it doesn't know about many classes
                                 # (e.g. FireXUid), so set active(safe=True)
@@ -157,16 +157,18 @@
         revoke_retries += 1
 
     if not maybe_active_tasks.celery_read_success:
         logger.info("Failed to read active tasks from celery. May shutdown with unrevoked tasks.")
     elif len(maybe_active_tasks.active_tasks) == 0:
         logger.info("Confirmed no active tasks after revoke.")
     elif revoke_retries >= max_revoke_retries:
-        logger.warning("Exceeded max revoke retry attempts, %s active tasks may not be revoked."
-                       % len(maybe_active_tasks.active_tasks))
+        t_count = len(maybe_active_tasks.active_tasks)
+        logger.warning(
+            f"Exceeded max revoke retry attempts, {t_count} active tasks may not be revoked."
+        )
 
 
 def init():
     parser = argparse.ArgumentParser()
     parser.add_argument("--logs_dir", help="Logs directory for the firexapp run to shutdown.",
                         required=True)
     parser.add_argument("--reason", help="A reason that will be logged for clarity.",
```

### Comparing `firexapp-5.4.7/firexapp/submit/submit.py` & `firexapp-5.4.9/firexapp/submit/submit.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/submit/tracking_service.py` & `firexapp-5.4.9/firexapp/submit/tracking_service.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/submit/uid.py` & `firexapp-5.4.9/firexapp/submit/uid.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,19 +94,25 @@
     def get_resources_path(cls, logs_dir):
         return os.path.join(logs_dir, cls._resources_dirname)
 
     @property
     def resources_dir(self):
         return self.get_resources_path(self.logs_dir)
 
-    def create_logs_dir(self):
-        path = os.path.join(self.base_logging_dir, self.identifier)
-        os.makedirs(path)
+    def _create_logs_dir_from_base(self, base_logging_dir):
+        path = os.path.join(base_logging_dir, self.identifier)
+        try:
+            os.makedirs(path)
+        except FileExistsError:
+            pass
         return path
 
+    def create_logs_dir(self):
+        return self._create_logs_dir_from_base(self.base_logging_dir)
+
     def create_debug_dir(self):
         path = os.path.join(self.logs_dir, self.debug_dirname)
         try:
             os.makedirs(path)
         except FileExistsError:
             # Could have been created by other dependencies (e.g. redis)
             pass
```

### Comparing `firexapp-5.4.7/firexapp/tasks/core_tasks.py` & `firexapp-5.4.9/firexapp/tasks/core_tasks.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/tasks/example.py` & `firexapp-5.4.9/firexapp/tasks/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 from getpass import getuser
 import time
+from typing import Optional
 
 from firexkit.argument_conversion import SingleArgDecorator
 from firexkit.chain import InjectArgs, returns
 from firexkit.task import FireXTask, flame, flame_collapse
 
 from firexapp.engine.celery import app
 from firexapp.submit.arguments import InputConverter
 from firexapp.tasks.core_tasks import CopyBogKeys
 
 
 @app.task
-def nop():
+def nop() -> None:
     return
 
 
 @app.task
-def sleep(sleep=None):
+def sleep(sleep: Optional[int] = None) -> None:
     if sleep:
         time.sleep(int(sleep))
     return
 
 
 @app.task(returns='username')
-def getusername():
+def getusername() -> str:
     return getuser()
 
 
 # The @app.task() makes this normal python function a FireX Service.
 @app.task(returns=['greeting'], flame=['greeting'])
-def greet(name=getuser()):
+def greet(name: str = getuser()) -> str:
     assert len(name) > 1, "Cannot greet a name with 1 or fewer characters."
     return 'Hello %s!' % name
 
 
 # Setting bind=True makes the first argument received by the service 'self'. It's most commonly used to invoke
 # (enqueue) other services, but provides much more functionality as outlined here:
 @app.task(bind=True, returns=['guests_greeting'], flame=['guests_greeting'])
-def greet_guests(self: FireXTask, guests):
+def greet_guests(self: FireXTask, guests: list[str]) -> str:
     child_promises = []
     for guest in guests:
         # Create a Celery Signature, see: https://docs.celeryproject.org/en/latest/userguide/canvas.html#signatures
         greet_signature = greet.s(name=guest)
         # enqueue_child by default schedules the supplied signature for execution asynchronously and immediately
         # returns the newly created child result promise.
         child_promise = self.enqueue_child(greet_signature)
@@ -58,20 +59,24 @@
         greetings.append("And apologies to those not mentioned.")
 
     return ' '.join(greetings)
 
 
 @InputConverter.register
 @SingleArgDecorator('guests')
-def to_list(guests):
+def to_list(guests: str) -> list[str]:
     return guests.split(',')
 
 
 @app.task(returns=['amplified_message'])
-def amplify(to_amplify, upper=True, surround_str=None, underline_char=None, overline_char=None):
+def amplify(to_amplify: str,
+            upper: bool = True,
+            surround_str: Optional[str] = None,
+            underline_char: Optional[str] = None,
+            overline_char: Optional[str] = None) -> str:
     result = to_amplify
     if upper:
         result = to_amplify.upper()
     if surround_str:
         result = surround_str + result + surround_str
     centerline_len = len(result)
     if underline_char:
@@ -79,30 +84,30 @@
 
     if overline_char:
         result = (overline_char * centerline_len) + '\n' + result
 
     return result
 
 
-def _amplified_greeting_formatter(args_and_maybe_results):
+def _amplified_greeting_formatter(args_and_maybe_results: dict) -> str:
     # Since 'amplified_greeting' is the return value name, it isn't available to the formatter when the task is first
     # started. It will be available if the task completes successfully.
     if 'amplified_greeting' in args_and_maybe_results:
         br_as_nl = args_and_maybe_results["amplified_greeting"].replace('\n', '<br>')
         return f'<h1 style="font-family: monospace;">{br_as_nl}</h1>'
 
     # Since 'guests' is an input argument, it will always be available to the formatter, even before the service
     # has completed.
     return f'Planning to greet: {",".join(args_and_maybe_results["guests"])}'
 
 
 @app.task(bind=True, returns=['amplified_greeting'])
 @flame('*', _amplified_greeting_formatter)
 @flame_collapse({'greet_guests': 'descendants'})
-def amplified_greet_guests(self: FireXTask, guests):
+def amplified_greet_guests(self: FireXTask, guests: list[str]) -> str:
     # Nonsense failure case to illustrate flame HTML data when the service fails (i.e. no return value present).
     assert len(guests) > 1, "Only willing to amplify greeting for more than one guest."
 
     # Create a chain that can be enqueued. The greet_guests service will produce a guests_greeting,
     # which will then be delivered to amplify as its to_amplify argument.
     amplified_greet_guests_chain = InjectArgs(**self.abog) | greet_guests.s() | amplify.s(to_amplify='@guests_greeting')
 
@@ -138,15 +143,15 @@
     return results['amplified_greeting']
 
 
 # A contrived example showing how CopyBogKeys can be used to copy values in between chained services, preventing
 # data from being trampled when multiple services within a chain return values with the same name.
 # Of course, in practice, it's preferable to enqueue the multiple calls to greet separately.
 @app.task(bind=True, returns=['lee_greeting', 'tom_greeting'])
-def greet_lee_and_tom(self: FireXTask):
+def greet_lee_and_tom(self: FireXTask) -> (str, str):
     chain = (greet.s("Lee")
              | CopyBogKeys.s({'greeting': 'lee_greeting'})
              | greet.s("Tom"))
     results = self.enqueue_child_and_get_results(chain)
     # Lee's greeting has been copied to 'lee_greeting', so it's still accessible after Tom's greet has executed.
     lee_greeting = results['lee_greeting']
     # Tom's greeting still has the return name specified in the greet service.
```

### Comparing `firexapp-5.4.7/firexapp/tasks/root_tasks.py` & `firexapp-5.4.9/firexapp/tasks/root_tasks.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/testing/config_base.py` & `firexapp-5.4.9/firexapp/testing/config_base.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/testing/config_interpreter.py` & `firexapp-5.4.9/firexapp/testing/config_interpreter.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/testing/coverage_plugin.py` & `firexapp-5.4.9/firexapp/testing/coverage_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/testing/pydev_debug_plugin.py` & `firexapp-5.4.9/firexapp/testing/pydev_debug_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp/testing/test_infra.py` & `firexapp-5.4.9/firexapp/testing/test_infra.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/firexapp.egg-info/PKG-INFO` & `firexapp-5.4.9/firexapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firexapp
-Version: 5.4.7
+Version: 5.4.9
 Summary: Core firex application libraries
 Home-page: https://github.com/FireXStuff/firexapp
 Author: Core FireX Team
 Author-email: firex-dev@gmail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `firexapp-5.4.7/firexapp.egg-info/SOURCES.txt` & `firexapp-5.4.9/firexapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/setup.py` & `firexapp-5.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.4.7/versioneer.py` & `firexapp-5.4.9/versioneer.py`

 * *Files identical despite different names*

