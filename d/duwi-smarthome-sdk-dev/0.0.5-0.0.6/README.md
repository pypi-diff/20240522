# Comparing `tmp/duwi_smarthome_sdk_dev-0.0.5.tar.gz` & `tmp/duwi_smarthome_sdk_dev-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smarthome_sdk_dev-0.0.5.tar", last modified: Wed May 22 07:01:45 2024, max compression
+gzip compressed data, was "duwi_smarthome_sdk_dev-0.0.6.tar", last modified: Wed May 22 07:12:48 2024, max compression
```

## Comparing `duwi_smarthome_sdk_dev-0.0.5.tar` & `duwi_smarthome_sdk_dev-0.0.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.517799 duwi_smarthome_sdk_dev-0.0.5/
--rw-rw-rw-   0        0        0      903 2024-05-22 07:01:45.516823 duwi_smarthome_sdk_dev-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-05-15 15:03:31.000000 duwi_smarthome_sdk_dev-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.452537 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.475971 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/__init__.py
--rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/account.py
--rw-rw-rw-   0        0        0     1779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/control.py
--rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/discover.py
--rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/floor.py
--rw-rw-rw-   0        0        0     4114 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/group.py
--rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/house.py
--rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/refresh_token.py
--rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/room.py
--rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/terminal.py
--rw-rw-rw-   0        0        0        0 2024-05-22 03:04:46.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/test_group.py
--rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.480849 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/const/__init__.py
--rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/const/status.py
--rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.481827 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.483780 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.494359 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/floor.py
--rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/group.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/room.py
--rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.499246 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.516823 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev.egg-info/
--rw-rw-rw-   0        0        0      903 2024-05-22 07:01:45.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2024-05-22 07:01:45.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 07:01:45.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-22 07:01:45.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 07:01:45.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-22 07:01:45.000000 duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 07:01:45.518771 duwi_smarthome_sdk_dev-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      950 2024-05-22 07:01:43.000000 duwi_smarthome_sdk_dev-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.501194 duwi_smarthome_sdk_dev-0.0.5/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.5/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:01:45.514865 duwi_smarthome_sdk_dev-0.0.5/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/__init__.py
--rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_account.py
--rw-rw-rw-   0        0        0      964 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_control.py
--rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_discover.py
--rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_floor.py
--rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_group.py
--rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_house.py
--rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_login.py
--rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_room.py
--rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_terminal.py
--rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.5/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.694822 duwi_smarthome_sdk_dev-0.0.6/
+-rw-rw-rw-   0        0        0      722 2024-05-22 07:12:48.693830 duwi_smarthome_sdk_dev-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2024-05-22 07:02:05.000000 duwi_smarthome_sdk_dev-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.638101 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.657631 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/__init__.py
+-rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/account.py
+-rw-rw-rw-   0        0        0     1779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/control.py
+-rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/discover.py
+-rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/floor.py
+-rw-rw-rw-   0        0        0     5121 2024-05-22 07:12:10.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/group.py
+-rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/house.py
+-rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/room.py
+-rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/terminal.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 03:04:46.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/test_group.py
+-rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.661537 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/const/__init__.py
+-rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/const/status.py
+-rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.662512 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.664469 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/req/__init__.py
+-rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.673257 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/floor.py
+-rw-rw-rw-   0        0        0     5369 2024-05-22 07:01:14.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/group.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/room.py
+-rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.677883 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.692606 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-05-22 07:12:48.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1902 2024-05-22 07:12:48.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:12:48.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-22 07:12:48.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 07:12:48.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-22 07:12:48.000000 duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:12:48.694822 duwi_smarthome_sdk_dev-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      950 2024-05-22 07:12:24.000000 duwi_smarthome_sdk_dev-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.679370 duwi_smarthome_sdk_dev-0.0.6/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.6/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:12:48.690655 duwi_smarthome_sdk_dev-0.0.6/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/__init__.py
+-rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_account.py
+-rw-rw-rw-   0        0        0      964 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_control.py
+-rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_group.py
+-rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_house.py
+-rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_login.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_room.py
+-rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_terminal.py
+-rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.6/test/api/test_ws.py
```

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/account.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/control.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/discover.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/floor.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/group.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/group.py`

 * *Files 21% similar despite different names*

