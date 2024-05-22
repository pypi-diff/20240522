# Comparing `tmp/ventures-1.3.0.tar.gz` & `tmp/ventures-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.3.0.tar", max compression
+gzip compressed data, was "ventures-1.3.1.tar", max compression
```

## Comparing `ventures-1.3.0.tar` & `ventures-1.3.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rwxr-xr-x   0        0        0      585 2024-05-22 01:14:46.773424 ventures-1.3.0/pyproject.toml
--rwxr-xr-x   0        0        0     2920 2024-05-22 01:14:07.029862 ventures-1.3.0/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.3.0/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.3.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.3.0/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.3.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.3.0/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.3.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   346881 2024-05-22 01:14:29.129631 ventures-1.3.0/venues/stages/ventures/_status/DB/records.json
--rw-r--r--   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-22 01:14:25.153673 ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rw-r--r--   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-22 01:14:27.185652 ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rw-r--r--   0        0        0      974 2024-05-22 00:50:05.019739 ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      787 2024-05-22 00:49:57.495796 ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-22 01:14:25.557669 ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.3.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.3.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rw-r--r--   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.3.0/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.3.0/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
--rwxr-xr-x   0        0        0      186 2024-05-22 01:14:28.225641 ventures-1.3.0/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.3.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.3.0/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      984 2024-05-21 22:50:00.483641 ventures-1.3.0/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.3.0/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.3.0/venues/stages/ventures/mixer.S.HTML
--rw-r--r--   0        0        0     1055 2024-05-22 01:14:22.929696 ventures-1.3.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rw-r--r--   0        0        0     1751 2024-05-22 00:50:05.059738 ventures-1.3.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rw-r--r--   0        0        0     1035 2024-05-22 01:05:13.047374 ventures-1.3.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1189 2024-05-22 01:14:18.249745 ventures-1.3.0/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0     2444 2024-05-22 00:49:57.543795 ventures-1.3.0/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     3292 2024-05-22 01:05:07.511430 ventures-1.3.0/venues/stages/ventures/plays/turn_on.py
--rw-r--r--   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.3.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
--rw-r--r--   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.3.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.3.0/venues/stages/ventures/plays_venture/is_on.py
--rw-r--r--   0        0        0     2226 2024-05-22 01:13:12.126436 ventures-1.3.0/venues/stages/ventures/plays_venture/turn_off/__init__.py
--rw-r--r--   0        0        0     1729 2024-05-22 01:14:22.933696 ventures-1.3.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.3.0/venues/stages/ventures/plays_venture/turn_on/__init__.py
--rw-r--r--   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.3.0/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2340 2024-05-22 01:12:32.694847 ventures-1.3.0/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.3.0/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive/__init__.py
--rw-r--r--   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.3.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rw-r--r--   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.3.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.3.0/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.3.0/venues/stages/ventures/utilities/map/scan.py
--rw-r--r--   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.3.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.3.0/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.3.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rw-r--r--   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.3.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.3.0/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.3.0/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 ventures-1.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2024-05-22 01:22:56.563168 ventures-1.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0     3135 2024-05-22 01:19:34.461653 ventures-1.3.1/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.3.1/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.3.1/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.3.1/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.3.1/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.3.1/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.3.1/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   348357 2024-05-22 01:20:22.701050 ventures-1.3.1/venues/stages/ventures/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-22 01:20:19.661088 ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-22 01:20:21.801061 ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rwxr-xr-x   0        0        0      974 2024-05-22 00:50:05.019739 ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      787 2024-05-22 00:49:57.495796 ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-22 01:20:20.865073 ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.3.1/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.3.1/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
+-rwxr-xr-x   0        0        0      184 2024-05-22 01:20:21.837061 ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.3.1/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.3.1/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      984 2024-05-21 22:50:00.483641 ventures-1.3.1/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.3.1/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.3.1/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1055 2024-05-22 01:14:22.929696 ventures-1.3.1/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rw-r--r--   0        0        0     1571 2024-05-22 01:19:56.709374 ventures-1.3.1/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1035 2024-05-22 01:05:13.047374 ventures-1.3.1/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1189 2024-05-22 01:14:18.249745 ventures-1.3.1/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0     2246 2024-05-22 01:18:53.454171 ventures-1.3.1/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     3292 2024-05-22 01:05:07.511430 ventures-1.3.1/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.3.1/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.3.1/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.3.1/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0     2270 2024-05-22 01:19:52.349429 ventures-1.3.1/venues/stages/ventures/plays_venture/turn_off/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-22 01:19:56.709374 ventures-1.3.1/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.3.1/venues/stages/ventures/plays_venture/turn_on/__init__.py
+-rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.3.1/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.3.1/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.3.1/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.3.1/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.3.1/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.3.1/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.3.1/venues/stages/ventures/utilities/map/scan.py
+-rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.3.1/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.3.1/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.3.1/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.3.1/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.3.1/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.3.1/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.3.1/PKG-INFO
```

### Comparing `ventures-1.3.0/pyproject.toml` & `ventures-1.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.3.0"
+version = "1.3.1"
 description = ""
 authors = []
 readme = "venues/stages/ventures/readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "GPL-3.0-only"
```

### Comparing `ventures-1.3.0/venues/stages/ventures/__init__.py` & `ventures-1.3.1/venues/stages/ventures/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -137,29 +137,39 @@
 				venture = find_venture (ventures, name)
 				rich.print_json (data = {
 					"venture": venture
 				})
 			
 				turn_off_venture ({
 					"venture": venture,
-					"map": the_map_path
+					"ventures_map_bracket": ventures_map_bracket
+				})
+				
+				etch_map ({
+					"path": the_map_path,
+					"bracket": ventures_map_bracket
 				})
 				
 				status = is_on ({
 					"ventures": ventures,
 					"ventures_map_bracket": ventures_map_bracket
 				});
 				
 				return;
 	
 		turn_off ({
 			"ventures": ventures,
-			"the_map_path": the_map_path
+			"ventures_map_bracket": ventures_map_bracket
 		});
 		
+		etch_map ({
+			"path": the_map_path,
+			"bracket": ventures_map_bracket
+		})
+		
 		status = is_on ({
 			"ventures": ventures,
 			"ventures_map_bracket": ventures_map_bracket
 		});
 	
 		return;
