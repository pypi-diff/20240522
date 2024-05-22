# Comparing `tmp/ventures-1.2.0.tar.gz` & `tmp/ventures-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.2.0.tar", max compression
+gzip compressed data, was "ventures-1.3.0.tar", max compression
```

## Comparing `ventures-1.2.0.tar` & `ventures-1.3.0.tar`

### file list

```diff
@@ -1,92 +1,99 @@
--rwxr-xr-x   0        0        0      585 2024-05-21 20:28:19.492089 ventures-1.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1120 2024-05-18 18:56:41.459616 ventures-1.2.0/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.2.0/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.2.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.2.0/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.2.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.2.0/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.2.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   199523 2024-05-21 20:28:06.460223 ventures-1.2.0/venues/stages/ventures/_status/DB/records.json
--rwxr-xr-x   0        0        0     1217 2024-05-20 03:37:43.477222 ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1133 2024-05-20 03:37:22.901492 ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-21 20:28:04.452244 ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1283 2024-05-19 23:18:17.298859 ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1428 2024-05-18 02:01:33.088701 ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-21 20:28:05.504233 ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rwxr-xr-x   0        0        0      964 2024-05-20 01:26:25.762311 ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      767 2024-05-20 01:26:19.954331 ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-21 20:28:04.836240 ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.2.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.2.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.2.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.2.0/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      463 2024-05-18 01:29:56.857560 ventures-1.2.0/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.2.0/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.2.0/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1133 2024-05-18 18:53:30.969670 ventures-1.2.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1755 2024-05-20 00:56:07.601346 ventures-1.2.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rw-r--r--   0        0        0     1857 2024-05-21 20:24:20.198551 ventures-1.2.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1200 2024-05-18 18:45:09.731099 ventures-1.2.0/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0     2439 2024-05-20 00:56:04.745365 ventures-1.2.0/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     3140 2024-05-21 20:24:14.846606 ventures-1.2.0/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.2.0/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:56.689210 ventures-1.2.0/venues/stages/ventures/plays_venture/turn_off.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:52.973247 ventures-1.2.0/venues/stages/ventures/plays_venture/turn_on.py
--rwxr-xr-x   0        0        0     1377 2024-05-20 03:44:44.816161 ventures-1.2.0/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.2.0/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2455 2024-05-21 20:21:09.968507 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive/__init__.py
--rw-r--r--   0        0        0     1911 2024-05-21 20:21:12.308483 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.2.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      486 2024-05-17 22:53:36.062918 ventures-1.2.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.2.0/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      230 2024-05-17 22:53:33.130949 ventures-1.2.0/venues/stages/ventures/utilities/map/scan.py
--rwxr-xr-x   0        0        0      919 2024-05-20 00:48:43.604121 ventures-1.2.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      676 2024-05-20 00:48:36.716162 ventures-1.2.0/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.2.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      381 2024-05-18 03:46:35.268323 ventures-1.2.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      181 2024-05-18 03:46:08.652619 ventures-1.2.0/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.2.0/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 ventures-1.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2024-05-22 01:14:46.773424 ventures-1.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0     2920 2024-05-22 01:14:07.029862 ventures-1.3.0/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.3.0/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.3.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.3.0/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.3.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.3.0/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.3.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   346881 2024-05-22 01:14:29.129631 ventures-1.3.0/venues/stages/ventures/_status/DB/records.json
+-rw-r--r--   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-22 01:14:25.153673 ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rw-r--r--   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-22 01:14:27.185652 ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rw-r--r--   0        0        0      974 2024-05-22 00:50:05.019739 ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      787 2024-05-22 00:49:57.495796 ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-22 01:14:25.557669 ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.3.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.3.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rw-r--r--   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.3.0/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.3.0/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
+-rwxr-xr-x   0        0        0      186 2024-05-22 01:14:28.225641 ventures-1.3.0/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.3.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.3.0/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      984 2024-05-21 22:50:00.483641 ventures-1.3.0/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.3.0/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.3.0/venues/stages/ventures/mixer.S.HTML
+-rw-r--r--   0        0        0     1055 2024-05-22 01:14:22.929696 ventures-1.3.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rw-r--r--   0        0        0     1751 2024-05-22 00:50:05.059738 ventures-1.3.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rw-r--r--   0        0        0     1035 2024-05-22 01:05:13.047374 ventures-1.3.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1189 2024-05-22 01:14:18.249745 ventures-1.3.0/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0     2444 2024-05-22 00:49:57.543795 ventures-1.3.0/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     3292 2024-05-22 01:05:07.511430 ventures-1.3.0/venues/stages/ventures/plays/turn_on.py
+-rw-r--r--   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.3.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
+-rw-r--r--   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.3.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.3.0/venues/stages/ventures/plays_venture/is_on.py
+-rw-r--r--   0        0        0     2226 2024-05-22 01:13:12.126436 ventures-1.3.0/venues/stages/ventures/plays_venture/turn_off/__init__.py
+-rw-r--r--   0        0        0     1729 2024-05-22 01:14:22.933696 ventures-1.3.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.3.0/venues/stages/ventures/plays_venture/turn_on/__init__.py
+-rw-r--r--   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.3.0/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2340 2024-05-22 01:12:32.694847 ventures-1.3.0/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.3.0/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rw-r--r--   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.3.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rw-r--r--   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.3.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.3.0/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.3.0/venues/stages/ventures/utilities/map/scan.py
+-rw-r--r--   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.3.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.3.0/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.3.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rw-r--r--   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.3.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.3.0/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.3.0/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 ventures-1.3.0/PKG-INFO
```

### Comparing `ventures-1.2.0/pyproject.toml` & `ventures-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.2.0"
+version = "1.3.0"
 description = ""
 authors = []
 readme = "venues/stages/ventures/readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "GPL-3.0-only"
