# Comparing `tmp/googleads-housekeeper-0.1.0.dev8.tar.gz` & `tmp/googleads-housekeeper-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleads-housekeeper-0.1.0.dev8.tar", last modified: Tue Mar  5 18:37:19 2024, max compression
+gzip compressed data, was "googleads-housekeeper-0.1.0.dev9.tar", last modified: Sun Mar 10 22:12:14 2024, max compression
```

## Comparing `googleads-housekeeper-0.1.0.dev8.tar` & `googleads-housekeeper-0.1.0.dev9.tar`

### file list

```diff
@@ -1,62 +1,70 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1836 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1567 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev8/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5623 2024-03-04 20:04:31.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/legacy_adapter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9395 2024-03-05 18:33:53.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/notifications.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7008 2024-03-05 12:38:35.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/orm.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2279 2024-02-26 13:14:54.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/publisher.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5015 2024-03-04 20:03:22.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/repository.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6746 2024-02-20 11:24:33.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/bootstrap.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2913 2024-03-04 20:03:32.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/commands.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-03-04 19:36:44.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    17318 2024-03-04 19:57:46.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/exclusion_specification.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2398 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/execution.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2541 2024-03-04 19:36:44.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/rules_parser.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1964 2024-03-05 06:52:51.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/settings.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5161 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/task.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1492 2024-02-26 13:14:54.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/events.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1860 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/base_parser.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6131 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/external_entity_parser.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4132 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/website_parser.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10099 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/youtube_data_parser.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/placement_handler/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/placement_handler/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9495 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/placement_handler/entities.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3467 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/placement_handler/negative_list_verifier.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    30503 2024-03-05 12:07:39.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/placement_handler/placement_service.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1415 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/enums.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    16747 2024-03-05 12:32:36.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/handlers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2253 2024-02-26 13:14:54.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/messagebus.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6229 2024-03-05 12:32:48.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/unit_of_work.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5219 2024-03-04 20:03:39.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/views.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1836 2024-03-05 18:37:19.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2137 2024-03-05 18:37:19.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-03-05 18:37:19.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      307 2024-03-05 18:37:19.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       28 2024-03-05 18:37:19.000000 googleads-housekeeper-0.1.0.dev8/googleads_housekeeper.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1078 2024-03-05 18:37:09.000000 googleads-housekeeper-0.1.0.dev8/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-05 18:37:19.451981 googleads-housekeeper-0.1.0.dev8/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev8/tests/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2808 2024-03-04 20:04:40.000000 googleads-housekeeper-0.1.0.dev8/tests/conftest.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    13730 2024-03-04 19:57:46.000000 googleads-housekeeper-0.1.0.dev8/tests/test_exclusion_specification.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2093 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/tests/test_external_entity_parser.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5510 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/tests/test_external_parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5934 2024-03-04 20:04:40.000000 googleads-housekeeper-0.1.0.dev8/tests/test_handlers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1239 2024-02-26 13:14:54.000000 googleads-housekeeper-0.1.0.dev8/tests/test_legacy_adapters.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2941 2024-03-05 18:36:24.000000 googleads-housekeeper-0.1.0.dev8/tests/test_notifications.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3447 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/tests/test_placement_info_extractor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      976 2024-03-04 19:59:20.000000 googleads-housekeeper-0.1.0.dev8/tests/test_placements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2316 2024-03-04 19:56:37.000000 googleads-housekeeper-0.1.0.dev8/tests/test_rules_parser.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.069714 googleads-housekeeper-0.1.0.dev9/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1836 2024-03-10 22:12:14.069714 googleads-housekeeper-0.1.0.dev9/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1567 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev9/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.061715 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.065714 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5623 2024-03-07 09:18:31.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/legacy_adapter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     9395 2024-03-07 19:56:22.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/notifications.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7008 2024-03-07 19:56:22.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/orm.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2279 2024-02-26 13:14:54.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/publisher.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5015 2024-03-07 09:15:50.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/repository.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6746 2024-02-20 11:24:33.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/bootstrap.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.065714 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2913 2024-03-07 09:15:50.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/commands.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.065714 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-03-04 19:36:44.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1964 2024-03-07 19:40:42.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/_settings.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      591 2024-03-09 21:10:36.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/entity.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    17324 2024-03-07 20:01:53.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/exclusion_specification.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2398 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/execution.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3000 2024-03-06 19:56:04.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/rules_parser.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1091 2024-03-07 19:45:27.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/settings.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5171 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/task.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1492 2024-02-26 13:14:54.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/events.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.065714 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1930 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/base_parser.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6131 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/external_entity_parser.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4132 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/website_parser.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10099 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/youtube_data_parser.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.065714 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-03-07 20:01:53.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    14263 2024-03-10 21:17:40.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/entities.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3467 2024-03-07 20:01:53.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/negative_list_verifier.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    17334 2024-03-10 21:53:41.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/placement_excluder.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    12369 2024-03-10 21:47:20.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/placement_fetcher.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2167 2024-03-07 20:01:53.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/placement_info_extractor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8392 2024-03-10 21:54:17.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/placement_service.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.065714 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6229 2024-03-07 19:51:02.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/_unit_of_work.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1415 2024-03-07 20:01:53.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/enums.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    16396 2024-03-10 21:49:11.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/handlers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2253 2024-02-26 13:14:54.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/messagebus.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5347 2024-03-07 19:56:17.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/unit_of_work.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5271 2024-03-07 09:18:25.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/views.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.061715 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1836 2024-03-10 22:12:14.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2553 2024-03-10 22:12:14.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-03-10 22:12:14.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      307 2024-03-10 22:12:14.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       28 2024-03-10 22:12:14.000000 googleads-housekeeper-0.1.0.dev9/googleads_housekeeper.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-03-10 22:12:14.069714 googleads-housekeeper-0.1.0.dev9/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1093 2024-03-10 22:11:30.000000 googleads-housekeeper-0.1.0.dev9/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-10 22:12:14.069714 googleads-housekeeper-0.1.0.dev9/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-11-28 07:29:22.000000 googleads-housekeeper-0.1.0.dev9/tests/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2808 2024-03-07 09:18:31.000000 googleads-housekeeper-0.1.0.dev9/tests/conftest.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    13730 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/tests/test_exclusion_specification.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2093 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/tests/test_external_entity_parser.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5510 2024-03-06 19:56:10.000000 googleads-housekeeper-0.1.0.dev9/tests/test_external_parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5934 2024-03-07 09:18:31.000000 googleads-housekeeper-0.1.0.dev9/tests/test_handlers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1239 2024-02-26 13:14:54.000000 googleads-housekeeper-0.1.0.dev9/tests/test_legacy_adapters.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3141 2024-03-07 20:01:53.000000 googleads-housekeeper-0.1.0.dev9/tests/test_notifications.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10246 2024-03-10 15:40:33.000000 googleads-housekeeper-0.1.0.dev9/tests/test_placement_excluder.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6846 2024-03-08 16:40:46.000000 googleads-housekeeper-0.1.0.dev9/tests/test_placement_fetcher.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3461 2024-03-07 20:01:53.000000 googleads-housekeeper-0.1.0.dev9/tests/test_placement_info_extractor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3811 2024-03-08 08:22:18.000000 googleads-housekeeper-0.1.0.dev9/tests/test_placements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2316 2024-03-06 19:55:55.000000 googleads-housekeeper-0.1.0.dev9/tests/test_rules_parser.py
```

### Comparing `googleads-housekeeper-0.1.0.dev8/PKG-INFO` & `googleads-housekeeper-0.1.0.dev9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleads-housekeeper
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: gcp
```

### Comparing `googleads-housekeeper-0.1.0.dev8/README.md` & `googleads-housekeeper-0.1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/legacy_adapter.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/legacy_adapter.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/notifications.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/notifications.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/orm.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/publisher.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/publisher.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/adapters/repository.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/bootstrap.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/bootstrap.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/commands.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/commands.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/exclusion_specification.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/exclusion_specification.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         exclusion_type:
             Type of the parseable entity, depending on it additional data might
             be fetched from the repository.
     """
 
     def __init__(self,
                  expression: str,
-                 exclusion_type: enums.ExclusionTypeEnum | None = None) -> None:
+                 exclusion_type: enums.ExclusionTypeEnum) -> None:
         """Constructor for the class.
 
         Args:
             expression: Exclusion expression in a form of `name > value`.
             exclusion_type: Type of the exclusion.
         """
         elements = [
@@ -212,22 +212,14 @@
 
     def __init__(self, expression) -> None:
         super().__init__(
             expression=expression,
             exclusion_type=enums.ExclusionTypeEnum.YOUTUBE_VIDEO_INFO)
 
 
-class NullSpecificationEntry(BaseExclusionSpecificationEntry):
-    """Handles unsupported rules."""
-
-    def __init__(self, specification_type, expression):
-        super().__init__(type)
-        raise ValueError(f'Incorrect type of rule: {specification_type}')
-
-
 def create_exclusion_specification_entry(
         specification_type: str,
         condition: str) -> BaseExclusionSpecificationEntry:
     """Builds concrete specification entry class based on type.
 
     Args:
         specification_type: Type of desired specification entry.