```

### Comparing `ventures-1.3.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.3.1/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/DB/records.json` & `ventures-1.3.1/venues/stages/ventures/_status/DB/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926470588235294%*

 * *Differences: {"'_default'": "{'68': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [9.220020729117095e-07, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'status_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), OrderedDict([('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('elapsed', [7.2900002123788e-07, 'seconds']), "*

 * *               "( […]*

```diff
@@ -10357,14 +10357,149 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "68": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                9.220020729117095e-07,
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
+                                7.2900002123788e-07,
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
+                                4.149391421000473,
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
+                                3.069298151000112,
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
+                                3.091639161000785,
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
+                                4.250006832997315,
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

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status.proc.py` & `ventures-1.3.1/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/clique.py` & `ventures-1.3.1/venues/stages/ventures/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 00:49:57 2024 UTC, .py size: 2444 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,108 @@
-00000000: 6f0d 0d0a 0000 0000 3541 4d66 8c09 0000  o.......5AMf....
+00000000: 6f0d 0d0a 0000 0000 3541 4d66 b808 0000  o.......5AMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6406 6407 6c09 5a09 6406 6407 6c0a  ..d.d.l.Z.d.d.l.
-00000070: 5a0a 6406 6407 6c0b 5a0b 6406 6407 6c0c  Z.d.d.l.Z.d.d.l.
-00000080: 5a0c 6406 6407 6c0d 5a0d 6408 6409 8400  Z.d.d.l.Z.d.d...
-00000090: 5a0e 6407 5300 290a 7a19 270a 0974 7572  Z.d.S.).z.'..tur
-000000a0: 6e5f 6f66 6620 287b 0a09 090a 097d 290a  n_off ({.....}).
-000000b0: 090a 22e9 0200 0000 2901 da08 6574 6368  ..".....)...etch
-000000c0: 5f6d 6170 2901 da08 7363 616e 5f6d 6170  _map)...scan_map
-000000d0: 2901 da0c 6669 6e64 5f76 656e 7475 7265  )...find_venture
-000000e0: 2901 da0b 6368 6563 6b5f 6973 5f6f 6ee9  )...check_is_on.
-000000f0: 0000 0000 4e63 0100 0000 0000 0000 0000  ....Nc..........
-00000100: 0000 0d00 0000 0800 0000 4300 0000 73de  ..........C...s.
-00000110: 0100 007c 0064 0119 007d 017c 0064 0219  ...|.d...}.|.d..
-00000120: 007d 0274 007c 0164 0383 028f 0d7d 0374  .}.t.|.d.....}.t
-00000130: 01a0 027c 03a1 017d 0457 0064 0004 0004  ...|...}.W.d....
-00000140: 0083 0301 006e 0831 0073 1d77 0101 0001  .....n.1.s.w....
-00000150: 0001 0059 0001 0074 0364 047c 0483 0201  ...Y...t.d.|....
-00000160: 0067 007d 057c 0444 005d ba7d 067c 047c  .g.}.|.D.].}.|.|
-00000170: 0619 007d 077c 0764 0519 007d 0874 046a  ...}.|.d...}.t.j
-00000180: 0564 067c 0764 079c 0264 088d 0101 007c  .d.|.d...d.....|
-00000190: 0864 096b 0272 9b7c 0764 0919 0064 0a6b  .d.k.r.|.d...d.k
-000001a0: 0372 9b7c 0764 0919 007d 0974 046a 0564  .r.|.d...}.t.j.d
-000001b0: 0674 067c 0983 0164 0b9c 0264 088d 0101  .t.|...d...d....
-000001c0: 0074 067c 0983 0164 0c6b 0372 9b74 07a0  .t.|...d.k.r.t..
-000001d0: 087c 0974 096a 0aa1 0201 0064 0a7c 047c  .|.t.j.....d.|.|
-000001e0: 0619 0064 093c 0064 0d7d 0a09 0074 067c  ...d.<.d.}...t.|
-000001f0: 0983 017d 0b74 046a 0564 067c 067c 0b64  ...}.t.j.d.|.|.d
-00000200: 0f9c 0264 109c 0264 088d 0101 007c 0b64  ...d...d.....|.d
-00000210: 0c6b 0272 826e 1974 0ba0 0c64 11a1 0101  .k.r.n.t...d....
-00000220: 007c 0a64 1137 007d 0a7c 0a64 126b 0272  .|.d.7.}.|.d.k.r
-00000230: 9a74 0d64 137c 0a9b 0064 147c 069b 0064  .t.d.|...d.|...d
-00000240: 159d 0583 0182 0171 6d7c 0864 166b 0272  .......qm|.d.k.r
-00000250: e574 0e7c 027c 0683 027d 0c7c 0c64 1719  .t.|.|...}.|.d..
-00000260: 0083 0064 0c6b 0372 e57c 0c64 0619 0083  ...d.k.r.|.d....
-00000270: 0001 0064 0d7d 0a09 007c 0c64 1719 0083  ...d.}...|.d....
-00000280: 007d 0b74 046a 0564 1864 197c 0a7c 0c64  .}.t.j.d.d.|.|.d
-00000290: 1a19 007c 0b64 1b9c 0469 0164 088d 0101  ...|.d...i.d....
-000002a0: 007c 0b64 0c6b 0272 cc6e 1974 0ba0 0c64  .|.d.k.r.n.t...d
-000002b0: 11a1 0101 007c 0a64 1137 007d 0a7c 0a64  .....|.d.7.}.|.d
-000002c0: 126b 0272 e474 0d64 137c 0a9b 0064 147c  .k.r.t.d.|...d.|
-000002d0: 069b 0064 159d 0583 0182 0171 b371 2b74  ...d.......q.q+t
-000002e0: 0f7c 017c 0464 1c9c 0283 0101 0064 0053  .|.|.d.......d.S
-000002f0: 0029 1d4e da0c 7468 655f 6d61 705f 7061  .).N..the_map_pa
-00000300: 7468 da08 7665 6e74 7572 6573 da01 727a  th..ventures..rz
-00000310: 1576 656e 7475 7265 735f 6d61 705f 6272  .ventures_map_br
-00000320: 6163 6b65 743a da04 6b69 6e64 7a08 7475  acket:..kindz.tu
-00000330: 726e 206f 6666 2902 da04 706c 6179 da09  rn off)...play..
-00000340: 6164 7665 6e74 7572 6529 01da 0464 6174  adventure)...dat
-00000350: 61da 1070 726f 6365 7373 5f69 6465 6e74  a..process_ident
-00000360: 6974 79da 0029 0272 0b00 0000 720e 0000  ity..).r....r...
-00000370: 00da 036f 6666 7206 0000 0054 2902 da04  ...offr....T)...
-00000380: 6e61 6d65 da06 7374 6174 7573 2902 720b  name..status).r.
-00000390: 0000 007a 1273 7461 7475 7320 6368 6563  ...z.status chec
-000003a0: 6b20 6379 636c 65e9 0100 0000 e90a 0000  k cycle.........
-000003b0: 007a 0641 6674 6572 207a 0820 6c6f 6f70  .z.After z. loop
-000003c0: 732c 207a 1220 6469 6420 6e6f 7420 7475  s, z. did not tu
-000003d0: 726e 206f 6666 2eda 0474 6173 6b7a 0569  rn off...taskz.i
-000003e0: 7320 6f6e 7a19 7665 6e74 7572 6520 7374  s onz.venture st
-000003f0: 6174 7573 2063 6865 636b 206c 6f6f 707a  atus check loopz
-00000400: 1761 6674 6572 2074 7572 6e20 6f66 6620  .after turn off 
-00000410: 7761 7320 7365 6e74 7211 0000 0029 04da  was sentr....)..
-00000420: 0477 6865 6eda 046c 6f6f 7072 1100 0000  .when..loopr....
-00000430: 7212 0000 0029 02da 0470 6174 68da 0762  r....)...path..b
-00000440: 7261 636b 6574 2910 da04 6f70 656e da04  racket)...open..
-00000450: 6a73 6f6e da04 6c6f 6164 da05 7072 696e  json..load..prin
-00000460: 74da 0472 6963 68da 0a70 7269 6e74 5f6a  t..rich..print_j
-00000470: 736f 6e72 0500 0000 da02 6f73 da04 6b69  sonr......os..ki
-00000480: 6c6c da06 7369 676e 616c da07 5349 4754  ll..signal..SIGT
-00000490: 4552 4dda 0474 696d 65da 0573 6c65 6570  ERM..time..sleep
-000004a0: da09 4578 6365 7074 696f 6e72 0400 0000  ..Exceptionr....
-000004b0: 7202 0000 0029 0dda 0670 6163 6b65 7472  r....)...packetr
-000004c0: 0700 0000 7208 0000 00da 0246 50da 1476  ....r......FP..v
-000004d0: 656e 7475 7265 735f 6d61 705f 6272 6163  entures_map_brac
-000004e0: 6b65 74da 0974 6f5f 6465 6c65 7465 7211  ket..to_deleter.
-000004f0: 0000 0072 0c00 0000 720a 0000 0072 0e00  ...r....r....r..
-00000500: 0000 7217 0000 0072 1200 0000 da07 7665  ..r....r......ve
-00000510: 6e74 7572 65a9 0072 2c00 0000 fa31 2f68  nture..r,....1/h
-00000520: 6162 6974 6174 2f76 656e 7565 732f 7374  abitat/venues/st
-00000530: 6167 6573 2f76 656e 7475 7265 732f 706c  ages/ventures/pl
-00000540: 6179 732f 7475 726e 5f6f 6666 2e70 79da  ays/turn_off.py.
-00000550: 0874 7572 6e5f 6f66 661e 0000 0073 8e00  .turn_off....s..
-00000560: 0000 0801 0801 0c02 0c01 1cff 0a03 0402  ................
-00000570: 0801 0801 0801 0403 0201 0201 0afe 0806  ................
-00000580: 0c01 0801 0402 0201 0601 0afe 0c05 0e01  ................
-00000590: 0c01 0403 0201 0801 0401 0201 0202 0201  ................
-000005a0: 04fe 0afe 0808 0201 0a02 0802 0801 0201  ................
-000005b0: 1001 04ff 02ef 0816 0a01 0e02 0a01 0402  ................
-000005c0: 0201 0a01 0402 0201 0201 0201 0601 0201  ................
-000005d0: 04fc 08ff 0809 0201 0a02 0802 0801 0201  ................
-000005e0: 1001 04ff 02ed 0280 021b 0201 0201 0cfe  ................
-000005f0: 722e 0000 0029 0fda 075f 5f64 6f63 5f5f  r....)...__doc__
-00000600: da12 7574 696c 6974 6965 732e 6d61 702e  ..utilities.map.
-00000610: 6574 6368 7202 0000 00da 1275 7469 6c69  etchr......utili
-00000620: 7469 6573 2e6d 6170 2e73 6361 6e72 0300  ties.map.scanr..
-00000630: 0000 da1f 7574 696c 6974 6965 732e 7665  ....utilities.ve
-00000640: 6e74 7572 6573 2e66 696e 645f 7665 6e74  ntures.find_vent
-00000650: 7572 6572 0400 0000 da1d 7574 696c 6974  urer......utilit
-00000660: 6965 732e 7072 6f63 6573 732e 6368 6563  ies.process.chec
-00000670: 6b5f 6973 5f6f 6e72 0500 0000 721e 0000  k_is_onr....r...
-00000680: 0072 1b00 0000 7222 0000 0072 2000 0000  .r....r"...r ...
-00000690: 7224 0000 0072 2e00 0000 722c 0000 0072  r$...r....r,...r
-000006a0: 2c00 0000 722c 0000 0072 2d00 0000 da08  ,...r,...r-.....
-000006b0: 3c6d 6f64 756c 653e 0100 0000 7316 0000  <module>....s...
-000006c0: 0004 020c 0a0c 010c 010c 0108 0308 0308  ................
-000006d0: 0108 0108 010c 05                        .......
+00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
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
+000004d0: 00a9 0072 2900 0000 fa39 2f68 6162 6974  ...r)....9/habit
+000004e0: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
+000004f0: 2f76 656e 7475 7265 732f 706c 6179 735f  /ventures/plays_
+00000500: 7665 6e74 7572 652f 7475 726e 5f6f 6666  venture/turn_off
+00000510: 2e70 79da 1074 7572 6e5f 6f66 665f 7665  .py..turn_off_ve
+00000520: 6e74 7572 6515 0000 0073 8a00 0000 0801  nture....s......
+00000530: 0c02 0801 0801 0a02 0802 0c04 0c01 1cff  ................
+00000540: 0403 0201 0201 0201 0201 0afc 0807 0802  ................
+00000550: 0c01 0801 0402 0201 0601 0afe 0c05 0e01  ................
+00000560: 0c01 0403 0201 0801 0401 0201 0202 0201  ................
+00000570: 04fe 0afe 0808 0201 0a02 0802 0801 0201  ................
+00000580: 1001 04ff 02ef 0816 0e01 0a01 0402 0201  ................
+00000590: 0a01 0402 0201 0201 0201 0601 0201 04fc  ................
+000005a0: 08ff 0809 0401 0a02 0802 0801 0201 1001  ................
+000005b0: 04ff 02ed 04fb 0401 722b 0000 0029 0eda  ........r+...)..
+000005c0: 1b76 656e 7475 7265 732e 7574 696c 6974  .ventures.utilit
+000005d0: 6965 732e 6d61 702e 6574 6368 7202 0000  ies.map.etchr...
+000005e0: 00da 1b76 656e 7475 7265 732e 7574 696c  ...ventures.util
+000005f0: 6974 6965 732e 6d61 702e 7363 616e 7203  ities.map.scanr.
+00000600: 0000 00da 2876 656e 7475 7265 732e 7574  ....(ventures.ut
+00000610: 696c 6974 6965 732e 7665 6e74 7572 6573  ilities.ventures
+00000620: 2e66 696e 645f 7665 6e74 7572 6572 0400  .find_venturer..
+00000630: 0000 da26 7665 6e74 7572 6573 2e75 7469  ...&ventures.uti
+00000640: 6c69 7469 6573 2e70 726f 6365 7373 2e63  lities.process.c
+00000650: 6865 636b 5f69 735f 6f6e 7205 0000 0072  heck_is_onr....r
+00000660: 1c00 0000 721a 0000 0072 2000 0000 721e  ....r....r ...r.
+00000670: 0000 0072 2200 0000 722b 0000 0072 2900  ...r"...r+...r).
+00000680: 0000 7229 0000 0072 2900 0000 722a 0000  ..r)...r)...r*..
+00000690: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000006a0: 1400 0000 0c04 0c01 0c01 0c01 0803 0803  ................
+000006b0: 0801 0801 0801 0c04                      ........
```

### Comparing `ventures-1.3.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/plays/is_on.py` & `ventures-1.3.1/venues/stages/ventures/plays/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/plays/turn_off.py` & `ventures-1.3.1/venues/stages/ventures/plays/turn_on.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,174 @@
 
-
-''''
-	turn_off ({
-		
-	})
-	
-"'''
-
-
 #++++
 #
-from ..utilities.map.etch import etch_map
-from ..utilities.map.scan import scan_map	
-from ..utilities.ventures.find_venture import find_venture
-from ..utilities.process.check_is_on import check_is_on
+from ventures.utilities.hike_passive import hike_passive
+from ventures.utilities.map.etch import etch_map
+from ventures.utilities.map.scan import scan_map	
+from ventures.utilities.ventures.find_venture import find_venture
+#
+from ventures.utilities.process.check_is_on import check_is_on
+#
+from ventures.plays_venture.turn_on import turn_on_venture
+
 #
 #
 import rich
 #
 #
-import json
-import signal
 import os
 import time
 #
 #++++
 
+''''
+	{
+		"name": "adventure_1",
+		"turn on": {
+			"adventure": "python3 -m http.server 8080",
+			"kind": "process_identity",
+			"Popen": {
+				"CWD": 
+			},
+		}
+	}
+	
+	{
+		"name": "adventure_2",
+		"turn on": {
+			"adventure": turn_on,
+			"kind": "task"
+		}
+	}
+"'''
+
 
-def turn_off (packet):
-	the_map_path = packet ["the_map_path"]
+def turn_on (packet):
 	ventures = packet ["ventures"]
+	ventures_map_bracket = packet ["ventures_map_bracket"]
 	
-	with open (the_map_path, 'r') as FP:
-		ventures_map_bracket = json.load (FP)
 
-	print ("ventures_map_bracket:", ventures_map_bracket)
+
+
+	for adventure in ventures:
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
 	
-	to_delete = []
-	for name in ventures_map_bracket:
-		adventure = ventures_map_bracket [ name ]
+		adventure_script = adventure ["turn on"] ["adventure"]
 		kind = adventure ["kind"]
+		name = adventure ["name"]
 		
 		
-		rich.print_json (data = {
-			"play": "turn off",
-			"adventure": adventure
-		})
-
+		#
+		#	check if is already on	
+		#
+		#
+		if (name in ventures_map_bracket):
+			if (kind == "process_identity"):
+				if (ventures_map_bracket [ name ] ["process_identity"] != ""):
+					status = check_is_on (ventures_map_bracket [ name ] ["process_identity"])
+					if (status == "on"):
+						#print (f'"{ name }" is already on')
+						continue;
+			
+			if (kind == "task"):
+				venture = find_venture (ventures, name)
+				status = venture ["is on"] ()
+				if (status == "on"):
+					continue;
 
+		
+		
 		if (kind == "process_identity"):
-			if (adventure ["process_identity"] != ""):
-				process_identity = adventure ["process_identity"]
+			print ("adventure:", adventure)
+		
+			Popen_keys = {}
+			if ("turn on" in adventure):
+				if ("Popen" in adventure ["turn on"]):
+					if (type (adventure ["turn on"] ["Popen"]) == dict):
+						Popen_keys = adventure ["turn on"] ["Popen"]
+		
+			process = hike_passive ({
+				"script": adventure_script,
+				"Popen": Popen_keys
+			})
 			
+			loop = 0
+			while True:
+				status = check_is_on (process ["process_identity"])	
 				rich.print_json (data = {
-					"play": "turn off",
-					"process_identity": check_is_on (process_identity)
+					"venture status check loop": {
+						"when": "after turn on was sent",
+						"loop": loop,
+						"name": name,
+						"status": status
+					}
 				})
-					
-				if (check_is_on (process_identity) != "off"):
-					os.kill (process_identity, signal.SIGTERM)
-					ventures_map_bracket [ name ] ["process_identity"] = ""
-					
-					#to_delete.append (name)
-					loop = 0
-					while True:
-						status = check_is_on (process_identity)	
-						rich.print_json (data = {
-							"play": "turn off",
-							"status check cycle": {
-								"name": name,
-								"status": status
-							}
-						})
-						
-						if (status == "off"):
-							break;
-						
-						time.sleep (1)
-
-						loop += 1
-						if (loop == 10):
-							raise Exception (
-								f"After { loop } loops, { name } did not turn off."
-							)
-					
+				
+				if (status == "on"):
+					break;
+				
+				time.sleep (1)
+
+				loop += 1
+				if (loop == 10):
+					raise Exception (
+						f"After { loop } loops, { name } did not turn on."
+					)
+		
+			ventures_map_bracket [ name ] = {
+				"kind": kind,
+				"process_identity": process ["process_identity"]
+			}
+		
+			continue;
 			
 		if (kind == "task"):
-			venture = find_venture (ventures, name)
+			adventure_script ()
 			
-			if (venture ["is on"] () != "off"):			
-				venture ["turn off"] ()
+			loop = 0
+			while True:
+				status = adventure ["is on"] ()		
+				rich.print_json (data = {
+					"venture status check loop": {
+						"when": "after turn on was sent",
+						"loop": loop,
+						"name": name,
+						"status": status
+					}
+				})
 				
-				loop = 0
-				while True:
-					status = venture ["is on"] ()		
-
-					rich.print_json (data = {
-						"venture status check loop": {
-							"when": "after turn off was sent",
-							"loop": loop,
-							"name": venture ["name"],
-							"status": status
-						}
-					})
-					
-					if (status == "off"):
-						break;
-					
-					time.sleep (1)
-
-					loop += 1
-					if (loop == 10):
-						raise Exception (
-							f"After { loop } loops, { name } did not turn off."
-						)
+				if (status == "on"):
+					break;
 				
-	#for name in to_delete:
-	#	del ventures_map_bracket [ name ]
+				time.sleep (1)
+
+				loop += 1
+				if (loop == 10):
+					raise Exception (
+						f"After { loop } loops, { name } did not turn on."
+					)
+			
+			ventures_map_bracket [ name ] = {
+				"kind": kind
+			}
+			
+		
+		else:
+			raise Exception (f'Kind "{ kind } was not found.')
+
+	
+	
 	
+	return {
+		"ventures_map_bracket": ventures_map_bracket
+	}
 	
-	etch_map ({
-		"path": the_map_path,
-		"bracket": ventures_map_bracket
-	})
```

### Comparing `ventures-1.3.0/venues/stages/ventures/plays/turn_on.py` & `ventures-1.3.1/venues/stages/ventures/plays_venture/turn_on/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,174 +1,144 @@
 
+
+'''
+	turn_on_venture ({
+		"venture": {
+			"kind": "",
+			"name": "",
+			"turn on": {
+				"adventure": ""
+			}
+		},
+		"ventures_map_bracket": 
+	})
+'''
+
 #++++
 #
-from ventures.utilities.hike_passive import hike_passive
+from ventures.utilities.map.scan import scan_map
 from ventures.utilities.map.etch import etch_map
-from ventures.utilities.map.scan import scan_map	
-from ventures.utilities.ventures.find_venture import find_venture
-#
 from ventures.utilities.process.check_is_on import check_is_on
+from ventures.utilities.hike_passive import hike_passive
 #
-from ventures.plays_venture.turn_on import turn_on_venture
-
+from ventures.utilities.ventures.find_venture import find_venture
 #
 #
 import rich
 #
 #
 import os
 import time
 #
 #++++
-
-''''
-	{
-		"name": "adventure_1",
-		"turn on": {
-			"adventure": "python3 -m http.server 8080",
-			"kind": "process_identity",
-			"Popen": {
-				"CWD": 
-			},
-		}
-	}
 	
-	{
-		"name": "adventure_2",
-		"turn on": {
-			"adventure": turn_on,
-			"kind": "task"
-		}
-	}
-"'''
+def turn_on_venture (packet):
+	venture = packet ["venture"]
 
-
-def turn_on (packet):
-	ventures = packet ["ventures"]
+	adventure_script = venture ["turn on"] ["adventure"]
+	kind = venture ["kind"]
+	name = venture ["name"]
+	
 	ventures_map_bracket = packet ["ventures_map_bracket"]
 	
-
-
-
-	for adventure in ventures:
-		turn_on_venture ({
-			"venture": adventure,
-			"ventures_map_bracket": ventures_map_bracket
-		})
+	#
+	#	check if is already on	
+	#
+	#
+	if (name in ventures_map_bracket):
+		if (kind == "process_identity"):
+			if (ventures_map_bracket [ name ] ["process_identity"] != ""):
+				status = check_is_on (ventures_map_bracket [ name ] ["process_identity"])
+				if (status == "on"):
+					#print (f'"{ name }" is already on')
+					return;
 		
-		rich.print_json (data = {
-			"proceeds of turn on": ventures_map_bracket
+		if (kind == "task"):
+			#venture = find_venture (ventures, name)
+			status = venture ["is on"] ()
+			if (status == "on"):
+				return;
+
+	
+	
+	if (kind == "process_identity"):
+		print ("venture:", venture)
+	
+		Popen_keys = {}
+		if ("turn on" in venture):
+			if ("Popen" in venture ["turn on"]):
+				if (type (venture ["turn on"] ["Popen"]) == dict):
+					Popen_keys = venture ["turn on"] ["Popen"]
+	
+		process = hike_passive ({
+			"script": adventure_script,
+			"Popen": Popen_keys
 		})
 		
-		continue;
+		loop = 0
+		while True:
+			status = check_is_on (process ["process_identity"])	
+			rich.print_json (data = {
+				"venture status check loop": {
+					"when": "after turn on was sent",
+					"loop": loop,
+					"name": name,
+					"status": status
+				}
+			})
 			
-	
-		adventure_script = adventure ["turn on"] ["adventure"]
-		kind = adventure ["kind"]
-		name = adventure ["name"]
-		
-		
-		#
-		#	check if is already on	
-		#
-		#
-		if (name in ventures_map_bracket):
-			if (kind == "process_identity"):
-				if (ventures_map_bracket [ name ] ["process_identity"] != ""):
-					status = check_is_on (ventures_map_bracket [ name ] ["process_identity"])
-					if (status == "on"):
-						#print (f'"{ name }" is already on')
-						continue;
+			if (status == "on"):
+				break;
 			
-			if (kind == "task"):
-				venture = find_venture (ventures, name)
-				status = venture ["is on"] ()
-				if (status == "on"):
-					continue;
+			time.sleep (1)
 
+			loop += 1
+			if (loop == 10):
+				raise Exception (
+					f"After { loop } loops, { name } did not turn on."
+				)
+	
+		ventures_map_bracket [ name ] = {
+			"kind": kind,
+			"process_identity": process ["process_identity"]
+		}
+	
 		
 		
-		if (kind == "process_identity"):
-			print ("adventure:", adventure)
+	elif (kind == "task"):
+		adventure_script ()
 		
-			Popen_keys = {}
-			if ("turn on" in adventure):
-				if ("Popen" in adventure ["turn on"]):
-					if (type (adventure ["turn on"] ["Popen"]) == dict):
-						Popen_keys = adventure ["turn on"] ["Popen"]
-		
-			process = hike_passive ({
-				"script": adventure_script,
-				"Popen": Popen_keys
+		loop = 0
+		while True:
+			status = venture ["is on"] ()		
+			rich.print_json (data = {
+				"venture status check loop": {
+					"when": "after turn on was sent",
+					"loop": loop,
+					"name": name,
+					"status": status
+				}
 			})
 			
-			loop = 0
-			while True:
-				status = check_is_on (process ["process_identity"])	
-				rich.print_json (data = {
-					"venture status check loop": {
-						"when": "after turn on was sent",
-						"loop": loop,
-						"name": name,
-						"status": status
-					}
-				})
-				
-				if (status == "on"):
-					break;
-				
-				time.sleep (1)
-
-				loop += 1
-				if (loop == 10):
-					raise Exception (
-						f"After { loop } loops, { name } did not turn on."
-					)
-		
-			ventures_map_bracket [ name ] = {
-				"kind": kind,
-				"process_identity": process ["process_identity"]
-			}
-		
-			continue;
-			
-		if (kind == "task"):
-			adventure_script ()
-			
-			loop = 0
-			while True:
-				status = adventure ["is on"] ()		
-				rich.print_json (data = {
-					"venture status check loop": {
-						"when": "after turn on was sent",
-						"loop": loop,
-						"name": name,
-						"status": status
-					}
-				})
-				
-				if (status == "on"):
-					break;
-				
-				time.sleep (1)
-
-				loop += 1
-				if (loop == 10):
-					raise Exception (
-						f"After { loop } loops, { name } did not turn on."
-					)
+			if (status == "on"):
+				break;
 			
-			ventures_map_bracket [ name ] = {
-				"kind": kind
-			}
-			
-		
-		else:
-			raise Exception (f'Kind "{ kind } was not found.')
+			time.sleep (1)
 
-	
-	
-	
-	return {
+			loop += 1
+			if (loop == 10):
+				raise Exception (
+					f"After { loop } loops, { name } did not turn on."
+				)
+		
+		ventures_map_bracket [ name ] = {
+			"kind": kind
+		}
+		
+	else:
+		raise Exception (f'Kind "{ kind } was not found.')
+		
+		
+	return 	{
 		"ventures_map_bracket": ventures_map_bracket
 	}
-	
+
```

### Comparing `ventures-1.3.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 00:49:57 2024 UTC, .py size: 2232 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,120 @@
-00000000: 6f0d 0d0a 0000 0000 3541 4d66 b808 0000  o.......5AMf....
+00000000: 6f0d 0d0a 0000 0000 9346 4d66 c40a 0000  o........FMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c08 5a08 6400 6405 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6405 6c0a 5a0a 6400 6405 6c0b 5a0b 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6405 6c0c 5a0c 6406 6407 8400 5a0d 6405  d.l.Z.d.d...Z.d.
-00000090: 5300 2908 e900 0000 0029 01da 0865 7463  S.)......)...etc
-000000a0: 685f 6d61 7029 01da 0873 6361 6e5f 6d61  h_map)...scan_ma
-000000b0: 7029 01da 0c66 696e 645f 7665 6e74 7572  p)...find_ventur
-000000c0: 6529 01da 0b63 6865 636b 5f69 735f 6f6e  e)...check_is_on
-000000d0: 4e63 0100 0000 0000 0000 0000 0000 0b00  Nc..............
-000000e0: 0000 0800 0000 4300 0000 73d6 0100 007c  ......C...s....|
-000000f0: 0064 0119 007d 017c 0164 0219 0064 0319  .d...}.|.d...d..
-00000100: 007d 027c 0164 0419 007d 037c 0164 0519  .}.|.d...}.|.d..
-00000110: 007d 0474 0064 067c 0183 0201 007c 0064  .}.t.d.|.....|.d
-00000120: 0719 007d 0574 017c 0564 0883 028f 0d7d  ...}.t.|.d.....}
-00000130: 0674 02a0 037c 06a1 017d 0757 0064 0004  .t...|...}.W.d..
-00000140: 0004 0083 0301 006e 0831 0073 3077 0101  .......n.1.s0w..
-00000150: 0001 0001 0059 0001 0074 046a 0564 097c  .....Y...t.j.d.|
-00000160: 017c 077c 0464 0a9c 0464 0b8d 0101 007c  .|.|.d...d.....|
-00000170: 077c 0419 007d 017c 0364 0c6b 0272 a17c  .|...}.|.d.k.r.|
-00000180: 0164 0c19 0064 0d6b 0372 a17c 0164 0c19  .d...d.k.r.|.d..
-00000190: 007d 0874 046a 0564 0974 067c 0883 0164  .}.t.j.d.t.|...d
-000001a0: 0e9c 0264 0b8d 0101 0074 067c 0883 0164  ...d.....t.|...d
-000001b0: 0f6b 0372 a174 07a0 087c 0874 096a 0aa1  .k.r.t...|.t.j..
-000001c0: 0201 0064 0d7c 077c 0419 0064 0c3c 0064  ...d.|.|...d.<.d
-000001d0: 107d 0909 0074 067c 0883 017d 0a74 046a  .}...t.|...}.t.j
-000001e0: 0564 097c 047c 0a64 129c 0264 139c 0264  .d.|.|.d...d...d
-000001f0: 0b8d 0101 007c 0a64 0f6b 0272 886e 1974  .....|.d.k.r.n.t
-00000200: 0ba0 0c64 14a1 0101 007c 0964 1437 007d  ...d.....|.d.7.}
-00000210: 097c 0964 156b 0272 a074 0d64 167c 099b  .|.d.k.r.t.d.|..
-00000220: 0064 177c 049b 0064 189d 0583 0182 0171  .d.|...d.......q
-00000230: 737c 0364 196b 0272 e77c 0164 1a19 0083  s|.d.k.r.|.d....
-00000240: 0064 0f6b 0372 e97c 0164 0919 0083 0001  .d.k.r.|.d......
-00000250: 0064 107d 0909 007c 0164 1a19 0083 007d  .d.}...|.d.....}
-00000260: 0a74 046a 0564 1b64 1c7c 097c 0164 0519  .t.j.d.d.|.|.d..
-00000270: 007c 0a64 1d9c 0469 0164 0b8d 0101 007c  .|.d...i.d.....|
-00000280: 0a64 0f6b 0272 ce64 0053 0074 0ba0 0c64  .d.k.r.d.S.t...d
-00000290: 14a1 0101 007c 0964 1437 007d 097c 0964  .....|.d.7.}.|.d
-000002a0: 156b 0272 e674 0d64 167c 099b 0064 177c  .k.r.t.d.|...d.|
-000002b0: 049b 0064 189d 0583 0182 0171 b464 0053  ...d.......q.d.S
-000002c0: 0064 0053 0029 1e4e da07 7665 6e74 7572  .d.S.).N..ventur
-000002d0: 657a 0774 7572 6e20 6f6e da09 6164 7665  ez.turn on..adve
-000002e0: 6e74 7572 65da 046b 696e 64da 046e 616d  nture..kind..nam
-000002f0: 657a 0876 656e 7475 7265 3ada 036d 6170  ez.venture:..map
-00000300: da01 727a 0874 7572 6e20 6f66 6629 04da  ..rz.turn off)..
-00000310: 0470 6c61 7972 0600 0000 da14 7665 6e74  .playr......vent
-00000320: 7572 6573 5f6d 6170 5f62 7261 636b 6574  ures_map_bracket
-00000330: 7209 0000 0029 01da 0464 6174 61da 1070  r....)...data..p
-00000340: 726f 6365 7373 5f69 6465 6e74 6974 79da  rocess_identity.
-00000350: 0029 0272 0c00 0000 720f 0000 00da 036f  .).r....r......o
-00000360: 6666 7201 0000 0054 2902 7209 0000 00da  ffr....T).r.....
-00000370: 0673 7461 7475 7329 0272 0c00 0000 7a12  .status).r....z.
-00000380: 7374 6174 7573 2063 6865 636b 2063 7963  status check cyc
-00000390: 6c65 e901 0000 00e9 0a00 0000 7a06 4166  le..........z.Af
-000003a0: 7465 7220 7a08 206c 6f6f 7073 2c20 7a12  ter z. loops, z.
-000003b0: 2064 6964 206e 6f74 2074 7572 6e20 6f66   did not turn of
-000003c0: 662e da04 7461 736b 7a05 6973 206f 6e7a  f...taskz.is onz
-000003d0: 1976 656e 7475 7265 2073 7461 7475 7320  .venture status 
-000003e0: 6368 6563 6b20 6c6f 6f70 7a17 6166 7465  check loopz.afte
-000003f0: 7220 7475 726e 206f 6666 2077 6173 2073  r turn off was s
-00000400: 656e 7429 04da 0477 6865 6eda 046c 6f6f  ent)...when..loo
-00000410: 7072 0900 0000 7212 0000 0029 0eda 0570  pr....r....)...p
-00000420: 7269 6e74 da04 6f70 656e da04 6a73 6f6e  rint..open..json
-00000430: da04 6c6f 6164 da04 7269 6368 da0a 7072  ..load..rich..pr
-00000440: 696e 745f 6a73 6f6e 7205 0000 00da 026f  int_jsonr......o
-00000450: 73da 046b 696c 6cda 0673 6967 6e61 6cda  s..kill..signal.
-00000460: 0753 4947 5445 524d da04 7469 6d65 da05  .SIGTERM..time..
-00000470: 736c 6565 70da 0945 7863 6570 7469 6f6e  sleep..Exception
-00000480: 290b da06 7061 636b 6574 7206 0000 00da  )...packetr.....
-00000490: 1061 6476 656e 7475 7265 5f73 6372 6970  .adventure_scrip
-000004a0: 7472 0800 0000 7209 0000 00da 0c74 6865  tr....r......the
-000004b0: 5f6d 6170 5f70 6174 68da 0246 5072 0d00  _map_path..FPr..
-000004c0: 0000 720f 0000 0072 1700 0000 7212 0000  ..r....r....r...
-000004d0: 00a9 0072 2900 0000 fa39 2f68 6162 6974  ...r)....9/habit
-000004e0: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
-000004f0: 2f76 656e 7475 7265 732f 706c 6179 735f  /ventures/plays_
-00000500: 7665 6e74 7572 652f 7475 726e 5f6f 6666  venture/turn_off
-00000510: 2e70 79da 1074 7572 6e5f 6f66 665f 7665  .py..turn_off_ve
-00000520: 6e74 7572 6515 0000 0073 8a00 0000 0801  nture....s......
-00000530: 0c02 0801 0801 0a02 0802 0c04 0c01 1cff  ................
-00000540: 0403 0201 0201 0201 0201 0afc 0807 0802  ................
-00000550: 0c01 0801 0402 0201 0601 0afe 0c05 0e01  ................
-00000560: 0c01 0403 0201 0801 0401 0201 0202 0201  ................
-00000570: 04fe 0afe 0808 0201 0a02 0802 0801 0201  ................
-00000580: 1001 04ff 02ef 0816 0e01 0a01 0402 0201  ................
-00000590: 0a01 0402 0201 0201 0201 0601 0201 04fc  ................
-000005a0: 08ff 0809 0401 0a02 0802 0801 0201 1001  ................
-000005b0: 04ff 02ed 04fb 0401 722b 0000 0029 0eda  ........r+...)..
-000005c0: 1b76 656e 7475 7265 732e 7574 696c 6974  .ventures.utilit
-000005d0: 6965 732e 6d61 702e 6574 6368 7202 0000  ies.map.etchr...
-000005e0: 00da 1b76 656e 7475 7265 732e 7574 696c  ...ventures.util
-000005f0: 6974 6965 732e 6d61 702e 7363 616e 7203  ities.map.scanr.
-00000600: 0000 00da 2876 656e 7475 7265 732e 7574  ....(ventures.ut
-00000610: 696c 6974 6965 732e 7665 6e74 7572 6573  ilities.ventures
-00000620: 2e66 696e 645f 7665 6e74 7572 6572 0400  .find_venturer..
-00000630: 0000 da26 7665 6e74 7572 6573 2e75 7469  ...&ventures.uti
-00000640: 6c69 7469 6573 2e70 726f 6365 7373 2e63  lities.process.c
-00000650: 6865 636b 5f69 735f 6f6e 7205 0000 0072  heck_is_onr....r
-00000660: 1c00 0000 721a 0000 0072 2000 0000 721e  ....r....r ...r.
-00000670: 0000 0072 2200 0000 722b 0000 0072 2900  ...r"...r+...r).
-00000680: 0000 7229 0000 0072 2900 0000 722a 0000  ..r)...r)...r*..
-00000690: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000006a0: 1400 0000 0c04 0c01 0c01 0c01 0803 0803  ................
-000006b0: 0801 0801 0801 0c04                      ........
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
+00000070: 6407 6c0b 5a0b 6401 6407 6c0c 5a0c 6401  d.l.Z.d.d.l.Z.d.
+00000080: 6407 6c0d 5a0d 6408 6409 8400 5a0e 6407  d.l.Z.d.d...Z.d.
+00000090: 5300 290a 7a8f 0a09 7475 726e 5f6f 6e5f  S.).z...turn_on_
+000000a0: 7665 6e74 7572 6520 287b 0a09 0922 7665  venture ({..."ve
+000000b0: 6e74 7572 6522 3a20 7b0a 0909 0922 6b69  nture": {...."ki
+000000c0: 6e64 223a 2022 222c 0a09 0909 226e 616d  nd": "",...."nam
+000000d0: 6522 3a20 2222 2c0a 0909 0922 7475 726e  e": "",...."turn
+000000e0: 206f 6e22 3a20 7b0a 0909 0909 2261 6476   on": {....."adv
+000000f0: 656e 7475 7265 223a 2022 220a 0909 097d  enture": ""....}
+00000100: 0a09 097d 2c0a 0909 2276 656e 7475 7265  ...},..."venture
+00000110: 735f 6d61 705f 6272 6163 6b65 7422 3a20  s_map_bracket": 
+00000120: 0a09 7d29 0ae9 0000 0000 2901 da08 7363  ..})......)...sc
+00000130: 616e 5f6d 6170 2901 da08 6574 6368 5f6d  an_map)...etch_m
+00000140: 6170 2901 da0b 6368 6563 6b5f 6973 5f6f  ap)...check_is_o
+00000150: 6e29 01da 0c68 696b 655f 7061 7373 6976  n)...hike_passiv
+00000160: 6529 01da 0c66 696e 645f 7665 6e74 7572  e)...find_ventur
+00000170: 654e 6301 0000 0000 0000 0000 0000 000a  eNc.............
+00000180: 0000 0007 0000 0043 0000 0073 f801 0000  .......C...s....
+00000190: 7c00 6401 1900 7d01 7c01 6402 1900 6403  |.d...}.|.d...d.
+000001a0: 1900 7d02 7c01 6404 1900 7d03 7c01 6405  ..}.|.d...}.|.d.
+000001b0: 1900 7d04 7c00 6406 1900 7d05 7c04 7c05  ..}.|.d...}.|.|.
+000001c0: 7600 7243 7c03 6407 6b02 7234 7c05 7c04  v.rC|.d.k.r4|.|.
+000001d0: 1900 6407 1900 6408 6b03 7234 7400 7c05  ..d...d.k.r4t.|.
+000001e0: 7c04 1900 6407 1900 8301 7d06 7c06 6409  |...d.....}.|.d.
+000001f0: 6b02 7234 6400 5300 7c03 640a 6b02 7243  k.r4d.S.|.d.k.rC
+00000200: 7c01 640b 1900 8300 7d06 7c06 6409 6b02  |.d.....}.|.d.k.
+00000210: 7243 6400 5300 7c03 6407 6b02 72b0 7401  rCd.S.|.d.k.r.t.
+00000220: 640c 7c01 8302 0100 6900 7d07 6402 7c01  d.|.....i.}.d.|.
+00000230: 7600 7268 640d 7c01 6402 1900 7600 7268  v.rhd.|.d...v.rh
+00000240: 7402 7c01 6402 1900 640d 1900 8301 7403  t.|.d...d.....t.
+00000250: 6b02 7268 7c01 6402 1900 640d 1900 7d07  k.rh|.d...d...}.
+00000260: 7404 7c02 7c07 640e 9c02 8301 7d08 640f  t.|.|.d.....}.d.
+00000270: 7d09 0900 7400 7c08 6407 1900 8301 7d06  }...t.|.d.....}.
+00000280: 7405 6a06 6411 6412 7c09 7c04 7c06 6413  t.j.d.d.|.|.|.d.
+00000290: 9c04 6901 6414 8d01 0100 7c06 6409 6b02  ..i.d.....|.d.k.
+000002a0: 728a 6e19 7407 a008 6415 a101 0100 7c09  r.n.t...d.....|.
+000002b0: 6415 3700 7d09 7c09 6416 6b02 72a2 7409  d.7.}.|.d.k.r.t.
+000002c0: 6417 7c09 9b00 6418 7c04 9b00 6419 9d05  d.|...d.|...d...
+000002d0: 8301 8201 7172 7c03 7c08 6407 1900 641a  ....qr|.|.d...d.
+000002e0: 9c02 7c05 7c04 3c00 6406 7c05 6901 5300  ..|.|.<.d.|.i.S.
+000002f0: 7c03 640a 6b02 72f4 7c02 8300 0100 640f  |.d.k.r.|.....d.
+00000300: 7d09 0900 7c01 640b 1900 8300 7d06 7405  }...|.d.....}.t.
+00000310: 6a06 6411 6412 7c09 7c04 7c06 6413 9c04  j.d.d.|.|.|.d...
+00000320: 6901 6414 8d01 0100 7c06 6409 6b02 72d1  i.d.....|.d.k.r.
+00000330: 6e19 7407 a008 6415 a101 0100 7c09 6415  n.t...d.....|.d.
+00000340: 3700 7d09 7c09 6416 6b02 72e9 7409 6417  7.}.|.d.k.r.t.d.
+00000350: 7c09 9b00 6418 7c04 9b00 6419 9d05 8301  |...d.|...d.....
+00000360: 8201 71ba 6404 7c03 6901 7c05 7c04 3c00  ..q.d.|.i.|.|.<.
+00000370: 6406 7c05 6901 5300 7409 641b 7c03 9b00  d.|.i.S.t.d.|...
+00000380: 641c 9d03 8301 8201 291d 4eda 0776 656e  d.......).N..ven
+00000390: 7475 7265 7a07 7475 726e 206f 6eda 0961  turez.turn on..a
+000003a0: 6476 656e 7475 7265 da04 6b69 6e64 da04  dventure..kind..
+000003b0: 6e61 6d65 da14 7665 6e74 7572 6573 5f6d  name..ventures_m
+000003c0: 6170 5f62 7261 636b 6574 da10 7072 6f63  ap_bracket..proc
+000003d0: 6573 735f 6964 656e 7469 7479 da00 da02  ess_identity....
+000003e0: 6f6e da04 7461 736b 7a05 6973 206f 6e7a  on..taskz.is onz
+000003f0: 0876 656e 7475 7265 3ada 0550 6f70 656e  .venture:..Popen
+00000400: 2902 da06 7363 7269 7074 7210 0000 0072  )...scriptr....r
+00000410: 0100 0000 547a 1976 656e 7475 7265 2073  ....Tz.venture s
+00000420: 7461 7475 7320 6368 6563 6b20 6c6f 6f70  tatus check loop
+00000430: 7a16 6166 7465 7220 7475 726e 206f 6e20  z.after turn on 
+00000440: 7761 7320 7365 6e74 2904 da04 7768 656e  was sent)...when
+00000450: da04 6c6f 6f70 720a 0000 00da 0673 7461  ..loopr......sta
+00000460: 7475 7329 01da 0464 6174 61e9 0100 0000  tus)...data.....
+00000470: e90a 0000 007a 0641 6674 6572 207a 0820  .....z.After z. 
+00000480: 6c6f 6f70 732c 207a 1120 6469 6420 6e6f  loops, z. did no
+00000490: 7420 7475 726e 206f 6e2e 2902 7209 0000  t turn on.).r...
+000004a0: 0072 0c00 0000 7a06 4b69 6e64 2022 7a0f  .r....z.Kind "z.
+000004b0: 2077 6173 206e 6f74 2066 6f75 6e64 2e29   was not found.)
+000004c0: 0a72 0400 0000 da05 7072 696e 74da 0474  .r......print..t
+000004d0: 7970 65da 0464 6963 7472 0500 0000 da04  ype..dictr......
+000004e0: 7269 6368 da0a 7072 696e 745f 6a73 6f6e  rich..print_json
+000004f0: da04 7469 6d65 da05 736c 6565 70da 0945  ..time..sleep..E
+00000500: 7863 6570 7469 6f6e 290a da06 7061 636b  xception)...pack
+00000510: 6574 7207 0000 00da 1061 6476 656e 7475  etr......adventu
+00000520: 7265 5f73 6372 6970 7472 0900 0000 720a  re_scriptr....r.
+00000530: 0000 0072 0b00 0000 7214 0000 00da 0a50  ...r....r......P
+00000540: 6f70 656e 5f6b 6579 73da 0770 726f 6365  open_keys..proce
+00000550: 7373 7213 0000 00a9 0072 2400 0000 fa41  ssr......r$....A
+00000560: 2f68 6162 6974 6174 2f76 656e 7565 732f  /habitat/venues/
+00000570: 7374 6167 6573 2f76 656e 7475 7265 732f  stages/ventures/
+00000580: 706c 6179 735f 7665 6e74 7572 652f 7475  plays_venture/tu
+00000590: 726e 5f6f 6e2f 5f5f 696e 6974 5f5f 2e70  rn_on/__init__.p
+000005a0: 79da 0f74 7572 6e5f 6f6e 5f76 656e 7475  y..turn_on_ventu
+000005b0: 7265 2200 0000 739c 0000 0008 010c 0208  re"...s.........
+000005c0: 0108 0108 0208 0608 0110 0110 0108 0104  ................
+000005d0: 0208 020a 0208 0104 0108 040a 0104 0208  ................
+000005e0: 010c 0114 010c 0102 0202 0102 0108 fe04  ................
+000005f0: 0502 010c 0104 0102 0102 0102 0102 0102  ................
+00000600: 0104 fc08 ff08 0902 010a 0208 0208 0102  ................
+00000610: 0110 0104 ff02 ee02 1706 010a fe04 2a04  ..............*.
+00000620: ff08 de06 0104 0202 010a 0104 0102 0102  ................
+00000630: 0102 0102 0102 0104 fc08 ff08 0902 010a  ................
+00000640: 0208 0208 0102 0110 0104 ff02 ee04 1708  ................
+00000650: ff04 0904 ff10 fd72 2600 0000 290f da07  .......r&...)...
+00000660: 5f5f 646f 635f 5fda 1b76 656e 7475 7265  __doc__..venture
+00000670: 732e 7574 696c 6974 6965 732e 6d61 702e  s.utilities.map.
+00000680: 7363 616e 7202 0000 00da 1b76 656e 7475  scanr......ventu
+00000690: 7265 732e 7574 696c 6974 6965 732e 6d61  res.utilities.ma
+000006a0: 702e 6574 6368 7203 0000 00da 2676 656e  p.etchr.....&ven
+000006b0: 7475 7265 732e 7574 696c 6974 6965 732e  tures.utilities.
+000006c0: 7072 6f63 6573 732e 6368 6563 6b5f 6973  process.check_is
+000006d0: 5f6f 6e72 0400 0000 da1f 7665 6e74 7572  _onr......ventur
+000006e0: 6573 2e75 7469 6c69 7469 6573 2e68 696b  es.utilities.hik
+000006f0: 655f 7061 7373 6976 6572 0500 0000 da28  e_passiver.....(
+00000700: 7665 6e74 7572 6573 2e75 7469 6c69 7469  ventures.utiliti
+00000710: 6573 2e76 656e 7475 7265 732e 6669 6e64  es.ventures.find
+00000720: 5f76 656e 7475 7265 7206 0000 0072 1b00  _venturer....r..
+00000730: 0000 da02 6f73 721d 0000 0072 2600 0000  ....osr....r&...
+00000740: 7224 0000 0072 2400 0000 7224 0000 0072  r$...r$...r$...r
+00000750: 2500 0000 da08 3c6d 6f64 756c 653e 0100  %.....<module>..
+00000760: 0000 7314 0000 0004 020c 0f0c 010c 010c  ..s.............
+00000770: 010c 0208 0308 0308 010c 04              ...........
```

### Comparing `ventures-1.3.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/plays_venture/turn_off/__init__.py` & `ventures-1.3.1/venues/stages/ventures/plays_venture/turn_off/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,21 @@
 
+'''
+	turn_off_venture ({
+		"venture": {
+			"kind": "",
+			"name": "",
+			"turn on": {
+				"adventure": ""
+			}
+		},
+		"ventures_map_bracket": 
+	})
+'''
+
 
 #++++
 #
 from ventures.utilities.map.etch import etch_map
 from ventures.utilities.map.scan import scan_map	
 from ventures.utilities.ventures.find_venture import find_venture
 from ventures.utilities.process.check_is_on import check_is_on
@@ -16,25 +29,21 @@
 import os
 import time
 #
 #++++
 
 def turn_off_venture (packet):
 	venture = packet ["venture"]
+	ventures_map_bracket = packet ["ventures_map_bracket"]
 
-	adventure_script = venture ["turn on"] ["adventure"]
 	kind = venture ["kind"]
 	name = venture ["name"]
 	
 	print ("venture:", venture)
 	
-	the_map_path = packet ["map"]
-	with open (the_map_path, 'r') as FP:
-		ventures_map_bracket = json.load (FP)
-
 	rich.print_json (data = {
 		"play": "turn off",
 		"venture": venture,
 		"ventures_map_bracket": ventures_map_bracket,
 		"name": name
 	})
```

### Comparing `ventures-1.3.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 01:13:12 2024 UTC, .py size: 2226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-00000000: 6f0d 0d0a 0000 0000 a846 4d66 b208 0000  o........FMf....
+00000000: 6f0d 0d0a 0000 0000 3848 4d66 de08 0000  o.......8HMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c08 5a08 6400 6405 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6405 6c0a 5a0a 6400 6405 6c0b 5a0b 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6405 6c0c 5a0c 6406 6407 8400 5a0d 6405  d.l.Z.d.d...Z.d.
-00000090: 5300 2908 e900 0000 0029 01da 0865 7463  S.)......)...etc
-000000a0: 685f 6d61 7029 01da 0873 6361 6e5f 6d61  h_map)...scan_ma
-000000b0: 7029 01da 0c66 696e 645f 7665 6e74 7572  p)...find_ventur
-000000c0: 6529 01da 0b63 6865 636b 5f69 735f 6f6e  e)...check_is_on
-000000d0: 4e63 0100 0000 0000 0000 0000 0000 0b00  Nc..............
-000000e0: 0000 0800 0000 4300 0000 73d6 0100 007c  ......C...s....|
-000000f0: 0064 0119 007d 017c 0164 0219 0064 0319  .d...}.|.d...d..
-00000100: 007d 027c 0164 0419 007d 037c 0164 0519  .}.|.d...}.|.d..
-00000110: 007d 0474 0064 067c 0183 0201 007c 0064  .}.t.d.|.....|.d
-00000120: 0719 007d 0574 017c 0564 0883 028f 0d7d  ...}.t.|.d.....}
-00000130: 0674 02a0 037c 06a1 017d 0757 0064 0004  .t...|...}.W.d..
-00000140: 0004 0083 0301 006e 0831 0073 3077 0101  .......n.1.s0w..
-00000150: 0001 0001 0059 0001 0074 046a 0564 097c  .....Y...t.j.d.|
-00000160: 017c 077c 0464 0a9c 0464 0b8d 0101 007c  .|.|.d...d.....|
-00000170: 077c 0419 007d 017c 0364 0c6b 0272 a17c  .|...}.|.d.k.r.|
-00000180: 0164 0c19 0064 0d6b 0372 a17c 0164 0c19  .d...d.k.r.|.d..
-00000190: 007d 0874 046a 0564 0974 067c 0883 0164  .}.t.j.d.t.|...d
-000001a0: 0e9c 0264 0b8d 0101 0074 067c 0883 0164  ...d.....t.|...d
-000001b0: 0f6b 0372 a174 07a0 087c 0874 096a 0aa1  .k.r.t...|.t.j..
-000001c0: 0201 0064 0d7c 077c 0419 0064 0c3c 0064  ...d.|.|...d.<.d
-000001d0: 107d 0909 0074 067c 0883 017d 0a74 046a  .}...t.|...}.t.j
-000001e0: 0564 097c 047c 0a64 129c 0264 139c 0264  .d.|.|.d...d...d
-000001f0: 0b8d 0101 007c 0a64 0f6b 0272 886e 1974  .....|.d.k.r.n.t
-00000200: 0ba0 0c64 14a1 0101 007c 0964 1437 007d  ...d.....|.d.7.}
-00000210: 097c 0964 156b 0272 a074 0d64 167c 099b  .|.d.k.r.t.d.|..
-00000220: 0064 177c 049b 0064 189d 0583 0182 0171  .d.|...d.......q
-00000230: 737c 0364 196b 0272 e77c 0164 1a19 0083  s|.d.k.r.|.d....
-00000240: 0064 0f6b 0372 e97c 0164 0919 0083 0001  .d.k.r.|.d......
-00000250: 0064 107d 0909 007c 0164 1a19 0083 007d  .d.}...|.d.....}
-00000260: 0a74 046a 0564 1b64 1c7c 097c 0164 0519  .t.j.d.d.|.|.d..
-00000270: 007c 0a64 1d9c 0469 0164 0b8d 0101 007c  .|.d...i.d.....|
-00000280: 0a64 0f6b 0272 ce64 0053 0074 0ba0 0c64  .d.k.r.d.S.t...d
-00000290: 14a1 0101 007c 0964 1437 007d 097c 0964  .....|.d.7.}.|.d
-000002a0: 156b 0272 e674 0d64 167c 099b 0064 177c  .k.r.t.d.|...d.|
-000002b0: 049b 0064 189d 0583 0182 0171 b464 0053  ...d.......q.d.S
-000002c0: 0064 0053 0029 1e4e da07 7665 6e74 7572  .d.S.).N..ventur
-000002d0: 657a 0774 7572 6e20 6f6e da09 6164 7665  ez.turn on..adve
-000002e0: 6e74 7572 65da 046b 696e 64da 046e 616d  nture..kind..nam
-000002f0: 657a 0876 656e 7475 7265 3ada 036d 6170  ez.venture:..map
-00000300: da01 727a 0874 7572 6e20 6f66 6629 04da  ..rz.turn off)..
-00000310: 0470 6c61 7972 0600 0000 da14 7665 6e74  .playr......vent
-00000320: 7572 6573 5f6d 6170 5f62 7261 636b 6574  ures_map_bracket
-00000330: 7209 0000 0029 01da 0464 6174 61da 1070  r....)...data..p
-00000340: 726f 6365 7373 5f69 6465 6e74 6974 79da  rocess_identity.
-00000350: 0029 0272 0c00 0000 720f 0000 00da 036f  .).r....r......o
-00000360: 6666 7201 0000 0054 2902 7209 0000 00da  ffr....T).r.....
-00000370: 0673 7461 7475 7329 0272 0c00 0000 7a12  .status).r....z.
-00000380: 7374 6174 7573 2063 6865 636b 2063 7963  status check cyc
-00000390: 6c65 e901 0000 00e9 0a00 0000 7a06 4166  le..........z.Af
-000003a0: 7465 7220 7a08 206c 6f6f 7073 2c20 7a12  ter z. loops, z.
-000003b0: 2064 6964 206e 6f74 2074 7572 6e20 6f66   did not turn of
-000003c0: 662e da04 7461 736b 7a05 6973 206f 6e7a  f...taskz.is onz
-000003d0: 1976 656e 7475 7265 2073 7461 7475 7320  .venture status 
-000003e0: 6368 6563 6b20 6c6f 6f70 7a17 6166 7465  check loopz.afte
-000003f0: 7220 7475 726e 206f 6666 2077 6173 2073  r turn off was s
-00000400: 656e 7429 04da 0477 6865 6eda 046c 6f6f  ent)...when..loo
-00000410: 7072 0900 0000 7212 0000 0029 0eda 0570  pr....r....)...p
-00000420: 7269 6e74 da04 6f70 656e da04 6a73 6f6e  rint..open..json
-00000430: da04 6c6f 6164 da04 7269 6368 da0a 7072  ..load..rich..pr
-00000440: 696e 745f 6a73 6f6e 7205 0000 00da 026f  int_jsonr......o
-00000450: 73da 046b 696c 6cda 0673 6967 6e61 6cda  s..kill..signal.
-00000460: 0753 4947 5445 524d da04 7469 6d65 da05  .SIGTERM..time..
-00000470: 736c 6565 70da 0945 7863 6570 7469 6f6e  sleep..Exception
-00000480: 290b da06 7061 636b 6574 7206 0000 00da  )...packetr.....
-00000490: 1061 6476 656e 7475 7265 5f73 6372 6970  .adventure_scrip
-000004a0: 7472 0800 0000 7209 0000 00da 0c74 6865  tr....r......the
-000004b0: 5f6d 6170 5f70 6174 68da 0246 5072 0d00  _map_path..FPr..
-000004c0: 0000 720f 0000 0072 1700 0000 7212 0000  ..r....r....r...
-000004d0: 00a9 0072 2900 0000 fa42 2f68 6162 6974  ...r)....B/habit
-000004e0: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
-000004f0: 2f76 656e 7475 7265 732f 706c 6179 735f  /ventures/plays_
-00000500: 7665 6e74 7572 652f 7475 726e 5f6f 6666  venture/turn_off
-00000510: 2f5f 5f69 6e69 745f 5f2e 7079 da10 7475  /__init__.py..tu
-00000520: 726e 5f6f 6666 5f76 656e 7475 7265 1500  rn_off_venture..
-00000530: 0000 738a 0000 0008 010c 0208 0108 010a  ..s.............
-00000540: 0208 020c 010c 011c ff04 0302 0102 0102  ................
-00000550: 0102 010a fc08 0708 020c 0108 0104 0202  ................
-00000560: 0106 010a fe0c 050e 010c 0104 0302 0108  ................
-00000570: 0104 0102 0102 0202 0104 fe0a fe08 0802  ................
-00000580: 010a 0208 0208 0102 0110 0104 ff02 ef08  ................
-00000590: 160e 010a 0104 0202 010a 0104 0202 0102  ................
-000005a0: 0102 0106 0102 0104 fc08 ff08 0904 010a  ................
-000005b0: 0208 0208 0102 0110 0104 ff02 ed04 fb04  ................
-000005c0: 0172 2b00 0000 290e da1b 7665 6e74 7572  .r+...)...ventur
-000005d0: 6573 2e75 7469 6c69 7469 6573 2e6d 6170  es.utilities.map
-000005e0: 2e65 7463 6872 0200 0000 da1b 7665 6e74  .etchr......vent
-000005f0: 7572 6573 2e75 7469 6c69 7469 6573 2e6d  ures.utilities.m
-00000600: 6170 2e73 6361 6e72 0300 0000 da28 7665  ap.scanr.....(ve
-00000610: 6e74 7572 6573 2e75 7469 6c69 7469 6573  ntures.utilities
-00000620: 2e76 656e 7475 7265 732e 6669 6e64 5f76  .ventures.find_v
-00000630: 656e 7475 7265 7204 0000 00da 2676 656e  enturer.....&ven
-00000640: 7475 7265 732e 7574 696c 6974 6965 732e  tures.utilities.
-00000650: 7072 6f63 6573 732e 6368 6563 6b5f 6973  process.check_is
-00000660: 5f6f 6e72 0500 0000 721c 0000 0072 1a00  _onr....r....r..
-00000670: 0000 7220 0000 0072 1e00 0000 7222 0000  ..r ...r....r"..
-00000680: 0072 2b00 0000 7229 0000 0072 2900 0000  .r+...r)...r)...
-00000690: 7229 0000 0072 2a00 0000 da08 3c6d 6f64  r)...r*.....<mod
-000006a0: 756c 653e 0100 0000 7314 0000 000c 040c  ule>....s.......
-000006b0: 010c 010c 0108 0308 0308 0108 0108 010c  ................
-000006c0: 04                                       .
+00000020: 0002 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 6401 6406 6c09 5a09 6401 6406 6c0a  ..d.d.l.Z.d.d.l.
+00000070: 5a0a 6401 6406 6c0b 5a0b 6401 6406 6c0c  Z.d.d.l.Z.d.d.l.
+00000080: 5a0c 6401 6406 6c0d 5a0d 6407 6408 8400  Z.d.d.l.Z.d.d...
+00000090: 5a0e 6406 5300 2909 7a90 0a09 7475 726e  Z.d.S.).z...turn
+000000a0: 5f6f 6666 5f76 656e 7475 7265 2028 7b0a  _off_venture ({.
+000000b0: 0909 2276 656e 7475 7265 223a 207b 0a09  .."venture": {..
+000000c0: 0909 226b 696e 6422 3a20 2222 2c0a 0909  .."kind": "",...
+000000d0: 0922 6e61 6d65 223a 2022 222c 0a09 0909  ."name": "",....
+000000e0: 2274 7572 6e20 6f6e 223a 207b 0a09 0909  "turn on": {....
+000000f0: 0922 6164 7665 6e74 7572 6522 3a20 2222  ."adventure": ""
+00000100: 0a09 0909 7d0a 0909 7d2c 0a09 0922 7665  ....}...},..."ve
+00000110: 6e74 7572 6573 5f6d 6170 5f62 7261 636b  ntures_map_brack
+00000120: 6574 223a 200a 097d 290a e900 0000 0029  et": ..})......)
+00000130: 01da 0865 7463 685f 6d61 7029 01da 0873  ...etch_map)...s
+00000140: 6361 6e5f 6d61 7029 01da 0c66 696e 645f  can_map)...find_
+00000150: 7665 6e74 7572 6529 01da 0b63 6865 636b  venture)...check
+00000160: 5f69 735f 6f6e 4e63 0100 0000 0000 0000  _is_onNc........
+00000170: 0000 0000 0800 0000 0700 0000 4300 0000  ............C...
+00000180: 7396 0100 007c 0064 0119 007d 017c 0064  s....|.d...}.|.d
+00000190: 0219 007d 027c 0164 0319 007d 037c 0164  ...}.|.d...}.|.d
+000001a0: 0419 007d 0474 0064 057c 0183 0201 0074  ...}.t.d.|.....t
+000001b0: 016a 0264 067c 017c 027c 0464 079c 0464  .j.d.|.|.|.d...d
+000001c0: 088d 0101 007c 027c 0419 007d 017c 0364  .....|.|...}.|.d
+000001d0: 096b 0272 817c 0164 0919 0064 0a6b 0372  .k.r.|.d...d.k.r
+000001e0: 817c 0164 0919 007d 0574 016a 0264 0674  .|.d...}.t.j.d.t
+000001f0: 037c 0583 0164 0b9c 0264 088d 0101 0074  .|...d...d.....t
+00000200: 037c 0583 0164 0c6b 0372 8174 04a0 057c  .|...d.k.r.t...|
+00000210: 0574 066a 07a1 0201 0064 0a7c 027c 0419  .t.j.....d.|.|..
+00000220: 0064 093c 0064 0d7d 0609 0074 037c 0583  .d.<.d.}...t.|..
+00000230: 017d 0774 016a 0264 067c 047c 0764 0f9c  .}.t.j.d.|.|.d..
+00000240: 0264 109c 0264 088d 0101 007c 0764 0c6b  .d...d.....|.d.k
+00000250: 0272 686e 1974 08a0 0964 11a1 0101 007c  .rhn.t...d.....|
+00000260: 0664 1137 007d 067c 0664 126b 0272 8074  .d.7.}.|.d.k.r.t
+00000270: 0a64 137c 069b 0064 147c 049b 0064 159d  .d.|...d.|...d..
+00000280: 0583 0182 0171 537c 0364 166b 0272 c77c  .....qS|.d.k.r.|
+00000290: 0164 1719 0083 0064 0c6b 0372 c97c 0164  .d.....d.k.r.|.d
+000002a0: 0619 0083 0001 0064 0d7d 0609 007c 0164  .......d.}...|.d
+000002b0: 1719 0083 007d 0774 016a 0264 1864 197c  .....}.t.j.d.d.|
+000002c0: 067c 0164 0419 007c 0764 1a9c 0469 0164  .|.d...|.d...i.d
+000002d0: 088d 0101 007c 0764 0c6b 0272 ae64 0053  .....|.d.k.r.d.S
+000002e0: 0074 08a0 0964 11a1 0101 007c 0664 1137  .t...d.....|.d.7
+000002f0: 007d 067c 0664 126b 0272 c674 0a64 137c  .}.|.d.k.r.t.d.|
+00000300: 069b 0064 147c 049b 0064 159d 0583 0182  ...d.|...d......
+00000310: 0171 9464 0053 0064 0053 0029 1b4e da07  .q.d.S.d.S.).N..
+00000320: 7665 6e74 7572 65da 1476 656e 7475 7265  venture..venture
+00000330: 735f 6d61 705f 6272 6163 6b65 74da 046b  s_map_bracket..k
+00000340: 696e 64da 046e 616d 657a 0876 656e 7475  ind..namez.ventu
+00000350: 7265 3a7a 0874 7572 6e20 6f66 6629 04da  re:z.turn off)..
+00000360: 0470 6c61 7972 0600 0000 7207 0000 0072  .playr....r....r
+00000370: 0900 0000 2901 da04 6461 7461 da10 7072  ....)...data..pr
+00000380: 6f63 6573 735f 6964 656e 7469 7479 da00  ocess_identity..
+00000390: 2902 720a 0000 0072 0c00 0000 da03 6f66  ).r....r......of
+000003a0: 6672 0100 0000 5429 0272 0900 0000 da06  fr....T).r......
+000003b0: 7374 6174 7573 2902 720a 0000 007a 1273  status).r....z.s
+000003c0: 7461 7475 7320 6368 6563 6b20 6379 636c  tatus check cycl
+000003d0: 65e9 0100 0000 e90a 0000 007a 0641 6674  e..........z.Aft
+000003e0: 6572 207a 0820 6c6f 6f70 732c 207a 1220  er z. loops, z. 
+000003f0: 6469 6420 6e6f 7420 7475 726e 206f 6666  did not turn off
+00000400: 2eda 0474 6173 6b7a 0569 7320 6f6e 7a19  ...taskz.is onz.
+00000410: 7665 6e74 7572 6520 7374 6174 7573 2063  venture status c
+00000420: 6865 636b 206c 6f6f 707a 1761 6674 6572  heck loopz.after
+00000430: 2074 7572 6e20 6f66 6620 7761 7320 7365   turn off was se
+00000440: 6e74 2904 da04 7768 656e da04 6c6f 6f70  nt)...when..loop
+00000450: 7209 0000 0072 0f00 0000 290b da05 7072  r....r....)...pr
+00000460: 696e 74da 0472 6963 68da 0a70 7269 6e74  int..rich..print
+00000470: 5f6a 736f 6e72 0500 0000 da02 6f73 da04  _jsonr......os..
+00000480: 6b69 6c6c da06 7369 676e 616c da07 5349  kill..signal..SI
+00000490: 4754 4552 4dda 0474 696d 65da 0573 6c65  GTERM..time..sle
+000004a0: 6570 da09 4578 6365 7074 696f 6e29 08da  ep..Exception)..
+000004b0: 0670 6163 6b65 7472 0600 0000 7207 0000  .packetr....r...
+000004c0: 0072 0800 0000 7209 0000 0072 0c00 0000  .r....r....r....
+000004d0: 7214 0000 0072 0f00 0000 a900 7220 0000  r....r......r ..
+000004e0: 00fa 422f 6861 6269 7461 742f 7665 6e75  ..B/habitat/venu
+000004f0: 6573 2f73 7461 6765 732f 7665 6e74 7572  es/stages/ventur
+00000500: 6573 2f70 6c61 7973 5f76 656e 7475 7265  es/plays_venture
+00000510: 2f74 7572 6e5f 6f66 662f 5f5f 696e 6974  /turn_off/__init
+00000520: 5f5f 2e70 79da 1074 7572 6e5f 6f66 665f  __.py..turn_off_
+00000530: 7665 6e74 7572 6522 0000 0073 8200 0000  venture"...s....
+00000540: 0801 0801 0802 0801 0a02 0402 0201 0201  ................
+00000550: 0201 0201 0afc 0807 0802 0c01 0801 0402  ................
+00000560: 0201 0601 0afe 0c05 0e01 0c01 0403 0201  ................
+00000570: 0801 0401 0201 0202 0201 04fe 0afe 0808  ................
+00000580: 0201 0a02 0802 0801 0201 1001 04ff 02ef  ................
+00000590: 0816 0e01 0a01 0402 0201 0a01 0402 0201  ................
+000005a0: 0201 0201 0601 0201 04fc 08ff 0809 0401  ................
+000005b0: 0a02 0802 0801 0201 1001 04ff 02ed 04fb  ................
+000005c0: 0401 7222 0000 0029 0fda 075f 5f64 6f63  ..r"...)...__doc
+000005d0: 5f5f da1b 7665 6e74 7572 6573 2e75 7469  __..ventures.uti
+000005e0: 6c69 7469 6573 2e6d 6170 2e65 7463 6872  lities.map.etchr
+000005f0: 0200 0000 da1b 7665 6e74 7572 6573 2e75  ......ventures.u
+00000600: 7469 6c69 7469 6573 2e6d 6170 2e73 6361  tilities.map.sca
+00000610: 6e72 0300 0000 da28 7665 6e74 7572 6573  nr.....(ventures
+00000620: 2e75 7469 6c69 7469 6573 2e76 656e 7475  .utilities.ventu
+00000630: 7265 732e 6669 6e64 5f76 656e 7475 7265  res.find_venture
+00000640: 7204 0000 00da 2676 656e 7475 7265 732e  r.....&ventures.
+00000650: 7574 696c 6974 6965 732e 7072 6f63 6573  utilities.proces
+00000660: 732e 6368 6563 6b5f 6973 5f6f 6e72 0500  s.check_is_onr..
+00000670: 0000 7216 0000 00da 046a 736f 6e72 1a00  ..r......jsonr..
+00000680: 0000 7218 0000 0072 1c00 0000 7222 0000  ..r....r....r"..
+00000690: 0072 2000 0000 7220 0000 0072 2000 0000  .r ...r ...r ...
+000006a0: 7221 0000 00da 083c 6d6f 6475 6c65 3e01  r!.....<module>.
+000006b0: 0000 0073 1600 0000 0401 0c10 0c01 0c01  ...s............
+000006c0: 0c01 0803 0803 0801 0801 0801 0c04       ..............
```

### Comparing `ventures-1.3.0/venues/stages/ventures/plays_venture/turn_on/__init__.py` & `ventures-1.3.1/venues/stages/ventures/plays/turn_off.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,116 @@
 
 
-'''
-	turn_on_venture ({
-		"venture": {
-			"kind": "",
-			"name": "",
-			"turn on": {
-				"adventure": ""
-			}
-		},
-		"ventures_map_bracket": 
+''''
+	turn_off ({
+		
 	})
-'''
+	
+"'''
+
 
 #++++
 #
-from ventures.utilities.map.scan import scan_map
-from ventures.utilities.map.etch import etch_map
-from ventures.utilities.process.check_is_on import check_is_on
-from ventures.utilities.hike_passive import hike_passive
-#
-from ventures.utilities.ventures.find_venture import find_venture
+from ..utilities.map.etch import etch_map
+from ..utilities.map.scan import scan_map	
+from ..utilities.ventures.find_venture import find_venture
+from ..utilities.process.check_is_on import check_is_on
 #
 #
 import rich
 #
 #
+import json
+import signal
 import os
 import time
 #
 #++++
-	
-def turn_on_venture (packet):
-	venture = packet ["venture"]
 
-	adventure_script = venture ["turn on"] ["adventure"]
-	kind = venture ["kind"]
-	name = venture ["name"]
-	
-	ventures_map_bracket = packet ["ventures_map_bracket"]
-	
-	#
-	#	check if is already on	
-	#
-	#
-	if (name in ventures_map_bracket):
-		if (kind == "process_identity"):
-			if (ventures_map_bracket [ name ] ["process_identity"] != ""):
-				status = check_is_on (ventures_map_bracket [ name ] ["process_identity"])
-				if (status == "on"):
-					#print (f'"{ name }" is already on')
-					return;
-		
-		if (kind == "task"):
-			#venture = find_venture (ventures, name)
-			status = venture ["is on"] ()
-			if (status == "on"):
-				return;
 
+def turn_off (packet):
+	ventures_map_bracket = packet ["ventures_map_bracket"]
+	ventures = packet ["ventures"]
 	
-	
-	if (kind == "process_identity"):
-		print ("venture:", venture)
-	
-		Popen_keys = {}
-		if ("turn on" in venture):
-			if ("Popen" in venture ["turn on"]):
-				if (type (venture ["turn on"] ["Popen"]) == dict):
-					Popen_keys = venture ["turn on"] ["Popen"]
-	
-		process = hike_passive ({
-			"script": adventure_script,
-			"Popen": Popen_keys
+	to_delete = []
+	for name in ventures_map_bracket:
+		adventure = ventures_map_bracket [ name ]
+		kind = adventure ["kind"]
+		
+		rich.print_json (data = {
+			"play": "turn off",
+			"adventure": adventure
 		})
-		
-		loop = 0
-		while True:
-			status = check_is_on (process ["process_identity"])	
-			rich.print_json (data = {
-				"venture status check loop": {
-					"when": "after turn on was sent",
-					"loop": loop,
-					"name": name,
-					"status": status
-				}
-			})
+
+
+		if (kind == "process_identity"):
+			if (adventure ["process_identity"] != ""):
+				process_identity = adventure ["process_identity"]
 			
-			if (status == "on"):
-				break;
+				rich.print_json (data = {
+					"play": "turn off",
+					"process_identity": check_is_on (process_identity)
+				})
+					
+				if (check_is_on (process_identity) != "off"):
+					os.kill (process_identity, signal.SIGTERM)
+					ventures_map_bracket [ name ] ["process_identity"] = ""
+					
+					#to_delete.append (name)
+					loop = 0
+					while True:
+						status = check_is_on (process_identity)	
+						rich.print_json (data = {
+							"play": "turn off",
+							"status check cycle": {
+								"name": name,
+								"status": status
+							}
+						})
+						
+						if (status == "off"):
+							break;
+						
+						time.sleep (1)
+
+						loop += 1
+						if (loop == 10):
+							raise Exception (
+								f"After { loop } loops, { name } did not turn off."
+							)
+					
 			
-			time.sleep (1)
-
-			loop += 1
-			if (loop == 10):
-				raise Exception (
-					f"After { loop } loops, { name } did not turn on."
-				)
+		if (kind == "task"):
+			venture = find_venture (ventures, name)
+			
+			if (venture ["is on"] () != "off"):			
+				venture ["turn off"] ()
+				
+				loop = 0
+				while True:
+					status = venture ["is on"] ()		
+
+					rich.print_json (data = {
+						"venture status check loop": {
+							"when": "after turn off was sent",
+							"loop": loop,
+							"name": venture ["name"],
+							"status": status
+						}
+					})
+					
+					if (status == "off"):
+						break;
+					
+					time.sleep (1)
+
+					loop += 1
+					if (loop == 10):
+						raise Exception (
+							f"After { loop } loops, { name } did not turn off."
+						)
+				
+	#for name in to_delete:
+	#	del ventures_map_bracket [ name ]
 	
-		ventures_map_bracket [ name ] = {
-			"kind": kind,
-			"process_identity": process ["process_identity"]
-		}
 	
-		
-		
-	elif (kind == "task"):
-		adventure_script ()
-		
-		loop = 0
-		while True:
-			status = venture ["is on"] ()		
-			rich.print_json (data = {
-				"venture status check loop": {
-					"when": "after turn on was sent",
-					"loop": loop,
-					"name": name,
-					"status": status
-				}
-			})
-			
-			if (status == "on"):
-				break;
-			
-			time.sleep (1)
-
-			loop += 1
-			if (loop == 10):
-				raise Exception (
-					f"After { loop } loops, { name } did not turn on."
-				)
-		
-		ventures_map_bracket [ name ] = {
-			"kind": kind
-		}
-		
-	else:
-		raise Exception (f'Kind "{ kind } was not found.')
-		
-		
-	return 	{
-		"ventures_map_bracket": ventures_map_bracket
-	}
-		
+
```

### Comparing `ventures-1.3.0/venues/stages/ventures/readme.md` & `ventures-1.3.1/venues/stages/ventures/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 		
 ## obtain
 ```
 pip install ventures
 ```
 
 ## tutorial
+
+```
+ventures_map_1.py
+```
 ```
 import os
 import pathlib
 from os.path import dirname, join, normpath
 import sys
 import time
```

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.3.1/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.3.1/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.3.1/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.3.1/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.0/PKG-INFO` & `ventures-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.3.0
+Version: 1.3.1
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -47,14 +47,18 @@
 		
 ## obtain
 ```
 pip install ventures
 ```
 
 ## tutorial
+
+```
+ventures_map_1.py
+```
 ```
 import os
 import pathlib
 from os.path import dirname, join, normpath
 import sys
 import time
```