```

### Comparing `ventures-1.2.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.3.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/DB/records.json` & `ventures-1.3.0/venues/stages/ventures/_status/DB/records.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8656716417910448%*

 * *Differences: {"'_default'": "{'50': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [8.650022209621966e-07, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'status_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), OrderedDict([('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('elapsed', [6.920017767697573e-07, "*

 * *               "'seconds']), […]*

```diff
@@ -5954,28 +5954,4417 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "50": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.650022209621966e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.920017767697573e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.1456223519999185,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.102681735999795,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.0778142460003437,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 0,
+                    "passes": 5
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "51": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                9.420036803930998e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.530034054070711e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.16352796999854,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.1351592270002584,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.0925516900024377,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 0,
+                    "passes": 5
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "52": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.150010787881911e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.2680029612965882e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.141126516995428,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.035985795002489,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.089497263994417,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.14879123600258,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 0,
+                    "passes": 6
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "53": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures_map_bracket' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 101, in turn_on_move",
+                                "    \"bracket\": ventures_map_bracket",
+                                "NameError: name 'ventures_map_bracket' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures_map_bracket' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 101, in turn_on_move",
+                                "    \"bracket\": ventures_map_bracket",
+                                "NameError: name 'ventures_map_bracket' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures_map_bracket' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 101, in turn_on_move",
+                                "    \"bracket\": ventures_map_bracket",
+                                "NameError: name 'ventures_map_bracket' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures_map_bracket' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 101, in turn_on_move",
+                                "    \"bracket\": ventures_map_bracket",
+                                "NameError: name 'ventures_map_bracket' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.6499917516484857e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.819965736009181e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures_map_bracket' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 101, in turn_on_move",
+                                "    \"bracket\": ventures_map_bracket",
+                                "NameError: name 'ventures_map_bracket' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures_map_bracket' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 101, in turn_on_move",
+                                "    \"bracket\": ventures_map_bracket",
+                                "NameError: name 'ventures_map_bracket' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures_map_bracket' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 101, in turn_on_move",
+                                "    \"bracket\": ventures_map_bracket",
+                                "NameError: name 'ventures_map_bracket' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures_map_bracket' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 101, in turn_on_move",
+                                "    \"bracket\": ventures_map_bracket",
+                                "NameError: name 'ventures_map_bracket' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "54": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('the_map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 103, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 29, in is_on",
+                                "    the_map = packet [\"the_map\"]",
+                                "KeyError: 'the_map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('the_map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 103, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 29, in is_on",
+                                "    the_map = packet [\"the_map\"]",
+                                "KeyError: 'the_map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('the_map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 103, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 29, in is_on",
+                                "    the_map = packet [\"the_map\"]",
+                                "KeyError: 'the_map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('the_map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 103, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 29, in is_on",
+                                "    the_map = packet [\"the_map\"]",
+                                "KeyError: 'the_map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.2900002123788e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.710026016458869e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('the_map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 103, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 29, in is_on",
+                                "    the_map = packet [\"the_map\"]",
+                                "KeyError: 'the_map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('the_map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 103, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 29, in is_on",
+                                "    the_map = packet [\"the_map\"]",
+                                "KeyError: 'the_map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('the_map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 103, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 29, in is_on",
+                                "    the_map = packet [\"the_map\"]",
+                                "KeyError: 'the_map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('the_map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 103, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 29, in is_on",
+                                "    the_map = packet [\"the_map\"]",
+                                "KeyError: 'the_map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "55": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.519993232563138e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.030015017837286e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.141085208000732,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.3888681050011655,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.076803126001323,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.175552822001919,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 0,
+                    "passes": 6
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "56": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.999995770864189e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.05003151576966e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.119041913996625,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.091213127001538,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.0928991379987565,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.172062531994015,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 0,
+                    "passes": 6
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "57": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 94, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 38, in turn_on_venture",
+                                "    the_map_path = packet [\"map\"]",
+                                "KeyError: 'map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 94, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 38, in turn_on_venture",
+                                "    the_map_path = packet [\"map\"]",
+                                "KeyError: 'map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 94, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 38, in turn_on_venture",
+                                "    the_map_path = packet [\"map\"]",
+                                "KeyError: 'map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 94, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 38, in turn_on_venture",
+                                "    the_map_path = packet [\"map\"]",
+                                "KeyError: 'map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.1969968909397721e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.619957275688648e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 94, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 38, in turn_on_venture",
+                                "    the_map_path = packet [\"map\"]",
+                                "KeyError: 'map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 94, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 38, in turn_on_venture",
+                                "    the_map_path = packet [\"map\"]",
+                                "KeyError: 'map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 94, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 38, in turn_on_venture",
+                                "    the_map_path = packet [\"map\"]",
+                                "KeyError: 'map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('map')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 94, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 38, in turn_on_venture",
+                                "    the_map_path = packet [\"map\"]",
+                                "KeyError: 'map'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "58": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'os' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 27, in check_1",
+                                "    ventures = ventures_map ({",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 66, in ventures_map",
+                                "    if os.path.exists (the_map_path):",
+                                "NameError: name 'os' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'os' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 32, in check_1",
+                                "    ventures = ventures_map ({",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 66, in ventures_map",
+                                "    if os.path.exists (the_map_path):",
+                                "NameError: name 'os' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'os' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 27, in check_1",
+                                "    ventures = ventures_map ({",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 66, in ventures_map",
+                                "    if os.path.exists (the_map_path):",
+                                "NameError: name 'os' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'os' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 38, in check_1",
+                                "    ventures = ventures_map ({",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 66, in ventures_map",
+                                "    if os.path.exists (the_map_path):",
+                                "NameError: name 'os' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.350011633709073e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.1669981176964939e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'os' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 27, in check_1",
+                                "    ventures = ventures_map ({",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 66, in ventures_map",
+                                "    if os.path.exists (the_map_path):",
+                                "NameError: name 'os' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'os' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 32, in check_1",
+                                "    ventures = ventures_map ({",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 66, in ventures_map",
+                                "    if os.path.exists (the_map_path):",
+                                "NameError: name 'os' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'os' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 27, in check_1",
+                                "    ventures = ventures_map ({",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 66, in ventures_map",
+                                "    if os.path.exists (the_map_path):",
+                                "NameError: name 'os' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'os' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 38, in check_1",
+                                "    ventures = ventures_map ({",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 66, in ventures_map",
+                                "    if os.path.exists (the_map_path):",
+                                "NameError: name 'os' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "59": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'the_map_path' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 148, in turn_on_venture",
+                                "    \"the_map_path\": the_map_path,",
+                                "NameError: name 'the_map_path' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'find_venture' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 62, in turn_on_venture",
+                                "    venture = find_venture (ventures, name)",
+                                "NameError: name 'find_venture' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'the_map_path' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 148, in turn_on_venture",
+                                "    \"the_map_path\": the_map_path,",
+                                "NameError: name 'the_map_path' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'the_map_path' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 148, in turn_on_venture",
+                                "    \"the_map_path\": the_map_path,",
+                                "NameError: name 'the_map_path' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.329945219680667e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.100017344579101e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'the_map_path' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 148, in turn_on_venture",
+                                "    \"the_map_path\": the_map_path,",
+                                "NameError: name 'the_map_path' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'find_venture' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 62, in turn_on_venture",
+                                "    venture = find_venture (ventures, name)",
+                                "NameError: name 'find_venture' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'the_map_path' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 148, in turn_on_venture",
+                                "    \"the_map_path\": the_map_path,",
+                                "NameError: name 'the_map_path' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'the_map_path' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 148, in turn_on_venture",
+                                "    \"the_map_path\": the_map_path,",
+                                "NameError: name 'the_map_path' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
         "6": {
             "alarms": [],
             "paths": [],
             "stats": {
                 "checks": {
                     "alarms": 0,
                     "passes": 0
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "60": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "TypeError(\"'NoneType' object is not subscriptable\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 111, in turn_on_move",
+                                "    \"bracket\": ventures_packet [\"ventures_map_bracket\"]",
+                                "TypeError: 'NoneType' object is not subscriptable"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'find_venture' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 62, in turn_on_venture",
+                                "    venture = find_venture (ventures, name)",
+                                "NameError: name 'find_venture' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "TypeError(\"'NoneType' object is not subscriptable\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 111, in turn_on_move",
+                                "    \"bracket\": ventures_packet [\"ventures_map_bracket\"]",
+                                "TypeError: 'NoneType' object is not subscriptable"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "TypeError(\"'NoneType' object is not subscriptable\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 111, in turn_on_move",
+                                "    \"bracket\": ventures_packet [\"ventures_map_bracket\"]",
+                                "TypeError: 'NoneType' object is not subscriptable"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.62002242077142e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.350019248202443e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "TypeError(\"'NoneType' object is not subscriptable\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 111, in turn_on_move",
+                                "    \"bracket\": ventures_packet [\"ventures_map_bracket\"]",
+                                "TypeError: 'NoneType' object is not subscriptable"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'find_venture' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 62, in turn_on_venture",
+                                "    venture = find_venture (ventures, name)",
+                                "NameError: name 'find_venture' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "TypeError(\"'NoneType' object is not subscriptable\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 111, in turn_on_move",
+                                "    \"bracket\": ventures_packet [\"ventures_map_bracket\"]",
+                                "TypeError: 'NoneType' object is not subscriptable"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "TypeError(\"'NoneType' object is not subscriptable\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 111, in turn_on_move",
+                                "    \"bracket\": ventures_packet [\"ventures_map_bracket\"]",
+                                "TypeError: 'NoneType' object is not subscriptable"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "61": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7c0803d45ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x7c0803d45ff0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7c0803d45ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 80, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9081\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7c0803d45ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'find_venture' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 62, in turn_on_venture",
+                                "    venture = find_venture (ventures, name)",
+                                "NameError: name 'find_venture' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x722ae8435c30>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x722ae8435c30>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x722ae8435c30>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 73, in check_1",
+                                "    assert (requests.get (\"http://0.0.0.0:15001\").status_code == 200)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x722ae8435c30>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.639966159127653e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.109977792017162e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7c0803d45ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x7c0803d45ff0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7c0803d45ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 80, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9081\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7c0803d45ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'find_venture' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 62, in turn_on_venture",
+                                "    venture = find_venture (ventures, name)",
+                                "NameError: name 'find_venture' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x722ae8435c30>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x722ae8435c30>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x722ae8435c30>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 73, in check_1",
+                                "    assert (requests.get (\"http://0.0.0.0:15001\").status_code == 200)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x722ae8435c30>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "62": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7f2b8f415ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x7f2b8f415ff0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7f2b8f415ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 80, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9081\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7f2b8f415ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 64, in turn_on_venture",
+                                "    venture = find_venture (ventures, name)",
+                                "NameError: name 'ventures' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x73d9f9811c30>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x73d9f9811c30>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x73d9f9811c30>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 73, in check_1",
+                                "    assert (requests.get (\"http://0.0.0.0:15001\").status_code == 200)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x73d9f9811c30>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.490066203288734e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.619949661195278e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7f2b8f415ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x7f2b8f415ff0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7f2b8f415ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 80, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9081\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7f2b8f415ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'ventures' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 64, in turn_on_venture",
+                                "    venture = find_venture (ventures, name)",
+                                "NameError: name 'ventures' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x73d9f9811c30>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x73d9f9811c30>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x73d9f9811c30>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 73, in check_1",
+                                "    assert (requests.get (\"http://0.0.0.0:15001\").status_code == 200)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x73d9f9811c30>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "63": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x70417a48d9c0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x70417a48d9c0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x70417a48d9c0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 80, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9081\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x70417a48d9c0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'time' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 133, in turn_on_venture",
+                                "    time.sleep (1)",
+                                "NameError: name 'time' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x77382eda1c30>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x77382eda1c30>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x77382eda1c30>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 73, in check_1",
+                                "    assert (requests.get (\"http://0.0.0.0:15001\").status_code == 200)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x77382eda1c30>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.500057108700275e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.650006980635226e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x70417a48d9c0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x70417a48d9c0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x70417a48d9c0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 80, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9081\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x70417a48d9c0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'time' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 104, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 57, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 133, in turn_on_venture",
+                                "    time.sleep (1)",
+                                "NameError: name 'time' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x77382eda1c30>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x77382eda1c30>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x77382eda1c30>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 73, in check_1",
+                                "    assert (requests.get (\"http://0.0.0.0:15001\").status_code == 200)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x77382eda1c30>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 4,
+                    "passes": 2
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "64": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7e6916b31ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x7e6916b31ff0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7e6916b31ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 80, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9081\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7e6916b31ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x75560d5a5bd0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x75560d5a5bd0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x75560d5a5bd0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 73, in check_1",
+                                "    assert (requests.get (\"http://0.0.0.0:15001\").status_code == 200)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x75560d5a5bd0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/5_refresh_1/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.179995347745717e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.559995770454407e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7e6916b31ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x7e6916b31ff0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7e6916b31ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 80, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9081\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9081): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7e6916b31ff0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.396770114006358,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x75560d5a5bd0>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x75560d5a5bd0>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 589, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x75560d5a5bd0>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 73, in check_1",
+                                "    assert (requests.get (\"http://0.0.0.0:15001\").status_code == 200)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 622, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=15001): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x75560d5a5bd0>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 3,
+                    "passes": 3
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "65": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.480040610767901e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.57004420645535e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.156574612999975,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.3828901189990574,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.200421029003337,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 1,
+                    "passes": 5
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "66": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.220013114623725e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.57003659196198e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.1964204209944,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.39937179700064,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.1075821880003787,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.247277722002764,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 0,
+                    "passes": 6
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "67": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.979971658438444e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.4499756768345833e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.174977820002823,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.3506875230013975,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.094955010994454,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.214158178998332,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_refresh_1/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 0,
+                    "passes": 6
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
         "7": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 20 03:37:22 2024 UTC, .py size: 1133 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 72c5 4a66 6d04 0000  o.......r.Jfm...
+00000000: 6f0d 0d0a 0000 0000 3541 4d66 8104 0000  o.......5AMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6403 6c0a  m.Z.m.Z...d.d.l.
 00000070: 5a0a 6401 6403 6c0b 5a0b 6405 6406 8400  Z.d.d.l.Z.d.d...
@@ -24,54 +24,54 @@
 00000170: a00d 640b a101 7d03 7c03 6a0e 640c 6b02  ..d...}.|.j.d.k.
 00000180: 733d 4a00 8201 7c02 640d 1900 8300 0100  s=J...|.d.......
 00000190: 740a a00b 640a a101 0100 640e 7d04 7a07  t...d.....d.}.z.
 000001a0: 740c a00d 640b a101 7d03 5700 6e0d 0400  t...d...}.W.n...
 000001b0: 740c 6a0f 6a10 795d 0100 0100 0100 640f  t.j.j.y]......d.
 000001c0: 7d04 5900 6e01 7700 7c04 640f 6b02 7364  }.Y.n.w.|.d.k.sd
 000001d0: 4a00 8201 6400 5300 2910 4e7a 1176 656e  J...d.S.).Nz.ven
-000001e0: 7475 7265 735f 6d61 702e 4a53 4f4e 7a08  tures_map.JSONz.
-000001f0: 7468 655f 6d61 703a da18 315f 315f 7665  the_map:..1_1_ve
-00000200: 6e74 7572 655f 7079 7468 6f6e 335f 6874  nture_python3_ht
-00000210: 7470 da10 7072 6f63 6573 735f 6964 656e  tp..process_iden
-00000220: 7469 7479 2904 da07 7079 7468 6f6e 337a  tity)...python3z
-00000230: 022d 6d7a 0b68 7474 702e 7365 7276 6572  .-mz.http.server
-00000240: da04 3830 3830 2902 da09 6164 7665 6e74  ..8080)...advent
-00000250: 7572 65da 0550 6f70 656e 2903 da04 6e61  ure..Popen)...na
-00000260: 6d65 da04 6b69 6e64 fa07 7475 726e 206f  me..kind..turn o
-00000270: 6e29 02da 036d 6170 da08 7665 6e74 7572  n)...map..ventur
-00000280: 6573 720e 0000 00e9 0100 0000 7a13 6874  esr.........z.ht
-00000290: 7470 3a2f 2f30 2e30 2e30 2e30 3a38 3038  tp://0.0.0.0:808
-000002a0: 30e9 c800 0000 7a08 7475 726e 206f 6666  0.....z.turn off
-000002b0: da02 6e6f da03 7965 7329 11da 0770 6174  ..no..yes)...pat
-000002c0: 686c 6962 da04 5061 7468 da08 5f5f 6669  hlib..Path..__fi
-000002d0: 6c65 5f5f da06 7061 7265 6e74 da07 7265  le__..parent..re
-000002e0: 736f 6c76 65da 0373 7472 7205 0000 0072  solve..strr....r
-000002f0: 0400 0000 da05 7072 696e 7472 0200 0000  ......printr....
-00000300: da04 7469 6d65 da05 736c 6565 70da 0872  ..time..sleep..r
-00000310: 6571 7565 7374 73da 0367 6574 da0b 7374  equests..get..st
-00000320: 6174 7573 5f63 6f64 65da 0a65 7863 6570  atus_code..excep
-00000330: 7469 6f6e 73da 0f43 6f6e 6e65 6374 696f  tions..Connectio
-00000340: 6e45 7272 6f72 2905 da0b 7468 6973 5f66  nError)...this_f
-00000350: 6f6c 6465 72da 0774 6865 5f6d 6170 7210  older..the_mapr.
-00000360: 0000 00da 0872 6573 706f 6e73 65da 1463  .....response..c
-00000370: 6f6e 6e65 6374 696f 6e5f 6578 6365 7074  onnection_except
-00000380: 696f 6ea9 0072 2700 0000 fa48 2f68 6162  ion..r'....H/hab
-00000390: 6974 6174 2f76 656e 7565 732f 7374 6167  itat/venues/stag
-000003a0: 6573 2f76 656e 7475 7265 732f 5f73 7461  es/ventures/_sta
-000003b0: 7475 732f 6d6f 6e69 746f 7273 2f31 5f31  tus/monitors/1_1
-000003c0: 5f76 656e 7475 7265 2f73 7461 7475 735f  _venture/status_
-000003d0: 312e 7079 da07 6368 6563 6b5f 3110 0000  1.py..check_1...
-000003e0: 0073 3e00 0000 1001 0201 0401 0201 0201  .s>.............
-000003f0: 04fe 04ff 0a07 0202 0201 0203 0201 0602  ................
-00000400: 0206 04f9 04fd 02ff 08fe 0a13 0a07 0a01  ................
-00000410: 0e01 0a07 0a07 0401 0201 0e01 1001 0801  ................
-00000420: 02ff 1003 7229 0000 007a 0763 6865 636b  ....r)...z.check
-00000430: 2031 290e da07 5f5f 646f 635f 5f72 1000   1)...__doc__r..
-00000440: 0000 7202 0000 0072 1e00 0000 da02 6f73  ..r....r......os
-00000450: 7215 0000 00da 076f 732e 7061 7468 7203  r......os.pathr.
-00000460: 0000 0072 0400 0000 7205 0000 00da 0373  ...r....r......s
-00000470: 7973 721c 0000 0072 2900 0000 da06 6368  ysr....r).....ch
-00000480: 6563 6b73 7227 0000 0072 2700 0000 7227  ecksr'...r'...r'
-00000490: 0000 0072 2800 0000 da08 3c6d 6f64 756c  ...r(.....<modul
-000004a0: 653e 0100 0000 7316 0000 0004 010c 0408  e>....s.........
-000004b0: 0208 0208 0114 0108 0108 0108 0204 4108  ..............A.
-000004c0: ff                                       .
+000001e0: 7475 7265 735f 6d61 702e 4a53 4f4e 7a0d  tures_map.JSONz.
+000001f0: 7468 655f 6d61 705f 7061 7468 3ada 1831  the_map_path:..1
+00000200: 5f31 5f76 656e 7475 7265 5f70 7974 686f  _1_venture_pytho
+00000210: 6e33 5f68 7474 70da 1070 726f 6365 7373  n3_http..process
+00000220: 5f69 6465 6e74 6974 7929 04da 0770 7974  _identity)...pyt
+00000230: 686f 6e33 7a02 2d6d 7a0b 6874 7470 2e73  hon3z.-mz.http.s
+00000240: 6572 7665 72da 0438 3038 3029 02da 0961  erver..8080)...a
+00000250: 6476 656e 7475 7265 da05 506f 7065 6e29  dventure..Popen)
+00000260: 03da 046e 616d 65da 046b 696e 64fa 0774  ...name..kind..t
+00000270: 7572 6e20 6f6e 2902 da03 6d61 70da 0876  urn on)...map..v
+00000280: 656e 7475 7265 7372 0e00 0000 e901 0000  enturesr........
+00000290: 007a 1368 7474 703a 2f2f 302e 302e 302e  .z.http://0.0.0.
+000002a0: 303a 3830 3830 e9c8 0000 007a 0874 7572  0:8080.....z.tur
+000002b0: 6e20 6f66 66da 026e 6fda 0379 6573 2911  n off..no..yes).
+000002c0: da07 7061 7468 6c69 62da 0450 6174 68da  ..pathlib..Path.
+000002d0: 085f 5f66 696c 655f 5fda 0670 6172 656e  .__file__..paren
+000002e0: 74da 0772 6573 6f6c 7665 da03 7374 7272  t..resolve..strr
+000002f0: 0500 0000 7204 0000 00da 0570 7269 6e74  ....r......print
+00000300: 7202 0000 00da 0474 696d 65da 0573 6c65  r......time..sle
+00000310: 6570 da08 7265 7175 6573 7473 da03 6765  ep..requests..ge
+00000320: 74da 0b73 7461 7475 735f 636f 6465 da0a  t..status_code..
+00000330: 6578 6365 7074 696f 6e73 da0f 436f 6e6e  exceptions..Conn
+00000340: 6563 7469 6f6e 4572 726f 7229 05da 0b74  ectionError)...t
+00000350: 6869 735f 666f 6c64 6572 da0c 7468 655f  his_folder..the_
+00000360: 6d61 705f 7061 7468 7210 0000 00da 0872  map_pathr......r
+00000370: 6573 706f 6e73 65da 1463 6f6e 6e65 6374  esponse..connect
+00000380: 696f 6e5f 6578 6365 7074 696f 6ea9 0072  ion_exception..r
+00000390: 2700 0000 fa48 2f68 6162 6974 6174 2f76  '....H/habitat/v
+000003a0: 656e 7565 732f 7374 6167 6573 2f76 656e  enues/stages/ven
+000003b0: 7475 7265 732f 5f73 7461 7475 732f 6d6f  tures/_status/mo
+000003c0: 6e69 746f 7273 2f31 5f31 5f76 656e 7475  nitors/1_1_ventu
+000003d0: 7265 2f73 7461 7475 735f 312e 7079 da07  re/status_1.py..
+000003e0: 6368 6563 6b5f 3110 0000 0073 3e00 0000  check_1....s>...
+000003f0: 1001 0201 0401 0201 0201 04fe 04ff 0a07  ................
+00000400: 0202 0201 0203 0201 0602 0206 04f9 04fd  ................
+00000410: 02ff 08fe 0a13 0a07 0a01 0e01 0a07 0a07  ................
+00000420: 0401 0201 0e01 1001 0801 02ff 1003 7229  ..............r)
+00000430: 0000 007a 0763 6865 636b 2031 290e da07  ...z.check 1)...
+00000440: 5f5f 646f 635f 5f72 1000 0000 7202 0000  __doc__r....r...
+00000450: 0072 1e00 0000 da02 6f73 7215 0000 00da  .r......osr.....
+00000460: 076f 732e 7061 7468 7203 0000 0072 0400  .os.pathr....r..
+00000470: 0000 7205 0000 00da 0373 7973 721c 0000  ..r......sysr...
+00000480: 0072 2900 0000 da06 6368 6563 6b73 7227  .r).....checksr'
+00000490: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
+000004a0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000004b0: 7316 0000 0004 010c 0408 0208 0208 0114  s...............
+000004c0: 0108 0108 0108 0204 4108 ff              ........A..
```

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 import pathlib
 from os.path import dirname, join, normpath
 import sys
 import time
 
 def check_1 ():
 	this_folder = pathlib.Path (__file__).parent.resolve ()
-	the_map = str (
+	the_map_path = str (
 		normpath (join (
 			this_folder, 
 			"ventures_map.JSON"
 		))
 	)
 	
-	print ("the_map:", the_map)
+	print ("the_map_path:", the_map_path)
 	
 	ventures = ventures_map ({
-		"map": the_map,
+		"map": the_map_path,
 		"ventures": [
 			{
 				"name": "1_1_venture_python3_http",
 				"kind": "process_identity",
 				"turn on": {
 					"adventure": [ 
 						"python3",
```

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 18 02:01:33 2024 UTC, .py size: 1428 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 fd0b 4866 9405 0000  o.........Hf....
+00000000: 6f0d 0d0a 0000 0000 3541 4d66 a805 0000  o.......5AMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6403 6c0a  m.Z.m.Z...d.d.l.
 00000070: 5a0a 6401 6403 6c0b 5a0b 6405 6406 8400  Z.d.d.l.Z.d.d...
@@ -25,57 +25,57 @@
 00000180: 740a a00b 640e a101 0100 740c a00d 640f  t...d.....t...d.
 00000190: a101 7d03 7c03 6a0e 6410 6b02 7351 4a00  ..}.|.j.d.k.sQJ.
 000001a0: 8201 740c a00d 6411 a101 7d03 7c03 6a0e  ..t...d...}.|.j.
 000001b0: 6410 6b02 735d 4a00 8201 740c a00d 6412  d.k.s]J...t...d.
 000001c0: a101 7d03 7c03 6a0e 6410 6b02 7369 4a00  ..}.|.j.d.k.siJ.
 000001d0: 8201 7c02 6413 1900 8300 0100 6400 5300  ..|.d.......d.S.
 000001e0: 2914 4e7a 1176 656e 7475 7265 735f 6d61  ).Nz.ventures_ma
-000001f0: 702e 4a53 4f4e 7a08 7468 655f 6d61 703a  p.JSONz.the_map:
-00000200: da0b 6164 7665 6e74 7572 655f 31da 1070  ..adventure_1..p
-00000210: 726f 6365 7373 5f69 6465 6e74 6974 7929  rocess_identity)
-00000220: 04da 0770 7974 686f 6e33 fa02 2d6d fa0b  ...python3..-m..
-00000230: 6874 7470 2e73 6572 7665 72da 0439 3038  http.server..908
-00000240: 3029 02da 0961 6476 656e 7475 7265 da05  0)...adventure..
-00000250: 506f 7065 6e29 03da 046e 616d 65da 046b  Popen)...name..k
-00000260: 696e 64fa 0774 7572 6e20 6f6e da0b 6164  ind..turn on..ad
-00000270: 7665 6e74 7572 655f 3229 0472 0800 0000  venture_2).r....
-00000280: 7209 0000 0072 0a00 0000 da04 3930 3831  r....r......9081
-00000290: da0b 6164 7665 6e74 7572 655f 3329 0472  ..adventure_3).r
-000002a0: 0800 0000 7209 0000 0072 0a00 0000 da04  ....r....r......
-000002b0: 3930 3832 2902 da03 6d61 70da 0876 656e  9082)...map..ven
-000002c0: 7475 7265 7372 1000 0000 e901 0000 007a  turesr.........z
-000002d0: 1368 7474 703a 2f2f 302e 302e 302e 303a  .http://0.0.0.0:
-000002e0: 3930 3830 e9c8 0000 007a 1368 7474 703a  9080.....z.http:
-000002f0: 2f2f 302e 302e 302e 303a 3930 3831 7a13  //0.0.0.0:9081z.
-00000300: 6874 7470 3a2f 2f30 2e30 2e30 2e30 3a39  http://0.0.0.0:9
-00000310: 3038 327a 0874 7572 6e20 6f66 6629 0fda  082z.turn off)..
-00000320: 0770 6174 686c 6962 da04 5061 7468 da08  .pathlib..Path..
-00000330: 5f5f 6669 6c65 5f5f da06 7061 7265 6e74  __file__..parent
-00000340: da07 7265 736f 6c76 65da 0373 7472 7205  ..resolve..strr.
-00000350: 0000 0072 0400 0000 da05 7072 696e 7472  ...r......printr
-00000360: 0200 0000 da04 7469 6d65 da05 736c 6565  ......time..slee
-00000370: 70da 0872 6571 7565 7374 73da 0367 6574  p..requests..get
-00000380: da0b 7374 6174 7573 5f63 6f64 6529 04da  ..status_code)..
-00000390: 0b74 6869 735f 666f 6c64 6572 da07 7468  .this_folder..th
-000003a0: 655f 6d61 7072 1600 0000 da08 7265 7370  e_mapr......resp
-000003b0: 6f6e 7365 a900 7228 0000 00fa 492f 6861  onse..r(....I/ha
-000003c0: 6269 7461 742f 7665 6e75 6573 2f73 7461  bitat/venues/sta
-000003d0: 6765 732f 7665 6e74 7572 6573 2f5f 7374  ges/ventures/_st
-000003e0: 6174 7573 2f6d 6f6e 6974 6f72 732f 325f  atus/monitors/2_
-000003f0: 335f 7665 6e74 7572 6573 2f73 7461 7475  3_ventures/statu
-00000400: 735f 312e 7079 da07 6368 6563 6b5f 3110  s_1.py..check_1.
-00000410: 0000 0073 4e00 0000 1001 0201 0401 0201  ...sN...........
-00000420: 0201 04fe 04ff 0a07 0202 0201 0203 0201  ................
-00000430: 0602 0206 04f9 04fd 020e 0201 0602 0206  ................
-00000440: 04f9 04fd 020f 0201 0602 0206 04f9 04fd  ................
-00000450: 02e4 08fe 0a2e 0a02 0a02 0e01 0a02 0e01  ................
-00000460: 0a02 0e01 0e02 722a 0000 007a 0763 6865  ......r*...z.che
-00000470: 636b 2031 290e da07 5f5f 646f 635f 5f72  ck 1)...__doc__r
-00000480: 1600 0000 7202 0000 0072 2200 0000 da02  ....r....r".....
-00000490: 6f73 7219 0000 00da 076f 732e 7061 7468  osr......os.path
-000004a0: 7203 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
-000004b0: 0373 7973 7220 0000 0072 2a00 0000 da06  .sysr ...r*.....
-000004c0: 6368 6563 6b73 7228 0000 0072 2800 0000  checksr(...r(...
-000004d0: 7228 0000 0072 2900 0000 da08 3c6d 6f64  r(...r).....<mod
-000004e0: 756c 653e 0100 0000 7316 0000 0004 010c  ule>....s.......
-000004f0: 0408 0208 0208 0114 0108 0108 0108 0204  ................
-00000500: 4a08 ff                                  J..
+000001f0: 702e 4a53 4f4e 7a0d 7468 655f 6d61 705f  p.JSONz.the_map_
+00000200: 7061 7468 3ada 0b61 6476 656e 7475 7265  path:..adventure
+00000210: 5f31 da10 7072 6f63 6573 735f 6964 656e  _1..process_iden
+00000220: 7469 7479 2904 da07 7079 7468 6f6e 33fa  tity)...python3.
+00000230: 022d 6dfa 0b68 7474 702e 7365 7276 6572  .-m..http.server
+00000240: da04 3930 3830 2902 da09 6164 7665 6e74  ..9080)...advent
+00000250: 7572 65da 0550 6f70 656e 2903 da04 6e61  ure..Popen)...na
+00000260: 6d65 da04 6b69 6e64 fa07 7475 726e 206f  me..kind..turn o
+00000270: 6eda 0b61 6476 656e 7475 7265 5f32 2904  n..adventure_2).
+00000280: 7208 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
+00000290: 0439 3038 31da 0b61 6476 656e 7475 7265  .9081..adventure
+000002a0: 5f33 2904 7208 0000 0072 0900 0000 720a  _3).r....r....r.
+000002b0: 0000 00da 0439 3038 3229 02da 036d 6170  .....9082)...map
+000002c0: da08 7665 6e74 7572 6573 7210 0000 00e9  ..venturesr.....
+000002d0: 0100 0000 7a13 6874 7470 3a2f 2f30 2e30  ....z.http://0.0
+000002e0: 2e30 2e30 3a39 3038 30e9 c800 0000 7a13  .0.0:9080.....z.
+000002f0: 6874 7470 3a2f 2f30 2e30 2e30 2e30 3a39  http://0.0.0.0:9
+00000300: 3038 317a 1368 7474 703a 2f2f 302e 302e  081z.http://0.0.
+00000310: 302e 303a 3930 3832 7a08 7475 726e 206f  0.0:9082z.turn o
+00000320: 6666 290f da07 7061 7468 6c69 62da 0450  ff)...pathlib..P
+00000330: 6174 68da 085f 5f66 696c 655f 5fda 0670  ath..__file__..p
+00000340: 6172 656e 74da 0772 6573 6f6c 7665 da03  arent..resolve..
+00000350: 7374 7272 0500 0000 7204 0000 00da 0570  strr....r......p
+00000360: 7269 6e74 7202 0000 00da 0474 696d 65da  rintr......time.
+00000370: 0573 6c65 6570 da08 7265 7175 6573 7473  .sleep..requests
+00000380: da03 6765 74da 0b73 7461 7475 735f 636f  ..get..status_co
+00000390: 6465 2904 da0b 7468 6973 5f66 6f6c 6465  de)...this_folde
+000003a0: 72da 0c74 6865 5f6d 6170 5f70 6174 6872  r..the_map_pathr
+000003b0: 1600 0000 da08 7265 7370 6f6e 7365 a900  ......response..
+000003c0: 7228 0000 00fa 492f 6861 6269 7461 742f  r(....I/habitat/
+000003d0: 7665 6e75 6573 2f73 7461 6765 732f 7665  venues/stages/ve
+000003e0: 6e74 7572 6573 2f5f 7374 6174 7573 2f6d  ntures/_status/m
+000003f0: 6f6e 6974 6f72 732f 325f 335f 7665 6e74  onitors/2_3_vent
+00000400: 7572 6573 2f73 7461 7475 735f 312e 7079  ures/status_1.py
+00000410: da07 6368 6563 6b5f 3110 0000 0073 4e00  ..check_1....sN.
+00000420: 0000 1001 0201 0401 0201 0201 04fe 04ff  ................
+00000430: 0a07 0202 0201 0203 0201 0602 0206 04f9  ................
+00000440: 04fd 020e 0201 0602 0206 04f9 04fd 020f  ................
+00000450: 0201 0602 0206 04f9 04fd 02e4 08fe 0a2e  ................
+00000460: 0a02 0a02 0e01 0a02 0e01 0a02 0e01 0e02  ................
+00000470: 722a 0000 007a 0763 6865 636b 2031 290e  r*...z.check 1).
+00000480: da07 5f5f 646f 635f 5f72 1600 0000 7202  ..__doc__r....r.
+00000490: 0000 0072 2200 0000 da02 6f73 7219 0000  ...r".....osr...
+000004a0: 00da 076f 732e 7061 7468 7203 0000 0072  ...os.pathr....r
+000004b0: 0400 0000 7205 0000 00da 0373 7973 7220  ....r......sysr 
+000004c0: 0000 0072 2a00 0000 da06 6368 6563 6b73  ...r*.....checks
+000004d0: 7228 0000 0072 2800 0000 7228 0000 0072  r(...r(...r(...r
+000004e0: 2900 0000 da08 3c6d 6f64 756c 653e 0100  ).....<module>..
+000004f0: 0000 7316 0000 0004 010c 0408 0208 0208  ..s.............
+00000500: 0114 0108 0108 0108 0204 4a08 ff         ..........J..
```

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 import pathlib
 from os.path import dirname, join, normpath
 import sys
 import time
 
 def check_1 ():
 	this_folder = pathlib.Path (__file__).parent.resolve ()
-	the_map = str (
+	the_map_path = str (
 		normpath (join (
 			this_folder, 
 			"ventures_map.JSON"
 		))
 	)
 	
-	print ("the_map:", the_map)
+	print ("the_map_path:", the_map_path)
 	
 	ventures = ventures_map ({
-		"map": the_map,
+		"map": the_map_path,
 		"ventures": [
 			{
 				"name": "adventure_1",
 				"kind": "process_identity",
 				"turn on": {
 					"adventure": [ 
 						"python3",
```

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 20 01:26:19 2024 UTC, .py size: 767 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 bba6 4a66 ff02 0000  o.........Jf....
+00000000: 6f0d 0d0a 0000 0000 3541 4d66 1303 0000  o.......5AMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6403 6c0a  m.Z.m.Z...d.d.l.
 00000070: 5a0a 6401 6403 6c0b 5a0b 6401 6405 6c0c  Z.d.d.l.Z.d.d.l.
@@ -21,41 +21,41 @@
 00000140: 7406 7407 7c00 6401 8302 8301 8301 7d01  t.t.|.d.......}.
 00000150: 7408 6402 7c01 8302 0100 7409 7c01 740a  t.d.|.....t.|.t.
 00000160: 8300 6701 6403 9c02 8301 7d02 7c02 6404  ..g.d.....}.|.d.
 00000170: 1900 8300 0100 740b a00c 6405 a101 7d03  ......t...d...}.
 00000180: 7c03 6a0d 6406 6b02 7330 4a00 8201 7c02  |.j.d.k.s0J...|.
 00000190: 6407 1900 8300 0100 6400 5300 2908 4e7a  d.......d.S.).Nz
 000001a0: 1176 656e 7475 7265 735f 6d61 702e 4a53  .ventures_map.JS
-000001b0: 4f4e 7a08 7468 655f 6d61 703a 2902 da03  ONz.the_map:)...
-000001c0: 6d61 70da 0876 656e 7475 7265 737a 0774  map..venturesz.t
-000001d0: 7572 6e20 6f6e 7a14 6874 7470 3a2f 2f30  urn onz.http://0
-000001e0: 2e30 2e30 2e30 3a31 3030 3030 6994 0100  .0.0.0:10000i...
-000001f0: 007a 0874 7572 6e20 6f66 6629 0eda 0770  .z.turn off)...p
-00000200: 6174 686c 6962 da04 5061 7468 da08 5f5f  athlib..Path..__
-00000210: 6669 6c65 5f5f da06 7061 7265 6e74 da07  file__..parent..
-00000220: 7265 736f 6c76 65da 0373 7472 7205 0000  resolve..strr...
-00000230: 0072 0400 0000 da05 7072 696e 7472 0200  .r......printr..
-00000240: 0000 7206 0000 00da 0872 6571 7565 7374  ..r......request
-00000250: 73da 0367 6574 da0b 7374 6174 7573 5f63  s..get..status_c
-00000260: 6f64 6529 04da 0b74 6869 735f 666f 6c64  ode)...this_fold
-00000270: 6572 da07 7468 655f 6d61 7072 0800 0000  er..the_mapr....
-00000280: da08 7265 7370 6f6e 7365 a900 7216 0000  ..response..r...
-00000290: 00fa 432f 6861 6269 7461 742f 7665 6e75  ..C/habitat/venu
-000002a0: 6573 2f73 7461 6765 732f 7665 6e74 7572  es/stages/ventur
-000002b0: 6573 2f5f 7374 6174 7573 2f6d 6f6e 6974  es/_status/monit
-000002c0: 6f72 732f 335f 7461 736b 2f73 7461 7475  ors/3_task/statu
-000002d0: 735f 312e 7079 da07 6368 6563 6b5f 3115  s_1.py..check_1.
-000002e0: 0000 0073 2200 0000 1001 0201 0401 0201  ...s"...........
-000002f0: 0201 04fe 04ff 0a07 0202 0201 0402 02ff  ................
-00000300: 08fe 0a07 0a04 0e01 0e03 7218 0000 007a  ..........r....z
-00000310: 0763 6865 636b 2031 2910 da07 5f5f 646f  .check 1)...__do
-00000320: 635f 5f72 0800 0000 7202 0000 0072 1000  c__r....r....r..
-00000330: 0000 da02 6f73 7209 0000 00da 076f 732e  ....osr......os.
-00000340: 7061 7468 7203 0000 0072 0400 0000 7205  pathr....r....r.
-00000350: 0000 00da 0373 7973 da04 7469 6d65 da11  .....sys..time..
-00000360: 7361 6e69 7175 652e 6164 7665 6e74 7572  sanique.adventur
-00000370: 6572 0600 0000 7218 0000 00da 0663 6865  er....r......che
-00000380: 636b 7372 1600 0000 7216 0000 0072 1600  cksr....r....r..
-00000390: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000003a0: 3e01 0000 0073 1a00 0000 0403 0c04 0802  >....s..........
-000003b0: 0802 0801 1401 0801 0801 0c02 0601 0802  ................
-000003c0: 041f 08ff                                ....
+000001b0: 4f4e 7a0d 7468 655f 6d61 705f 7061 7468  ONz.the_map_path
+000001c0: 3a29 02da 036d 6170 da08 7665 6e74 7572  :)...map..ventur
+000001d0: 6573 7a07 7475 726e 206f 6e7a 1468 7474  esz.turn onz.htt
+000001e0: 703a 2f2f 302e 302e 302e 303a 3130 3030  p://0.0.0.0:1000
+000001f0: 3069 9401 0000 7a08 7475 726e 206f 6666  0i....z.turn off
+00000200: 290e da07 7061 7468 6c69 62da 0450 6174  )...pathlib..Pat
+00000210: 68da 085f 5f66 696c 655f 5fda 0670 6172  h..__file__..par
+00000220: 656e 74da 0772 6573 6f6c 7665 da03 7374  ent..resolve..st
+00000230: 7272 0500 0000 7204 0000 00da 0570 7269  rr....r......pri
+00000240: 6e74 7202 0000 0072 0600 0000 da08 7265  ntr....r......re
+00000250: 7175 6573 7473 da03 6765 74da 0b73 7461  quests..get..sta
+00000260: 7475 735f 636f 6465 2904 da0b 7468 6973  tus_code)...this
+00000270: 5f66 6f6c 6465 72da 0c74 6865 5f6d 6170  _folder..the_map
+00000280: 5f70 6174 6872 0800 0000 da08 7265 7370  _pathr......resp
+00000290: 6f6e 7365 a900 7216 0000 00fa 432f 6861  onse..r.....C/ha
+000002a0: 6269 7461 742f 7665 6e75 6573 2f73 7461  bitat/venues/sta
+000002b0: 6765 732f 7665 6e74 7572 6573 2f5f 7374  ges/ventures/_st
+000002c0: 6174 7573 2f6d 6f6e 6974 6f72 732f 335f  atus/monitors/3_
+000002d0: 7461 736b 2f73 7461 7475 735f 312e 7079  task/status_1.py
+000002e0: da07 6368 6563 6b5f 3115 0000 0073 2200  ..check_1....s".
+000002f0: 0000 1001 0201 0401 0201 0201 04fe 04ff  ................
+00000300: 0a07 0202 0201 0402 02ff 08fe 0a07 0a04  ................
+00000310: 0e01 0e03 7218 0000 007a 0763 6865 636b  ....r....z.check
+00000320: 2031 2910 da07 5f5f 646f 635f 5f72 0800   1)...__doc__r..
+00000330: 0000 7202 0000 0072 1000 0000 da02 6f73  ..r....r......os
+00000340: 7209 0000 00da 076f 732e 7061 7468 7203  r......os.pathr.
+00000350: 0000 0072 0400 0000 7205 0000 00da 0373  ...r....r......s
+00000360: 7973 da04 7469 6d65 da11 7361 6e69 7175  ys..time..saniqu
+00000370: 652e 6164 7665 6e74 7572 6572 0600 0000  e.adventurer....
+00000380: 7218 0000 00da 0663 6865 636b 7372 1600  r......checksr..
+00000390: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+000003a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000003b0: 1a00 0000 0403 0c04 0802 0802 0801 1401  ................
+000003c0: 0801 0801 0c02 0601 0802 041f 08ff       ..............
```

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 import time
 
 from sanique.adventure import sanique_adventure
 sanique_adventure ()
 
 def check_1 ():
 	this_folder = pathlib.Path (__file__).parent.resolve ()
-	the_map = str (
+	the_map_path = str (
 		normpath (join (
 			this_folder, 
 			"ventures_map.JSON"
 		))
 	)
 	
-	print ("the_map:", the_map)
+	print ("the_map_path:", the_map_path)
 	
 	ventures = ventures_map ({
-		"map": the_map,
+		"map": the_map_path,
 		"ventures": [
 			sanique_adventure ()
 		]
 	})
 	
 	ventures ["turn on"] ()
```

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status.proc.py` & `ventures-1.3.0/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 18 18:45:09 2024 UTC, .py size: 1200 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 35f7 4866 b004 0000  o.......5.Hf....
+00000000: 6f0d 0d0a 0000 0000 ea46 4d66 a504 0000  o........FMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 8400 5a07 6406 6407 8400 5a08 6402  d...Z.d.d...Z.d.
 00000070: 5300 2908 7a05 270a 090a 22e9 0000 0000  S.).z.'...".....
@@ -19,53 +19,48 @@
 00000120: 7372 0300 0000 da07 7665 6e74 7572 65a9  sr......venture.
 00000130: 0072 0700 0000 fa2e 2f68 6162 6974 6174  .r....../habitat
 00000140: 2f76 656e 7565 732f 7374 6167 6573 2f76  /venues/stages/v
 00000150: 656e 7475 7265 732f 706c 6179 732f 6973  entures/plays/is
 00000160: 5f6f 6e2e 7079 da0c 6669 6e64 5f76 656e  _on.py..find_ven
 00000170: 7475 7265 1400 0000 730a 0000 0008 010c  ture....s.......
 00000180: 0108 0102 ff10 0372 0900 0000 6301 0000  .......r....c...
-00000190: 0000 0000 0000 0000 000c 0000 0008 0000  ................
-000001a0: 0043 0000 0073 d600 0000 7c00 6401 1900  .C...s....|.d...
-000001b0: 7d01 7c00 6402 1900 7d02 7400 7c01 6403  }.|.d...}.t.|.d.
-000001c0: 8302 8f0d 7d03 7401 a002 7c03 a101 7d04  ....}.t...|...}.
-000001d0: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-000001e0: 731d 7701 0100 0100 0100 5900 0100 6900  s.w.......Y...i.
-000001f0: 7d05 7c04 4400 5d3a 7d06 7c04 7c06 1900  }.|.D.]:}.|.|...
-00000200: 7d07 7c07 6404 1900 7d08 7c08 6405 6b02  }.|.d...}.|.d.k.
-00000210: 7244 7c07 6405 1900 7d09 7403 7c09 8301  rD|.d...}.t.|...
-00000220: 7d0a 7c09 7c0a 6406 9c02 7c05 7c06 3c00  }.|.|.d...|.|.<.
-00000230: 7126 7c08 6407 6b02 7259 7404 7c02 7c06  q&|.d.k.rYt.|.|.
-00000240: 8302 7d0b 7c0b 6408 1900 8300 7d0a 6409  ..}.|.d.....}.d.
-00000250: 7c0a 6901 7c05 7c06 3c00 7126 7405 640a  |.i.|.|.<.q&t.d.
-00000260: 7c08 9b00 640b 9d03 8301 8201 7406 6a07  |...d.......t.j.
-00000270: 640c 7c05 6901 640d 8d01 0100 6400 5300  d.|.i.d.....d.S.
-00000280: 290e 4eda 0774 6865 5f6d 6170 7205 0000  ).N..the_mapr...
-00000290: 00da 0172 da04 6b69 6e64 da10 7072 6f63  ...r..kind..proc
-000002a0: 6573 735f 6964 656e 7469 7479 2902 720d  ess_identity).r.
-000002b0: 0000 00da 0673 7461 7475 73da 0474 6173  .....status..tas
-000002c0: 6b7a 0569 7320 6f6e 720e 0000 007a 064b  kz.is onr....z.K
-000002d0: 696e 6420 227a 0c22 206e 6f74 2066 6f75  ind "z." not fou
-000002e0: 6e64 2eda 0873 7461 7475 7365 7329 01da  nd...statuses)..
-000002f0: 0464 6174 6129 08da 046f 7065 6eda 046a  .data)...open..j
-00000300: 736f 6eda 046c 6f61 6472 0200 0000 7209  son..loadr....r.
-00000310: 0000 0072 0400 0000 da04 7269 6368 da0a  ...r......rich..
-00000320: 7072 696e 745f 6a73 6f6e 290c da06 7061  print_json)...pa
-00000330: 636b 6574 720a 0000 0072 0500 0000 da02  cketr....r......
-00000340: 4650 da07 6272 6163 6b65 7472 1000 0000  FP..bracketr....
-00000350: da09 6164 7665 6e74 7572 65da 1161 6476  ..adventure..adv
-00000360: 656e 7475 7265 5f64 6574 6169 6c73 720c  enture_detailsr.
-00000370: 0000 0072 0d00 0000 720e 0000 0072 0600  ...r....r....r..
-00000380: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
-00000390: 00da 0569 735f 6f6e 1c00 0000 7336 0000  ...is_on....s6..
-000003a0: 0008 0108 010c 020c 011c ff04 0408 0108  ................
-000003b0: 0108 0108 0308 0108 0102 0302 010a fe02  ................
-000003c0: 0508 020a 010a 0104 0308 ff02 0410 0204  ................
-000003d0: 0204 0108 ff04 0472 1c00 0000 2909 da07  .......r....)...
-000003e0: 5f5f 646f 635f 5fda 0670 7375 7469 6cda  __doc__..psutil.
-000003f0: 0474 696d 6572 1300 0000 7215 0000 00da  .timer....r.....
-00000400: 2676 656e 7475 7265 732e 7574 696c 6974  &ventures.utilit
-00000410: 6965 732e 7072 6f63 6573 732e 6368 6563  ies.process.chec
-00000420: 6b5f 6973 5f6f 6e72 0200 0000 7209 0000  k_is_onr....r...
-00000430: 0072 1c00 0000 7207 0000 0072 0700 0000  .r....r....r....
-00000440: 7207 0000 0072 0800 0000 da08 3c6d 6f64  r....r......<mod
-00000450: 756c 653e 0100 0000 7310 0000 0004 0108  ule>....s.......
-00000460: 0608 0108 0108 030c 0308 040c 08         .............
+00000190: 0000 0000 0000 0000 000a 0000 0005 0000  ................
+000001a0: 0043 0000 0073 a200 0000 7c00 6401 1900  .C...s....|.d...
+000001b0: 7d01 7c00 6402 1900 7d02 6900 7d03 7c01  }.|.d...}.i.}.|.
+000001c0: 4400 5d3a 7d04 7c01 7c04 1900 7d05 7c05  D.]:}.|.|...}.|.
+000001d0: 6403 1900 7d06 7c06 6404 6b02 722a 7c05  d...}.|.d.k.r*|.
+000001e0: 6404 1900 7d07 7400 7c07 8301 7d08 7c07  d...}.t.|...}.|.
+000001f0: 7c08 6405 9c02 7c03 7c04 3c00 710c 7c06  |.d...|.|.<.q.|.
+00000200: 6406 6b02 723f 7401 7c02 7c04 8302 7d09  d.k.r?t.|.|...}.
+00000210: 7c09 6407 1900 8300 7d08 6408 7c08 6901  |.d.....}.d.|.i.
+00000220: 7c03 7c04 3c00 710c 7402 6409 7c06 9b00  |.|.<.q.t.d.|...
+00000230: 640a 9d03 8301 8201 7403 6a04 640b 7c03  d.......t.j.d.|.
+00000240: 6901 640c 8d01 0100 6400 5300 290d 4eda  i.d.....d.S.).N.
+00000250: 1476 656e 7475 7265 735f 6d61 705f 6272  .ventures_map_br
+00000260: 6163 6b65 7472 0500 0000 da04 6b69 6e64  acketr......kind
+00000270: da10 7072 6f63 6573 735f 6964 656e 7469  ..process_identi
+00000280: 7479 2902 720c 0000 00da 0673 7461 7475  ty).r......statu
+00000290: 73da 0474 6173 6b7a 0569 7320 6f6e 720d  s..taskz.is onr.
+000002a0: 0000 007a 064b 696e 6420 227a 0c22 206e  ...z.Kind "z." n
+000002b0: 6f74 2066 6f75 6e64 2eda 0873 7461 7475  ot found...statu
+000002c0: 7365 7329 01da 0464 6174 6129 0572 0200  ses)...data).r..
+000002d0: 0000 7209 0000 0072 0400 0000 da04 7269  ..r....r......ri
+000002e0: 6368 da0a 7072 696e 745f 6a73 6f6e 290a  ch..print_json).
+000002f0: da06 7061 636b 6574 720a 0000 0072 0500  ..packetr....r..
+00000300: 0000 720f 0000 00da 0961 6476 656e 7475  ..r......adventu
+00000310: 7265 da11 6164 7665 6e74 7572 655f 6465  re..adventure_de
+00000320: 7461 696c 7372 0b00 0000 720c 0000 0072  tailsr....r....r
+00000330: 0d00 0000 7206 0000 0072 0700 0000 7207  ....r....r....r.
+00000340: 0000 0072 0800 0000 da05 6973 5f6f 6e1c  ...r......is_on.
+00000350: 0000 0073 3000 0000 0801 0801 0403 0801  ...s0...........
+00000360: 0801 0801 0803 0801 0801 0203 0201 0afe  ................
+00000370: 0205 0802 0a01 0a01 0403 08ff 0204 1002  ................
+00000380: 0402 0401 08ff 0404 7216 0000 0029 09da  ........r....)..
+00000390: 075f 5f64 6f63 5f5f da06 7073 7574 696c  .__doc__..psutil
+000003a0: da04 7469 6d65 da04 6a73 6f6e 7211 0000  ..time..jsonr...
+000003b0: 00da 2676 656e 7475 7265 732e 7574 696c  ..&ventures.util
+000003c0: 6974 6965 732e 7072 6f63 6573 732e 6368  ities.process.ch
+000003d0: 6563 6b5f 6973 5f6f 6e72 0200 0000 7209  eck_is_onr....r.
+000003e0: 0000 0072 1600 0000 7207 0000 0072 0700  ...r....r....r..
+000003f0: 0000 7207 0000 0072 0800 0000 da08 3c6d  ..r....r......<m
+00000400: 6f64 756c 653e 0100 0000 7310 0000 0004  odule>....s.....
+00000410: 0108 0608 0108 0108 030c 0308 040c 08    ...............
```

### Comparing `ventures-1.2.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 20 00:56:04 2024 UTC, .py size: 2439 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a49f 4a66 8709 0000  o.........Jf....
+00000000: 6f0d 0d0a 0000 0000 3541 4d66 8c09 0000  o.......5AMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6406 6407 6c09 5a09 6406 6407 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 6406 6407 6c0b 5a0b 6406 6407 6c0c  Z.d.d.l.Z.d.d.l.
@@ -41,70 +41,70 @@
 00000280: 007d 0b74 046a 0564 1864 197c 0a7c 0c64  .}.t.j.d.d.|.|.d
 00000290: 1a19 007c 0b64 1b9c 0469 0164 088d 0101  ...|.d...i.d....
 000002a0: 007c 0b64 0c6b 0272 cc6e 1974 0ba0 0c64  .|.d.k.r.n.t...d
 000002b0: 11a1 0101 007c 0a64 1137 007d 0a7c 0a64  .....|.d.7.}.|.d
 000002c0: 126b 0272 e474 0d64 137c 0a9b 0064 147c  .k.r.t.d.|...d.|
 000002d0: 069b 0064 159d 0583 0182 0171 b371 2b74  ...d.......q.q+t
 000002e0: 0f7c 017c 0464 1c9c 0283 0101 0064 0053  .|.|.d.......d.S
-000002f0: 0029 1d4e da07 7468 655f 6d61 70da 0876  .).N..the_map..v
-00000300: 656e 7475 7265 73da 0172 7a15 7665 6e74  entures..rz.vent
-00000310: 7572 6573 5f6d 6170 5f62 7261 636b 6574  ures_map_bracket
-00000320: 3ada 046b 696e 647a 0874 7572 6e20 6f66  :..kindz.turn of
-00000330: 6629 02da 0470 6c61 79da 0961 6476 656e  f)...play..adven
-00000340: 7475 7265 2901 da04 6461 7461 da10 7072  ture)...data..pr
-00000350: 6f63 6573 735f 6964 656e 7469 7479 da00  ocess_identity..
-00000360: 2902 720b 0000 0072 0e00 0000 da03 6f66  ).r....r......of
-00000370: 6672 0600 0000 5429 02da 046e 616d 65da  fr....T)...name.
-00000380: 0673 7461 7475 7329 0272 0b00 0000 7a12  .status).r....z.
-00000390: 7374 6174 7573 2063 6865 636b 2063 7963  status check cyc
-000003a0: 6c65 e901 0000 00e9 0a00 0000 7a06 4166  le..........z.Af
-000003b0: 7465 7220 7a08 206c 6f6f 7073 2c20 7a12  ter z. loops, z.
-000003c0: 2064 6964 206e 6f74 2074 7572 6e20 6f66   did not turn of
-000003d0: 662e da04 7461 736b 7a05 6973 206f 6e7a  f...taskz.is onz
-000003e0: 1976 656e 7475 7265 2073 7461 7475 7320  .venture status 
-000003f0: 6368 6563 6b20 6c6f 6f70 7a17 6166 7465  check loopz.afte
-00000400: 7220 7475 726e 206f 6666 2077 6173 2073  r turn off was s
-00000410: 656e 7472 1100 0000 2904 da04 7768 656e  entr....)...when
-00000420: da04 6c6f 6f70 7211 0000 0072 1200 0000  ..loopr....r....
-00000430: 2902 da04 7061 7468 da07 6272 6163 6b65  )...path..bracke
-00000440: 7429 10da 046f 7065 6eda 046a 736f 6eda  t)...open..json.
-00000450: 046c 6f61 64da 0570 7269 6e74 da04 7269  .load..print..ri
-00000460: 6368 da0a 7072 696e 745f 6a73 6f6e 7205  ch..print_jsonr.
-00000470: 0000 00da 026f 73da 046b 696c 6cda 0673  .....os..kill..s
-00000480: 6967 6e61 6cda 0753 4947 5445 524d da04  ignal..SIGTERM..
-00000490: 7469 6d65 da05 736c 6565 70da 0945 7863  time..sleep..Exc
-000004a0: 6570 7469 6f6e 7204 0000 0072 0200 0000  eptionr....r....
-000004b0: 290d da06 7061 636b 6574 da0c 7468 655f  )...packet..the_
-000004c0: 6d61 705f 7061 7468 7208 0000 00da 0246  map_pathr......F
-000004d0: 50da 1476 656e 7475 7265 735f 6d61 705f  P..ventures_map_
-000004e0: 6272 6163 6b65 74da 0974 6f5f 6465 6c65  bracket..to_dele
-000004f0: 7465 7211 0000 0072 0c00 0000 720a 0000  ter....r....r...
-00000500: 0072 0e00 0000 7217 0000 0072 1200 0000  .r....r....r....
-00000510: da07 7665 6e74 7572 65a9 0072 2d00 0000  ..venture..r-...
-00000520: fa31 2f68 6162 6974 6174 2f76 656e 7565  .1/habitat/venue
-00000530: 732f 7374 6167 6573 2f76 656e 7475 7265  s/stages/venture
-00000540: 732f 706c 6179 732f 7475 726e 5f6f 6666  s/plays/turn_off
-00000550: 2e70 79da 0874 7572 6e5f 6f66 661e 0000  .py..turn_off...
-00000560: 0073 8e00 0000 0801 0801 0c02 0c01 1cff  .s..............
-00000570: 0a03 0402 0801 0801 0801 0403 0201 0201  ................
-00000580: 0afe 0806 0c01 0801 0402 0201 0601 0afe  ................
-00000590: 0c05 0e01 0c01 0403 0201 0801 0401 0201  ................
-000005a0: 0202 0201 04fe 0afe 0808 0201 0a02 0802  ................
-000005b0: 0801 0201 1001 04ff 02ef 0816 0a01 0e02  ................
-000005c0: 0a01 0402 0201 0a01 0402 0201 0201 0201  ................
-000005d0: 0601 0201 04fc 08ff 0809 0201 0a02 0802  ................
-000005e0: 0801 0201 1001 04ff 02ed 0280 021b 0201  ................
-000005f0: 0201 0cfe 722f 0000 0029 0fda 075f 5f64  ....r/...)...__d
-00000600: 6f63 5f5f da12 7574 696c 6974 6965 732e  oc__..utilities.
-00000610: 6d61 702e 6574 6368 7202 0000 00da 1275  map.etchr......u
-00000620: 7469 6c69 7469 6573 2e6d 6170 2e73 6361  tilities.map.sca
-00000630: 6e72 0300 0000 da1f 7574 696c 6974 6965  nr......utilitie
-00000640: 732e 7665 6e74 7572 6573 2e66 696e 645f  s.ventures.find_
-00000650: 7665 6e74 7572 6572 0400 0000 da1d 7574  venturer......ut
-00000660: 696c 6974 6965 732e 7072 6f63 6573 732e  ilities.process.
-00000670: 6368 6563 6b5f 6973 5f6f 6e72 0500 0000  check_is_onr....
-00000680: 721e 0000 0072 1b00 0000 7222 0000 0072  r....r....r"...r
-00000690: 2000 0000 7224 0000 0072 2f00 0000 722d   ...r$...r/...r-
-000006a0: 0000 0072 2d00 0000 722d 0000 0072 2e00  ...r-...r-...r..
-000006b0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000006c0: 7316 0000 0004 020c 0a0c 010c 010c 0108  s...............
-000006d0: 0308 0308 0108 0108 010c 05              ...........
+000002f0: 0029 1d4e da0c 7468 655f 6d61 705f 7061  .).N..the_map_pa
+00000300: 7468 da08 7665 6e74 7572 6573 da01 727a  th..ventures..rz
+00000310: 1576 656e 7475 7265 735f 6d61 705f 6272  .ventures_map_br
+00000320: 6163 6b65 743a da04 6b69 6e64 7a08 7475  acket:..kindz.tu
+00000330: 726e 206f 6666 2902 da04 706c 6179 da09  rn off)...play..
+00000340: 6164 7665 6e74 7572 6529 01da 0464 6174  adventure)...dat
+00000350: 61da 1070 726f 6365 7373 5f69 6465 6e74  a..process_ident
+00000360: 6974 79da 0029 0272 0b00 0000 720e 0000  ity..).r....r...
+00000370: 00da 036f 6666 7206 0000 0054 2902 da04  ...offr....T)...
+00000380: 6e61 6d65 da06 7374 6174 7573 2902 720b  name..status).r.
+00000390: 0000 007a 1273 7461 7475 7320 6368 6563  ...z.status chec
+000003a0: 6b20 6379 636c 65e9 0100 0000 e90a 0000  k cycle.........
+000003b0: 007a 0641 6674 6572 207a 0820 6c6f 6f70  .z.After z. loop
+000003c0: 732c 207a 1220 6469 6420 6e6f 7420 7475  s, z. did not tu
+000003d0: 726e 206f 6666 2eda 0474 6173 6b7a 0569  rn off...taskz.i
+000003e0: 7320 6f6e 7a19 7665 6e74 7572 6520 7374  s onz.venture st
+000003f0: 6174 7573 2063 6865 636b 206c 6f6f 707a  atus check loopz
+00000400: 1761 6674 6572 2074 7572 6e20 6f66 6620  .after turn off 
+00000410: 7761 7320 7365 6e74 7211 0000 0029 04da  was sentr....)..
+00000420: 0477 6865 6eda 046c 6f6f 7072 1100 0000  .when..loopr....
+00000430: 7212 0000 0029 02da 0470 6174 68da 0762  r....)...path..b
+00000440: 7261 636b 6574 2910 da04 6f70 656e da04  racket)...open..
+00000450: 6a73 6f6e da04 6c6f 6164 da05 7072 696e  json..load..prin
+00000460: 74da 0472 6963 68da 0a70 7269 6e74 5f6a  t..rich..print_j
+00000470: 736f 6e72 0500 0000 da02 6f73 da04 6b69  sonr......os..ki
+00000480: 6c6c da06 7369 676e 616c da07 5349 4754  ll..signal..SIGT
+00000490: 4552 4dda 0474 696d 65da 0573 6c65 6570  ERM..time..sleep
+000004a0: da09 4578 6365 7074 696f 6e72 0400 0000  ..Exceptionr....
+000004b0: 7202 0000 0029 0dda 0670 6163 6b65 7472  r....)...packetr
+000004c0: 0700 0000 7208 0000 00da 0246 50da 1476  ....r......FP..v
+000004d0: 656e 7475 7265 735f 6d61 705f 6272 6163  entures_map_brac
+000004e0: 6b65 74da 0974 6f5f 6465 6c65 7465 7211  ket..to_deleter.
+000004f0: 0000 0072 0c00 0000 720a 0000 0072 0e00  ...r....r....r..
+00000500: 0000 7217 0000 0072 1200 0000 da07 7665  ..r....r......ve
+00000510: 6e74 7572 65a9 0072 2c00 0000 fa31 2f68  nture..r,....1/h
+00000520: 6162 6974 6174 2f76 656e 7565 732f 7374  abitat/venues/st
+00000530: 6167 6573 2f76 656e 7475 7265 732f 706c  ages/ventures/pl
+00000540: 6179 732f 7475 726e 5f6f 6666 2e70 79da  ays/turn_off.py.
+00000550: 0874 7572 6e5f 6f66 661e 0000 0073 8e00  .turn_off....s..
+00000560: 0000 0801 0801 0c02 0c01 1cff 0a03 0402  ................
+00000570: 0801 0801 0801 0403 0201 0201 0afe 0806  ................
+00000580: 0c01 0801 0402 0201 0601 0afe 0c05 0e01  ................
+00000590: 0c01 0403 0201 0801 0401 0201 0202 0201  ................
+000005a0: 04fe 0afe 0808 0201 0a02 0802 0801 0201  ................
+000005b0: 1001 04ff 02ef 0816 0a01 0e02 0a01 0402  ................
+000005c0: 0201 0a01 0402 0201 0201 0201 0601 0201  ................
+000005d0: 04fc 08ff 0809 0201 0a02 0802 0801 0201  ................
+000005e0: 1001 04ff 02ed 0280 021b 0201 0201 0cfe  ................
+000005f0: 722e 0000 0029 0fda 075f 5f64 6f63 5f5f  r....)...__doc__
+00000600: da12 7574 696c 6974 6965 732e 6d61 702e  ..utilities.map.
+00000610: 6574 6368 7202 0000 00da 1275 7469 6c69  etchr......utili
+00000620: 7469 6573 2e6d 6170 2e73 6361 6e72 0300  ties.map.scanr..
+00000630: 0000 da1f 7574 696c 6974 6965 732e 7665  ....utilities.ve
+00000640: 6e74 7572 6573 2e66 696e 645f 7665 6e74  ntures.find_vent
+00000650: 7572 6572 0400 0000 da1d 7574 696c 6974  urer......utilit
+00000660: 6965 732e 7072 6f63 6573 732e 6368 6563  ies.process.chec
+00000670: 6b5f 6973 5f6f 6e72 0500 0000 721e 0000  k_is_onr....r...
+00000680: 0072 1b00 0000 7222 0000 0072 2000 0000  .r....r"...r ...
+00000690: 7224 0000 0072 2e00 0000 722c 0000 0072  r$...r....r,...r
+000006a0: 2c00 0000 722c 0000 0072 2d00 0000 da08  ,...r,...r-.....
+000006b0: 3c6d 6f64 756c 653e 0100 0000 7316 0000  <module>....s...
+000006c0: 0004 020c 0a0c 010c 010c 0108 0308 0308  ................
+000006d0: 0108 0108 010c 05                        .......
```

### Comparing `ventures-1.2.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 21 20:24:14 2024 UTC, .py size: 3140 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,109 @@
-00000000: 6f0d 0d0a 0000 0000 ee02 4d66 440c 0000  o.........MfD...
+00000000: 6f0d 0d0a 0000 0000 a846 4d66 b208 0000  o........FMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
+00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
-00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
-00000070: 5a0a 6405 6407 6c0b 5a0b 6405 6407 6c0c  Z.d.d.l.Z.d.d.l.
-00000080: 5a0c 0900 6408 6409 8400 5a0d 6407 5300  Z...d.d...Z.d.S.
-00000090: 290a e902 0000 0029 01da 0c68 696b 655f  )......)...hike_
-000000a0: 7061 7373 6976 6529 01da 0865 7463 685f  passive)...etch_
-000000b0: 6d61 7029 01da 0873 6361 6e5f 6d61 7029  map)...scan_map)
-000000c0: 01da 0c66 696e 645f 7665 6e74 7572 65e9  ...find_venture.
-000000d0: 0000 0000 2901 da0b 6368 6563 6b5f 6973  ....)...check_is
-000000e0: 5f6f 6e4e 6301 0000 0000 0000 0000 0000  _onNc...........
-000000f0: 000d 0000 0008 0000 0043 0000 0073 2a02  .........C...s*.
-00000100: 0000 7c00 6401 1900 7d01 7c00 6402 1900  ..|.d...}.|.d...
-00000110: 7d02 6900 7d03 7400 6a01 a002 7c02 a101  }.i.}.t.j...|...
-00000120: 7216 7403 6403 7c02 6901 8301 7d03 7c01  r.t.d.|.i...}.|.
-00000130: 4400 5df3 7d04 7c04 6404 1900 6405 1900  D.].}.|.d...d...
-00000140: 7d05 7c04 6406 1900 7d06 7c04 6407 1900  }.|.d...}.|.d...
-00000150: 7d07 7c07 7c03 7600 7258 7c06 6408 6b02  }.|.|.v.rX|.d.k.
-00000160: 7245 7c03 7c07 1900 6408 1900 6409 6b03  rE|.|...d...d.k.
-00000170: 7245 7404 7c03 7c07 1900 6408 1900 8301  rEt.|.|...d.....
-00000180: 7d08 7c08 640a 6b02 7245 7118 7c06 640b  }.|.d.k.rEq.|.d.
-00000190: 6b02 7258 7405 7c01 7c07 8302 7d09 7c09  k.rXt.|.|...}.|.
-000001a0: 640c 1900 8300 7d08 7c08 640a 6b02 7258  d.....}.|.d.k.rX
-000001b0: 7118 7c06 6408 6b02 72c2 7406 640d 7c04  q.|.d.k.r.t.d.|.
-000001c0: 8302 0100 6900 7d0a 6404 7c04 7600 727d  ....i.}.d.|.v.r}
-000001d0: 640e 7c04 6404 1900 7600 727d 7407 7c04  d.|.d...v.r}t.|.
-000001e0: 6404 1900 640e 1900 8301 7408 6b02 727d  d...d.....t.k.r}
-000001f0: 7c04 6404 1900 640e 1900 7d0a 7409 7c05  |.d...d...}.t.|.
-00000200: 7c0a 640f 9c02 8301 7d0b 6410 7d0c 0900  |.d.....}.d.}...
-00000210: 7404 7c0b 6408 1900 8301 7d08 740a 6a0b  t.|.d.....}.t.j.
-00000220: 6412 6413 7c0c 7c07 7c08 6414 9c04 6901  d.d.|.|.|.d...i.
-00000230: 6415 8d01 0100 7c08 640a 6b02 729f 6e19  d.....|.d.k.r.n.
-00000240: 740c a00d 6416 a101 0100 7c0c 6416 3700  t...d.....|.d.7.
-00000250: 7d0c 7c0c 6417 6b02 72b7 740e 6418 7c0c  }.|.d.k.r.t.d.|.
-00000260: 9b00 6419 7c07 9b00 641a 9d05 8301 8201  ..d.|...d.......
-00000270: 7187 7c06 7c0b 6408 1900 641b 9c02 7c03  q.|.|.d...d...|.
-00000280: 7c07 3c00 7118 7c06 640b 6b02 9001 7204  |.<.q.|.d.k...r.
-00000290: 7c05 8300 0100 6410 7d0c 0900 7c04 640c  |.....d.}...|.d.
-000002a0: 1900 8300 7d08 740a 6a0b 6412 6413 7c0c  ....}.t.j.d.d.|.
-000002b0: 7c07 7c08 6414 9c04 6901 6415 8d01 0100  |.|.d...i.d.....
-000002c0: 7c08 640a 6b02 72e4 6e19 740c a00d 6416  |.d.k.r.n.t...d.
-000002d0: a101 0100 7c0c 6416 3700 7d0c 7c0c 6417  ....|.d.7.}.|.d.
-000002e0: 6b02 72fc 740e 6418 7c0c 9b00 6419 7c07  k.r.t.d.|...d.|.
-000002f0: 9b00 641a 9d05 8301 8201 71cd 6406 7c06  ..d.......q.d.|.
-00000300: 6901 7c03 7c07 3c00 7118 740e 641c 7c06  i.|.|.<.q.t.d.|.
-00000310: 9b00 641d 9d03 8301 8201 740f 7c02 7c03  ..d.......t.|.|.
-00000320: 641e 9c02 8301 0100 7c03 5300 291f 4eda  d.......|.S.).N.
-00000330: 0876 656e 7475 7265 73da 036d 6170 da04  .ventures..map..
-00000340: 7061 7468 7a07 7475 726e 206f 6eda 0961  pathz.turn on..a
-00000350: 6476 656e 7475 7265 da04 6b69 6e64 da04  dventure..kind..
-00000360: 6e61 6d65 da10 7072 6f63 6573 735f 6964  name..process_id
-00000370: 656e 7469 7479 da00 da02 6f6e da04 7461  entity....on..ta
-00000380: 736b 7a05 6973 206f 6e7a 0a61 6476 656e  skz.is onz.adven
-00000390: 7475 7265 3ada 0550 6f70 656e 2902 da06  ture:..Popen)...
-000003a0: 7363 7269 7074 7212 0000 0072 0600 0000  scriptr....r....
-000003b0: 547a 1976 656e 7475 7265 2073 7461 7475  Tz.venture statu
-000003c0: 7320 6368 6563 6b20 6c6f 6f70 7a16 6166  s check loopz.af
-000003d0: 7465 7220 7475 726e 206f 6e20 7761 7320  ter turn on was 
-000003e0: 7365 6e74 2904 da04 7768 656e da04 6c6f  sent)...when..lo
-000003f0: 6f70 720d 0000 00da 0673 7461 7475 7329  opr......status)
-00000400: 01da 0464 6174 61e9 0100 0000 e90a 0000  ...data.........
-00000410: 007a 0641 6674 6572 207a 0820 6c6f 6f70  .z.After z. loop
-00000420: 732c 207a 1120 6469 6420 6e6f 7420 7475  s, z. did not tu
-00000430: 726e 206f 6e2e 2902 720c 0000 0072 0e00  rn on.).r....r..
-00000440: 0000 7a06 4b69 6e64 2022 7a0f 2077 6173  ..z.Kind "z. was
-00000450: 206e 6f74 2066 6f75 6e64 2e29 0272 0a00   not found.).r..
-00000460: 0000 da07 6272 6163 6b65 7429 10da 026f  ....bracket)...o
-00000470: 7372 0a00 0000 da06 6578 6973 7473 7204  sr......existsr.
-00000480: 0000 0072 0700 0000 7205 0000 00da 0570  ...r....r......p
-00000490: 7269 6e74 da04 7479 7065 da04 6469 6374  rint..type..dict
-000004a0: 7202 0000 00da 0472 6963 68da 0a70 7269  r......rich..pri
-000004b0: 6e74 5f6a 736f 6eda 0474 696d 65da 0573  nt_json..time..s
-000004c0: 6c65 6570 da09 4578 6365 7074 696f 6e72  leep..Exceptionr
-000004d0: 0300 0000 290d da06 7061 636b 6574 7208  ....)...packetr.
-000004e0: 0000 00da 0c74 6865 5f6d 6170 5f70 6174  .....the_map_pat
-000004f0: 68da 1476 656e 7475 7265 735f 6d61 705f  h..ventures_map_
-00000500: 6272 6163 6b65 7472 0b00 0000 da10 6164  bracketr......ad
-00000510: 7665 6e74 7572 655f 7363 7269 7074 720c  venture_scriptr.
-00000520: 0000 0072 0d00 0000 7216 0000 00da 0776  ...r....r......v
-00000530: 656e 7475 7265 da0a 506f 7065 6e5f 6b65  enture..Popen_ke
-00000540: 7973 da07 7072 6f63 6573 7372 1500 0000  ys..processr....
-00000550: a900 722c 0000 00fa 302f 6861 6269 7461  ..r,....0/habita
-00000560: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
-00000570: 7665 6e74 7572 6573 2f70 6c61 7973 2f74  ventures/plays/t
-00000580: 7572 6e5f 6f6e 2e70 79da 0774 7572 6e5f  urn_on.py..turn_
-00000590: 6f6e 2a00 0000 73ae 0000 0008 0108 0104  on*...s.........
-000005a0: 040c 0102 0104 0106 ff08 040c 0108 0108  ................
-000005b0: 0108 0708 0110 0110 0108 0102 0208 020a  ................
-000005c0: 010a 0108 0102 0108 040a 0104 0208 010c  ................
-000005d0: 0114 010c 0102 0202 0102 0108 fe04 0502  ................
-000005e0: 010c 0104 0102 0102 0102 0102 0102 0104  ................
-000005f0: fc08 ff08 0902 010a 0208 0208 0102 0110  ................
-00000600: 0104 ff02 ee02 1706 010a fe02 050a 0206  ................
-00000610: 0104 0202 010a 0104 0102 0102 0102 0102  ................
-00000620: 0102 0104 fc08 ff08 0902 010a 0208 0208  ................
-00000630: 0102 0110 0104 ff02 ee04 170a ff10 0602  ................
-00000640: 0302 0102 0108 fe04 0572 2e00 0000 290e  .........r....).
-00000650: da16 7574 696c 6974 6965 732e 6869 6b65  ..utilities.hike
-00000660: 5f70 6173 7369 7665 7202 0000 00da 1275  _passiver......u
-00000670: 7469 6c69 7469 6573 2e6d 6170 2e65 7463  tilities.map.etc
-00000680: 6872 0300 0000 da12 7574 696c 6974 6965  hr......utilitie
-00000690: 732e 6d61 702e 7363 616e 7204 0000 00da  s.map.scanr.....
-000006a0: 1f75 7469 6c69 7469 6573 2e76 656e 7475  .utilities.ventu
-000006b0: 7265 732e 6669 6e64 5f76 656e 7475 7265  res.find_venture
-000006c0: 7205 0000 00da 2676 656e 7475 7265 732e  r.....&ventures.
-000006d0: 7574 696c 6974 6965 732e 7072 6f63 6573  utilities.proces
-000006e0: 732e 6368 6563 6b5f 6973 5f6f 6e72 0700  s.check_is_onr..
-000006f0: 0000 7220 0000 0072 1b00 0000 7222 0000  ..r ...r....r"..
-00000700: 0072 2e00 0000 722c 0000 0072 2c00 0000  .r....r,...r,...
-00000710: 722c 0000 0072 2d00 0000 da08 3c6d 6f64  r,...r-.....<mod
-00000720: 756c 653e 0100 0000 7314 0000 000c 030c  ule>....s.......
-00000730: 010c 010c 010c 0208 0308 0308 0102 040c  ................
-00000740: 16                                       .
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 5a08 6400 6405 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6405 6c0a 5a0a 6400 6405 6c0b 5a0b 6400  d.l.Z.d.d.l.Z.d.
+00000080: 6405 6c0c 5a0c 6406 6407 8400 5a0d 6405  d.l.Z.d.d...Z.d.
+00000090: 5300 2908 e900 0000 0029 01da 0865 7463  S.)......)...etc
+000000a0: 685f 6d61 7029 01da 0873 6361 6e5f 6d61  h_map)...scan_ma
+000000b0: 7029 01da 0c66 696e 645f 7665 6e74 7572  p)...find_ventur
+000000c0: 6529 01da 0b63 6865 636b 5f69 735f 6f6e  e)...check_is_on
+000000d0: 4e63 0100 0000 0000 0000 0000 0000 0b00  Nc..............
+000000e0: 0000 0800 0000 4300 0000 73d6 0100 007c  ......C...s....|
+000000f0: 0064 0119 007d 017c 0164 0219 0064 0319  .d...}.|.d...d..
+00000100: 007d 027c 0164 0419 007d 037c 0164 0519  .}.|.d...}.|.d..
+00000110: 007d 0474 0064 067c 0183 0201 007c 0064  .}.t.d.|.....|.d
+00000120: 0719 007d 0574 017c 0564 0883 028f 0d7d  ...}.t.|.d.....}
+00000130: 0674 02a0 037c 06a1 017d 0757 0064 0004  .t...|...}.W.d..
+00000140: 0004 0083 0301 006e 0831 0073 3077 0101  .......n.1.s0w..
+00000150: 0001 0001 0059 0001 0074 046a 0564 097c  .....Y...t.j.d.|
+00000160: 017c 077c 0464 0a9c 0464 0b8d 0101 007c  .|.|.d...d.....|
+00000170: 077c 0419 007d 017c 0364 0c6b 0272 a17c  .|...}.|.d.k.r.|
+00000180: 0164 0c19 0064 0d6b 0372 a17c 0164 0c19  .d...d.k.r.|.d..
+00000190: 007d 0874 046a 0564 0974 067c 0883 0164  .}.t.j.d.t.|...d
+000001a0: 0e9c 0264 0b8d 0101 0074 067c 0883 0164  ...d.....t.|...d
+000001b0: 0f6b 0372 a174 07a0 087c 0874 096a 0aa1  .k.r.t...|.t.j..
+000001c0: 0201 0064 0d7c 077c 0419 0064 0c3c 0064  ...d.|.|...d.<.d
+000001d0: 107d 0909 0074 067c 0883 017d 0a74 046a  .}...t.|...}.t.j
+000001e0: 0564 097c 047c 0a64 129c 0264 139c 0264  .d.|.|.d...d...d
+000001f0: 0b8d 0101 007c 0a64 0f6b 0272 886e 1974  .....|.d.k.r.n.t
+00000200: 0ba0 0c64 14a1 0101 007c 0964 1437 007d  ...d.....|.d.7.}
+00000210: 097c 0964 156b 0272 a074 0d64 167c 099b  .|.d.k.r.t.d.|..
+00000220: 0064 177c 049b 0064 189d 0583 0182 0171  .d.|...d.......q
+00000230: 737c 0364 196b 0272 e77c 0164 1a19 0083  s|.d.k.r.|.d....
+00000240: 0064 0f6b 0372 e97c 0164 0919 0083 0001  .d.k.r.|.d......
+00000250: 0064 107d 0909 007c 0164 1a19 0083 007d  .d.}...|.d.....}
+00000260: 0a74 046a 0564 1b64 1c7c 097c 0164 0519  .t.j.d.d.|.|.d..
+00000270: 007c 0a64 1d9c 0469 0164 0b8d 0101 007c  .|.d...i.d.....|
+00000280: 0a64 0f6b 0272 ce64 0053 0074 0ba0 0c64  .d.k.r.d.S.t...d
+00000290: 14a1 0101 007c 0964 1437 007d 097c 0964  .....|.d.7.}.|.d
+000002a0: 156b 0272 e674 0d64 167c 099b 0064 177c  .k.r.t.d.|...d.|
+000002b0: 049b 0064 189d 0583 0182 0171 b464 0053  ...d.......q.d.S
+000002c0: 0064 0053 0029 1e4e da07 7665 6e74 7572  .d.S.).N..ventur
+000002d0: 657a 0774 7572 6e20 6f6e da09 6164 7665  ez.turn on..adve
+000002e0: 6e74 7572 65da 046b 696e 64da 046e 616d  nture..kind..nam
+000002f0: 657a 0876 656e 7475 7265 3ada 036d 6170  ez.venture:..map
+00000300: da01 727a 0874 7572 6e20 6f66 6629 04da  ..rz.turn off)..
+00000310: 0470 6c61 7972 0600 0000 da14 7665 6e74  .playr......vent
+00000320: 7572 6573 5f6d 6170 5f62 7261 636b 6574  ures_map_bracket
+00000330: 7209 0000 0029 01da 0464 6174 61da 1070  r....)...data..p
+00000340: 726f 6365 7373 5f69 6465 6e74 6974 79da  rocess_identity.
+00000350: 0029 0272 0c00 0000 720f 0000 00da 036f  .).r....r......o
+00000360: 6666 7201 0000 0054 2902 7209 0000 00da  ffr....T).r.....
+00000370: 0673 7461 7475 7329 0272 0c00 0000 7a12  .status).r....z.
+00000380: 7374 6174 7573 2063 6865 636b 2063 7963  status check cyc
+00000390: 6c65 e901 0000 00e9 0a00 0000 7a06 4166  le..........z.Af
+000003a0: 7465 7220 7a08 206c 6f6f 7073 2c20 7a12  ter z. loops, z.
+000003b0: 2064 6964 206e 6f74 2074 7572 6e20 6f66   did not turn of
+000003c0: 662e da04 7461 736b 7a05 6973 206f 6e7a  f...taskz.is onz
+000003d0: 1976 656e 7475 7265 2073 7461 7475 7320  .venture status 
+000003e0: 6368 6563 6b20 6c6f 6f70 7a17 6166 7465  check loopz.afte
+000003f0: 7220 7475 726e 206f 6666 2077 6173 2073  r turn off was s
+00000400: 656e 7429 04da 0477 6865 6eda 046c 6f6f  ent)...when..loo
+00000410: 7072 0900 0000 7212 0000 0029 0eda 0570  pr....r....)...p
+00000420: 7269 6e74 da04 6f70 656e da04 6a73 6f6e  rint..open..json
+00000430: da04 6c6f 6164 da04 7269 6368 da0a 7072  ..load..rich..pr
+00000440: 696e 745f 6a73 6f6e 7205 0000 00da 026f  int_jsonr......o
+00000450: 73da 046b 696c 6cda 0673 6967 6e61 6cda  s..kill..signal.
+00000460: 0753 4947 5445 524d da04 7469 6d65 da05  .SIGTERM..time..
+00000470: 736c 6565 70da 0945 7863 6570 7469 6f6e  sleep..Exception
+00000480: 290b da06 7061 636b 6574 7206 0000 00da  )...packetr.....
+00000490: 1061 6476 656e 7475 7265 5f73 6372 6970  .adventure_scrip
+000004a0: 7472 0800 0000 7209 0000 00da 0c74 6865  tr....r......the
+000004b0: 5f6d 6170 5f70 6174 68da 0246 5072 0d00  _map_path..FPr..
+000004c0: 0000 720f 0000 0072 1700 0000 7212 0000  ..r....r....r...
+000004d0: 00a9 0072 2900 0000 fa42 2f68 6162 6974  ...r)....B/habit
+000004e0: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
+000004f0: 2f76 656e 7475 7265 732f 706c 6179 735f  /ventures/plays_
+00000500: 7665 6e74 7572 652f 7475 726e 5f6f 6666  venture/turn_off
+00000510: 2f5f 5f69 6e69 745f 5f2e 7079 da10 7475  /__init__.py..tu
+00000520: 726e 5f6f 6666 5f76 656e 7475 7265 1500  rn_off_venture..
+00000530: 0000 738a 0000 0008 010c 0208 0108 010a  ..s.............
+00000540: 0208 020c 010c 011c ff04 0302 0102 0102  ................
+00000550: 0102 010a fc08 0708 020c 0108 0104 0202  ................
+00000560: 0106 010a fe0c 050e 010c 0104 0302 0108  ................
+00000570: 0104 0102 0102 0202 0104 fe0a fe08 0802  ................
+00000580: 010a 0208 0208 0102 0110 0104 ff02 ef08  ................
+00000590: 160e 010a 0104 0202 010a 0104 0202 0102  ................
+000005a0: 0102 0106 0102 0104 fc08 ff08 0904 010a  ................
+000005b0: 0208 0208 0102 0110 0104 ff02 ed04 fb04  ................
+000005c0: 0172 2b00 0000 290e da1b 7665 6e74 7572  .r+...)...ventur
+000005d0: 6573 2e75 7469 6c69 7469 6573 2e6d 6170  es.utilities.map
+000005e0: 2e65 7463 6872 0200 0000 da1b 7665 6e74  .etchr......vent
+000005f0: 7572 6573 2e75 7469 6c69 7469 6573 2e6d  ures.utilities.m
+00000600: 6170 2e73 6361 6e72 0300 0000 da28 7665  ap.scanr.....(ve
+00000610: 6e74 7572 6573 2e75 7469 6c69 7469 6573  ntures.utilities
+00000620: 2e76 656e 7475 7265 732e 6669 6e64 5f76  .ventures.find_v
+00000630: 656e 7475 7265 7204 0000 00da 2676 656e  enturer.....&ven
+00000640: 7475 7265 732e 7574 696c 6974 6965 732e  tures.utilities.
+00000650: 7072 6f63 6573 732e 6368 6563 6b5f 6973  process.check_is
+00000660: 5f6f 6e72 0500 0000 721c 0000 0072 1a00  _onr....r....r..
+00000670: 0000 7220 0000 0072 1e00 0000 7222 0000  ..r ...r....r"..
+00000680: 0072 2b00 0000 7229 0000 0072 2900 0000  .r+...r)...r)...
+00000690: 7229 0000 0072 2a00 0000 da08 3c6d 6f64  r)...r*.....<mod
+000006a0: 756c 653e 0100 0000 7314 0000 000c 040c  ule>....s.......
+000006b0: 010c 010c 0108 0308 0308 0108 0108 010c  ................
+000006c0: 04                                       .
```

### Comparing `ventures-1.2.0/venues/stages/ventures/plays/is_on.py` & `ventures-1.3.0/venues/stages/ventures/plays/is_on.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,24 +22,21 @@
 		if (name == venture ["name"]):
 			return venture;
 			
 	raise Exception (f"Venture with name '{ name }' not found.")
 	
 	
 def is_on (packet):