@@ -240,15 +232,15 @@
         return AdsExclusionSpecificationEntry(condition)
     if specification_type == 'WEBSITE_INFO':
         return ContentExclusionSpecificationEntry(condition)
     if specification_type == 'YOUTUBE_CHANNEL_INFO':
         return YouTubeChannelExclusionSpecificationEntry(condition)
     if specification_type == 'YOUTUBE_VIDEO_INFO':
         return YouTubeVideoExclusionSpecificationEntry(condition)
-    return NullSpecificationEntry(specification_type, condition)
+    raise ValueError(f'Incorrect type of rule: {specification_type}')
 
 
 class ExclusionSpecification:
     """Verifies whether entities matches set of specification entries.
 
     Attributes:
         specifications: All specification entries within the specification.
@@ -411,27 +403,33 @@
             is_regular_query=is_regular_query,
             is_conversion_query=is_conversion_query,
             conversion_name=conversion_name,
             conversion_rules=conversion_rules)
 
     @classmethod
     def from_rules(
-            cls, parsed_rules: list[list[rules_parser.Rule]]
+            cls, parsed_rules: list[list[rules_parser.Rule]] | None
     ) -> ExclusionSpecification:
-        """Convert raw string rules into specifications."""
+        """Convert Exclusion rules into specifications."""
+        if not parsed_rules:
+            return ExclusionSpecification()
         specifications = []
         for rules in parsed_rules:
             specification_entry = []
             for rule in rules:
                 specification_entry.append(
                     create_exclusion_specification_entry(
                         rule.exclusion_type, rule.exclusion_rule))
             specifications.append(specification_entry)
         return ExclusionSpecification(specifications)
 
+    @classmethod
+    def from_expression(cls, rule_expression: str) -> ExclusionSpecification:
+        """Convert raw string rules into specifications."""
+        return ExclusionSpecification.from_rules(
+            rules_parser.generate_rules(rule_expression))
+
     def __eq__(self, other) -> bool:
         return self.specifications == other.specifications
 
     def __bool__(self) -> bool:
-        if not self.specifications:
-            return False
-        return len(self.specifications) > 0
+        return bool(self.specifications)
```

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/execution.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/execution.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/rules_parser.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/rules_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,26 @@
 class Rule:
     """Holds information on exclusion rule."""
     exclusion_type: str
     exclusion_rule: str
 
 
 def generate_rules(raw_rules: str | Sequence[str]) -> list[list[Rule]] | None:
-    """Convert raw string rules into list of Rules."""
+    """Convert raw string rules into list of Rules.
+
+    Rule as raw string can be expressed in an explicit
+    (`exclusion_type:exclusion_rule`), implicit (`exclusion_rule`) format.
+
+    Rules in each of these formats can be represented as sequence or a single
+    string. And-rules are separated by `AND` keyword or comma (`,`),
+    Or-rules are separated by `OR` keyword.
+
+    If `exclusion_type` is not specified for a given rule it's treated
+    as GOOGLE_ADS_INFO.
+    """
     if not raw_rules:
         return None
     rules: list[list[Rule]] = []
     default_exclusion_type = 'GOOGLE_ADS_INFO'
     if isinstance(raw_rules, str):
         raw_rules = _format_raw_rules(raw_rules)
     for rule in raw_rules:
@@ -58,14 +69,15 @@
                 Rule(exclusion_type.strip(), exclusion_rule.strip()))
         rules.append(rule_entry)
     return rules
 
 
 def _format_raw_rules(raw_rules: str) -> list[str]:
     """Applies formatting to raw string rule."""
-    # remove brackets
+    # Removes brackets.
     raw_rules = re.sub('[(|)]', '', raw_rules)
-    # add whitespace in front of operators
+    # Adds whitespace in front of operators.
     raw_rules = re.sub('([>|<|>=|<=|!=|=])', r' \1 ', raw_rules)
-    # split rules by OR operator
+    # Trims extra whitespace.
     raw_rules = re.sub(' +', ' ', raw_rules)
+    # Split rules by OR operator.
     return raw_rules.split(' OR ')
```

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/settings.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/_settings.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/core/task.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/core/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,34 +21,32 @@
 
 from croniter import croniter
 
 from googleads_housekeeper.services import enums
 
 
 class TaskStatus(enum.Enum):
-    """
-    An enumeration representing the status of a task.
+    """An enumeration representing the status of a task.
 
     Attributes:
         ACTIVE (int): Represents an active task.
         INACTIVE (int): Represents an inactive task.
-  """
+    """
     ACTIVE = 0
     INACTIVE = 1
 
 
 class TaskOutput(enum.Enum):
-    """
-    An enumeration representing the artifact/output options for a task.
+    """An enumeration representing the artifact/output options for a task.
 
     Attributes:
         NOTIFY (int): Output option to notify about the task.
         EXCLUDE (int): Output option to exclude the task.
         EXCLUDE_AND_NOTIFY (int): Output option to exclude the task and notify about it.
-  """
+    """
     NOTIFY = 1
     EXCLUDE = 2
     EXCLUDE_AND_NOTIFY = 3
 
 
 @dataclasses.dataclass
 class Task:
@@ -86,14 +84,18 @@
         """Ensures safe casting to proper enums."""
         self.output = self._cast_to_enum(TaskOutput, self.output)
         self.status = self._cast_to_enum(TaskStatus, self.status)
         self.exclusion_level = self._cast_to_enum(enums.ExclusionLevelEnum,
                                                   self.exclusion_level)
 
     def to_dict(self) -> dict:
+        """Convert class to dictionary.
+
+        Enum attributes of the class are represented as names.
+        """
         task_dict = {}
         for key, value in dataclasses.asdict(self).items():
             if hasattr(value, 'value'):
                 task_dict[key] = value.name
             else:
                 task_dict[key] = value
         return task_dict
@@ -121,17 +123,14 @@
 
     @property
     def end_date(self) -> str:
         """Returns formatted end_date."""
         return (datetime.datetime.now() - datetime.timedelta(
             days=int(self.from_days_ago))).date().strftime('%Y-%m-%d')
 
-    def get_start_end_date(self) -> tuple[str, str]:
-        return self.start_date, self.end_date
-
     @property
     def accounts(self) -> list[str]:
         """Returns formatted account list."""
         return self.customer_ids.split(',') if isinstance(
             self.customer_ids, str) else self.customer_ids
 
     @property
```

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/events.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/events.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/base_parser.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/base_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 class BaseParser(abc.ABC):
     """Base class for all external parsers."""
 
     @abc.abstractmethod
     def parse(self, placements: collections.abs.Sequence[str]) -> list[T]:
         """Parses provided placements.
 
