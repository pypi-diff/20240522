# Comparing `tmp/ventures-1.3.1.tar.gz` & `tmp/ventures-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.3.1.tar", max compression
+gzip compressed data, was "ventures-1.3.2.tar", max compression
```

## Comparing `ventures-1.3.1.tar` & `ventures-1.3.2.tar`

### file list

```diff
@@ -1,99 +1,100 @@
--rwxr-xr-x   0        0        0      585 2024-05-22 01:22:56.563168 ventures-1.3.1/pyproject.toml
--rwxr-xr-x   0        0        0     3135 2024-05-22 01:19:34.461653 ventures-1.3.1/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.3.1/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.3.1/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.3.1/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.3.1/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.3.1/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.3.1/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   348357 2024-05-22 01:20:22.701050 ventures-1.3.1/venues/stages/ventures/_status/DB/records.json
--rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-22 01:20:19.661088 ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-22 01:20:21.801061 ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rwxr-xr-x   0        0        0      974 2024-05-22 00:50:05.019739 ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      787 2024-05-22 00:49:57.495796 ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-22 01:20:20.865073 ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.3.1/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.3.1/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
--rwxr-xr-x   0        0        0      184 2024-05-22 01:20:21.837061 ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.3.1/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.3.1/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      984 2024-05-21 22:50:00.483641 ventures-1.3.1/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.3.1/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.3.1/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1055 2024-05-22 01:14:22.929696 ventures-1.3.1/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rw-r--r--   0        0        0     1571 2024-05-22 01:19:56.709374 ventures-1.3.1/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1035 2024-05-22 01:05:13.047374 ventures-1.3.1/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1189 2024-05-22 01:14:18.249745 ventures-1.3.1/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0     2246 2024-05-22 01:18:53.454171 ventures-1.3.1/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     3292 2024-05-22 01:05:07.511430 ventures-1.3.1/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.3.1/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.3.1/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.3.1/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0     2270 2024-05-22 01:19:52.349429 ventures-1.3.1/venues/stages/ventures/plays_venture/turn_off/__init__.py
--rw-r--r--   0        0        0     1742 2024-05-22 01:19:56.709374 ventures-1.3.1/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.3.1/venues/stages/ventures/plays_venture/turn_on/__init__.py
--rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.3.1/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.3.1/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.3.1/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive/__init__.py
--rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.3.1/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.3.1/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.3.1/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.3.1/venues/stages/ventures/utilities/map/scan.py
--rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.3.1/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.3.1/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.3.1/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.3.1/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.3.1/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.3.1/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2024-05-22 01:37:11.845326 ventures-1.3.2/pyproject.toml
+-rwxr-xr-x   0        0        0     3135 2024-05-22 01:19:34.461653 ventures-1.3.2/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.3.2/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.3.2/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.3.2/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.3.2/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.3.2/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.3.2/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   359693 2024-05-22 01:36:45.865616 ventures-1.3.2/venues/stages/ventures/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-22 01:36:41.897661 ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-22 01:36:42.897650 ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-22 01:36:42.325656 ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.3.2/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.3.2/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
+-rwxr-xr-x   0        0        0      184 2024-05-22 01:36:44.909627 ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.3.2/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.3.2/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      984 2024-05-21 22:50:00.483641 ventures-1.3.2/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.3.2/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.3.2/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1055 2024-05-22 01:14:22.929696 ventures-1.3.2/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1024 2024-05-22 01:31:58.024861 ventures-1.3.2/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      838 2024-05-22 01:28:15.483410 ventures-1.3.2/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1189 2024-05-22 01:14:18.249745 ventures-1.3.2/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.3.2/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0      994 2024-05-22 01:26:13.120834 ventures-1.3.2/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.3.2/venues/stages/ventures/plays/turn_on_v1.py
+-rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.3.2/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.3.2/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.3.2/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0     2288 2024-05-22 01:36:34.565743 ventures-1.3.2/venues/stages/ventures/plays_venture/turn_off/__init__.py
+-rwxr-xr-x   0        0        0     1690 2024-05-22 01:36:39.645686 ventures-1.3.2/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.3.2/venues/stages/ventures/plays_venture/turn_on/__init__.py
+-rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.3.2/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.3.2/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.3.2/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.3.2/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.3.2/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.3.2/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.3.2/venues/stages/ventures/utilities/map/scan.py
+-rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.3.2/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.3.2/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.3.2/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.3.2/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.3.2/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.3.2/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.3.2/PKG-INFO
```

### Comparing `ventures-1.3.1/pyproject.toml` & `ventures-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.3.1"
+version = "1.3.2"
 description = ""
 authors = []
 readme = "venues/stages/ventures/readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "GPL-3.0-only"
