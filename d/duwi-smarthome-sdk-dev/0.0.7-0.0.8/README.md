# Comparing `tmp/duwi_smarthome_sdk_dev-0.0.7.tar.gz` & `tmp/duwi_smarthome_sdk_dev-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smarthome_sdk_dev-0.0.7.tar", last modified: Wed May 22 07:17:38 2024, max compression
+gzip compressed data, was "duwi_smarthome_sdk_dev-0.0.8.tar", last modified: Wed May 22 07:36:41 2024, max compression
```

## Comparing `duwi_smarthome_sdk_dev-0.0.7.tar` & `duwi_smarthome_sdk_dev-0.0.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.532527 duwi_smarthome_sdk_dev-0.0.7/
--rw-rw-rw-   0        0        0      722 2024-05-22 07:17:38.531551 duwi_smarthome_sdk_dev-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.456010 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.484965 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/__init__.py
--rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/account.py
--rw-rw-rw-   0        0        0     1779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/control.py
--rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/discover.py
--rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/floor.py
--rw-rw-rw-   0        0        0     5131 2024-05-22 07:14:56.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/group.py
--rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/house.py
--rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/refresh_token.py
--rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/room.py
--rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/terminal.py
--rw-rw-rw-   0        0        0        0 2024-05-22 03:04:46.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/test_group.py
--rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.489565 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/const/__init__.py
--rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/const/status.py
--rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.490537 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.492491 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.505185 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/floor.py
--rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/group.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/room.py
--rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.511049 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.530579 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/
--rw-rw-rw-   0        0        0      722 2024-05-22 07:17:38.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2024-05-22 07:17:38.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 07:17:38.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-22 07:17:38.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 07:17:38.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-22 07:17:38.000000 duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 07:17:38.533510 duwi_smarthome_sdk_dev-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      950 2024-05-22 07:17:36.000000 duwi_smarthome_sdk_dev-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.512021 duwi_smarthome_sdk_dev-0.0.7/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.7/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:17:38.528626 duwi_smarthome_sdk_dev-0.0.7/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/__init__.py
--rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_account.py
--rw-rw-rw-   0        0        0      964 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_control.py
--rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_discover.py
--rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_floor.py
--rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_group.py
--rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_house.py
--rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_login.py
--rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_room.py
--rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_terminal.py
--rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.7/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.396190 duwi_smarthome_sdk_dev-0.0.8/
+-rw-rw-rw-   0        0        0      722 2024-05-22 07:36:41.394231 duwi_smarthome_sdk_dev-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.120114 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.289737 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/__init__.py
+-rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/account.py
+-rw-rw-rw-   0        0        0     2018 2024-05-22 07:30:27.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/control.py
+-rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/discover.py
+-rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/floor.py
+-rw-rw-rw-   0        0        0     5084 2024-05-22 07:35:29.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/group.py
+-rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/house.py
+-rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/room.py
+-rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/terminal.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 03:04:46.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/test_group.py
+-rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.304488 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/__init__.py
+-rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/status.py
+-rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.307417 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.311747 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/req/__init__.py
+-rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.339798 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/floor.py
+-rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/group.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/room.py
+-rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.352053 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.392277 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1902 2024-05-22 07:36:41.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-22 07:36:40.000000 duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:36:41.396190 duwi_smarthome_sdk_dev-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      950 2024-05-22 07:36:27.000000 duwi_smarthome_sdk_dev-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.355962 duwi_smarthome_sdk_dev-0.0.8/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.8/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:36:41.390325 duwi_smarthome_sdk_dev-0.0.8/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/__init__.py
+-rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_account.py
+-rw-rw-rw-   0        0        0      964 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_control.py
+-rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_group.py
+-rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_house.py
+-rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_login.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_room.py
+-rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_terminal.py
+-rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.8/test/api/test_ws.py
```

### Comparing `duwi_smarthome_sdk_dev-0.0.7/PKG-INFO` & `duwi_smarthome_sdk_dev-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.0.7
+Version: 0.0.8
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/account.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/control.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/refresh_token.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import json
-from typing import Optional
 
+from duwi_smarthome_sdk_dev.const.const import URL
+from duwi_smarthome_sdk_dev.util.http import put
+from duwi_smarthome_sdk_dev.const.status import Code
 from duwi_smarthome_sdk_dev.util.sign import md5_encrypt
 from duwi_smarthome_sdk_dev.util.timestamp import current_timestamp
-from duwi_smarthome_sdk_dev.const.const import URL
-from duwi_smarthome_sdk_dev.util.http import post
-from duwi_smarthome_sdk_dev.model.req.device_control import ControlDevice
-
+from duwi_smarthome_sdk_dev.model.resp.auth import AuthToken
 
-class ControlClient:
 