+        Placement could be website URL, YouTube channel or video id.
+
         Args:
             placements: Sequence of placements identifiers.
         Returns:
             List of parsed entities in subclass *Info format.
         """
         raise NotImplementedError
```

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/external_entity_parser.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/external_entity_parser.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/website_parser.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/website_parser.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/external_parsers/youtube_data_parser.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/external_parsers/youtube_data_parser.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/placement_handler/entities.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/entities.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,58 +14,106 @@
 """Contains classes and function to work with Placements from Google Ads API."""
 from __future__ import annotations
 
 import dataclasses
 import datetime
 import uuid
 
-from gaarf import base_query
+import gaarf
 
+from googleads_housekeeper.domain.core import entity
 from googleads_housekeeper.services import enums
 
 
-class Placements(base_query.BaseQuery):
+class Placements(entity.ExcludableEntity):
     """Contains placement meta information and it's performance.
 
     Placements is a wrapper on BaseQuery that builds GAQL query (located in
     `query_text` attribute) based on provided and validated inputs.
+
+    Attributes:
+        query_text: Gaarf query to be sent to Google Ads API.
     """
 
     _today = datetime.datetime.today()
     _start_date = _today - datetime.timedelta(days=7)
     _end_date = _today - datetime.timedelta(days=1)
     _campaign_types = {c.name for c in enums.CampaignTypeEnum}
     _placement_types = {p.name for p in enums.PlacementTypeEnum}
     _non_excludable_placements = ('youtube.com', 'mail.google.com',
                                   'adsenseformobileapps.com')
     _non_supported_campaign_types = ('MULTI_CHANNEL',)
+    base_query_text = """
+        SELECT
+            customer.descriptive_name AS account_name,
+            customer.id AS customer_id,
+            campaign.id AS campaign_id,
+            campaign.name AS campaign_name,
+            campaign.advertising_channel_type AS campaign_type,
+            ad_group.id AS ad_group_id,
+            ad_group.name AS ad_group_name,
+            {placement_level_granularity}.{parent_url} AS base_url,
+            {placement_level_granularity}.target_url AS url,
+            {placement_level_granularity}.placement AS placement,
+            {placement_level_granularity}.placement_type AS placement_type,
+            {placement_level_granularity}.resource_name AS resource_name,
+            {placement_level_granularity}.display_name AS name,
+            {placement_level_granularity}.resource_name~0 AS criterion_id,
+            metrics.clicks AS clicks,
+            metrics.impressions AS impressions,
+            metrics.cost_micros / 1e6 AS cost,
+            metrics.conversions AS conversions,
+            metrics.video_views AS video_views,
+            metrics.interactions AS interactions,
+            metrics.all_conversions AS all_conversions,
+            metrics.all_conversions_value AS all_conversions_value,
+            metrics.view_through_conversions AS view_through_conversions,
+            metrics.conversions_value AS conversions_value
+        FROM {placement_level_granularity}
+        WHERE segments.date >= "{start_date}"
+            AND segments.date <= "{end_date}"
+            AND {placement_level_granularity}.placement_type IN
+                ("{placement_types}")
+            AND {placement_level_granularity}.target_url NOT IN
+                ("{non_excludable_placements}")
+            AND campaign.advertising_channel_type IN ("{campaign_types}")
+            AND metrics.clicks >= {clicks}
+            AND metrics.impressions > {impressions}
+            AND metrics.ctr < {ctr}
+            AND metrics.cost_micros >= {cost}
+        """
 
     def __init__(self,
                  placement_types: tuple[str, ...] | None = None,
                  campaign_types: tuple[str, ...] | None = None,
                  placement_level_granularity: str = 'group_placement_view',
                  start_date: str = _start_date.strftime('%Y-%m-%d'),
                  end_date: str = _end_date.strftime('%Y-%m-%d'),
                  clicks: int = 0,
                  cost: int = 0,
                  impressions: int = 0,
                  ctr: float = 1.0):
-        """Constructor for the class.
+        """Creates Gaarf query for fetching placements data.
 
         Args:
             placement_types: List of campaign types that need to be fetched.
             placement_types: List of placement types that need to be fetched
                 for exclusion.
+            placement_level_granularity: API Resource to fetch data from.
             start_date: Start_date of the period.
             end_date: Start_date of the period.
             clicks: Number of clicks for the period.
             impressions: Number of impressions for the period.
             cost: Cost for the period.
             impressions: Impressions for the period.
             ctr: Average CTR for the period.
+
+        Raises:
+            ValueError: If campaign_type, placement_type or
+            placement_level_granularity are incorrect.
         """
         if campaign_types:
             if isinstance(campaign_types, str):
                 campaign_types = tuple(campaign_types.split(','))
             if (wrong_types :=
                     set(campaign_types).difference(self._campaign_types)):
                 raise ValueError('Wrong campaign type(s): ',
@@ -94,89 +142,88 @@
         self.start_date = start_date
         self.end_date = end_date
         self.non_excludable_placements = '","'.join(
             self._non_excludable_placements)
         self.parent_url = ('group_placement_target_url'
                            if self.placement_level_granularity
                            == 'detail_placement_view' else 'target_url')
-        self.query_text = f"""
-        SELECT
-            customer.descriptive_name AS account_name,
-            customer.id AS customer_id,
-            campaign.id AS campaign_id,
-            campaign.name AS campaign_name,
-            campaign.advertising_channel_type AS campaign_type,
-            ad_group.id AS ad_group_id,
-            ad_group.name AS ad_group_name,
-            {self.placement_level_granularity}.{self.parent_url} AS base_url,
-            {self.placement_level_granularity}.target_url AS url,
-            {self.placement_level_granularity}.placement AS placement,
-            {self.placement_level_granularity}.placement_type AS placement_type,
-            {self.placement_level_granularity}.resource_name AS resource_name,
-            {self.placement_level_granularity}.display_name AS name,
-            {self.placement_level_granularity}.resource_name~0 AS criterion_id,
-            metrics.clicks AS clicks,
-            metrics.impressions AS impressions,
-            metrics.cost_micros / 1e6 AS cost,
-            metrics.conversions AS conversions,
-            metrics.video_views AS video_views,
-            metrics.interactions AS interactions,
-            metrics.all_conversions AS all_conversions,
-            metrics.all_conversions_value AS all_conversions_value,
-            metrics.view_through_conversions AS view_through_conversions,
-            metrics.conversions_value AS conversions_value
-        FROM {self.placement_level_granularity}
-        WHERE segments.date >= "{self.start_date}"
-            AND segments.date <= "{self.end_date}"
-            AND {self.placement_level_granularity}.placement_type IN
-                ("{self.placement_types}")
-            AND {self.placement_level_granularity}.target_url NOT IN
-                ("{self.non_excludable_placements}")
-            AND campaign.advertising_channel_type IN ("{self.campaign_types}")
-            AND metrics.clicks >= {clicks}
-            AND metrics.impressions > {impressions}
-            AND metrics.ctr < {ctr}
-            AND metrics.cost_micros >= {int(cost*1e6)}
-        """
+        self.clicks = clicks
+        self.impressions = impressions
+        self.cost = int(cost * 1e6)
+        self.ctr = ctr
+        self.query_text = self.base_query_text.format(**self.__dict__)
 
     def validate_dates(self, start_date: str, end_date: str) -> None:
-        """Checks whether provides start and end dates are valid."""
+        """Checks whether provides start and end dates are valid.
+
+        Args:
+            start_date: Date in "YYYY-MM-DD" format.
+            end_date: Date in "YYYY-MM-DD" format.
+
+        Raises:
+            ValueError: if start or end_date have incorrect format or
+            start_date greater than end_date.
+        """
         if not self.is_valid_date(start_date):
             raise ValueError(f'Invalid start_date: {start_date}')
 
         if not self.is_valid_date(end_date):
             raise ValueError(f'Invalid end_date: {end_date}')
 
         if (datetime.datetime.strptime(start_date, '%Y-%m-%d')
                 > datetime.datetime.strptime(end_date, '%Y-%m-%d')):
             raise ValueError('start_date cannot be greater than end_date: '
                              f'{start_date} > {end_date}')
 
     def is_valid_date(self, date_string: str) -> bool:
+        """Validates date.
+
+        Args:
+            date_string: Date to be validated.
+
+        Returns:
+            Whether or not the date is a string in "YYYY-MM-DD" format.
+
+        Raises:
+            ValueError: If string format is incorrect.
+        """
         try:
             datetime.datetime.strptime(date_string, '%Y-%m-%d')
             return True
         except ValueError:
             return False
 
 
 class PlacementsConversionSplit(Placements):
-    """Placement conversion performance by each conversion name."""
+    """Placement conversion performance by each conversion name.
+
+    Attributes:
+        query_text: Gaarf query to be sent to Google Ads API.
+    """
     _today = datetime.datetime.today()
     _start_date = _today - datetime.timedelta(days=7)
     _end_date = _today - datetime.timedelta(days=1)
 
     def __init__(
         self,
         placement_types: tuple[str, ...] | None = None,
         campaign_types: tuple[str, ...] | None = None,
         placement_level_granularity: str = 'group_placement_view',
         start_date: str = _start_date.strftime('%Y-%m-%d'),
         end_date: str = _end_date.strftime('%Y-%m-%d')
     ) -> None:
+        """Creates Gaarf query for fetching placements conversion split data.
+        Args:
+            placement_types: List of placement types that need to be fetched
+                for exclusion.
+            campaign_types: List of campaign types that need to be fetched.
+            placement_level_granularity: API Resource to fetch data from.
+            start_date: Start_date of the period.
+            end_date: Start_date of the period.
+        """
         super().__init__(placement_types, campaign_types,
                          placement_level_granularity, start_date, end_date)
         self.query_text = f"""
         SELECT
             campaign.advertising_channel_type AS campaign_type,
             ad_group.id AS ad_group_id,
             segments.conversion_action_name AS conversion_name,
@@ -190,25 +237,95 @@
                 ("{self.placement_types}")
             AND {self.placement_level_granularity}.target_url NOT IN
                 ("{self.non_excludable_placements}")
             AND campaign.advertising_channel_type IN ("{self.campaign_types}")
         """
 
 
-class NegativePlacementsLists(base_query.BaseQuery):
+class PlacementExclusionLists(gaarf.base_query.BaseQuery):
+    """Contains Gaarf query for getting placement exclusion lists.
+
+    Attributes:
+        query_text: Gaarf query to be sent to Google Ads API.
+    """
 
     def __init__(self):
+        """Creates Gaarf query for placement exclusion lists."""
         self.query_text = """
             SELECT
                 shared_set.name AS name,
                 shared_set.resource_name AS resource_name
             FROM shared_set
             WHERE shared_set.type = 'NEGATIVE_PLACEMENTS'
             AND shared_set.status = 'ENABLED'
         """
 
+
+class AlreadyExcludedPlacements(gaarf.base_query.BaseQuery):
+    """Contains Gaarf query for negative placement criteria.
+
+    Negative placements can be specified on multiple levels (ACCOUNT, CAMPAIGN,
+    AD_GROUP). AlreadyExcludedPlacements builds the query depending on the
+    specified level.
+
+    Attributes:
+        query_text: Gaarf query to be sent to Google Ads API.
+    """
+
+    placement_types = '","'.join([
+        'PLACEMENT', 'YOUTUBE_CHANNEL', 'YOUTUBE_VIDEO', 'MOBILE_APPLICATION',
+        'MOBILE_APP_CATEGORY', 'WEBPAGE'
+    ])
+
+    def __init__(self, exclusion_level: enums.ExclusionTypeEnum) -> None:
+        """Creates Gaarf query based on specified exclusion level."""
+        if exclusion_level == enums.ExclusionLevelEnum.ACCOUNT:
+            self.query_text = f"""
+                SELECT
+                    customer.id AS level_id,
+                    customer_negative_criterion.placement.url AS website_url,
+                    customer_negative_criterion.mobile_application.app_id AS app_id,
+                    customer_negative_criterion.youtube_video.video_id AS video_id,
+                    customer_negative_criterion.youtube_channel.channel_id AS channel_id
+                FROM customer_negative_criterion
+                WHERE customer_negative_criterion.type IN ("{self.placement_types}")
+            """
+        elif exclusion_level == enums.ExclusionLevelEnum.CAMPAIGN:
+            self.query_text = f"""
+                SELECT
+                    campaign.id AS level_id,
+                    campaign_criterion.placement.url AS website_url,
+                    campaign_criterion.mobile_application.app_id AS app_id,
+                    campaign_criterion.youtube_video.video_id AS video_id,
+                    campaign_criterion.youtube_channel.channel_id AS channel_id
+                FROM campaign_criterion
+                WHERE campaign_criterion.type IN ("{self.placement_types}")
+                    AND campaign_criterion.negative = true
+            """
+        elif exclusion_level == enums.ExclusionLevelEnum.AD_GROUP:
+            self.query_text = f"""
+                SELECT
+                    ad_group.id AS level_id,
+                    ad_group_criterion.placement.url AS website_url,
+                    ad_group_criterion.mobile_application.app_id AS app_id,
+                    ad_group_criterion.youtube_video.video_id AS video_id,
+                    ad_group_criterion.youtube_channel.channel_id AS channel_id
+                FROM ad_group_criterion
+                WHERE ad_group_criterion.type IN ("{self.placement_types}")
+                    AND ad_group_criterion.negative = true
+            """
+
+
 @dataclasses.dataclass
 class AllowlistedPlacement:
+    """Contains information on allowlisting status of a given placement.
+
+    Attributes:
+        type: Placement type (i.e website or YouTube channel).
+        name: Name of a placement (i.e. website url, channel id)
+        account_id: Account where this placement is allowlisted.
+        id: Unique identifier of the allowlisted placement.
+    """
     type: enums.PlacementTypeEnum
     name: str
     account_id: str
     id: str = dataclasses.field(default_factory=lambda: str(uuid.uuid4()))
```

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/domain/placement_handler/negative_list_verifier.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/domain/placement_handler/negative_list_verifier.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/enums.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/enums.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/handlers.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,19 @@
 from gaarf.query_executor import AdsReportFetcher
 from gaarf.report import GaarfReport
 
 from googleads_housekeeper.adapters.notifications import MessagePayload
 from googleads_housekeeper.adapters.publisher import BasePublisher
 from googleads_housekeeper.domain import commands
 from googleads_housekeeper.domain import events
-from googleads_housekeeper.domain.core import exclusion_specification
 from googleads_housekeeper.domain.core import execution
-from googleads_housekeeper.domain.core import rules_parser
 from googleads_housekeeper.domain.core import settings
 from googleads_housekeeper.domain.core import task
 from googleads_housekeeper.domain.placement_handler import entities as placement_entities
+from googleads_housekeeper.domain.placement_handler import placement_excluder
 from googleads_housekeeper.domain.placement_handler import placement_service
 from googleads_housekeeper.services import unit_of_work
 from googleads_housekeeper.services.enums import ExclusionLevelEnum
 
 
 def get_mcc_accounts(
         cmd: commands.GetMccIds, uow: unit_of_work.AbstractUnitOfWork,
@@ -142,21 +141,26 @@
     return result
 
 
 def run_manual_exclusion_task(
         cmd: commands.RunManualExclusion, uow: unit_of_work.AbstractUnitOfWork,
         ads_api_client: GoogleAdsApiClient) -> dict[str, int]:
     with uow:
-        placement_excluder = placement_service.PlacementExcluder(
-            ads_api_client, uow)
-        exclusion_result = placement_excluder.exclude_placements(
+        excluder = placement_excluder.PlacementExcluder(ads_api_client)
+        exclusion_result = excluder.exclude_placements(
             to_be_excluded_placements=GaarfReport(
                 results=cmd.placements, column_names=cmd.header),
             exclusion_level=ExclusionLevelEnum[cmd.exclusion_level])
-    return asdict(exclusion_result)
+        n_excluded_placements = len(exclusion_result.excluded_placements or [])
+        n_associated_with_list_placements = len(
+            exclusion_result.associated_with_list_placements or [])
+        return {
+            'excluded_placements': n_excluded_placements,
+            'associated_with_list_placements': n_associated_with_list_placements
+        }
 
 
 def task_created(event: events.TaskCreated, publisher: BasePublisher) -> None:
     publisher.publish('task_created', event)
 
 
 def task_with_schedule_created(event: events.TaskWithScheduleCreated,
@@ -183,105 +187,92 @@
 
 
 def run_task(cmd: commands.RunTask,
              uow: unit_of_work.AbstractUnitOfWork,
              ads_api_client: GoogleAdsApiClient,
              publisher: BasePublisher | None = None,
              save_to_db: bool = True) -> tuple[dict, MessagePayload | None]:
-    n_excluded_placements = 0
     with copy(uow) as uow:
         settings = uow.settings.list()
         task_obj = uow.tasks.get(task_id=cmd.id)
-        report_fetcher = AdsReportFetcher(api_client=ads_api_client)
-        specification = exclusion_specification.ExclusionSpecification.from_rules(
-            rules_parser.generate_rules(task_obj.exclusion_rule))
-        placement_excluder = placement_service.PlacementExcluder(
-            ads_api_client, uow)
         start_time = datetime.now()
-        to_be_excluded_placements = placement_service.find_placements_for_exclusion(
-            task_obj, uow, report_fetcher, specification)
-
-        if to_be_excluded_placements and task_obj.output in (
-                task.TaskOutput.EXCLUDE, task.TaskOutput.EXCLUDE_AND_NOTIFY):
-            exclusion_result = placement_excluder.exclude_placements(
-                to_be_excluded_placements, task_obj.exclusion_level)
-
-            end_time = datetime.now()
-            n_excluded_placements = exclusion_result.excluded_placements
-        else:
-            exclusion_result = placement_service.ExclusionResult()
-            end_time = datetime.now()
+        exclusion_result = placement_service.exclude_placements(
+            task_obj=task_obj,
+            uow=uow,
+            client=ads_api_client,
+            runtime_options=placement_service.RuntimeOptions(
+                always_fetch_youtube_preview_mode=False))
+        end_time = datetime.now()
+        n_excluded_placements = len(exclusion_result.excluded_placements or [])
+        n_associated_with_list_placements = len(
+            exclusion_result.associated_with_list_placements or [])
         execution_obj = execution.Execution(
             task=cmd.id,
             start_time=start_time,
             end_time=end_time,
             placements_excluded=n_excluded_placements,
             type=cmd.type)
         uow.executions.add(execution_obj)
-        if save_to_db and n_excluded_placements:
-            for placement in to_be_excluded_placements:
+        if save_to_db and exclusion_result.excluded_placements:
+            for placement in exclusion_result.excluded_placements:
                 if hasattr(placement, 'reason'):
                     exclusion_reason = placement.reason
                 else:
                     exclusion_reason = ''
                 uow.execution_details.add(
                     execution.ExecutionDetails(
                         execution_id=execution_obj.id,
                         placement=placement.name,
                         placement_type=placement.placement_type,
                         reason=exclusion_reason))
         uow.commit()
         if task_obj.output in (task.TaskOutput.NOTIFY,
                                task.TaskOutput.EXCLUDE_AND_NOTIFY):
             publisher.publish('task_run', execution_obj)
-            if to_be_excluded_placements:
+            if excluded_placements := exclusion_result.excluded_placements:
                 message_payload = MessagePayload(
                     task_name=cmd.id,
-                    placements_excluded_sample=to_be_excluded_placements[0:10],
-                    total_placement_excluded=exclusion_result
-                    .excluded_placements,
+                    placements_excluded_sample=excluded_placements[0:10],
+                    total_placement_excluded=len(excluded_placements),
                     recipient=settings[0].email_address)
             else:
                 message_payload = MessagePayload(
                     task_name=cmd.id,
                     placements_excluded_sample=None,
                     total_placement_excluded=0,
                     recipient=settings[0].email_address)
         else:
             message_payload = None
-        return asdict(exclusion_result), message_payload
+        return {
+            'excluded_placements': n_excluded_placements,
+            'associated_with_list_placements': n_associated_with_list_placements
+        }, message_payload
 
 
 def preview_placements(cmd: commands.PreviewPlacements,
                        uow: unit_of_work.AbstractUnitOfWork,
                        ads_api_client: GoogleAdsApiClient,
                        always_fetch_youtube_preview_mode: bool = True,
                        save_to_db: bool = True) -> dict[str, Any]:
     report_fetcher = AdsReportFetcher(api_client=ads_api_client)
-    if cmd.exclusion_rule:
-        specification = (
-            exclusion_specification.ExclusionSpecification.from_rules(
-                rules_parser.generate_rules(cmd.exclusion_rule)))
-    else:
-        specification = exclusion_specification.ExclusionSpecification()
     task_obj = task.Task(
         name='',
         exclusion_rule=cmd.exclusion_rule,
         customer_ids=cmd.customer_ids,
         date_range=cmd.date_range,
         from_days_ago=cmd.from_days_ago,
         exclusion_level=cmd.exclusion_level,
         placement_types=cmd.placement_types)
     to_be_excluded_placements = placement_service.find_placements_for_exclusion(
-        task=task_obj,
+        task_obj=task_obj,
         uow=uow,
         report_fetcher=report_fetcher,
-        specification=specification,
-        always_fetch_youtube_preview_mode=always_fetch_youtube_preview_mode,
-        save_to_db=save_to_db)
+        runtime_options=placement_service.RuntimeOptions(
+            always_fetch_youtube_preview_mode=always_fetch_youtube_preview_mode,
+            save_to_db=save_to_db))
     if not to_be_excluded_placements:
         data = {}
     else:
         data = json.loads(
             to_be_excluded_placements.to_pandas().to_json(orient='index'))
     return {
         'data': data,
```

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/messagebus.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/messagebus.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/services/unit_of_work.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/services/_unit_of_work.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper/views.py` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Pre-build views for simplifying reads from DB."""
 from __future__ import annotations
 
 from dataclasses import asdict
 from typing import Any
 
 from googleads_housekeeper.services import unit_of_work
 
@@ -32,17 +33,17 @@
 def tasks(uow: unit_of_work.AbstractUnitOfWork) -> list[dict[str, Any]]:
     with uow:
         uow_tasks: list[dict[str, Any]] = []
         for uow_task in uow.tasks.list():
             task_dict = uow_task.to_dict()
             task_dict['next_run'] = uow_task.next_run
             accounts = customer_ids(
-                uow, accounts=uow_task.customer_ids.split(','))
+                uow=uow, accounts=uow_task.customer_ids.split(','))
             task_dict['accounts'] = list(
-                set([a.get('account_name') for a in accounts]))
+                {a.get('account_name') for a in accounts})
             if task_executions := executions(uow_task.id, uow):
                 for current_execution in sorted(
                         task_executions,
                         key=lambda x: x.get('end_time'),
                         reverse=True):
                     task_dict['placements_excluded'] = current_execution.get(
                         'placements_excluded')
```

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper.egg-info/PKG-INFO` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleads-housekeeper
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: gcp
```

### Comparing `googleads-housekeeper-0.1.0.dev8/googleads_housekeeper.egg-info/SOURCES.txt` & `googleads-housekeeper-0.1.0.dev9/googleads_housekeeper.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -14,37 +14,45 @@
 googleads_housekeeper/adapters/orm.py
 googleads_housekeeper/adapters/publisher.py
 googleads_housekeeper/adapters/repository.py
 googleads_housekeeper/domain/__init__.py
 googleads_housekeeper/domain/commands.py
 googleads_housekeeper/domain/events.py
 googleads_housekeeper/domain/core/__init__.py
+googleads_housekeeper/domain/core/_settings.py
+googleads_housekeeper/domain/core/entity.py
 googleads_housekeeper/domain/core/exclusion_specification.py
 googleads_housekeeper/domain/core/execution.py
 googleads_housekeeper/domain/core/rules_parser.py
 googleads_housekeeper/domain/core/settings.py
 googleads_housekeeper/domain/core/task.py
 googleads_housekeeper/domain/external_parsers/__init__.py
 googleads_housekeeper/domain/external_parsers/base_parser.py
 googleads_housekeeper/domain/external_parsers/external_entity_parser.py
 googleads_housekeeper/domain/external_parsers/website_parser.py
 googleads_housekeeper/domain/external_parsers/youtube_data_parser.py
 googleads_housekeeper/domain/placement_handler/__init__.py
 googleads_housekeeper/domain/placement_handler/entities.py
 googleads_housekeeper/domain/placement_handler/negative_list_verifier.py
+googleads_housekeeper/domain/placement_handler/placement_excluder.py
+googleads_housekeeper/domain/placement_handler/placement_fetcher.py
+googleads_housekeeper/domain/placement_handler/placement_info_extractor.py
 googleads_housekeeper/domain/placement_handler/placement_service.py
 googleads_housekeeper/services/__init__.py
+googleads_housekeeper/services/_unit_of_work.py
 googleads_housekeeper/services/enums.py
 googleads_housekeeper/services/handlers.py
 googleads_housekeeper/services/messagebus.py
 googleads_housekeeper/services/unit_of_work.py
 tests/__init__.py
 tests/conftest.py
 tests/test_exclusion_specification.py
 tests/test_external_entity_parser.py
 tests/test_external_parsers.py
 tests/test_handlers.py
 tests/test_legacy_adapters.py
 tests/test_notifications.py
+tests/test_placement_excluder.py
+tests/test_placement_fetcher.py
 tests/test_placement_info_extractor.py
 tests/test_placements.py
 tests/test_rules_parser.py
```

### Comparing `googleads-housekeeper-0.1.0.dev8/setup.py` & `googleads-housekeeper-0.1.0.dev9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,24 @@
         'appengine-python-standard>=1.0.0'
     ]
 }
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     name='googleads-housekeeper',
-    version='0.1.0-dev8',
+    version='0.1.0.dev9',
     long_description=README,
     long_description_content_type='text/markdown',
     author='Google Inc. (gTech gPS CSE team)',
     author_email='no-reply@google.com',
     license='Apache 2.0',
     python_requires='>3.8',
     packages=find_packages(),
     install_requires=[
         'google-ads-api-report-fetcher>=1.12.0', 'SQLAlchemy==1.4.46',
         'beautifulsoup4', 'google-api-python-client', 'psycopg2-binary',
         'croniter', 'aiohttp', 'slack_sdk'
     ],
     extras_require=EXTRAS_REQUIRE,
     setup_requires=['pytest-runner'],