```

### Comparing `ventures-1.3.1/venues/stages/ventures/__init__.py` & `ventures-1.3.2/venues/stages/ventures/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.3.2/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/DB/records.json` & `ventures-1.3.2/venues/stages/ventures/_status/DB/records.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788732394366197%*

 * *Differences: {"'_default'": "{'69': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [5.440015229396522e-07, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'status_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), OrderedDict([('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('elapsed', [6.059999577701092e-07, "*

 * *               "'seconds']), […]*

```diff
@@ -10492,14 +10492,185 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "69": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('is on')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 47, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 159, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 41, in turn_off",
+                                "    turn_off_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_off/__init__.py\", line 90, in turn_off_venture",
+                                "    if (venture [\"is on\"] () != \"off\"):",
+                                "KeyError: 'is on'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.440015229396522e-07,
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
+                                6.059999577701092e-07,
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
+                                4.189450294004928,
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
+                            "exception": "KeyError('is on')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 47, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 159, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 41, in turn_off",
+                                "    turn_off_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_off/__init__.py\", line 90, in turn_off_venture",
+                                "    if (venture [\"is on\"] () != \"off\"):",
+                                "KeyError: 'is on'"
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
+                            "elapsed": [
+                                3.107390006996866,
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
+                                3.327641372998187,
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
         "7": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
@@ -10547,14 +10718,386 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "70": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('is on')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 86, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 159, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 53, in turn_off",
+                                "    turn_off_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_off/__init__.py\", line 42, in turn_off_venture",
+                                "    print (\"venture is on:\", venture [\"is on\"])",
+                                "KeyError: 'is on'"
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
+                            "exception": "KeyError('is on')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 62, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 159, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 53, in turn_off",
+                                "    turn_off_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_off/__init__.py\", line 42, in turn_off_venture",
+                                "    print (\"venture is on:\", venture [\"is on\"])",
+                                "KeyError: 'is on'"
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
+                            "exception": "KeyError('is on')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 79, in check_1",
+                                "    ventures [\"turn off\"] ({ \"name\": \"quest_1\" })",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 142, in turn_off_move",
+                                "    turn_off_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_off/__init__.py\", line 42, in turn_off_venture",
+                                "    print (\"venture is on:\", venture [\"is on\"])",
+                                "KeyError: 'is on'"
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
+                                7.830021786503494e-07,
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
+                                5.920010153204203e-07,
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
+                            "exception": "KeyError('is on')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 86, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 159, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 53, in turn_off",
+                                "    turn_off_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_off/__init__.py\", line 42, in turn_off_venture",
+                                "    print (\"venture is on:\", venture [\"is on\"])",
+                                "KeyError: 'is on'"
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
+                                2.3690053980026278,
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
+                            "exception": "KeyError('is on')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 62, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 159, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 53, in turn_off",
+                                "    turn_off_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_off/__init__.py\", line 42, in turn_off_venture",
+                                "    print (\"venture is on:\", venture [\"is on\"])",
+                                "KeyError: 'is on'"
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
+                            "exception": "KeyError('is on')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 79, in check_1",
+                                "    ventures [\"turn off\"] ({ \"name\": \"quest_1\" })",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 142, in turn_off_move",
+                                "    turn_off_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_off/__init__.py\", line 42, in turn_off_venture",
+                                "    print (\"venture is on:\", venture [\"is on\"])",
+                                "KeyError: 'is on'"
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
+        "71": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.269976099953055e-07,
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
+                                5.460024112835526e-07,
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
+                                3.155964651006798,
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
+                                2.3692924979986856,
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
+                                3.096976454995456,
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
+                                5.176048295004875,
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
         "8": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 00:49:57 2024 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3541 4d66 1303 0000  o.......5AMf....
+00000000: 6f0d 0d0a 0000 0000 b94a 4d66 1403 0000  o........JMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6403 6c0a  m.Z.m.Z...d.d.l.
 00000070: 5a0a 6401 6403 6c0b 5a0b 6401 6405 6c0c  Z.d.d.l.Z.d.d.l.
```

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 		]
 	})
 	
 	ventures ["turn on"] ()
 	
 	#time.sleep (10)
 
