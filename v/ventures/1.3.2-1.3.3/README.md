# Comparing `tmp/ventures-1.3.2.tar.gz` & `tmp/ventures-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.3.2.tar", max compression
+gzip compressed data, was "ventures-1.3.3.tar", max compression
```

## Comparing `ventures-1.3.2.tar` & `ventures-1.3.3.tar`

### file list

```diff
@@ -1,100 +1,101 @@
--rwxr-xr-x   0        0        0      585 2024-05-22 01:37:11.845326 ventures-1.3.2/pyproject.toml
--rwxr-xr-x   0        0        0     3135 2024-05-22 01:19:34.461653 ventures-1.3.2/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.3.2/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.3.2/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.3.2/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.3.2/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.3.2/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.3.2/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   359693 2024-05-22 01:36:45.865616 ventures-1.3.2/venues/stages/ventures/_status/DB/records.json
--rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-22 01:36:41.897661 ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-22 01:36:42.897650 ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-22 01:36:42.325656 ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.3.2/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.3.2/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
--rwxr-xr-x   0        0        0      184 2024-05-22 01:36:44.909627 ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.3.2/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.3.2/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      984 2024-05-21 22:50:00.483641 ventures-1.3.2/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.3.2/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.3.2/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1055 2024-05-22 01:14:22.929696 ventures-1.3.2/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1024 2024-05-22 01:31:58.024861 ventures-1.3.2/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0      838 2024-05-22 01:28:15.483410 ventures-1.3.2/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1189 2024-05-22 01:14:18.249745 ventures-1.3.2/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.3.2/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0      994 2024-05-22 01:26:13.120834 ventures-1.3.2/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.3.2/venues/stages/ventures/plays/turn_on_v1.py
--rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.3.2/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.3.2/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.3.2/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0     2288 2024-05-22 01:36:34.565743 ventures-1.3.2/venues/stages/ventures/plays_venture/turn_off/__init__.py
--rwxr-xr-x   0        0        0     1690 2024-05-22 01:36:39.645686 ventures-1.3.2/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.3.2/venues/stages/ventures/plays_venture/turn_on/__init__.py
--rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.3.2/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.3.2/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.3.2/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive/__init__.py
--rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.3.2/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.3.2/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.3.2/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.3.2/venues/stages/ventures/utilities/map/scan.py
--rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.3.2/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.3.2/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.3.2/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.3.2/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.3.2/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.3.2/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2024-05-22 01:39:04.240070 ventures-1.3.3/pyproject.toml
+-rwxr-xr-x   0        0        0     3135 2024-05-22 01:19:34.461653 ventures-1.3.3/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.3.3/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.3.3/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.3.3/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.3.3/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.3.3/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.3.3/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   361169 2024-05-22 01:38:55.132171 ventures-1.3.3/venues/stages/ventures/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-22 01:38:51.068217 ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-22 01:38:53.136194 ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-22 01:38:52.244204 ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.3.3/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.3.3/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
+-rwxr-xr-x   0        0        0      184 2024-05-22 01:38:54.144183 ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.3.3/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.3.3/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      984 2024-05-21 22:50:00.483641 ventures-1.3.3/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.3.3/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.3.3/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1055 2024-05-22 01:14:22.929696 ventures-1.3.3/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rw-r--r--   0        0        0      846 2024-05-22 01:38:48.876241 ventures-1.3.3/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      838 2024-05-22 01:28:15.483410 ventures-1.3.3/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1189 2024-05-22 01:14:18.249745 ventures-1.3.3/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0      691 2024-05-22 01:38:30.720444 ventures-1.3.3/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.3.3/venues/stages/ventures/plays/turn_off_v1.py
+-rwxr-xr-x   0        0        0      994 2024-05-22 01:26:13.120834 ventures-1.3.3/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.3.3/venues/stages/ventures/plays/turn_on_v1.py
+-rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.3.3/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.3.3/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.3.3/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0     2136 2024-05-22 01:37:25.861169 ventures-1.3.3/venues/stages/ventures/plays_venture/turn_off/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-22 01:38:48.876241 ventures-1.3.3/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.3.3/venues/stages/ventures/plays_venture/turn_on/__init__.py
+-rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.3.3/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.3.3/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.3.3/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.3.3/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.3.3/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.3.3/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.3.3/venues/stages/ventures/utilities/map/scan.py
+-rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.3.3/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.3.3/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.3.3/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.3.3/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.3.3/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.3.3/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.3.3/PKG-INFO
```

### Comparing `ventures-1.3.2/pyproject.toml` & `ventures-1.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.3.2"
+version = "1.3.3"
 description = ""
 authors = []
 readme = "venues/stages/ventures/readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "GPL-3.0-only"