-    tests_requires=['pytest'],
+    tests_requires=['pytest', 'pytest-mock'],
 )
```

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/conftest.py` & `googleads-housekeeper-0.1.0.dev9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/test_exclusion_specification.py` & `googleads-housekeeper-0.1.0.dev9/tests/test_exclusion_specification.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/test_external_entity_parser.py` & `googleads-housekeeper-0.1.0.dev9/tests/test_external_entity_parser.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/test_external_parsers.py` & `googleads-housekeeper-0.1.0.dev9/tests/test_external_parsers.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/test_handlers.py` & `googleads-housekeeper-0.1.0.dev9/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/test_legacy_adapters.py` & `googleads-housekeeper-0.1.0.dev9/tests/test_legacy_adapters.py`

 * *Files identical despite different names*

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/test_notifications.py` & `googleads-housekeeper-0.1.0.dev9/tests/test_notifications.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,20 @@
         with pytest.raises(ValueError):
             notification_service.send(empty_payload)
 
 
 class TestGoogleCloudAppEngineEmailNotifications:
 
     def test_prepare_message_returns_correct_message_elements_for_empty_payload(
-            self, empty_payload):
+            self):
+        empty_payload =  notifications.MessagePayload(
+            task_name='test_task',
+            placements_excluded_sample=None,
+            total_placement_excluded=0,
+            recipient='test_recipient')
         sender = notifications.GoogleCloudAppEngineEmailNotifications(
             project_id='fake-project')
         message = sender._prepare_message(empty_payload)
         assert message.body == ''
         assert message.to == ['test_recipient']
         assert message.subject == 'No placements were excluded'
         assert message.sender == (
```

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/test_placement_info_extractor.py` & `googleads-housekeeper-0.1.0.dev9/tests/test_placement_info_extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 import gaarf
 import pytest
 
 from googleads_housekeeper.domain.external_parsers import website_parser
 from googleads_housekeeper.domain.external_parsers import youtube_data_parser
-from googleads_housekeeper.domain.placement_handler import placement_service
+from googleads_housekeeper.domain.placement_handler import placement_info_extractor
 
 
 class TestPlacementInfoExtractor:
 
     @pytest.fixture
     def extractor(self, bus):
-        return placement_service.PlacementInfoExtractor(bus.uow)
+        return placement_info_extractor.PlacementInfoExtractor(bus.uow)
 
     def test_extract_placement_info_returns_website_info(self, extractor):
         gaarf_row = gaarf.report.GaarfRow(
             data=['example.com', 'WEBSITE'],
             column_names=['placement', 'placement_type'])
         expected_result = {
             'website_info':
```

### Comparing `googleads-housekeeper-0.1.0.dev8/tests/test_rules_parser.py` & `googleads-housekeeper-0.1.0.dev9/tests/test_rules_parser.py`

 * *Files identical despite different names*

