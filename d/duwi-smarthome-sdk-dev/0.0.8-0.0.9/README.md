# Comparing `tmp/duwi_smarthome_sdk_dev-0.0.8.tar.gz` & `tmp/duwi_smarthome_sdk_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smarthome_sdk_dev-0.0.8.tar", last modified: Wed May 22 07:36:41 2024, max compression
+gzip compressed data, was "duwi_smarthome_sdk_dev-0.0.9.tar", last modified: Wed May 22 07:56:11 2024, max compression
```

## Comparing `duwi_smarthome_sdk_dev-0.0.8.tar` & `duwi_smarthome_sdk_dev-0.0.9.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.396190 duwi_smarthome_sdk_dev-0.0.8/
--rw-rw-rw-   0        0        0      722 2024-05-22 07:36:41.394231 duwi_smarthome_sdk_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.120114 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.289737 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/__init__.py
--rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/account.py
--rw-rw-rw-   0        0        0     2018 2024-05-22 07:30:27.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/control.py
--rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/discover.py
--rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/floor.py
--rw-rw-rw-   0        0        0     5084 2024-05-22 07:35:29.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/group.py
--rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/house.py
--rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/refresh_token.py
--rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/room.py
--rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/terminal.py
--rw-rw-rw-   0        0        0        0 2024-05-22 03:04:46.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/test_group.py
--rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.304488 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/__init__.py
--rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/status.py
--rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.307417 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.311747 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.339798 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/floor.py
--rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/group.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/room.py
--rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.352053 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.392277 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/
--rw-rw-rw-   0        0        0      722 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2024-05-22 07:36:41.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 07:36:41.396190 duwi_smarthome_sdk_dev-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      950 2024-05-22 07:36:27.000000 duwi_smarthome_sdk_dev-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.355962 duwi_smarthome_sdk_dev-0.0.8/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.390325 duwi_smarthome_sdk_dev-0.0.8/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/__init__.py
--rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_account.py
--rw-rw-rw-   0        0        0      964 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_control.py
--rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_discover.py
--rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_floor.py
--rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_group.py
--rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_house.py
--rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_login.py
--rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_room.py
--rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_terminal.py
--rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.596632 duwi_smarthome_sdk_dev-0.0.9/
+-rw-rw-rw-   0        0        0      722 2024-05-22 07:56:11.595654 duwi_smarthome_sdk_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.527725 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.548865 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/__init__.py
+-rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/account.py
+-rw-rw-rw-   0        0        0     2037 2024-05-22 07:46:30.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/control.py
+-rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/discover.py
+-rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/floor.py
+-rw-rw-rw-   0        0        0     5084 2024-05-22 07:35:29.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/group.py
+-rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/house.py
+-rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/room.py
+-rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/terminal.py
+-rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.554726 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/const/__init__.py
+-rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/const/status.py
+-rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.555701 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.557687 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-05-22 07:55:19.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.568428 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/floor.py
+-rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/group.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/room.py
+-rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.574172 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.593702 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-05-22 07:56:11.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1861 2024-05-22 07:56:11.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:56:11.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-22 07:56:11.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 07:56:11.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-22 07:56:11.000000 duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:56:11.596632 duwi_smarthome_sdk_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      950 2024-05-22 07:55:32.000000 duwi_smarthome_sdk_dev-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.575155 duwi_smarthome_sdk_dev-0.0.9/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.9/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:56:11.591753 duwi_smarthome_sdk_dev-0.0.9/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/__init__.py
+-rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_account.py
+-rw-rw-rw-   0        0        0      995 2024-05-22 07:46:58.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_control.py
+-rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_group.py
+-rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_house.py
+-rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_login.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_room.py
+-rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_terminal.py
+-rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.9/test/api/test_ws.py
```

### Comparing `duwi_smarthome_sdk_dev-0.0.8/PKG-INFO` & `duwi_smarthome_sdk_dev-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/account.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/control.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,15 @@
             'secret': self._app_secret,
             'time': str(current_timestamp()),
             'sign': sign,
             'appVersion': self._app_version,
             'clientVersion': self._client_version,
             'clientModel': self._client_model
         }
-
+        global status
         body_dict = body.to_dict() if body else None
-
         if self._is_group:
             status, message, res = await post(f"{self._url}/deviceGroup/batchCommandOperate", headers, body_dict)
         else:
             status, message, res = await post(f"{self._url}/device/batchCommandOperate", headers, body_dict)
 
         return status
```

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/discover.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/floor.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/group.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/house.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/refresh_token.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/room.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/terminal.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/ws.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/status.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/type_map.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/req/device_control.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/req/device_control.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
             'value': self.paramValue
         }
 
 
 class ControlDevice:
     def __init__(self, device_no, house_no):
         self.device_no = device_no
+        self.device_group_no = device_no
         self.house_no = house_no
         self.commands = []
 
     def add_param_info(self, code, value):
         commands = Commands(code, value)
         self.commands.append(commands)
 
@@ -27,10 +28,11 @@
         commands_list = [
             command.to_dict()
             for command in self.commands
         ]
 
         return {
             'deviceNo': self.device_no,
+            'deviceGroupNo': self.device_group_no,
             'houseNo': self.house_no,
             'commands': commands_list,
         }
```

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/auth.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/device.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/floor.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/group.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/house.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/room.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/terminal.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/model/resp/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/http.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/sign.py` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/PKG-INFO` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt` & `duwi_smarthome_sdk_dev-0.0.9/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 duwi_smarthome_sdk_dev/api/discover.py
 duwi_smarthome_sdk_dev/api/floor.py
 duwi_smarthome_sdk_dev/api/group.py
 duwi_smarthome_sdk_dev/api/house.py
 duwi_smarthome_sdk_dev/api/refresh_token.py
 duwi_smarthome_sdk_dev/api/room.py
 duwi_smarthome_sdk_dev/api/terminal.py
-duwi_smarthome_sdk_dev/api/test_group.py
 duwi_smarthome_sdk_dev/api/ws.py
 duwi_smarthome_sdk_dev/const/__init__.py
 duwi_smarthome_sdk_dev/const/const.py
 duwi_smarthome_sdk_dev/const/status.py
 duwi_smarthome_sdk_dev/const/type_map.py
 duwi_smarthome_sdk_dev/model/__init__.py
 duwi_smarthome_sdk_dev/model/req/__init__.py
```

### Comparing `duwi_smarthome_sdk_dev-0.0.8/setup.py` & `duwi_smarthome_sdk_dev-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smarthome_sdk_dev",
     version=VERSION,
     author="duwi",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_account.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_control.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_control.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,18 @@
             cc = ControlClient(
                 app_key="2e479831-1fb7-751e-7017-7534f7f99fc1",
                 app_secret="26af4883a943083a4c34083897fcea10",
                 access_token="715d1c63-85c0-4d74-9a89-5a0aa4806f74",
                 app_version="0.0.1",
                 client_version="0.0.1",
                 client_model="homeassistant",
+                is_group=False
             )
             cd = ControlDevice(
                 device_no="F15000000001-4",
                 house_no="c7bf567d-225a-4533-ab72-5dc080b794f5",
             )
             cd.add_param_info("switch", "off")
-            res =  await cc.control(cd)
+            res = await cc.control(cd)
             print(res)
 
         asyncio.run(run_test())
```

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_discover.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_floor.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_group.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_house.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_login.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_room.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_terminal.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.8/test/api/test_ws.py` & `duwi_smarthome_sdk_dev-0.0.9/test/api/test_ws.py`

 * *Files identical despite different names*