-	response = requests.get("http://0.0.0.0:10000")
+	response = requests.get ("http://0.0.0.0:10000")
 	assert (response.status_code == 404)
 	
 	
 	ventures ["turn off"] ()
 	
 	#time.sleep (10)
```

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status.proc.py` & `ventures-1.3.2/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/clique.py` & `ventures-1.3.2/venues/stages/ventures/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 01:05:07 2024 UTC, .py size: 3292 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-00000000: 6f0d 0d0a 0000 0000 c344 4d66 dc0c 0000  o........DMf....
+00000000: 6f0d 0d0a 0000 0000 0a4b 4d66 880a 0000  o........KMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0b 5a0b 0100 6400 6407 6c0c 5a0c 6400  m.Z...d.d.l.Z.d.
-00000080: 6407 6c0d 5a0d 6400 6407 6c0e 5a0e 0900  d.l.Z.d.d.l.Z...
-00000090: 6408 6409 8400 5a0f 6407 5300 290a e900  d.d...Z.d.S.)...
-000000a0: 0000 0029 01da 0c68 696b 655f 7061 7373  ...)...hike_pass
-000000b0: 6976 6529 01da 0865 7463 685f 6d61 7029  ive)...etch_map)
-000000c0: 01da 0873 6361 6e5f 6d61 7029 01da 0c66  ...scan_map)...f
-000000d0: 696e 645f 7665 6e74 7572 6529 01da 0b63  ind_venture)...c
-000000e0: 6865 636b 5f69 735f 6f6e 2901 da0f 7475  heck_is_on)...tu
-000000f0: 726e 5f6f 6e5f 7665 6e74 7572 654e 6301  rn_on_ventureNc.
-00000100: 0000 0000 0000 0000 0000 000c 0000 0005  ................
-00000110: 0000 0043 0000 0073 4000 0000 7c00 6401  ...C...s@...|.d.
-00000120: 1900 7d01 7c00 6402 1900 7d02 7c01 4400  ..}.|.d...}.|.D.
-00000130: 5d11 7d03 7400 7c03 7c02 6403 9c02 8301  ].}.t.|.|.d.....
-00000140: 0100 7401 6a02 6404 7c02 6901 6405 8d01  ..t.j.d.|.i.d...
-00000150: 0100 710a 6402 7c02 6901 5300 2906 4eda  ..q.d.|.i.S.).N.
-00000160: 0876 656e 7475 7265 73da 1476 656e 7475  .ventures..ventu
-00000170: 7265 735f 6d61 705f 6272 6163 6b65 7429  res_map_bracket)
-00000180: 02da 0776 656e 7475 7265 7209 0000 007a  ...venturer....z
-00000190: 1370 726f 6365 6564 7320 6f66 2074 7572  .proceeds of tur
-000001a0: 6e20 6f6e 2901 da04 6461 7461 290c 7207  n on)...data).r.
-000001b0: 0000 00da 0472 6963 68da 0a70 7269 6e74  .....rich..print
-000001c0: 5f6a 736f 6e72 0600 0000 7205 0000 00da  _jsonr....r.....
-000001d0: 0570 7269 6e74 da04 7479 7065 da04 6469  .print..type..di
-000001e0: 6374 7202 0000 00da 0474 696d 65da 0573  ctr......time..s
-000001f0: 6c65 6570 da09 4578 6365 7074 696f 6e29  leep..Exception)
-00000200: 0cda 0670 6163 6b65 7472 0800 0000 7209  ...packetr....r.
-00000210: 0000 00da 0961 6476 656e 7475 7265 da10  .....adventure..
-00000220: 6164 7665 6e74 7572 655f 7363 7269 7074  adventure_script
-00000230: da04 6b69 6e64 da04 6e61 6d65 da06 7374  ..kind..name..st
-00000240: 6174 7573 720a 0000 00da 0a50 6f70 656e  atusr......Popen
-00000250: 5f6b 6579 73da 0770 726f 6365 7373 da04  _keys..process..
-00000260: 6c6f 6f70 a900 721d 0000 00fa 302f 6861  loop..r.....0/ha
-00000270: 6269 7461 742f 7665 6e75 6573 2f73 7461  bitat/venues/sta
-00000280: 6765 732f 7665 6e74 7572 6573 2f70 6c61  ges/ventures/pla
-00000290: 7973 2f74 7572 6e5f 6f6e 2e70 79da 0774  ys/turn_on.py..t
-000002a0: 7572 6e5f 6f6e 2d00 0000 731a 0000 0008  urn_on-...s.....
-000002b0: 0108 0108 0502 0102 0102 0108 fe04 0504  ................
-000002c0: 0108 ff02 0404 6e04 ff72 1f00 0000 2910  ......n..r....).
-000002d0: da1f 7665 6e74 7572 6573 2e75 7469 6c69  ..ventures.utili
-000002e0: 7469 6573 2e68 696b 655f 7061 7373 6976  ties.hike_passiv
-000002f0: 6572 0200 0000 da1b 7665 6e74 7572 6573  er......ventures
-00000300: 2e75 7469 6c69 7469 6573 2e6d 6170 2e65  .utilities.map.e
-00000310: 7463 6872 0300 0000 da1b 7665 6e74 7572  tchr......ventur
-00000320: 6573 2e75 7469 6c69 7469 6573 2e6d 6170  es.utilities.map
-00000330: 2e73 6361 6e72 0400 0000 da28 7665 6e74  .scanr.....(vent
-00000340: 7572 6573 2e75 7469 6c69 7469 6573 2e76  ures.utilities.v
-00000350: 656e 7475 7265 732e 6669 6e64 5f76 656e  entures.find_ven
-00000360: 7475 7265 7205 0000 00da 2676 656e 7475  turer.....&ventu
-00000370: 7265 732e 7574 696c 6974 6965 732e 7072  res.utilities.pr
-00000380: 6f63 6573 732e 6368 6563 6b5f 6973 5f6f  ocess.check_is_o
-00000390: 6e72 0600 0000 da1e 7665 6e74 7572 6573  nr......ventures
-000003a0: 2e70 6c61 7973 5f76 656e 7475 7265 2e74  .plays_venture.t
-000003b0: 7572 6e5f 6f6e 7207 0000 0072 0c00 0000  urn_onr....r....
-000003c0: da02 6f73 7211 0000 0072 1f00 0000 721d  ..osr....r....r.
-000003d0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-000003e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000003f0: 7316 0000 000c 030c 010c 010c 010c 020c  s...............
-00000400: 0208 0408 0308 0102 040c 16              ...........
+00000020: 0002 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
+00000070: 6407 6c0b 5a0b 6401 6407 6c0c 5a0c 6401  d.l.Z.d.d.l.Z.d.
+00000080: 6407 6c0d 5a0d 6401 6407 6c0e 5a0e 6401  d.l.Z.d.d.l.Z.d.
+00000090: 6407 6c0f 5a0f 6408 6409 8400 5a10 6407  d.l.Z.d.d...Z.d.
+000000a0: 5300 290a 7a19 270a 0974 7572 6e5f 6f66  S.).z.'..turn_of
+000000b0: 6620 287b 0a09 090a 097d 290a 090a 22e9  f ({.....})...".
+000000c0: 0000 0000 2901 da08 6574 6368 5f6d 6170  ....)...etch_map
+000000d0: 2901 da08 7363 616e 5f6d 6170 2901 da0c  )...scan_map)...
+000000e0: 6669 6e64 5f76 656e 7475 7265 2901 da0b  find_venture)...
+000000f0: 6368 6563 6b5f 6973 5f6f 6e29 01da 1074  check_is_on)...t
+00000100: 7572 6e5f 6f66 665f 7665 6e74 7572 654e  urn_off_ventureN
+00000110: 6301 0000 0000 0000 0000 0000 000b 0000  c...............
+00000120: 0005 0000 0043 0000 0073 4c00 0000 7c00  .....C...sL...|.
+00000130: 6401 1900 7d01 7c00 6402 1900 7d02 6700  d...}.|.d...}.g.
+00000140: 7d03 7c01 4400 5d17 7d04 7c01 7c04 1900  }.|.D.].}.|.|...
+00000150: 7d05 7c05 6403 1900 7d06 7400 7c02 7c04  }.|.d...}.t.|.|.
+00000160: 8302 7d07 0900 7401 7c07 7c01 6404 9c02  ..}...t.|.|.d...
+00000170: 8301 0100 710c 6400 5300 2905 4eda 1476  ....q.d.S.).N..v
+00000180: 656e 7475 7265 735f 6d61 705f 6272 6163  entures_map_brac
+00000190: 6b65 74da 0876 656e 7475 7265 73da 046b  ket..ventures..k
+000001a0: 696e 6429 02da 0776 656e 7475 7265 7207  ind)...venturer.
+000001b0: 0000 0029 0c72 0400 0000 7206 0000 00da  ...).r....r.....
+000001c0: 0472 6963 68da 0a70 7269 6e74 5f6a 736f  .rich..print_jso
+000001d0: 6e72 0500 0000 da02 6f73 da04 6b69 6c6c  nr......os..kill
+000001e0: da06 7369 676e 616c da07 5349 4754 4552  ..signal..SIGTER
+000001f0: 4dda 0474 696d 65da 0573 6c65 6570 da09  M..time..sleep..
+00000200: 4578 6365 7074 696f 6e29 0bda 0670 6163  Exception)...pac
+00000210: 6b65 7472 0700 0000 7208 0000 00da 0974  ketr....r......t
+00000220: 6f5f 6465 6c65 7465 da04 6e61 6d65 da09  o_delete..name..
+00000230: 6164 7665 6e74 7572 6572 0900 0000 720a  adventurer....r.
+00000240: 0000 00da 1070 726f 6365 7373 5f69 6465  .....process_ide
+00000250: 6e74 6974 79da 046c 6f6f 70da 0673 7461  ntity..loop..sta
+00000260: 7475 73a9 0072 1b00 0000 fa31 2f68 6162  tus..r.....1/hab
+00000270: 6974 6174 2f76 656e 7565 732f 7374 6167  itat/venues/stag
+00000280: 6573 2f76 656e 7475 7265 732f 706c 6179  es/ventures/play
+00000290: 732f 7475 726e 5f6f 6666 2e70 79da 0874  s/turn_off.py..t
+000002a0: 7572 6e5f 6f66 6620 0000 0073 1c00 0000  urn_off ...s....
+000002b0: 0801 0801 0402 0801 0801 0801 0a02 0202  ................
+000002c0: 020a 0201 0201 08fe 0205 04eb 721d 0000  ............r...
+000002d0: 0029 11da 075f 5f64 6f63 5f5f da1b 7665  .)...__doc__..ve
+000002e0: 6e74 7572 6573 2e75 7469 6c69 7469 6573  ntures.utilities
+000002f0: 2e6d 6170 2e65 7463 6872 0200 0000 da1b  .map.etchr......
+00000300: 7665 6e74 7572 6573 2e75 7469 6c69 7469  ventures.utiliti
+00000310: 6573 2e6d 6170 2e73 6361 6e72 0300 0000  es.map.scanr....
+00000320: da28 7665 6e74 7572 6573 2e75 7469 6c69  .(ventures.utili
+00000330: 7469 6573 2e76 656e 7475 7265 732e 6669  ties.ventures.fi
+00000340: 6e64 5f76 656e 7475 7265 7204 0000 00da  nd_venturer.....
+00000350: 2676 656e 7475 7265 732e 7574 696c 6974  &ventures.utilit
+00000360: 6965 732e 7072 6f63 6573 732e 6368 6563  ies.process.chec
+00000370: 6b5f 6973 5f6f 6e72 0500 0000 da1f 7665  k_is_onr......ve
+00000380: 6e74 7572 6573 2e70 6c61 7973 5f76 656e  ntures.plays_ven
+00000390: 7475 7265 2e74 7572 6e5f 6f66 6672 0600  ture.turn_offr..
+000003a0: 0000 720b 0000 00da 046a 736f 6e72 0f00  ..r......jsonr..
+000003b0: 0000 720d 0000 0072 1100 0000 721d 0000  ..r....r....r...
+000003c0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+000003d0: 721c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000003e0: 0000 0073 1800 0000 0402 0c0a 0c01 0c01  ...s............
+000003f0: 0c01 0c02 0803 0803 0801 0801 0801 0c05  ................
```