```diff
@@ -79,26 +79,44 @@
         """
         Converts a dictionary representing a device group into a Group object.
 
         :param group_dict: A dictionary containing device group details.
         :return: A Group object.
         """
         return Group(
-            device_group_no=group_dict.get("deviceGroupNo", ""),
-            device_group_name=group_dict.get("deviceGroupName", ""),
-            house_no=group_dict.get("houseNo", ""),
-            room_no=group_dict.get("roomNo", ""),
-            icon=group_dict.get("icon", ""),
-            is_favorite=group_dict.get("isFavorite", False),
-            favorite_time=group_dict.get("favoriteTime", ""),
-            create_time=group_dict.get("createTime", ""),
-            update_time=group_dict.get("updateTime", ""),
-            execute_way=group_dict.get("executeWay", 0),
-            device_group_type=group_dict.get("deviceGroupType", ""),
-            seq=group_dict.get("seq", 0),
-            value=group_dict.get("value", {}),
-            sync_host_sequences=group_dict.get("syncHostSequences", [])
+            device_group_no=group_dict.get("deviceGroupNo"),
+            device_group_name=group_dict.get("deviceGroupName"),
+            house_no=group_dict.get("houseNo"),
+            room_no=group_dict.get("roomNo"),
+            icon=group_dict.get("icon"),
+            is_favorite=group_dict.get("isFavorite"),
+            favorite_time=group_dict.get("favoriteTime"),
+            create_time=group_dict.get("createTime"),
+            update_time=group_dict.get("updateTime"),
+            execute_way=group_dict.get("executeWay"),
+            device_group_type=group_dict.get("deviceGroupType"),
+            seq=group_dict.get("seq"),
+            value=group_dict.get("value"),
+            sync_host_sequences=group_dict.get("syncHostSequences"),
+            device_no=group_dict.get("deviceNo"),
+            device_name=group_dict.get("deviceName"),
+            terminal_sequence=group_dict.get("terminalSequence"),
+            route_num=group_dict.get("routeNum"),
+            device_type_no=group_dict.get("deviceTypeNo"),
+            device_sub_type_no=group_dict.get("deviceSubTypeNo"),
+            room_name=group_dict.get("roomName"),
+            floor_no=group_dict.get("floorNo"),
+            floor_name=group_dict.get("floorName"),
+            is_use=group_dict.get("isUse"),
+            is_online=group_dict.get("isOnline"),
+            create_time_device=group_dict.get("createTimeDevice"),
+            seq_device=group_dict.get("seqDevice"),
+            is_favorite_device=group_dict.get("isFavoriteDevice"),
+            favorite_time_device=group_dict.get("favoriteTimeDevice"),
+            key_binding_quantity=group_dict.get("keyBindingQuantity"),
+            key_mapping_quantity=group_dict.get("keyMappingQuantity"),
+            value_device=group_dict.get("valueDevice")
         )
 
 
 if __name__ == '__main__':
-    GroupClient()
+    GroupClient()
```

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/house.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/refresh_token.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/room.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/terminal.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/api/ws.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/const/status.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/const/type_map.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/req/device_control.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/auth.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/device.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/floor.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/group.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/house.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/room.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/model/resp/terminal.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/model/resp/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/util/http.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev/util/sign.py` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt` & `duwi_smarthome_sdk_dev-0.0.6/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/setup.py` & `duwi_smarthome_sdk_dev-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smarthome_sdk_dev",
     version=VERSION,
     author="duwi",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_account.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_control.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_discover.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_floor.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_group.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_group.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_house.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_login.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_room.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_terminal.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.5/test/api/test_ws.py` & `duwi_smarthome_sdk_dev-0.0.6/test/api/test_ws.py`

 * *Files identical despite different names*

