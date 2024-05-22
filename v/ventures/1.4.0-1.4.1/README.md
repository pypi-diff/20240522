# Comparing `tmp/ventures-1.4.0.tar.gz` & `tmp/ventures-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.4.0.tar", max compression
+gzip compressed data, was "ventures-1.4.1.tar", max compression
```

## Comparing `ventures-1.4.0.tar` & `ventures-1.4.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rwxr-xr-x   0        0        0      585 2024-05-22 02:27:25.345879 ventures-1.4.0/pyproject.toml
--rwxr-xr-x   0        0        0     2988 2024-05-22 01:50:56.204575 ventures-1.4.0/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.4.0/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.4.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.4.0/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.4.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.4.0/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.4.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   380192 2024-05-22 02:26:21.642724 ventures-1.4.0/venues/stages/ventures/_status/DB/records.json
--rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-22 02:26:17.558779 ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-22 02:26:19.614751 ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-22 02:26:18.686763 ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.4.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.4.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
--rwxr-xr-x   0        0        0      184 2024-05-22 02:26:20.654737 ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.4.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.4.0/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0     1450 2024-05-22 01:51:45.688162 ventures-1.4.0/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.4.0/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.4.0/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1043 2024-05-22 02:08:02.966812 ventures-1.4.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      846 2024-05-22 01:38:48.876241 ventures-1.4.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0      838 2024-05-22 01:28:15.483410 ventures-1.4.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1370 2024-05-22 02:07:55.802884 ventures-1.4.0/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0      691 2024-05-22 01:38:30.720444 ventures-1.4.0/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.4.0/venues/stages/ventures/plays/turn_off_v1.py
--rwxr-xr-x   0        0        0      994 2024-05-22 01:26:13.120834 ventures-1.4.0/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.4.0/venues/stages/ventures/plays/turn_on_v1.py
--rwxr-xr-x   0        0        0      940 2024-05-22 02:10:17.449440 ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      924 2024-05-22 02:10:12.141494 ventures-1.4.0/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0     2136 2024-05-22 01:37:25.861169 ventures-1.4.0/venues/stages/ventures/plays_venture/turn_off/__init__.py
--rwxr-xr-x   0        0        0     1686 2024-05-22 01:38:48.876241 ventures-1.4.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.4.0/venues/stages/ventures/plays_venture/turn_on/__init__.py
--rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.4.0/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.4.0/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.4.0/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive/__init__.py
--rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.4.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.4.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.4.0/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.4.0/venues/stages/ventures/utilities/map/scan.py
--rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.4.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.4.0/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.4.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.4.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.4.0/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.4.0/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2024-05-22 02:45:05.641317 ventures-1.4.1/pyproject.toml
+-rwxr-xr-x   0        0        0     2991 2024-05-22 02:44:57.205412 ventures-1.4.1/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.4.1/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.4.1/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.4.1/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.4.1/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.4.1/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.4.1/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   380192 2024-05-22 02:26:21.642724 ventures-1.4.1/venues/stages/ventures/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-22 02:26:17.558779 ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-22 02:26:19.614751 ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-22 02:26:18.686763 ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.4.1/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.4.1/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
+-rwxr-xr-x   0        0        0      184 2024-05-22 02:26:20.654737 ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.4.1/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.4.1/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0     1450 2024-05-22 01:51:45.688162 ventures-1.4.1/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.4.1/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.4.1/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1043 2024-05-22 02:08:02.966812 ventures-1.4.1/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      846 2024-05-22 01:38:48.876241 ventures-1.4.1/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      838 2024-05-22 01:28:15.483410 ventures-1.4.1/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1370 2024-05-22 02:07:55.802884 ventures-1.4.1/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0      691 2024-05-22 01:38:30.720444 ventures-1.4.1/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.4.1/venues/stages/ventures/plays/turn_off_v1.py
+-rwxr-xr-x   0        0        0      994 2024-05-22 01:26:13.120834 ventures-1.4.1/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.4.1/venues/stages/ventures/plays/turn_on_v1.py
+-rwxr-xr-x   0        0        0      940 2024-05-22 02:10:17.449440 ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      924 2024-05-22 02:10:12.141494 ventures-1.4.1/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0     2136 2024-05-22 01:37:25.861169 ventures-1.4.1/venues/stages/ventures/plays_venture/turn_off/__init__.py
+-rwxr-xr-x   0        0        0     1686 2024-05-22 01:38:48.876241 ventures-1.4.1/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.4.1/venues/stages/ventures/plays_venture/turn_on/__init__.py
+-rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.4.1/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.4.1/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.4.1/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.4.1/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.4.1/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.4.1/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.4.1/venues/stages/ventures/utilities/map/scan.py
+-rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.4.1/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.4.1/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.4.1/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.4.1/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.4.1/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.4.1/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.4.1/PKG-INFO
```

### Comparing `ventures-1.4.0/pyproject.toml` & `ventures-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.4.0"
+version = "1.4.1"
 description = ""
 authors = []
 readme = "venues/stages/ventures/readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "GPL-3.0-only"
```

### Comparing `ventures-1.4.0/venues/stages/ventures/__init__.py` & `ventures-1.4.1/venues/stages/ventures/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 	def turn_on_move (packet = {}):
 		print ('turn on move', packet)
 	
 		if (type (packet) == dict and "name" in packet):
 			name = packet ["name"]
 		
 			venture = find_venture (ventures, name)
-			rich.print_json (data = {
-				"venture": venture
-			})
+			#rich.print_json (data = {
+			#	"venture": venture
+			#})
 		
 			the_venture_packet = turn_on_venture ({
 				"venture": venture,
 				"ventures_map_bracket": ventures_map_bracket
 			})
 			
 			etch_map ({
```

### Comparing `ventures-1.4.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.4.1/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/DB/records.json` & `ventures-1.4.1/venues/stages/ventures/_status/DB/records.json`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status.proc.py` & `ventures-1.4.1/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/clique.py` & `ventures-1.4.1/venues/stages/ventures/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays/is_on.py` & `ventures-1.4.1/venues/stages/ventures/plays/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays/turn_off.py` & `ventures-1.4.1/venues/stages/ventures/plays/turn_off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays/turn_off_v1.py` & `ventures-1.4.1/venues/stages/ventures/plays/turn_off_v1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays/turn_on.py` & `ventures-1.4.1/venues/stages/ventures/plays/turn_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays/turn_on_v1.py` & `ventures-1.4.1/venues/stages/ventures/plays/turn_on_v1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays_venture/is_on.py` & `ventures-1.4.1/venues/stages/ventures/plays_venture/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays_venture/turn_off/__init__.py` & `ventures-1.4.1/venues/stages/ventures/plays_venture/turn_off/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays_venture/turn_on/__init__.py` & `ventures-1.4.1/venues/stages/ventures/plays_venture/turn_on/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/readme.md` & `ventures-1.4.1/venues/stages/ventures/readme.md`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.4.1/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.4.1/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.4.1/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.4.1/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.4.0/PKG-INFO` & `ventures-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.4.0
+Version: 1.4.1
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