### Comparing `ventures-1.3.1/venues/stages/ventures/plays/is_on.py` & `ventures-1.3.2/venues/stages/ventures/plays/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/plays/turn_off.py` & `ventures-1.3.2/venues/stages/ventures/plays_venture/turn_off/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,83 @@
 
-
-''''
-	turn_off ({
-		
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
 	})
-	
-"'''
+'''
 
 
 #++++
 #
-from ..utilities.map.etch import etch_map
-from ..utilities.map.scan import scan_map	
-from ..utilities.ventures.find_venture import find_venture
-from ..utilities.process.check_is_on import check_is_on
+from ventures.utilities.map.etch import etch_map
+from ventures.utilities.map.scan import scan_map	
+from ventures.utilities.ventures.find_venture import find_venture
+from ventures.utilities.process.check_is_on import check_is_on
 #
 #
 import rich
 #
 #
 import json
 import signal
 import os
 import time
 #
 #++++
 
-
-def turn_off (packet):
+def turn_off_venture (packet):
+	venture = packet ["venture"]
 	ventures_map_bracket = packet ["ventures_map_bracket"]
-	ventures = packet ["ventures"]
-	
-	to_delete = []
-	for name in ventures_map_bracket:
-		adventure = ventures_map_bracket [ name ]
-		kind = adventure ["kind"]
-		
-		rich.print_json (data = {
-			"play": "turn off",
-			"adventure": adventure
-		})
 
+	kind = venture ["kind"]
+	name = venture ["name"]
+	
+	print ("venture:", venture)
+	
+	'''
+	rich.print_json (data = {
+		"play": "turn off",
+		"venture": venture,
+		"ventures_map_bracket": ventures_map_bracket,
+		"name": name
+	})
+	'''
 
-		if (kind == "process_identity"):
-			if (adventure ["process_identity"] != ""):
-				process_identity = adventure ["process_identity"]
-			
-				rich.print_json (data = {
-					"play": "turn off",
-					"process_identity": check_is_on (process_identity)
-				})
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
+	
 
-						loop += 1
-						if (loop == 10):
-							raise Exception (
-								f"After { loop } loops, { name } did not turn off."
-							)
-					
-			
-		if (kind == "task"):
-			venture = find_venture (ventures, name)
-			
-			if (venture ["is on"] () != "off"):			
-				venture ["turn off"] ()
+	if (kind == "process_identity"):
+		venture = ventures_map_bracket [ name ]
+		
+		if (venture ["process_identity"] != ""):
+			process_identity = venture ["process_identity"]
+		
+			rich.print_json (data = {
+				"play": "turn off",
+				"process_identity": check_is_on (process_identity)
+			})
+				
+			if (check_is_on (process_identity) != "off"):
+				os.kill (process_identity, signal.SIGTERM)
+				ventures_map_bracket [ name ] ["process_identity"] = ""
 				
+				#to_delete.append (name)
 				loop = 0
 				while True:
-					status = venture ["is on"] ()		
-
+					status = check_is_on (process_identity)	
 					rich.print_json (data = {
-						"venture status check loop": {
-							"when": "after turn off was sent",
-							"loop": loop,
-							"name": venture ["name"],
+						"play": "turn off",
+						"status check cycle": {
+							"name": name,
 							"status": status
 						}
 					})
 					
 					if (status == "off"):
 						break;
 					
@@ -105,12 +85,36 @@
 
 					loop += 1
 					if (loop == 10):
 						raise Exception (
 							f"After { loop } loops, { name } did not turn off."
 						)
 				
-	#for name in to_delete:
-	#	del ventures_map_bracket [ name ]
-	
-	
-	
+		
+	if (kind == "task"):
+		if (venture ["is on"] () != "off"):			
+			venture ["turn off"] ()
+			
+			loop = 0
+			while True:
+				status = venture ["is on"] ()		
+
+				rich.print_json (data = {
+					"venture status check loop": {
+						"when": "after turn off was sent",
+						"loop": loop,
+						"name": venture ["name"],
+						"status": status
+					}
+				})
+				
+				if (status == "off"):
+					break;
+				
+				time.sleep (1)
+
+				loop += 1
+				if (loop == 10):
+					raise Exception (
+						f"After { loop } loops, { name } did not turn off."
+						
+					)
```

### Comparing `ventures-1.3.1/venues/stages/ventures/plays/turn_on.py` & `ventures-1.3.2/venues/stages/ventures/plays/turn_on_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 		
 		rich.print_json (data = {
 			"proceeds of turn on": ventures_map_bracket
 		})
 		
 		continue;
 			
-	
+		'''
 		adventure_script = adventure ["turn on"] ["adventure"]
 		kind = adventure ["kind"]
 		name = adventure ["name"]
 		
 		
 		#
 		#	check if is already on	