-	the_map = packet ["the_map"]
+	ventures_map_bracket = packet ["ventures_map_bracket"]
 	ventures = packet ["ventures"]
-	
-	with open (the_map, 'r') as FP:
-		bracket = json.load (FP)
-	
+
 	
 	statuses = {}
-	for adventure in bracket:
-		adventure_details = bracket [ adventure ]
+	for adventure in ventures_map_bracket:
+		adventure_details = ventures_map_bracket [ adventure ]
 		kind = adventure_details ["kind"]
 		#print (ventures)
 		
 		if (kind == "process_identity"):
 			process_identity = adventure_details ["process_identity"]
 			status = check_is_on (process_identity)
```

### Comparing `ventures-1.2.0/venues/stages/ventures/plays/turn_off.py` & `ventures-1.3.0/venues/stages/ventures/plays/turn_off.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import os
 import time
 #
 #++++
 
 
 def turn_off (packet):
-	the_map_path = packet ["the_map"]
+	the_map_path = packet ["the_map_path"]
 	ventures = packet ["ventures"]
 	
 	with open (the_map_path, 'r') as FP:
 		ventures_map_bracket = json.load (FP)
 
 	print ("ventures_map_bracket:", ventures_map_bracket)
```

### Comparing `ventures-1.2.0/venues/stages/ventures/plays/turn_on.py` & `ventures-1.3.0/venues/stages/ventures/plays/turn_on.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 
 #++++
 #