```

### Comparing `ventures-1.3.2/venues/stages/ventures/__init__.py` & `ventures-1.3.3/venues/stages/ventures/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.3.3/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/DB/records.json` & `ventures-1.3.3/venues/stages/ventures/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'_default'": "{'72': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [5.67000824958086e-07, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'status_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), OrderedDict([('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('elapsed', [5.43994246982038e-07, "*

 * *               "'seconds']), ( […]*

```diff
@@ -11090,14 +11090,149 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "72": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.67000824958086e-07,
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
+                                5.43994246982038e-07,
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
+                                4.14791422199778,
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
+                                3.084309876001498,
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
+                                3.0985858919957536,
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
+                                5.161003872999572,
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

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status.proc.py` & `ventures-1.3.3/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/clique.py` & `ventures-1.3.3/venues/stages/ventures/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 01:31:54 2024 UTC, .py size: 2696 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0a4b 4d66 880a 0000  o........KMf....
+00000000: 6f0d 0d0a 0000 0000 964c 4d66 b302 0000  o........LMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 5a0b 6401 6407 6c0c 5a0c 6401  d.l.Z.d.d.l.Z.d.
@@ -11,54 +11,43 @@
 000000a0: 5300 290a 7a19 270a 0974 7572 6e5f 6f66  S.).z.'..turn_of
 000000b0: 6620 287b 0a09 090a 097d 290a 090a 22e9  f ({.....})...".
 000000c0: 0000 0000 2901 da08 6574 6368 5f6d 6170  ....)...etch_map
 000000d0: 2901 da08 7363 616e 5f6d 6170 2901 da0c  )...scan_map)...
 000000e0: 6669 6e64 5f76 656e 7475 7265 2901 da0b  find_venture)...
 000000f0: 6368 6563 6b5f 6973 5f6f 6e29 01da 1074  check_is_on)...t
 00000100: 7572 6e5f 6f66 665f 7665 6e74 7572 654e  urn_off_ventureN
-00000110: 6301 0000 0000 0000 0000 0000 000b 0000  c...............
-00000120: 0005 0000 0043 0000 0073 4c00 0000 7c00  .....C...sL...|.
-00000130: 6401 1900 7d01 7c00 6402 1900 7d02 6700  d...}.|.d...}.g.
-00000140: 7d03 7c01 4400 5d17 7d04 7c01 7c04 1900  }.|.D.].}.|.|...
-00000150: 7d05 7c05 6403 1900 7d06 7400 7c02 7c04  }.|.d...}.t.|.|.
-00000160: 8302 7d07 0900 7401 7c07 7c01 6404 9c02  ..}...t.|.|.d...
-00000170: 8301 0100 710c 6400 5300 2905 4eda 1476  ....q.d.S.).N..v
-00000180: 656e 7475 7265 735f 6d61 705f 6272 6163  entures_map_brac
-00000190: 6b65 74da 0876 656e 7475 7265 73da 046b  ket..ventures..k
-000001a0: 696e 6429 02da 0776 656e 7475 7265 7207  ind)...venturer.
-000001b0: 0000 0029 0c72 0400 0000 7206 0000 00da  ...).r....r.....
-000001c0: 0472 6963 68da 0a70 7269 6e74 5f6a 736f  .rich..print_jso
-000001d0: 6e72 0500 0000 da02 6f73 da04 6b69 6c6c  nr......os..kill
-000001e0: da06 7369 676e 616c da07 5349 4754 4552  ..signal..SIGTER
-000001f0: 4dda 0474 696d 65da 0573 6c65 6570 da09  M..time..sleep..
-00000200: 4578 6365 7074 696f 6e29 0bda 0670 6163  Exception)...pac
-00000210: 6b65 7472 0700 0000 7208 0000 00da 0974  ketr....r......t
-00000220: 6f5f 6465 6c65 7465 da04 6e61 6d65 da09  o_delete..name..
-00000230: 6164 7665 6e74 7572 6572 0900 0000 720a  adventurer....r.
-00000240: 0000 00da 1070 726f 6365 7373 5f69 6465  .....process_ide
-00000250: 6e74 6974 79da 046c 6f6f 70da 0673 7461  ntity..loop..sta
-00000260: 7475 73a9 0072 1b00 0000 fa31 2f68 6162  tus..r.....1/hab
-00000270: 6974 6174 2f76 656e 7565 732f 7374 6167  itat/venues/stag
-00000280: 6573 2f76 656e 7475 7265 732f 706c 6179  es/ventures/play
-00000290: 732f 7475 726e 5f6f 6666 2e70 79da 0874  s/turn_off.py..t
-000002a0: 7572 6e5f 6f66 6620 0000 0073 1c00 0000  urn_off ...s....
-000002b0: 0801 0801 0402 0801 0801 0801 0a02 0202  ................
-000002c0: 020a 0201 0201 08fe 0205 04eb 721d 0000  ............r...
-000002d0: 0029 11da 075f 5f64 6f63 5f5f da1b 7665  .)...__doc__..ve
-000002e0: 6e74 7572 6573 2e75 7469 6c69 7469 6573  ntures.utilities
-000002f0: 2e6d 6170 2e65 7463 6872 0200 0000 da1b  .map.etchr......
-00000300: 7665 6e74 7572 6573 2e75 7469 6c69 7469  ventures.utiliti
-00000310: 6573 2e6d 6170 2e73 6361 6e72 0300 0000  es.map.scanr....
-00000320: da28 7665 6e74 7572 6573 2e75 7469 6c69  .(ventures.utili
-00000330: 7469 6573 2e76 656e 7475 7265 732e 6669  ties.ventures.fi
-00000340: 6e64 5f76 656e 7475 7265 7204 0000 00da  nd_venturer.....
-00000350: 2676 656e 7475 7265 732e 7574 696c 6974  &ventures.utilit
-00000360: 6965 732e 7072 6f63 6573 732e 6368 6563  ies.process.chec
-00000370: 6b5f 6973 5f6f 6e72 0500 0000 da1f 7665  k_is_onr......ve
-00000380: 6e74 7572 6573 2e70 6c61 7973 5f76 656e  ntures.plays_ven
-00000390: 7475 7265 2e74 7572 6e5f 6f66 6672 0600  ture.turn_offr..
-000003a0: 0000 720b 0000 00da 046a 736f 6e72 0f00  ..r......jsonr..
-000003b0: 0000 720d 0000 0072 1100 0000 721d 0000  ..r....r....r...
-000003c0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
-000003d0: 721c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000003e0: 0000 0073 1800 0000 0402 0c0a 0c01 0c01  ...s............
-000003f0: 0c01 0c02 0803 0803 0801 0801 0801 0c05  ................
+00000110: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00000120: 0005 0000 0043 0000 0073 3200 0000 7c00  .....C...s2...|.
+00000130: 6401 1900 7d01 7c00 6402 1900 7d02 7c01  d...}.|.d...}.|.
+00000140: 4400 5d0c 7d03 7400 7401 7c02 7c03 8302  D.].}.t.t.|.|...
+00000150: 7c01 6403 9c02 8301 0100 710a 6400 5300  |.d.......q.d.S.
+00000160: 2904 4eda 1476 656e 7475 7265 735f 6d61  ).N..ventures_ma
+00000170: 705f 6272 6163 6b65 74da 0876 656e 7475  p_bracket..ventu
+00000180: 7265 7329 02da 0776 656e 7475 7265 7207  res)...venturer.
+00000190: 0000 0029 0272 0600 0000 7204 0000 0029  ...).r....r....)
+000001a0: 04da 0670 6163 6b65 7472 0700 0000 7208  ...packetr....r.
+000001b0: 0000 00da 046e 616d 65a9 0072 0c00 0000  .....name..r....
+000001c0: fa31 2f68 6162 6974 6174 2f76 656e 7565  .1/habitat/venue
+000001d0: 732f 7374 6167 6573 2f76 656e 7475 7265  s/stages/venture
+000001e0: 732f 706c 6179 732f 7475 726e 5f6f 6666  s/plays/turn_off
+000001f0: 2e70 79da 0874 7572 6e5f 6f66 6620 0000  .py..turn_off ..
+00000200: 0073 1000 0000 0801 0801 0802 0201 0801  .s..............
+00000210: 0201 0afe 04ff 720e 0000 0029 11da 075f  ......r....)..._
+00000220: 5f64 6f63 5f5f da1b 7665 6e74 7572 6573  _doc__..ventures
+00000230: 2e75 7469 6c69 7469 6573 2e6d 6170 2e65  .utilities.map.e
+00000240: 7463 6872 0200 0000 da1b 7665 6e74 7572  tchr......ventur
+00000250: 6573 2e75 7469 6c69 7469 6573 2e6d 6170  es.utilities.map
+00000260: 2e73 6361 6e72 0300 0000 da28 7665 6e74  .scanr.....(vent
+00000270: 7572 6573 2e75 7469 6c69 7469 6573 2e76  ures.utilities.v
+00000280: 656e 7475 7265 732e 6669 6e64 5f76 656e  entures.find_ven
+00000290: 7475 7265 7204 0000 00da 2676 656e 7475  turer.....&ventu
+000002a0: 7265 732e 7574 696c 6974 6965 732e 7072  res.utilities.pr
+000002b0: 6f63 6573 732e 6368 6563 6b5f 6973 5f6f  ocess.check_is_o
+000002c0: 6e72 0500 0000 da1f 7665 6e74 7572 6573  nr......ventures
+000002d0: 2e70 6c61 7973 5f76 656e 7475 7265 2e74  .plays_venture.t
+000002e0: 7572 6e5f 6f66 6672 0600 0000 da04 7269  urn_offr......ri
+000002f0: 6368 da04 6a73 6f6e da06 7369 676e 616c  ch..json..signal
+00000300: da02 6f73 da04 7469 6d65 720e 0000 0072  ..os..timer....r
+00000310: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+00000320: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000330: 0073 1800 0000 0402 0c0a 0c01 0c01 0c01  .s..............
+00000340: 0c02 0803 0803 0801 0801 0801 0c05       ..............
```

### Comparing `ventures-1.3.2/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays/is_on.py` & `ventures-1.3.3/venues/stages/ventures/plays/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays/turn_off.py` & `ventures-1.3.3/venues/stages/ventures/plays/turn_off_v1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays/turn_on.py` & `ventures-1.3.3/venues/stages/ventures/plays/turn_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays/turn_on_v1.py` & `ventures-1.3.3/venues/stages/ventures/plays/turn_on_v1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays_venture/turn_off/__init__.py` & `ventures-1.3.3/venues/stages/ventures/plays_venture/turn_off/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,25 +35,15 @@
 	venture = packet ["venture"]
 	ventures_map_bracket = packet ["ventures_map_bracket"]
 
 	kind = venture ["kind"]
 	name = venture ["name"]
 	
 	print ("venture:", venture)
-	
-	'''
-	rich.print_json (data = {
-		"play": "turn off",
-		"venture": venture,
-		"ventures_map_bracket": ventures_map_bracket,
-		"name": name
-	})
-	'''
 
-	
 
 	if (kind == "process_identity"):
 		venture = ventures_map_bracket [ name ]
 		
 		if (venture ["process_identity"] != ""):
 			process_identity = venture ["process_identity"]
```

### Comparing `ventures-1.3.2/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 01:36:34 2024 UTC, .py size: 2288 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 224c 4d66 f008 0000  o......."LMf....
+00000000: 6f0d 0d0a 0000 0000 554c 4d66 5808 0000  o.......ULMfX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 5a09 6401 6406 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 6401 6406 6c0b 5a0b 6401 6406 6c0c  Z.d.d.l.Z.d.d.l.
@@ -18,89 +18,89 @@
 00000110: 6e74 7572 6573 5f6d 6170 5f62 7261 636b  ntures_map_brack
 00000120: 6574 223a 200a 097d 290a e900 0000 0029  et": ..})......)
 00000130: 01da 0865 7463 685f 6d61 7029 01da 0873  ...etch_map)...s
 00000140: 6361 6e5f 6d61 7029 01da 0c66 696e 645f  can_map)...find_
 00000150: 7665 6e74 7572 6529 01da 0b63 6865 636b  venture)...check
 00000160: 5f69 735f 6f6e 4e63 0100 0000 0000 0000  _is_onNc........
 00000170: 0000 0000 0800 0000 0700 0000 4300 0000  ............C...
-00000180: 7382 0100 007c 0064 0119 007d 017c 0064  s....|.d...}.|.d
+00000180: 7380 0100 007c 0064 0119 007d 017c 0064  s....|.d...}.|.d
 00000190: 0219 007d 027c 0164 0319 007d 037c 0164  ...}.|.d...}.|.d