@@ -160,15 +160,15 @@
 			ventures_map_bracket [ name ] = {
 				"kind": kind
 			}
 			
 		
 		else:
 			raise Exception (f'Kind "{ kind } was not found.')
-
+		'''
 	
 	
 	
 	return {
 		"ventures_map_bracket": ventures_map_bracket
 	}
```

### Comparing `ventures-1.3.1/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/plays_venture/turn_off/__init__.py` & `ventures-1.3.2/venues/stages/ventures/plays/turn_off.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,127 @@
 
-'''
-	turn_off_venture ({
-		"venture": {
-			"kind": "",
-			"name": "",
-			"turn on": {
-				"adventure": ""
-			}
-		},
-		"ventures_map_bracket": 
+
+''''
+	turn_off ({
+		
 	})
-'''
+	
+"'''
 
 
 #++++
 #
 from ventures.utilities.map.etch import etch_map
 from ventures.utilities.map.scan import scan_map	
 from ventures.utilities.ventures.find_venture import find_venture
 from ventures.utilities.process.check_is_on import check_is_on
 #
+from ventures.plays_venture.turn_off import turn_off_venture
+#
 #
 import rich
 #
 #
 import json
 import signal
 import os
 import time
 #
 #++++
 
-def turn_off_venture (packet):
-	venture = packet ["venture"]
-	ventures_map_bracket = packet ["ventures_map_bracket"]
 
-	kind = venture ["kind"]
-	name = venture ["name"]
+def turn_off (packet):
+	ventures_map_bracket = packet ["ventures_map_bracket"]
+	ventures = packet ["ventures"]
 	
-	print ("venture:", venture)
+	to_delete = []
+	for name in ventures_map_bracket:
+		adventure = ventures_map_bracket [ name ]
+		kind = adventure ["kind"]
 	
-	rich.print_json (data = {
-		"play": "turn off",
-		"venture": venture,
-		"ventures_map_bracket": ventures_map_bracket,
-		"name": name
-	})
+		venture = find_venture (ventures, name)
+		
+		'''
+						"venture": {
+				"kind": kind,
+				"name": name,
+				"turn on": {
+					"adventure": adventure
+				}
+			},
+		'''
+	
+		turn_off_venture ({
+			"venture": venture,
+			"ventures_map_bracket": ventures_map_bracket
+		})
+	
+		continue;
+	
+		adventure = ventures_map_bracket [ name ]
+		kind = adventure ["kind"]
+		
+		rich.print_json (data = {
+			"play": "turn off",
+			"adventure": adventure
+		})
 
-	venture = ventures_map_bracket [name]
 
-	if (kind == "process_identity"):
-		if (venture ["process_identity"] != ""):
-			process_identity = venture ["process_identity"]
-		
-			rich.print_json (data = {
-				"play": "turn off",
-				"process_identity": check_is_on (process_identity)
-			})
-				
-			if (check_is_on (process_identity) != "off"):
-				os.kill (process_identity, signal.SIGTERM)
-				ventures_map_bracket [ name ] ["process_identity"] = ""
+		if (kind == "process_identity"):
+			if (adventure ["process_identity"] != ""):
+				process_identity = adventure ["process_identity"]
+			
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
+			
+		if (kind == "task"):
+			venture = find_venture (ventures, name)
+			
+			if (venture ["is on"] () != "off"):			
+				venture ["turn off"] ()
 				
-				#to_delete.append (name)
 				loop = 0
 				while True:
-					status = check_is_on (process_identity)	
+					status = venture ["is on"] ()		
+
 					rich.print_json (data = {
-						"play": "turn off",
-						"status check cycle": {
-							"name": name,
+						"venture status check loop": {
+							"when": "after turn off was sent",
+							"loop": loop,
+							"name": venture ["name"],
 							"status": status
 						}
 					})
 					
 					if (status == "off"):
 						break;
 					
@@ -81,36 +129,12 @@
 
 					loop += 1
 					if (loop == 10):
 						raise Exception (
 							f"After { loop } loops, { name } did not turn off."
 						)
 				
-		
-	if (kind == "task"):
-		if (venture ["is on"] () != "off"):			
-			venture ["turn off"] ()
-			
-			loop = 0
-			while True:
-				status = venture ["is on"] ()		
-
-				rich.print_json (data = {
-					"venture status check loop": {
-						"when": "after turn off was sent",
-						"loop": loop,
-						"name": venture ["name"],
-						"status": status
-					}
-				})
-				
-				if (status == "off"):
-					break;
-				
-				time.sleep (1)
-
-				loop += 1
-				if (loop == 10):
-					raise Exception (
-						f"After { loop } loops, { name } did not turn off."
-						
-					)
+	#for name in to_delete:
+	#	del ventures_map_bracket [ name ]
+	
+	
+
```

### Comparing `ventures-1.3.1/venues/stages/ventures/plays_venture/turn_on/__init__.py` & `ventures-1.3.2/venues/stages/ventures/plays_venture/turn_on/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/readme.md` & `ventures-1.3.2/venues/stages/ventures/readme.md`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.3.2/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.3.2/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.3.2/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.3.2/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.1/PKG-INFO` & `ventures-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.3.1
+Version: 1.3.2
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

