# Comparing `tmp/duwi_smarthome_sdk_dev-0.0.2.tar.gz` & `tmp/duwi_smarthome_sdk_dev-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smarthome_sdk_dev-0.0.2.tar", last modified: Wed May 15 15:03:32 2024, max compression
+gzip compressed data, was "duwi_smarthome_sdk_dev-0.0.4.tar", last modified: Wed May 22 03:29:56 2024, max compression
```

## Comparing `duwi_smarthome_sdk_dev-0.0.2.tar` & `duwi_smarthome_sdk_dev-0.0.4.tar`

### file list

```diff
@@ -1,51 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.627428 duwi_smarthome_sdk_dev-0.0.2/
--rw-rw-rw-   0        0        0      903 2024-05-15 15:03:32.625289 duwi_smarthome_sdk_dev-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-05-15 15:03:31.000000 duwi_smarthome_sdk_dev-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.536287 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.579512 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/__init__.py
--rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/account.py
--rw-rw-rw-   0        0        0     1779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/control.py
--rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/discover.py
--rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/floor.py
--rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/house.py
--rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/refresh_token.py
--rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/room.py
--rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/terminal.py
--rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.588101 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/const/__init__.py
--rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.590776 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.595151 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.613383 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/floor.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/room.py
--rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.620321 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.624048 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev.egg-info/
--rw-rw-rw-   0        0        0      903 2024-05-15 15:03:32.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1525 2024-05-15 15:03:32.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 15:03:32.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-15 15:03:32.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-15 15:03:32.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-15 15:03:32.000000 duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 15:03:32.627428 duwi_smarthome_sdk_dev-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      950 2024-05-15 15:03:31.000000 duwi_smarthome_sdk_dev-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 15:03:32.621907 duwi_smarthome_sdk_dev-0.0.2/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.590056 duwi_smarthome_sdk_dev-0.0.4/
+-rw-rw-rw-   0        0        0      903 2024-05-22 03:29:56.589056 duwi_smarthome_sdk_dev-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-05-15 15:03:31.000000 duwi_smarthome_sdk_dev-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.528365 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.549366 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/__init__.py
+-rw-rw-rw-   0        0        0     2452 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/account.py
+-rw-rw-rw-   0        0        0     1779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/control.py
+-rw-rw-rw-   0        0        0     4560 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/discover.py
+-rw-rw-rw-   0        0        0     2671 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/floor.py
+-rw-rw-rw-   0        0        0     4114 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/group.py
+-rw-rw-rw-   0        0        0     2699 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/house.py
+-rw-rw-rw-   0        0        0     2169 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2779 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/room.py
+-rw-rw-rw-   0        0        0     3161 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/terminal.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 03:04:46.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/test_group.py
+-rw-rw-rw-   0        0        0     4808 2024-05-15 13:10:03.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.554364 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/const/__init__.py
+-rw-rw-rw-   0        0        0       81 2024-05-15 13:06:39.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/const/status.py
+-rw-rw-rw-   0        0        0     1470 2024-05-22 03:24:18.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.555364 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.557364 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/req/__init__.py
+-rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.568057 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/floor.py
+-rw-rw-rw-   0        0        0     2417 2024-05-22 02:15:06.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/group.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/room.py
+-rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.572057 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.588057 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev.egg-info/
+-rw-rw-rw-   0        0        0      903 2024-05-22 03:29:56.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1902 2024-05-22 03:29:56.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 03:29:56.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-22 03:29:56.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 03:29:56.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-05-22 03:29:56.000000 duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 03:29:56.590056 duwi_smarthome_sdk_dev-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      950 2024-05-22 03:29:55.000000 duwi_smarthome_sdk_dev-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.573057 duwi_smarthome_sdk_dev-0.0.4/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk_dev-0.0.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:29:56.587057 duwi_smarthome_sdk_dev-0.0.4/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:20:40.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/__init__.py
+-rw-rw-rw-   0        0        0      731 2024-05-22 03:11:13.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_account.py
+-rw-rw-rw-   0        0        0      964 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_control.py
+-rw-rw-rw-   0        0        0      829 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      796 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      765 2024-05-22 03:16:30.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_group.py
+-rw-rw-rw-   0        0        0      695 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_house.py
+-rw-rw-rw-   0        0        0      648 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_login.py
+-rw-rw-rw-   0        0        0      732 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_room.py
+-rw-rw-rw-   0        0        0      740 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_terminal.py
+-rw-rw-rw-   0        0        0     1228 2024-05-22 03:12:03.000000 duwi_smarthome_sdk_dev-0.0.4/test/api/test_ws.py
```

### Comparing `duwi_smarthome_sdk_dev-0.0.2/PKG-INFO` & `duwi_smarthome_sdk_dev-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.0.2
+Version: 0.0.4
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/account.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/control.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/discover.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/floor.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/house.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/refresh_token.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/room.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/terminal.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/api/ws.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/const/status.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/req/device_control.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/auth.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/device.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/floor.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/house.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/room.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/model/resp/terminal.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/model/resp/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/util/http.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev/util/sign.py` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk_dev-0.0.2/duwi_smarthome_sdk_dev.egg-info/PKG-INFO` & `duwi_smarthome_sdk_dev-0.0.4/duwi_smarthome_sdk_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk_dev
-Version: 0.0.2
+Version: 0.0.4
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk_dev-0.0.2/setup.py` & `duwi_smarthome_sdk_dev-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.4'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smarthome_sdk_dev",
     version=VERSION,
     author="duwi",
     author_email="ledgerbiggg@gmail.com",
```