-000001a0: 0419 007d 0474 0064 057c 0183 0201 0009  ...}.t.d.|......
-000001b0: 007c 0364 066b 0272 777c 027c 0419 007d  .|.d.k.rw|.|...}
-000001c0: 017c 0164 0619 0064 076b 0372 777c 0164  .|.d...d.k.rw|.d
-000001d0: 0619 007d 0574 016a 0264 0874 037c 0583  ...}.t.j.d.t.|..
-000001e0: 0164 099c 0264 0a8d 0101 0074 037c 0583  .d...d.....t.|..
-000001f0: 0164 0b6b 0372 7774 04a0 057c 0574 066a  .d.k.rwt...|.t.j
-00000200: 07a1 0201 0064 077c 027c 0419 0064 063c  .....d.|.|...d.<
-00000210: 0064 0c7d 0609 0074 037c 0583 017d 0774  .d.}...t.|...}.t
-00000220: 016a 0264 087c 047c 0764 0e9c 0264 0f9c  .j.d.|.|.d...d..
-00000230: 0264 0a8d 0101 007c 0764 0b6b 0272 5e6e  .d.....|.d.k.r^n
-00000240: 1974 08a0 0964 10a1 0101 007c 0664 1037  .t...d.....|.d.7
-00000250: 007d 067c 0664 116b 0272 7674 0a64 127c  .}.|.d.k.rvt.d.|
-00000260: 069b 0064 137c 049b 0064 149d 0583 0182  ...d.|...d......
-00000270: 0171 497c 0364 156b 0272 bd7c 0164 1619  .qI|.d.k.r.|.d..
-00000280: 0083 0064 0b6b 0372 bf7c 0164 0819 0083  ...d.k.r.|.d....
-00000290: 0001 0064 0c7d 0609 007c 0164 1619 0083  ...d.}...|.d....
-000002a0: 007d 0774 016a 0264 1764 187c 067c 0164  .}.t.j.d.d.|.|.d
-000002b0: 0419 007c 0764 199c 0469 0164 0a8d 0101  ...|.d...i.d....
-000002c0: 007c 0764 0b6b 0272 a464 0053 0074 08a0  .|.d.k.r.d.S.t..
-000002d0: 0964 10a1 0101 007c 0664 1037 007d 067c  .d.....|.d.7.}.|
-000002e0: 0664 116b 0272 bc74 0a64 127c 069b 0064  .d.k.r.t.d.|...d
-000002f0: 137c 049b 0064 149d 0583 0182 0171 8a64  .|...d.......q.d
-00000300: 0053 0064 0053 0029 1a4e da07 7665 6e74  .S.d.S.).N..vent
-00000310: 7572 65da 1476 656e 7475 7265 735f 6d61  ure..ventures_ma
-00000320: 705f 6272 6163 6b65 74da 046b 696e 64da  p_bracket..kind.
-00000330: 046e 616d 657a 0876 656e 7475 7265 3ada  .namez.venture:.
-00000340: 1070 726f 6365 7373 5f69 6465 6e74 6974  .process_identit
-00000350: 79da 007a 0874 7572 6e20 6f66 6629 02da  y..z.turn off)..
-00000360: 0470 6c61 7972 0a00 0000 2901 da04 6461  .playr....)...da
-00000370: 7461 da03 6f66 6672 0100 0000 5429 0272  ta..offr....T).r
-00000380: 0900 0000 da06 7374 6174 7573 2902 720c  ......status).r.
-00000390: 0000 007a 1273 7461 7475 7320 6368 6563  ...z.status chec
-000003a0: 6b20 6379 636c 65e9 0100 0000 e90a 0000  k cycle.........
-000003b0: 007a 0641 6674 6572 207a 0820 6c6f 6f70  .z.After z. loop
-000003c0: 732c 207a 1220 6469 6420 6e6f 7420 7475  s, z. did not tu
-000003d0: 726e 206f 6666 2eda 0474 6173 6b7a 0569  rn off...taskz.i
-000003e0: 7320 6f6e 7a19 7665 6e74 7572 6520 7374  s onz.venture st
-000003f0: 6174 7573 2063 6865 636b 206c 6f6f 707a  atus check loopz
-00000400: 1761 6674 6572 2074 7572 6e20 6f66 6620  .after turn off 
-00000410: 7761 7320 7365 6e74 2904 da04 7768 656e  was sent)...when
-00000420: da04 6c6f 6f70 7209 0000 0072 0f00 0000  ..loopr....r....
-00000430: 290b da05 7072 696e 74da 0472 6963 68da  )...print..rich.
-00000440: 0a70 7269 6e74 5f6a 736f 6e72 0500 0000  .print_jsonr....
-00000450: da02 6f73 da04 6b69 6c6c da06 7369 676e  ..os..kill..sign
-00000460: 616c da07 5349 4754 4552 4dda 0474 696d  al..SIGTERM..tim
-00000470: 65da 0573 6c65 6570 da09 4578 6365 7074  e..sleep..Except
-00000480: 696f 6e29 08da 0670 6163 6b65 7472 0600  ion)...packetr..
-00000490: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
-000004a0: 0072 0a00 0000 7214 0000 0072 0f00 0000  .r....r....r....
-000004b0: a900 7220 0000 00fa 422f 6861 6269 7461  ..r ....B/habita
-000004c0: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
-000004d0: 7665 6e74 7572 6573 2f70 6c61 7973 5f76  ventures/plays_v
-000004e0: 656e 7475 7265 2f74 7572 6e5f 6f66 662f  enture/turn_off/
-000004f0: 5f5f 696e 6974 5f5f 2e70 79da 1074 7572  __init__.py..tur
-00000500: 6e5f 6f66 665f 7665 6e74 7572 6522 0000  n_off_venture"..
-00000510: 0073 7800 0000 0801 0801 0802 0801 0a02  .sx.............
-00000520: 0202 080b 0801 0c02 0801 0402 0201 0601  ................
-00000530: 0afe 0c05 0e01 0c01 0403 0201 0801 0401  ................
-00000540: 0201 0202 0201 04fe 0afe 0808 0201 0a02  ................
-00000550: 0802 0801 0201 1001 04ff 02ef 0816 0e01  ................
-00000560: 0a01 0402 0201 0a01 0402 0201 0201 0201  ................
-00000570: 0601 0201 04fc 08ff 0809 0401 0a02 0802  ................
-00000580: 0801 0201 1001 04ff 02ed 04fb 0401 7222  ..............r"
-00000590: 0000 0029 0fda 075f 5f64 6f63 5f5f da1b  ...)...__doc__..
-000005a0: 7665 6e74 7572 6573 2e75 7469 6c69 7469  ventures.utiliti
-000005b0: 6573 2e6d 6170 2e65 7463 6872 0200 0000  es.map.etchr....
-000005c0: da1b 7665 6e74 7572 6573 2e75 7469 6c69  ..ventures.utili
-000005d0: 7469 6573 2e6d 6170 2e73 6361 6e72 0300  ties.map.scanr..
-000005e0: 0000 da28 7665 6e74 7572 6573 2e75 7469  ...(ventures.uti
-000005f0: 6c69 7469 6573 2e76 656e 7475 7265 732e  lities.ventures.
-00000600: 6669 6e64 5f76 656e 7475 7265 7204 0000  find_venturer...
-00000610: 00da 2676 656e 7475 7265 732e 7574 696c  ..&ventures.util
-00000620: 6974 6965 732e 7072 6f63 6573 732e 6368  ities.process.ch
-00000630: 6563 6b5f 6973 5f6f 6e72 0500 0000 7216  eck_is_onr....r.
-00000640: 0000 00da 046a 736f 6e72 1a00 0000 7218  .....jsonr....r.
-00000650: 0000 0072 1c00 0000 7222 0000 0072 2000  ...r....r"...r .
-00000660: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
-00000670: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000680: 1600 0000 0401 0c10 0c01 0c01 0c01 0803  ................
-00000690: 0803 0801 0801 0801 0c04                 ..........
+000001a0: 0419 007d 0474 0064 057c 0183 0201 007c  ...}.t.d.|.....|
+000001b0: 0364 066b 0272 767c 027c 0419 007d 017c  .d.k.rv|.|...}.|
+000001c0: 0164 0619 0064 076b 0372 767c 0164 0619  .d...d.k.rv|.d..
+000001d0: 007d 0574 016a 0264 0874 037c 0583 0164  .}.t.j.d.t.|...d
+000001e0: 099c 0264 0a8d 0101 0074 037c 0583 0164  ...d.....t.|...d
+000001f0: 0b6b 0372 7674 04a0 057c 0574 066a 07a1  .k.rvt...|.t.j..
+00000200: 0201 0064 077c 027c 0419 0064 063c 0064  ...d.|.|...d.<.d
+00000210: 0c7d 0609 0074 037c 0583 017d 0774 016a  .}...t.|...}.t.j
+00000220: 0264 087c 047c 0764 0e9c 0264 0f9c 0264  .d.|.|.d...d...d
+00000230: 0a8d 0101 007c 0764 0b6b 0272 5d6e 1974  .....|.d.k.r]n.t
+00000240: 08a0 0964 10a1 0101 007c 0664 1037 007d  ...d.....|.d.7.}
+00000250: 067c 0664 116b 0272 7574 0a64 127c 069b  .|.d.k.rut.d.|..
+00000260: 0064 137c 049b 0064 149d 0583 0182 0171  .d.|...d.......q
+00000270: 487c 0364 156b 0272 bc7c 0164 1619 0083  H|.d.k.r.|.d....
+00000280: 0064 0b6b 0372 be7c 0164 0819 0083 0001  .d.k.r.|.d......
+00000290: 0064 0c7d 0609 007c 0164 1619 0083 007d  .d.}...|.d.....}
+000002a0: 0774 016a 0264 1764 187c 067c 0164 0419  .t.j.d.d.|.|.d..
+000002b0: 007c 0764 199c 0469 0164 0a8d 0101 007c  .|.d...i.d.....|
+000002c0: 0764 0b6b 0272 a364 0053 0074 08a0 0964  .d.k.r.d.S.t...d
+000002d0: 10a1 0101 007c 0664 1037 007d 067c 0664  .....|.d.7.}.|.d
+000002e0: 116b 0272 bb74 0a64 127c 069b 0064 137c  .k.r.t.d.|...d.|
+000002f0: 049b 0064 149d 0583 0182 0171 8964 0053  ...d.......q.d.S
+00000300: 0064 0053 0029 1a4e da07 7665 6e74 7572  .d.S.).N..ventur
+00000310: 65da 1476 656e 7475 7265 735f 6d61 705f  e..ventures_map_
+00000320: 6272 6163 6b65 74da 046b 696e 64da 046e  bracket..kind..n
+00000330: 616d 657a 0876 656e 7475 7265 3ada 1070  amez.venture:..p
+00000340: 726f 6365 7373 5f69 6465 6e74 6974 79da  rocess_identity.
+00000350: 007a 0874 7572 6e20 6f66 6629 02da 0470  .z.turn off)...p
+00000360: 6c61 7972 0a00 0000 2901 da04 6461 7461  layr....)...data
+00000370: da03 6f66 6672 0100 0000 5429 0272 0900  ..offr....T).r..
+00000380: 0000 da06 7374 6174 7573 2902 720c 0000  ....status).r...
+00000390: 007a 1273 7461 7475 7320 6368 6563 6b20  .z.status check 
+000003a0: 6379 636c 65e9 0100 0000 e90a 0000 007a  cycle..........z
+000003b0: 0641 6674 6572 207a 0820 6c6f 6f70 732c  .After z. loops,
+000003c0: 207a 1220 6469 6420 6e6f 7420 7475 726e   z. did not turn
+000003d0: 206f 6666 2eda 0474 6173 6b7a 0569 7320   off...taskz.is 
+000003e0: 6f6e 7a19 7665 6e74 7572 6520 7374 6174  onz.venture stat
+000003f0: 7573 2063 6865 636b 206c 6f6f 707a 1761  us check loopz.a
+00000400: 6674 6572 2074 7572 6e20 6f66 6620 7761  fter turn off wa
+00000410: 7320 7365 6e74 2904 da04 7768 656e da04  s sent)...when..
+00000420: 6c6f 6f70 7209 0000 0072 0f00 0000 290b  loopr....r....).
+00000430: da05 7072 696e 74da 0472 6963 68da 0a70  ..print..rich..p
+00000440: 7269 6e74 5f6a 736f 6e72 0500 0000 da02  rint_jsonr......
+00000450: 6f73 da04 6b69 6c6c da06 7369 676e 616c  os..kill..signal
+00000460: da07 5349 4754 4552 4dda 0474 696d 65da  ..SIGTERM..time.
+00000470: 0573 6c65 6570 da09 4578 6365 7074 696f  .sleep..Exceptio
+00000480: 6e29 08da 0670 6163 6b65 7472 0600 0000  n)...packetr....
+00000490: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+000004a0: 0a00 0000 7214 0000 0072 0f00 0000 a900  ....r....r......
+000004b0: 7220 0000 00fa 422f 6861 6269 7461 742f  r ....B/habitat/
+000004c0: 7665 6e75 6573 2f73 7461 6765 732f 7665  venues/stages/ve
+000004d0: 6e74 7572 6573 2f70 6c61 7973 5f76 656e  ntures/plays_ven
+000004e0: 7475 7265 2f74 7572 6e5f 6f66 662f 5f5f  ture/turn_off/__
+000004f0: 696e 6974 5f5f 2e70 79da 1074 7572 6e5f  init__.py..turn_
+00000500: 6f66 665f 7665 6e74 7572 6522 0000 0073  off_venture"...s
+00000510: 7600 0000 0801 0801 0802 0801 0a02 0803  v...............
+00000520: 0801 0c02 0801 0402 0201 0601 0afe 0c05  ................
+00000530: 0e01 0c01 0403 0201 0801 0401 0201 0202  ................
+00000540: 0201 04fe 0afe 0808 0201 0a02 0802 0801  ................
+00000550: 0201 1001 04ff 02ef 0816 0e01 0a01 0402  ................
+00000560: 0201 0a01 0402 0201 0201 0201 0601 0201  ................
+00000570: 04fc 08ff 0809 0401 0a02 0802 0801 0201  ................
+00000580: 1001 04ff 02ed 04fb 0401 7222 0000 0029  ..........r"...)
+00000590: 0fda 075f 5f64 6f63 5f5f da1b 7665 6e74  ...__doc__..vent
+000005a0: 7572 6573 2e75 7469 6c69 7469 6573 2e6d  ures.utilities.m
+000005b0: 6170 2e65 7463 6872 0200 0000 da1b 7665  ap.etchr......ve
+000005c0: 6e74 7572 6573 2e75 7469 6c69 7469 6573  ntures.utilities
+000005d0: 2e6d 6170 2e73 6361 6e72 0300 0000 da28  .map.scanr.....(
+000005e0: 7665 6e74 7572 6573 2e75 7469 6c69 7469  ventures.utiliti
+000005f0: 6573 2e76 656e 7475 7265 732e 6669 6e64  es.ventures.find
+00000600: 5f76 656e 7475 7265 7204 0000 00da 2676  _venturer.....&v
+00000610: 656e 7475 7265 732e 7574 696c 6974 6965  entures.utilitie
+00000620: 732e 7072 6f63 6573 732e 6368 6563 6b5f  s.process.check_
+00000630: 6973 5f6f 6e72 0500 0000 7216 0000 00da  is_onr....r.....
+00000640: 046a 736f 6e72 1a00 0000 7218 0000 0072  .jsonr....r....r
+00000650: 1c00 0000 7222 0000 0072 2000 0000 7220  ....r"...r ...r 
+00000660: 0000 0072 2000 0000 7221 0000 00da 083c  ...r ...r!.....<
+00000670: 6d6f 6475 6c65 3e01 0000 0073 1600 0000  module>....s....
+00000680: 0401 0c10 0c01 0c01 0c01 0803 0803 0801  ................
+00000690: 0801 0801 0c04                           ......
```

### Comparing `ventures-1.3.2/venues/stages/ventures/plays_venture/turn_on/__init__.py` & `ventures-1.3.3/venues/stages/ventures/plays_venture/turn_on/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/readme.md` & `ventures-1.3.3/venues/stages/ventures/readme.md`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.3.3/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.3.3/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.3.3/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.3.3/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.2/PKG-INFO` & `ventures-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.3.2
+Version: 1.3.3
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

