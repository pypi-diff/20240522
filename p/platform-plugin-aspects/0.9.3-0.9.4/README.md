# Comparing `tmp/platform_plugin_aspects-0.9.3.tar.gz` & `tmp/platform_plugin_aspects-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform_plugin_aspects-0.9.3.tar", last modified: Thu May 16 19:47:21 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.9.4.tar", last modified: Wed May 22 17:00:25 2024, max compression
```

## Comparing `platform_plugin_aspects-0.9.3.tar` & `platform_plugin_aspects-0.9.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.931549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.931549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.931549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 19:47:21.000000 platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:47:21.935549 platform_plugin_aspects-0.9.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 19:47:21.939549 platform_plugin_aspects-0.9.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-16 19:47:18.000000 platform_plugin_aspects-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.387469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.387469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.387469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.387469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.383469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.383469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 17:00:25.000000 platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-22 17:00:25.391469 platform_plugin_aspects-0.9.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6997 2024-05-22 17:00:22.000000 platform_plugin_aspects-0.9.4/setup.py
```

### Comparing `platform_plugin_aspects-0.9.3/CHANGELOG.rst` & `platform_plugin_aspects-0.9.4/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.4 - 2024-05-16
+******************
+
+Fixes
+=====
+
+* Allow to serialize dates as strings in JSON.
+
 0.9.3 - 2024-05-15
 ******************
 
 Fixes
 =====
 
 * Change wording of the "go to Superset" link, and make it optional.
```

### Comparing `platform_plugin_aspects-0.9.3/LICENSE` & `platform_plugin_aspects-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/PKG-INFO` & `platform_plugin_aspects-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.9.3
+Version: 0.9.4
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,14 +272,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.4 - 2024-05-16
+******************
+
+Fixes
+=====
+
+* Allow to serialize dates as strings in JSON.
+
 0.9.3 - 2024-05-15
 ******************
 
 Fixes
 =====
 
 * Change wording of the "go to Superset" link, and make it optional.
```

### Comparing `platform_plugin_aspects-0.9.3/README.rst` & `platform_plugin_aspects-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/extensions/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,15 +67,14 @@
             "course_id": str(context.get("course_id")),
             "superset_guest_token_url": str(context.get("superset_guest_token_url")),
             "superset_url": str(context.get("superset_url")),
             "template_path_prefix": TEMPLATE_ABSOLUTE_PATH,
             "show_dashboard_link": show_dashboard_link,
         }
 
-        print(section_data)
         context["sections"].append(section_data)
         return {
             "context": context,
         }
 
     def resource_string(self, path):
         """Handy helper for getting resources from our kit."""
```

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,14 @@
         insert = (
             f"INSERT INTO {self.ch_runs_table} (run_id, event_type, extra) FORMAT CSV "
         )
 
         output = io.StringIO()
         writer = csv.writer(output)
         writer.writerow((self.run_id, event_type, json.dumps(extra)))
-        print(output.getvalue().encode("utf-8"))
 
         response = requests.post(
             url=self.ch_url,
             auth=self.ch_auth,
             params={"database": self.ch_database, "query": insert},
             data=output.getvalue().encode("utf-8"),
             timeout=self.ch_timeout_secs,
```

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,18 @@
         # Once the test has ended we will wait for the backend to drain the
         # backlog before exiting. This tracks the "in between" state.
         shutting_down = False
 
         while True:
             start = datetime.datetime.now()
             log.info(f"----------- {start} --------")
+            lag = None
 
             current_stats = {"clickhouse": self.get_clickhouse_stats()}
+            lag = -1
             if collect_redis_bus:
                 current_stats["redis_bus"] = self.get_redis_bus_stats()
                 lag = current_stats["redis_bus"]["lag"]
             elif collect_celery:
                 current_stats["celery"] = self.get_celery_stats()
                 lag = current_stats["celery"]["lag"]
             elif collect_kafka_bus:
```

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/common.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/serializers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,44 @@
 """Django serializers for the event_sink_clickhouse app."""
 
 import json
 import uuid
+from datetime import date, datetime
 
 from django.utils import timezone
+from pytz import UTC
 from rest_framework import serializers
 
 from platform_plugin_aspects.utils import get_model, get_tags_for_block
 
 
+class DateTimeJSONEncoder(json.JSONEncoder):
+    """JSON encoder aware of datetime.datetime and datetime.date objects"""
+
+    def default(self, obj):  # pylint: disable=arguments-renamed
+        """
+        Serialize datetime and date objects of iso format.
+
+        datetime objects are converted to UTC.
+        """
+
+        if isinstance(obj, datetime):
+            if obj.tzinfo is None:
+                # Localize to UTC naive datetime objects
+                obj = UTC.localize(obj)  # pylint: disable=no-value-for-parameter
+            else:
+                # Convert to UTC datetime objects from other timezones
+                obj = obj.astimezone(UTC)
+            return obj.isoformat()
+        elif isinstance(obj, date):
+            return obj.isoformat()
+
+        return super().default(obj)
+
+
 class BaseSinkSerializer(serializers.Serializer):  # pylint: disable=abstract-method
     """Base sink serializer for ClickHouse."""
 
     dump_id = serializers.SerializerMethodField()
     time_last_dumped = serializers.SerializerMethodField()
 
     class Meta:
@@ -144,12 +170,12 @@
             "effort": getattr(overview, "effort", ""),
             "enable_proctored_exams": getattr(overview, "enable_proctored_exams", ""),
             "entrance_exam_enabled": getattr(overview, "entrance_exam_enabled", ""),
             "external_id": getattr(overview, "external_id", ""),
             "language": getattr(overview, "language", ""),
             "tags": get_tags_for_block(overview.id),
         }
-        return json.dumps(json_fields)
+        return json.dumps(json_fields, cls=DateTimeJSONEncoder)
 
     def get_course_key(self, overview):
         """Return the course key as a string."""
         return str(overview.id)
```

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/urls.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/urls.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/utils.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/views.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/views.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects/xblock.py` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects/xblock.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/PKG-INFO` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.9.3
+Version: 0.9.4
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -272,14 +272,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+0.9.4 - 2024-05-16
+******************
+
+Fixes
+=====
+
+* Allow to serialize dates as strings in JSON.
+
 0.9.3 - 2024-05-15
 ******************
 
 Fixes
 =====
 
 * Change wording of the "go to Superset" link, and make it optional.
```

### Comparing `platform_plugin_aspects-0.9.3/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.9.4/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/requirements/constraints.txt` & `platform_plugin_aspects-0.9.4/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.9.3/setup.py` & `platform_plugin_aspects-0.9.4/setup.py`

 * *Files identical despite different names*