-from ..utilities.hike_passive import hike_passive
-from ..utilities.map.etch import etch_map
-from ..utilities.map.scan import scan_map	
-from ..utilities.ventures.find_venture import find_venture
+from ventures.utilities.hike_passive import hike_passive
+from ventures.utilities.map.etch import etch_map
+from ventures.utilities.map.scan import scan_map	
+from ventures.utilities.ventures.find_venture import find_venture
 #
 from ventures.utilities.process.check_is_on import check_is_on
 #
+from ventures.plays_venture.turn_on import turn_on_venture
+
+#
 #
 import rich
 #
 #
 import os
 import time
 #
 #++++
 
-'''
+''''
 	{
 		"name": "adventure_1",
 		"turn on": {
 			"adventure": "python3 -m http.server 8080",
 			"kind": "process_identity",
 			"Popen": {
 				"CWD": 
@@ -32,30 +35,37 @@
 	{
 		"name": "adventure_2",
 		"turn on": {
 			"adventure": turn_on,
 			"kind": "task"
 		}
 	}
-'''
+"'''
 
 
 def turn_on (packet):
 	ventures = packet ["ventures"]
-	the_map_path = packet ["map"]
-	
+	ventures_map_bracket = packet ["ventures_map_bracket"]
 	
 
-	ventures_map_bracket = {}
-	if os.path.exists (the_map_path):
-		ventures_map_bracket = scan_map ({
-			"path": the_map_path
-		})
+
 
 	for adventure in ventures:
+		turn_on_venture ({
+			"venture": adventure,
+			"ventures_map_bracket": ventures_map_bracket
+		})
+		
+		rich.print_json (data = {
+			"proceeds of turn on": ventures_map_bracket
+		})
+		
+		continue;
+			
+	
 		adventure_script = adventure ["turn on"] ["adventure"]
 		kind = adventure ["kind"]
 		name = adventure ["name"]
 		
 		
 		#
 		#	check if is already on	
@@ -152,13 +162,13 @@
 			}
 			
 		
 		else:
 			raise Exception (f'Kind "{ kind } was not found.')
 
 	
-	etch_map ({
-		"path": the_map_path,
-		"bracket": ventures_map_bracket
-	})
 	
-	return ventures_map_bracket
+	
+	return {
+		"ventures_map_bracket": ventures_map_bracket
+	}
+
```

### Comparing `ventures-1.2.0/venues/stages/ventures/readme.md` & `ventures-1.3.0/venues/stages/ventures/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -46,19 +46,27 @@
 
 def turn_on_sanique ():
 	return;
 	
 def turn_off_sanique ():
 	return;
 	
+	
+#
+#	This needs to return either "on" or "off",
+#	"turn on" runs this function to check whether
+#	the adventure is "on" or "off.
+#
 def check_sanique_is_on ():
-	return;
+	return "off"
 
 from ventures import ventures_map
-ventures = ventures_map ({
+from ventures.clique import ventures_clique
+
+the_ventures = ventures_map ({
 	"map": the_map,
 	"ventures": [
 		{
 			"name": "adventure_1",
 			"turn on": {
 				"adventure": [ 
 					"python3",
@@ -69,29 +77,65 @@
 				
 				"Popen": {},
 				
 				"kind": "process_identity"
 			}
 		},
 		{
-			"name": "adventure_1_sanique",
+			"name": "adventure_2",
 			"kind": "task",
 			"turn on": {
 				"adventure": turn_on_sanique,
 			},
 			"turn off": turn_off_sanique,
 			"is on": check_sanique_is_on
 		}
 	]
 })
+```
 
-ventures ["turn on"] ()
-
-time.sleep (10)
-
-ventures ["is on"] ()
-
-time.sleep (5)
+## option 1, continued from above
+This is the interface to turn on and off ventures
+```
+the_ventures ["turn on"] ()
+the_ventures ["is on"] ()
+the_ventures ["turn off"] ()
+the_ventures ["turn on"] ({
+	"name": "adventure_1"
+})
+the_ventures ["turn off"] ({
+	"name": "adventure_1"
+})
+the_ventures ["is on"] ()
+```
 
-ventures ["turn off"] ()
+## option 2, continued from above
+Ventures has a click interface group that can be 
+added to a click interface.
+```
+import click	
+def clique ():
+	@click.group ()
+	def group ():
+		pass
+
+	group.add_command (ventures_clique ({
+		"ventures": the_ventures
+	}))
+	group ()
+	
+clique ()
+```
 
-```
+### The click interface options
+Assuming the name of the interface is "voyages".   
+```
+voyages ventures on
+voyages ventures off
+voyages ventures status
+```
+
+The adventures can be turned on and off by name.   
+```
+voyages ventures on --name adventure_1
+voyages ventures off --name adventure_1
+```
```

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 '''
-	from vaccines.mixes.ventures_map.hike_passive import hike_passive
+	from ventures.utilities.hike_passive import hike_passive
 	hike_passive ({
 		"script": [
 		
 		]
 	})
 '''
```

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 21 20:21:09 2024 UTC, .py size: 2455 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,120 +1,119 @@
-00000000: 6f0d 0d0a 0000 0000 3502 4d66 9709 0000  o.......5.Mf....
+00000000: 6f0d 0d0a 0000 0000 f41b 4d66 8e09 0000  o.........Mf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 0100 6401 6404  d.d.l.m.Z...d.d.
 00000050: 6c05 5a05 6401 6405 6c06 6d07 5a07 0100  l.Z.d.d.l.m.Z...
 00000060: 6401 6406 6c08 6d09 5a09 0100 6401 6404  d.d.l.m.Z...d.d.
 00000070: 6c0a 5a0a 6401 6404 6c0b 5a0b 6401 6404  l.Z.d.d.l.Z.d.d.
 00000080: 6c0c 5a0c 6401 6404 6c0d 5a0d 6401 6404  l.Z.d.d.l.Z.d.d.
 00000090: 6c0e 5a0e 6401 6404 6c0d 5a0d 6401 6404  l.Z.d.d.l.Z.d.d.
 000000a0: 6c0f 5a0f 6401 6404 6c0b 5a0b 6407 6408  l.Z.d.d.l.Z.d.d.
-000000b0: 8400 5a10 6404 5300 2909 7a6e 0a09 6672  ..Z.d.S.).zn..fr
-000000c0: 6f6d 2076 6163 6369 6e65 732e 6d69 7865  om vaccines.mixe
-000000d0: 732e 7665 6e74 7572 6573 5f6d 6170 2e68  s.ventures_map.h
-000000e0: 696b 655f 7061 7373 6976 6520 696d 706f  ike_passive impo
-000000f0: 7274 2068 696b 655f 7061 7373 6976 650a  rt hike_passive.
-00000100: 0968 696b 655f 7061 7373 6976 6520 287b  .hike_passive ({
-00000110: 0a09 0922 7363 7269 7074 223a 205b 0a09  ..."script": [..
-00000120: 090a 0909 5d0a 097d 290a e900 0000 0029  ....]..})......)
-00000130: 01da 1568 696b 655f 7061 7373 6976 655f  ...hike_passive_
-00000140: 705f 6578 7065 6374 2901 da13 7072 6f63  p_expect)...proc
-00000150: 6573 735f 6f6e 5f69 6d70 6c69 6369 744e  ess_on_implicitN
-00000160: 2901 da05 6d65 7267 6529 01da 0846 7261  )...merge)...Fra
-00000170: 6374 696f 6e63 0100 0000 0000 0000 0000  ctionc..........
-00000180: 0000 0700 0000 0400 0000 0300 0000 737e  ..............s~
-00000190: 0000 007c 0064 0119 007d 0169 007d 0264  ...|.d...}.i.}.d
-000001a0: 027c 0076 0072 1674 007c 0064 0219 0083  .|.v.r.t.|.d....
-000001b0: 0174 016b 0272 167c 0064 0219 007d 0264  .t.k.r.|.d...}.d
-000001c0: 0364 0484 0089 0087 0066 0164 0564 0684  .d.......f.d.d..
-000001d0: 087d 0374 0264 0764 0869 017c 0283 027d  .}.t.d.d.i.|...}
-000001e0: 0474 0364 097c 0483 0201 0074 0364 0a7c  .t.d.|.....t.d.|
-000001f0: 0083 0201 0074 046a 057c 0166 0169 007c  .....t.j.|.f.i.|
-00000200: 04a4 018e 017d 0564 0b7c 056a 0669 0153  .....}.d.|.j.i.S
-00000210: 0029 0c4e da06 7363 7269 7074 da05 506f  .).N..script..Po
-00000220: 7065 6e63 0000 0000 0000 0000 0000 0000  penc............
-00000230: 0100 0000 0300 0000 5300 0000 739c 0000  ........S...s...
-00000240: 0074 00a0 01a1 007d 007c 0064 016b 0472  .t.....}.|.d.k.r
-00000250: 0d74 02a0 0364 01a1 0101 0074 00a0 04a1  .t...d.....t....
-00000260: 0001 0074 00a0 01a1 007d 007c 0064 016b  ...t.....}.|.d.k
-00000270: 0472 1e74 02a0 0364 01a1 0101 0074 00a0  .r.t...d.....t..
-00000280: 0564 02a1 0101 0074 00a0 0664 01a1 0101  .d.....t...d....
-00000290: 0074 026a 07a0 08a1 0001 0074 026a 09a0  .t.j.......t.j..
-000002a0: 08a1 0001 0074 026a 0aa0 08a1 0001 0074  .....t.j.......t
-000002b0: 0b74 006a 0c64 0383 0274 025f 0774 0b74  .t.j.d...t._.t.t
-000002c0: 006a 0c64 0483 0274 025f 0974 0b74 006a  .j.d...t._.t.t.j
-000002d0: 0c64 0483 0274 025f 0a64 0053 0029 054e  .d...t._.d.S.).N
-000002e0: 7201 0000 00fa 012f da01 72da 0177 290d  r....../..r..w).
-000002f0: da02 6f73 da04 666f 726b da03 7379 73da  ..os..fork..sys.
-00000300: 0465 7869 74da 0673 6574 7369 64da 0563  .exit..setsid..c
-00000310: 6864 6972 da05 756d 6173 6bda 0573 7464  hdir..umask..std
-00000320: 696e da05 636c 6f73 65da 0673 7464 6f75  in..close..stdou
-00000330: 74da 0673 7464 6572 72da 046f 7065 6eda  t..stderr..open.
-00000340: 0764 6576 6e75 6c6c 2901 da03 7069 64a9  .devnull)...pid.
-00000350: 0072 1900 0000 fa42 2f68 6162 6974 6174  .r.....B/habitat
-00000360: 2f76 656e 7565 732f 7374 6167 6573 2f76  /venues/stages/v
-00000370: 656e 7475 7265 732f 7574 696c 6974 6965  entures/utilitie
-00000380: 732f 6869 6b65 5f70 6173 7369 7665 2f5f  s/hike_passive/_
-00000390: 5f69 6e69 745f 5f2e 7079 da09 6461 656d  _init__.py..daem
-000003a0: 6f6e 697a 6537 0000 0073 1e00 0000 0802  onize7...s......
-000003b0: 0801 0a02 0803 0803 0801 0a02 0a03 0a03  ................
-000003c0: 0a03 0a01 0a01 0e03 0e01 1201 7a1f 6869  ............z.hi
-000003d0: 6b65 5f70 6173 7369 7665 2e3c 6c6f 6361  ke_passive.<loca
-000003e0: 6c73 3e2e 6461 656d 6f6e 697a 6563 0100  ls>.daemonizec..
-000003f0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00000400: 0000 1300 0000 734a 0000 007c 0064 0119  ......sJ...|.d..
-00000410: 007d 0174 00a0 01a1 007d 027c 0264 026b  .}.t.....}.|.d.k
-00000420: 0272 2388 0083 0001 0074 026a 037c 0164  .r#......t.j.|.d
-00000430: 0364 048d 027d 0374 0464 057c 036a 0583  .d...}.t.d.|.j..
-00000440: 0201 0074 00a0 0664 02a1 0101 0064 0053  ...t...d.....d.S
-00000450: 007c 0253 0029 064e 7206 0000 0072 0100  .|.S.).Nr....r..
-00000460: 0000 5429 01da 0573 6865 6c6c 7a33 0a09  ..T)...shellz3..
-00000470: 0909 0a09 0909 0a09 0909 0963 6869 6c64  ...........child
-00000480: 2070 726f 6365 7373 2070 6964 3a0a 0909   process pid:...
-00000490: 0909 0a09 0909 090a 0909 0909 0a09 0909  ................
-000004a0: 0929 0772 0b00 0000 720c 0000 00da 0a73  .).r....r......s
-000004b0: 7562 7072 6f63 6573 7372 0700 0000 da05  ubprocessr......
-000004c0: 7072 696e 7472 1800 0000 da05 5f65 7869  printr......_exi
-000004d0: 7429 04da 0763 6f6d 6d61 6e64 7206 0000  t)...commandr...
-000004e0: 0072 1800 0000 da0b 7468 655f 7072 6f63  .r......the_proc
-000004f0: 6573 73a9 0172 1b00 0000 7219 0000 0072  ess..r....r....r
-00000500: 1a00 0000 da16 7374 6172 745f 6465 7461  ......start_deta
-00000510: 6368 6564 5f70 726f 6365 7373 5700 0000  ched_processW...
-00000520: 7314 0000 0008 0108 0308 0206 030e 0204  s...............
-00000530: 0204 0704 f90e 0a04 047a 2c68 696b 655f  .........z,hike_
-00000540: 7061 7373 6976 652e 3c6c 6f63 616c 733e  passive.<locals>
-00000550: 2e73 7461 7274 5f64 6574 6163 6865 645f  .start_detached_
-00000560: 7072 6f63 6573 73da 0963 6c6f 7365 5f66  process..close_f
-00000570: 6473 547a 0c6d 6572 6765 645f 6469 6374  dsTz.merged_dict
-00000580: 3a7a 0770 6163 6b65 743a da10 7072 6f63  :z.packet:..proc
-00000590: 6573 735f 6964 656e 7469 7479 2908 da04  ess_identity)...
-000005a0: 7479 7065 da04 6469 6374 7204 0000 0072  type..dictr....r
-000005b0: 1e00 0000 721d 0000 0072 0700 0000 7218  ....r....r....r.
-000005c0: 0000 00da 046a 6f69 6e29 07da 0670 6163  .....join)...pac
-000005d0: 6b65 7472 0600 0000 da0a 506f 7065 6e5f  ketr......Popen_
-000005e0: 6b65 7973 7223 0000 00da 0b6d 6572 6765  keysr#.....merge
-000005f0: 645f 6469 6374 7221 0000 00da 1464 6574  d_dictr!.....det
-00000600: 6163 6865 645f 7072 6f63 6573 735f 7069  ached_process_pi
-00000610: 6472 1900 0000 7222 0000 0072 1a00 0000  dr....r"...r....
-00000620: da0c 6869 6b65 5f70 6173 7369 7665 2f00  ..hike_passive/.
-00000630: 0000 732a 0000 0008 0104 0208 0110 0108  ..s*............
-00000640: 0108 020c 2002 1e04 0102 ff02 0204 fe0a  .... ...........
-00000650: 040a 0104 0202 0104 ff02 0206 fe06 0604  ................
-00000660: ff72 2d00 0000 2911 da07 5f5f 646f 635f  .r-...)...__doc_
-00000670: 5fda 2876 656e 7475 7265 732e 7574 696c  _.(ventures.util
-00000680: 6974 6965 732e 6869 6b65 5f70 6173 7369  ities.hike_passi
-00000690: 7665 5f70 5f65 7870 6563 7472 0200 0000  ve_p_expectr....
-000006a0: da33 7665 6e74 7572 6573 2e75 7469 6c69  .3ventures.utili
-000006b0: 7469 6573 2e68 696b 655f 7061 7373 6976  ties.hike_passiv
-000006c0: 655f 705f 6578 7065 6374 5f32 2e69 6d70  e_p_expect_2.imp
-000006d0: 6c69 6369 7472 0300 0000 da04 7269 6368  licitr......rich
-000006e0: da06 7079 6461 7368 7204 0000 00da 0966  ..pydashr......f
-000006f0: 7261 6374 696f 6e73 7205 0000 00da 0f6d  ractionsr......m
-00000700: 756c 7469 7072 6f63 6573 7369 6e67 721d  ultiprocessingr.
-00000710: 0000 00da 0474 696d 6572 0b00 0000 da06  .....timer......
-00000720: 6174 6578 6974 720d 0000 0072 2d00 0000  atexitr....r-...
-00000730: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00000740: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000750: 0000 7320 0000 0004 0a02 090c 060c 0108  ..s ............
-00000760: 030c 010c 0308 0108 0108 0108 0108 0108  ................
-00000770: 0108 0108 010c 05                        .......
+000000b0: 8400 5a10 6404 5300 2909 7a65 0a09 6672  ..Z.d.S.).ze..fr
+000000c0: 6f6d 2076 656e 7475 7265 732e 7574 696c  om ventures.util
+000000d0: 6974 6965 732e 6869 6b65 5f70 6173 7369  ities.hike_passi
+000000e0: 7665 2069 6d70 6f72 7420 6869 6b65 5f70  ve import hike_p
+000000f0: 6173 7369 7665 0a09 6869 6b65 5f70 6173  assive..hike_pas
+00000100: 7369 7665 2028 7b0a 0909 2273 6372 6970  sive ({..."scrip
+00000110: 7422 3a20 5b0a 0909 0a09 095d 0a09 7d29  t": [......]..})
+00000120: 0ae9 0000 0000 2901 da15 6869 6b65 5f70  ......)...hike_p
+00000130: 6173 7369 7665 5f70 5f65 7870 6563 7429  assive_p_expect)
+00000140: 01da 1370 726f 6365 7373 5f6f 6e5f 696d  ...process_on_im
+00000150: 706c 6963 6974 4e29 01da 056d 6572 6765  plicitN)...merge
+00000160: 2901 da08 4672 6163 7469 6f6e 6301 0000  )...Fractionc...
+00000170: 0000 0000 0000 0000 0007 0000 0004 0000  ................
+00000180: 0003 0000 0073 7e00 0000 7c00 6401 1900  .....s~...|.d...
+00000190: 7d01 6900 7d02 6402 7c00 7600 7216 7400  }.i.}.d.|.v.r.t.
+000001a0: 7c00 6402 1900 8301 7401 6b02 7216 7c00  |.d.....t.k.r.|.
+000001b0: 6402 1900 7d02 6403 6404 8400 8900 8700  d...}.d.d.......
+000001c0: 6601 6405 6406 8408 7d03 7402 6407 6408  f.d.d...}.t.d.d.
+000001d0: 6901 7c02 8302 7d04 7403 6409 7c04 8302  i.|...}.t.d.|...
+000001e0: 0100 7403 640a 7c00 8302 0100 7404 6a05  ..t.d.|.....t.j.
+000001f0: 7c01 6601 6900 7c04 a401 8e01 7d05 640b  |.f.i.|.....}.d.
+00000200: 7c05 6a06 6901 5300 290c 4eda 0673 6372  |.j.i.S.).N..scr
+00000210: 6970 74da 0550 6f70 656e 6300 0000 0000  ipt..Popenc.....
+00000220: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
+00000230: 0000 0073 9c00 0000 7400 a001 a100 7d00  ...s....t.....}.
+00000240: 7c00 6401 6b04 720d 7402 a003 6401 a101  |.d.k.r.t...d...
+00000250: 0100 7400 a004 a100 0100 7400 a001 a100  ..t.......t.....
+00000260: 7d00 7c00 6401 6b04 721e 7402 a003 6401  }.|.d.k.r.t...d.
+00000270: a101 0100 7400 a005 6402 a101 0100 7400  ....t...d.....t.
+00000280: a006 6401 a101 0100 7402 6a07 a008 a100  ..d.....t.j.....
+00000290: 0100 7402 6a09 a008 a100 0100 7402 6a0a  ..t.j.......t.j.
+000002a0: a008 a100 0100 740b 7400 6a0c 6403 8302  ......t.t.j.d...
+000002b0: 7402 5f07 740b 7400 6a0c 6404 8302 7402  t._.t.t.j.d...t.
+000002c0: 5f09 740b 7400 6a0c 6404 8302 7402 5f0a  _.t.t.j.d...t._.
+000002d0: 6400 5300 2905 4e72 0100 0000 fa01 2fda  d.S.).Nr....../.
+000002e0: 0172 da01 7729 0dda 026f 73da 0466 6f72  .r..w)...os..for
+000002f0: 6bda 0373 7973 da04 6578 6974 da06 7365  k..sys..exit..se
+00000300: 7473 6964 da05 6368 6469 72da 0575 6d61  tsid..chdir..uma
+00000310: 736b da05 7374 6469 6eda 0563 6c6f 7365  sk..stdin..close
+00000320: da06 7374 646f 7574 da06 7374 6465 7272  ..stdout..stderr
+00000330: da04 6f70 656e da07 6465 766e 756c 6c29  ..open..devnull)
+00000340: 01da 0370 6964 a900 7219 0000 00fa 422f  ...pid..r.....B/
+00000350: 6861 6269 7461 742f 7665 6e75 6573 2f73  habitat/venues/s
+00000360: 7461 6765 732f 7665 6e74 7572 6573 2f75  tages/ventures/u
+00000370: 7469 6c69 7469 6573 2f68 696b 655f 7061  tilities/hike_pa
+00000380: 7373 6976 652f 5f5f 696e 6974 5f5f 2e70  ssive/__init__.p
+00000390: 79da 0964 6165 6d6f 6e69 7a65 3700 0000  y..daemonize7...
+000003a0: 731e 0000 0008 0208 010a 0208 0308 0308  s...............
+000003b0: 010a 020a 030a 030a 030a 010a 010e 030e  ................
+000003c0: 0112 017a 1f68 696b 655f 7061 7373 6976  ...z.hike_passiv
+000003d0: 652e 3c6c 6f63 616c 733e 2e64 6165 6d6f  e.<locals>.daemo
+000003e0: 6e69 7a65 6301 0000 0000 0000 0000 0000  nizec...........
+000003f0: 0004 0000 0004 0000 0013 0000 0073 4a00  .............sJ.
+00000400: 0000 7c00 6401 1900 7d01 7400 a001 a100  ..|.d...}.t.....
+00000410: 7d02 7c02 6402 6b02 7223 8800 8300 0100  }.|.d.k.r#......
+00000420: 7402 6a03 7c01 6403 6404 8d02 7d03 7404  t.j.|.d.d...}.t.
+00000430: 6405 7c03 6a05 8302 0100 7400 a006 6402  d.|.j.....t...d.
+00000440: a101 0100 6400 5300 7c02 5300 2906 4e72  ....d.S.|.S.).Nr
+00000450: 0600 0000 7201 0000 0054 2901 da05 7368  ....r....T)...sh
+00000460: 656c 6c7a 330a 0909 090a 0909 090a 0909  ellz3...........
+00000470: 0909 6368 696c 6420 7072 6f63 6573 7320  ..child process 
+00000480: 7069 643a 0a09 0909 090a 0909 0909 0a09  pid:............
+00000490: 0909 090a 0909 0909 2907 720b 0000 0072  ........).r....r
+000004a0: 0c00 0000 da0a 7375 6270 726f 6365 7373  ......subprocess
+000004b0: 7207 0000 00da 0570 7269 6e74 7218 0000  r......printr...
+000004c0: 00da 055f 6578 6974 2904 da07 636f 6d6d  ..._exit)...comm
+000004d0: 616e 6472 0600 0000 7218 0000 00da 0b74  andr....r......t
+000004e0: 6865 5f70 726f 6365 7373 a901 721b 0000  he_process..r...
+000004f0: 0072 1900 0000 721a 0000 00da 1673 7461  .r....r......sta
+00000500: 7274 5f64 6574 6163 6865 645f 7072 6f63  rt_detached_proc
+00000510: 6573 7357 0000 0073 1400 0000 0801 0803  essW...s........
+00000520: 0802 0603 0e02 0402 0407 04f9 0e0a 0404  ................
+00000530: 7a2c 6869 6b65 5f70 6173 7369 7665 2e3c  z,hike_passive.<
+00000540: 6c6f 6361 6c73 3e2e 7374 6172 745f 6465  locals>.start_de
+00000550: 7461 6368 6564 5f70 726f 6365 7373 da09  tached_process..
+00000560: 636c 6f73 655f 6664 7354 7a0c 6d65 7267  close_fdsTz.merg
+00000570: 6564 5f64 6963 743a 7a07 7061 636b 6574  ed_dict:z.packet
+00000580: 3ada 1070 726f 6365 7373 5f69 6465 6e74  :..process_ident
+00000590: 6974 7929 08da 0474 7970 65da 0464 6963  ity)...type..dic
+000005a0: 7472 0400 0000 721e 0000 0072 1d00 0000  tr....r....r....
+000005b0: 7207 0000 0072 1800 0000 da04 6a6f 696e  r....r......join
+000005c0: 2907 da06 7061 636b 6574 7206 0000 00da  )...packetr.....
+000005d0: 0a50 6f70 656e 5f6b 6579 7372 2300 0000  .Popen_keysr#...
+000005e0: da0b 6d65 7267 6564 5f64 6963 7472 2100  ..merged_dictr!.
+000005f0: 0000 da14 6465 7461 6368 6564 5f70 726f  ....detached_pro
+00000600: 6365 7373 5f70 6964 7219 0000 0072 2200  cess_pidr....r".
+00000610: 0000 721a 0000 00da 0c68 696b 655f 7061  ..r......hike_pa
+00000620: 7373 6976 652f 0000 0073 2a00 0000 0801  ssive/...s*.....
+00000630: 0402 0801 1001 0801 0802 0c20 021e 0401  ........... ....
+00000640: 02ff 0202 04fe 0a04 0a01 0402 0201 04ff  ................
+00000650: 0202 06fe 0606 04ff 722d 0000 0029 11da  ........r-...)..
+00000660: 075f 5f64 6f63 5f5f da28 7665 6e74 7572  .__doc__.(ventur
+00000670: 6573 2e75 7469 6c69 7469 6573 2e68 696b  es.utilities.hik
+00000680: 655f 7061 7373 6976 655f 705f 6578 7065  e_passive_p_expe
+00000690: 6374 7202 0000 00da 3376 656e 7475 7265  ctr.....3venture
+000006a0: 732e 7574 696c 6974 6965 732e 6869 6b65  s.utilities.hike
+000006b0: 5f70 6173 7369 7665 5f70 5f65 7870 6563  _passive_p_expec
+000006c0: 745f 322e 696d 706c 6963 6974 7203 0000  t_2.implicitr...
+000006d0: 00da 0472 6963 68da 0670 7964 6173 6872  ...rich..pydashr
+000006e0: 0400 0000 da09 6672 6163 7469 6f6e 7372  ......fractionsr
+000006f0: 0500 0000 da0f 6d75 6c74 6970 726f 6365  ......multiproce
+00000700: 7373 696e 6772 1d00 0000 da04 7469 6d65  ssingr......time
+00000710: 720b 0000 00da 0661 7465 7869 7472 0d00  r......atexitr..
+00000720: 0000 722d 0000 0072 1900 0000 7219 0000  ..r-...r....r...
+00000730: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
+00000740: 6475 6c65 3e01 0000 0073 2000 0000 040a  dule>....s .....
+00000750: 0209 0c06 0c01 0803 0c01 0c03 0801 0801  ................
+00000760: 0801 0801 0801 0801 0801 0801 0c05       ..............
```

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.3.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 20 00:48:36 2024 UTC, .py size: 676 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-00000000: 6f0d 0d0a 0000 0000 e49d 4a66 a402 0000  o.........Jf....
+00000000: 6f0d 0d0a 0000 0000 e73a 4d66 9d02 0000  o........:Mf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c01  Z.d.d.l.Z.d.d.l.
-00000040: 5a01 6403 6404 8400 5a02 6405 6406 8400  Z.d.d...Z.d.d...
-00000050: 5a03 6402 5300 2907 7a55 0a09 6672 6f6d  Z.d.S.).zU..from
-00000060: 2076 656e 7475 7265 732e 7574 696c 6974   ventures.utilit
-00000070: 6965 732e 6368 6563 6b5f 6973 5f6f 6e20  ies.check_is_on 
-00000080: 696d 706f 7274 2063 6865 636b 5f69 735f  import check_is_
-00000090: 6f6e 0a09 7374 6174 7573 203d 2063 6865  on..status = che
-000000a0: 636b 5f69 735f 6f6e 2028 7069 6429 0ae9  ck_is_on (pid)..
-000000b0: 0000 0000 4e63 0100 0000 0000 0000 0000  ....Nc..........
-000000c0: 0000 0200 0000 0800 0000 4300 0000 7332  ..........C...s2
-000000d0: 0000 007a 0d74 00a0 017c 00a1 017d 017c  ...z.t...|...}.|
-000000e0: 01a0 02a1 0074 006a 036b 0257 0053 0004  .....t.j.k.W.S..
-000000f0: 0074 006a 0479 1801 0001 0001 0059 0064  .t.j.y.......Y.d
-00000100: 0153 0077 0029 024e 4629 05da 0670 7375  .S.w.).NF)...psu
-00000110: 7469 6cda 0750 726f 6365 7373 da06 7374  til..Process..st
-00000120: 6174 7573 da0d 5354 4154 5553 5f5a 4f4d  atus..STATUS_ZOM
-00000130: 4249 45da 0d4e 6f53 7563 6850 726f 6365  BIE..NoSuchProce
-00000140: 7373 2902 da03 7069 64da 0770 726f 6365  ss)...pid..proce
-00000150: 7373 a900 7209 0000 00fa 402f 6861 6269  ss..r.....@/habi
-00000160: 7461 742f 7665 6e75 6573 2f73 7461 6765  tat/venues/stage
-00000170: 732f 7665 6e74 7572 6573 2f75 7469 6c69  s/ventures/utili
-00000180: 7469 6573 2f70 726f 6365 7373 2f63 6865  ties/process/che
-00000190: 636b 5f69 735f 6f6e 2e70 79da 1269 735f  ck_is_on.py..is_
-000001a0: 7072 6f63 6573 735f 6465 6675 6e63 740b  process_defunct.
-000001b0: 0000 0073 0c00 0000 0201 0a01 1001 0e01  ...s............
-000001c0: 0601 02ff 720b 0000 0063 0100 0000 0000  ....r....c......
-000001d0: 0000 0000 0000 0400 0000 0a00 0000 4300  ..............C.
-000001e0: 0000 7386 0000 007a 2a7c 0064 016b 0272  ..s....z*|.d.k.r
-000001f0: 0857 0064 0253 0074 007c 0083 017d 0074  .W.d.S.t.|...}.t
-00000200: 0164 037c 0083 0201 0074 027c 0083 017d  .d.|.....t.|...}
-00000210: 017c 0164 046b 0272 1c57 0064 0253 0074  .|.d.k.r.W.d.S.t
-00000220: 03a0 047c 00a1 017d 027c 0264 046b 0272  ...|...}.|.d.k.r
-00000230: 2857 0064 0553 0057 0064 0253 0004 0074  (W.d.S.W.d.S...t
-00000240: 0579 4201 007d 0301 007a 0c74 0164 067c  .yB..}...z.t.d.|
-00000250: 0383 0201 0057 0059 0064 007d 037e 0364  .....W.Y.d.}.~.d
-00000260: 0753 0064 007d 037e 0377 0177 0029 084e  .S.d.}.~.w.w.).N
-00000270: da00 da03 6f66 667a 1063 6865 636b 696e  ....offz.checkin
-00000280: 6720 6f6e 2070 6964 3a54 da02 6f6e 7a1a  g on pid:T..onz.
-00000290: 7072 6f63 6573 7320 7374 6174 7573 2065  process status e
-000002a0: 7863 6570 7469 6f6e 203a da07 756e 6b6e  xception :..unkn
-000002b0: 6f77 6e29 06da 0369 6e74 da05 7072 696e  own)...int..prin
-000002c0: 7472 0b00 0000 7202 0000 00da 0a70 6964  tr....r......pid
-000002d0: 5f65 7869 7374 73da 0945 7863 6570 7469  _exists..Excepti
-000002e0: 6f6e 2904 7207 0000 00da 0a69 735f 6465  on).r......is_de
-000002f0: 6675 6e63 74da 0665 7869 7374 73da 0145  funct..exists..E
-00000300: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
-00000310: 0b63 6865 636b 5f69 735f 6f6e 1200 0000  .check_is_on....
-00000320: 7322 0000 0002 0108 0106 0108 020a 0208  s"..............
-00000330: 0208 0106 010a 0208 0106 0106 020e 0214  ................
-00000340: 0104 0208 8002 fd72 1700 0000 2904 da07  .......r....)...
-00000350: 5f5f 646f 635f 5f72 0200 0000 720b 0000  __doc__r....r...
-00000360: 0072 1700 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000370: 7209 0000 0072 0a00 0000 da08 3c6d 6f64  r....r......<mod
-00000380: 756c 653e 0100 0000 730a 0000 0004 0108  ule>....s.......
-00000390: 0508 0208 020c 07                        .......
+00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
+00000030: 5a00 6401 6402 6c01 5a01 6403 6404 8400  Z.d.d.l.Z.d.d...
+00000040: 5a02 6405 6406 8400 5a03 6402 5300 2907  Z.d.d...Z.d.S.).
+00000050: 7a5c 0a09 6672 6f6d 2076 656e 7475 7265  z\..from venture
+00000060: 732e 7574 696c 6974 6965 732e 706f 6365  s.utilities.poce
+00000070: 7373 2e63 6865 636b 5f69 735f 6f6e 2069  ss.check_is_on i
+00000080: 6d70 6f72 7420 6368 6563 6b5f 6973 5f6f  mport check_is_o
+00000090: 6e0a 0973 7461 7475 7320 3d20 6368 6563  n..status = chec
+000000a0: 6b5f 6973 5f6f 6e20 2870 6964 290a e900  k_is_on (pid)...
+000000b0: 0000 004e 6301 0000 0000 0000 0000 0000  ...Nc...........
+000000c0: 0002 0000 0008 0000 0043 0000 0073 3200  .........C...s2.
+000000d0: 0000 7a0d 7400 a001 7c00 a101 7d01 7c01  ..z.t...|...}.|.
+000000e0: a002 a100 7400 6a03 6b02 5700 5300 0400  ....t.j.k.W.S...
+000000f0: 7400 6a04 7918 0100 0100 0100 5900 6401  t.j.y.......Y.d.
+00000100: 5300 7700 2902 4e46 2905 da06 7073 7574  S.w.).NF)...psut
+00000110: 696c da07 5072 6f63 6573 73da 0673 7461  il..Process..sta
+00000120: 7475 73da 0d53 5441 5455 535f 5a4f 4d42  tus..STATUS_ZOMB
+00000130: 4945 da0d 4e6f 5375 6368 5072 6f63 6573  IE..NoSuchProces
+00000140: 7329 02da 0370 6964 da07 7072 6f63 6573  s)...pid..proces
+00000150: 73a9 0072 0900 0000 fa40 2f68 6162 6974  s..r.....@/habit
+00000160: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
+00000170: 2f76 656e 7475 7265 732f 7574 696c 6974  /ventures/utilit
+00000180: 6965 732f 7072 6f63 6573 732f 6368 6563  ies/process/chec
+00000190: 6b5f 6973 5f6f 6e2e 7079 da12 6973 5f70  k_is_on.py..is_p
+000001a0: 726f 6365 7373 5f64 6566 756e 6374 0900  rocess_defunct..
+000001b0: 0000 730c 0000 0002 010a 0110 010e 0106  ..s.............
+000001c0: 0102 ff72 0b00 0000 6301 0000 0000 0000  ...r....c.......
+000001d0: 0000 0000 0004 0000 000a 0000 0043 0000  .............C..
+000001e0: 0073 7c00 0000 7a25 7c00 6401 6b02 7208  .s|...z%|.d.k.r.
+000001f0: 5700 6402 5300 7400 7c00 8301 7d00 7401  W.d.S.t.|...}.t.
+00000200: 7c00 8301 7d01 7c01 6403 6b02 7217 5700  |...}.|.d.k.r.W.
+00000210: 6402 5300 7402 a003 7c00 a101 7d02 7c02  d.S.t...|...}.|.
+00000220: 6403 6b02 7223 5700 6404 5300 5700 6402  d.k.r#W.d.S.W.d.
+00000230: 5300 0400 7404 793d 0100 7d03 0100 7a0c  S...t.y=..}...z.
+00000240: 7405 6405 7c03 8302 0100 5700 5900 6400  t.d.|.....W.Y.d.
+00000250: 7d03 7e03 6406 5300 6400 7d03 7e03 7701  }.~.d.S.d.}.~.w.
+00000260: 7700 2907 4eda 00da 036f 6666 54da 026f  w.).N....offT..o
+00000270: 6e7a 1a70 726f 6365 7373 2073 7461 7475  nz.process statu
+00000280: 7320 6578 6365 7074 696f 6e20 3ada 0775  s exception :..u
+00000290: 6e6b 6e6f 776e 2906 da03 696e 7472 0b00  nknown)...intr..
+000002a0: 0000 7202 0000 00da 0a70 6964 5f65 7869  ..r......pid_exi
+000002b0: 7374 73da 0945 7863 6570 7469 6f6e da05  sts..Exception..
+000002c0: 7072 696e 7429 0472 0700 0000 da0a 6973  print).r......is
+000002d0: 5f64 6566 756e 6374 da06 6578 6973 7473  _defunct..exists
+000002e0: da01 4572 0900 0000 7209 0000 0072 0a00  ..Er....r....r..
+000002f0: 0000 da0b 6368 6563 6b5f 6973 5f6f 6e10  ....check_is_on.
+00000300: 0000 0073 2000 0000 0201 0801 0601 0802  ...s ...........
+00000310: 0804 0801 0601 0a02 0801 0601 0602 0e02  ................
+00000320: 1401 0402 0880 02fd 7217 0000 0029 04da  ........r....)..
+00000330: 075f 5f64 6f63 5f5f 7202 0000 0072 0b00  .__doc__r....r..
+00000340: 0000 7217 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000350: 0072 0900 0000 720a 0000 00da 083c 6d6f  .r....r......<mo
+00000360: 6475 6c65 3e01 0000 0073 0800 0000 0401  dule>....s......
+00000370: 0805 0802 0c07                           ......
```

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.3.0/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 
 '''
-	from ventures.utilities.check_is_on import check_is_on
+	from ventures.utilities.pocess.check_is_on import check_is_on
 	status = check_is_on (pid)
 '''
 
 import psutil
 
-import psutil
-
 def is_process_defunct(pid):
 	try:
 		process = psutil.Process(pid)
 		return process.status() == psutil.STATUS_ZOMBIE
 	except psutil.NoSuchProcess:
 		return False
 
 def check_is_on (pid):
 	try:
 		if (pid == ""):
 			return "off"
 	
 		pid = int (pid)
 		
-		print ("checking on pid:", pid)
+		#print ("checking on pid:", pid)
 		
 		is_defunct = is_process_defunct (pid)
 		if (is_defunct == True):
 			return "off"
 		
 		exists = psutil.pid_exists (pid)
 		if (exists == True):
```

### Comparing `ventures-1.2.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.3.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.2.0/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.3.0/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