+class AuthTokenRefresherClient:
     def __init__(self,
                  app_key: str,
                  app_secret: str,
                  access_token: str,
                  app_version: str,
                  client_version: str,
                  client_model: str = None
@@ -22,29 +21,37 @@
         self._app_key = app_key
         self._app_secret = app_secret
         self._access_token = access_token
         self._app_version = app_version
         self._client_version = client_version
         self._client_model = client_model
 
-    async def control(self, body: Optional[ControlDevice]) -> str:
-        body_string = json.dumps(body.to_dict(), separators=(',', ':')) if body else ""
+    async def refresh(self, refresh_token: str) -> tuple[str, AuthToken | None]:
+        body = {
+            "refreshToken": refresh_token,
+        }
 
-        sign = md5_encrypt(f"{body_string}{self._app_secret}{current_timestamp()}")
+        body_string = json.dumps(body, separators=(',', ':'))
+        sign = md5_encrypt(body_string + self._app_secret + str(current_timestamp()))
 
         headers = {
             'Content-Type': 'application/json',
             'accessToken': self._access_token,
             'appkey': self._app_key,
             'secret': self._app_secret,
             'time': str(current_timestamp()),
             'sign': sign,
             'appVersion': self._app_version,
             'clientVersion': self._client_version,
             'clientModel': self._client_model
         }
 
-        body_dict = body.to_dict() if body else None
-
-        status, message, res = await post(f"{self._url}/device/batchCommandOperate", headers, body_dict)
-
-        return status
+        status, message, res = await put(self._url + "/account/token", headers, body)
+        if status == Code.SUCCESS.value:
+            return status, AuthToken(
+                access_token=res.get("accessToken"),
+                access_token_expire_time=res.get("accessTokenExpireTime"),
+                refresh_token=res.get("refreshToken"),
+                refresh_token_expire_time=res.get("refreshTokenExpireTime")
+            )
+        else:
+            return status, None
```

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/discover.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/floor.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/group.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,9 +114,7 @@
             favorite_time_device=group_dict.get("favoriteTimeDevice"),
             key_binding_quantity=group_dict.get("keyBindingQuantity"),
             key_mapping_quantity=group_dict.get("keyMappingQuantity"),
             value_device=group_dict.get("valueDevice")
         )
 
 
-if __name__ == '__main__':
-    GroupClient()
```

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/house.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/refresh_token.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/control.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 import json
+from typing import Optional
 
-from duwi_smarthome_sdk_dev.const.const import URL
-from duwi_smarthome_sdk_dev.util.http import put
-from duwi_smarthome_sdk_dev.const.status import Code
 from duwi_smarthome_sdk_dev.util.sign import md5_encrypt
 from duwi_smarthome_sdk_dev.util.timestamp import current_timestamp
-from duwi_smarthome_sdk_dev.model.resp.auth import AuthToken
+from duwi_smarthome_sdk_dev.const.const import URL
+from duwi_smarthome_sdk_dev.util.http import post
+from duwi_smarthome_sdk_dev.model.req.device_control import ControlDevice
+
 
+class ControlClient:
 
-class AuthTokenRefresherClient:
     def __init__(self,
                  app_key: str,
                  app_secret: str,
                  access_token: str,
                  app_version: str,
                  client_version: str,
-                 client_model: str = None
+                 client_model: str = None,
+                 is_group: bool = False
                  ):
         self._url = URL
         self._app_key = app_key
         self._app_secret = app_secret
         self._access_token = access_token
         self._app_version = app_version
         self._client_version = client_version
         self._client_model = client_model
+        self._is_group = is_group
 
-    async def refresh(self, refresh_token: str) -> tuple[str, AuthToken | None]:
-        body = {
-            "refreshToken": refresh_token,
-        }
+    async def control(self, body: Optional[ControlDevice]) -> str:
+        body_string = json.dumps(body.to_dict(), separators=(',', ':')) if body else ""
 
-        body_string = json.dumps(body, separators=(',', ':'))
-        sign = md5_encrypt(body_string + self._app_secret + str(current_timestamp()))
+        sign = md5_encrypt(f"{body_string}{self._app_secret}{current_timestamp()}")
 
         headers = {
             'Content-Type': 'application/json',
             'accessToken': self._access_token,
             'appkey': self._app_key,
             'secret': self._app_secret,
             'time': str(current_timestamp()),
             'sign': sign,
             'appVersion': self._app_version,
             'clientVersion': self._client_version,
             'clientModel': self._client_model
         }
 
-        status, message, res = await put(self._url + "/account/token", headers, body)
-        if status == Code.SUCCESS.value:
-            return status, AuthToken(
-                access_token=res.get("accessToken"),
-                access_token_expire_time=res.get("accessTokenExpireTime"),
-                refresh_token=res.get("refreshToken"),
-                refresh_token_expire_time=res.get("refreshTokenExpireTime")
-            )
+        body_dict = body.to_dict() if body else None
+
+        if self._is_group:
+            status, message, res = await post(f"{self._url}/deviceGroup/batchCommandOperate", headers, body_dict)
         else:
-            return status, None
+            status, message, res = await post(f"{self._url}/device/batchCommandOperate", headers, body_dict)
+
+        return status
```

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/room.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/terminal.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/api/ws.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/const/status.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/const/type_map.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/req/device_control.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/auth.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/device.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/floor.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/group.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/house.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/room.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/model/resp/terminal.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/model/resp/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/util/http.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev/util/sign.py` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/PKG-INFO` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.0.7
+Version: 0.0.8
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.0.7/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt` & `duwi_smarthome_sdk_dev-0.0.8/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/setup.py` & `duwi_smarthome_sdk_dev-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smarthome_sdk_dev",
     version=VERSION,
     author="duwi",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_account.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_control.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_discover.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_floor.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_group.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_house.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_login.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_room.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_terminal.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.7/test/api/test_ws.py` & `duwi_smarthome_sdk_dev-0.0.8/test/api/test_ws.py`

 * *Files identical despite different names*

