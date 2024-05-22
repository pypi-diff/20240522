# Comparing `tmp/ventures-1.4.1.tar.gz` & `tmp/ventures-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.4.1.tar", max compression
+gzip compressed data, was "ventures-1.5.0.tar", max compression
```

## Comparing `ventures-1.4.1.tar` & `ventures-1.5.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rwxr-xr-x   0        0        0      585 2024-05-22 02:45:05.641317 ventures-1.4.1/pyproject.toml
--rwxr-xr-x   0        0        0     2991 2024-05-22 02:44:57.205412 ventures-1.4.1/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.4.1/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.4.1/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.4.1/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.4.1/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.4.1/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.4.1/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   380192 2024-05-22 02:26:21.642724 ventures-1.4.1/venues/stages/ventures/_status/DB/records.json
--rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-22 02:26:17.558779 ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-22 02:26:19.614751 ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-22 02:26:18.686763 ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.4.1/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.4.1/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
--rwxr-xr-x   0        0        0      184 2024-05-22 02:26:20.654737 ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.4.1/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.4.1/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0     1450 2024-05-22 01:51:45.688162 ventures-1.4.1/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.4.1/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.4.1/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1043 2024-05-22 02:08:02.966812 ventures-1.4.1/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      846 2024-05-22 01:38:48.876241 ventures-1.4.1/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0      838 2024-05-22 01:28:15.483410 ventures-1.4.1/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1370 2024-05-22 02:07:55.802884 ventures-1.4.1/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0      691 2024-05-22 01:38:30.720444 ventures-1.4.1/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.4.1/venues/stages/ventures/plays/turn_off_v1.py
--rwxr-xr-x   0        0        0      994 2024-05-22 01:26:13.120834 ventures-1.4.1/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.4.1/venues/stages/ventures/plays/turn_on_v1.py
--rwxr-xr-x   0        0        0      940 2024-05-22 02:10:17.449440 ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      924 2024-05-22 02:10:12.141494 ventures-1.4.1/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0     2136 2024-05-22 01:37:25.861169 ventures-1.4.1/venues/stages/ventures/plays_venture/turn_off/__init__.py
--rwxr-xr-x   0        0        0     1686 2024-05-22 01:38:48.876241 ventures-1.4.1/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.4.1/venues/stages/ventures/plays_venture/turn_on/__init__.py
--rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.4.1/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.4.1/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.4.1/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive/__init__.py
--rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.4.1/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.4.1/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.4.1/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.4.1/venues/stages/ventures/utilities/map/scan.py
--rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.4.1/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.4.1/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.4.1/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.4.1/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.4.1/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.4.1/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2024-05-22 18:08:52.457840 ventures-1.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0     2991 2024-05-22 18:08:22.478094 ventures-1.5.0/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.5.0/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.5.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.5.0/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.5.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.5.0/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.5.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   384634 2024-05-22 18:08:08.426213 ventures-1.5.0/venues/stages/ventures/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.5.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.5.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-22 18:08:03.370255 ventures-1.5.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.5.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.5.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-22 18:08:06.410230 ventures-1.5.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.5.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.5.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-22 18:08:04.774243 ventures-1.5.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.5.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.5.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.5.0/venues/stages/ventures/_status/monitors/5_on_and_off_1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.5.0/venues/stages/ventures/_status/monitors/5_on_and_off_1/status_1.py
+-rwxr-xr-x   0        0        0      184 2024-05-22 18:08:07.454221 ventures-1.5.0/venues/stages/ventures/_status/monitors/5_on_and_off_1/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.5.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.5.0/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0     1450 2024-05-22 01:51:45.688162 ventures-1.5.0/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.5.0/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.5.0/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1043 2024-05-22 02:08:02.966812 ventures-1.5.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rw-r--r--   0        0        0      970 2024-05-22 18:06:02.683241 ventures-1.5.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rw-r--r--   0        0        0      962 2024-05-22 18:07:04.742741 ventures-1.5.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1370 2024-05-22 02:07:55.802884 ventures-1.5.0/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0      835 2024-05-22 18:04:33.371931 ventures-1.5.0/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.5.0/venues/stages/ventures/plays/turn_off_v1.py
+-rwxr-xr-x   0        0        0     1064 2024-05-22 18:07:00.822773 ventures-1.5.0/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.5.0/venues/stages/ventures/plays/turn_on_v1.py
+-rwxr-xr-x   0        0        0      940 2024-05-22 02:10:17.449440 ventures-1.5.0/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.5.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.5.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      924 2024-05-22 02:10:12.141494 ventures-1.5.0/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0     2136 2024-05-22 01:37:25.861169 ventures-1.5.0/venues/stages/ventures/plays_venture/turn_off/__init__.py
+-rwxr-xr-x   0        0        0     1686 2024-05-22 01:38:48.876241 ventures-1.5.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.5.0/venues/stages/ventures/plays_venture/turn_on/__init__.py
+-rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.5.0/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.5.0/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.5.0/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.5.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.5.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.5.0/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.5.0/venues/stages/ventures/utilities/map/scan.py
+-rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.5.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.5.0/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.5.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.5.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.5.0/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.5.0/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.5.0/PKG-INFO
```

### Comparing `ventures-1.4.1/pyproject.toml` & `ventures-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.4.1"
+version = "1.5.0"
 description = ""
 authors = []
 readme = "venues/stages/ventures/readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "GPL-3.0-only"
```

### Comparing `ventures-1.4.1/venues/stages/ventures/__init__.py` & `ventures-1.5.0/venues/stages/ventures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,18 +99,17 @@
 			
 			return;
 	
 		ventures_packet = turn_on ({
 			"ventures": ventures,
 			"ventures_map_bracket": ventures_map_bracket
 		})
-		
-		rich.print_json (data = {
-			"proceeds after turn on": ventures_map_bracket
-		})
+		#rich.print_json (data = {
+		#	"proceeds after turn on": ventures_map_bracket
+		#})
 		
 		etch_map ({
 			"path": the_map_path,
 			"bracket": ventures_map_bracket
 		})
 		status = is_on ({
 			"ventures": ventures,
```

### Comparing `ventures-1.4.1/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.5.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/DB/records.json` & `ventures-1.5.0/venues/stages/ventures/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9817073170731707%*

 * *Differences: {"'_default'": "{'80': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [6.66000232740771e-07, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'status_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), OrderedDict([('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('elapsed', [7.690005077165551e-07, "*

 * *               "'seconds']),  […]*

```diff
@@ -12390,14 +12390,419 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "80": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.66000232740771e-07,
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
+                                7.690005077165551e-07,
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
+                                4.132510880000154,
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
+                                3.0973321120000037,
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
+                                3.1175697099997706,
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
+                                5.192795154000123,
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
+        "81": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.400003596558236e-07,
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
+                                6.039999789209105e-07,
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
+                                4.131768858999749,
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
+                                2.297101336000196,
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
+                                3.0905412319998504,
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
+                                5.154403706999801,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_on_and_off_1/status_1.py",
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
+        "82": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.919999577803537e-07,
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
+                                4.109997462364845e-07,
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
+                                4.147221326999897,
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
+                                2.351712659000441,
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
+                                2.125753025999984,
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
+                                5.190625850000288,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5_on_and_off_1/status_1.py",
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
         "9": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/5_on_and_off_1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/5_on_and_off_1/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status.proc.py` & `ventures-1.5.0/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.5.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/clique.py` & `ventures-1.5.0/venues/stages/ventures/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 01:38:30 2024 UTC, .py size: 691 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 964c 4d66 b302 0000  o........LMf....
+00000000: 6f0d 0d0a 0000 0000 b133 4e66 4303 0000  o........3NfC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 5a0b 6401 6407 6c0c 5a0c 6401  d.l.Z.d.d.l.Z.d.
@@ -11,43 +11,51 @@
 000000a0: 5300 290a 7a19 270a 0974 7572 6e5f 6f66  S.).z.'..turn_of
 000000b0: 6620 287b 0a09 090a 097d 290a 090a 22e9  f ({.....})...".
 000000c0: 0000 0000 2901 da08 6574 6368 5f6d 6170  ....)...etch_map
 000000d0: 2901 da08 7363 616e 5f6d 6170 2901 da0c  )...scan_map)...
 000000e0: 6669 6e64 5f76 656e 7475 7265 2901 da0b  find_venture)...
 000000f0: 6368 6563 6b5f 6973 5f6f 6e29 01da 1074  check_is_on)...t
 00000100: 7572 6e5f 6f66 665f 7665 6e74 7572 654e  urn_off_ventureN
-00000110: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-00000120: 0005 0000 0043 0000 0073 3200 0000 7c00  .....C...s2...|.
-00000130: 6401 1900 7d01 7c00 6402 1900 7d02 7c01  d...}.|.d...}.|.
-00000140: 4400 5d0c 7d03 7400 7401 7c02 7c03 8302  D.].}.t.t.|.|...
-00000150: 7c01 6403 9c02 8301 0100 710a 6400 5300  |.d.......q.d.S.
-00000160: 2904 4eda 1476 656e 7475 7265 735f 6d61  ).N..ventures_ma
-00000170: 705f 6272 6163 6b65 74da 0876 656e 7475  p_bracket..ventu
-00000180: 7265 7329 02da 0776 656e 7475 7265 7207  res)...venturer.
-00000190: 0000 0029 0272 0600 0000 7204 0000 0029  ...).r....r....)
-000001a0: 04da 0670 6163 6b65 7472 0700 0000 7208  ...packetr....r.
-000001b0: 0000 00da 046e 616d 65a9 0072 0c00 0000  .....name..r....
-000001c0: fa31 2f68 6162 6974 6174 2f76 656e 7565  .1/habitat/venue
-000001d0: 732f 7374 6167 6573 2f76 656e 7475 7265  s/stages/venture
-000001e0: 732f 706c 6179 732f 7475 726e 5f6f 6666  s/plays/turn_off
-000001f0: 2e70 79da 0874 7572 6e5f 6f66 6620 0000  .py..turn_off ..
-00000200: 0073 1000 0000 0801 0801 0802 0201 0801  .s..............
-00000210: 0201 0afe 04ff 720e 0000 0029 11da 075f  ......r....)..._
-00000220: 5f64 6f63 5f5f da1b 7665 6e74 7572 6573  _doc__..ventures
-00000230: 2e75 7469 6c69 7469 6573 2e6d 6170 2e65  .utilities.map.e
-00000240: 7463 6872 0200 0000 da1b 7665 6e74 7572  tchr......ventur
-00000250: 6573 2e75 7469 6c69 7469 6573 2e6d 6170  es.utilities.map
-00000260: 2e73 6361 6e72 0300 0000 da28 7665 6e74  .scanr.....(vent
-00000270: 7572 6573 2e75 7469 6c69 7469 6573 2e76  ures.utilities.v
-00000280: 656e 7475 7265 732e 6669 6e64 5f76 656e  entures.find_ven
-00000290: 7475 7265 7204 0000 00da 2676 656e 7475  turer.....&ventu
-000002a0: 7265 732e 7574 696c 6974 6965 732e 7072  res.utilities.pr
-000002b0: 6f63 6573 732e 6368 6563 6b5f 6973 5f6f  ocess.check_is_o
-000002c0: 6e72 0500 0000 da1f 7665 6e74 7572 6573  nr......ventures
-000002d0: 2e70 6c61 7973 5f76 656e 7475 7265 2e74  .plays_venture.t
-000002e0: 7572 6e5f 6f66 6672 0600 0000 da04 7269  urn_offr......ri
-000002f0: 6368 da04 6a73 6f6e da06 7369 676e 616c  ch..json..signal
-00000300: da02 6f73 da04 7469 6d65 720e 0000 0072  ..os..timer....r
-00000310: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000320: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000330: 0073 1800 0000 0402 0c0a 0c01 0c01 0c01  .s..............
-00000340: 0c02 0803 0803 0801 0801 0801 0c05       ..............
+00000110: 6301 0000 0000 0000 0000 0000 0006 0000  c...............
+00000120: 000b 0000 0043 0000 0073 7000 0000 7c00  .....C...sp...|.
+00000130: 6401 1900 7d01 7c00 6402 1900 7d02 6700  d...}.|.d...}.g.
+00000140: 7d03 7c01 4400 5d27 7d04 7a0c 7400 7401  }.|.D.]'}.z.t.t.
+00000150: 7c02 7c04 8302 7c01 6403 9c02 8301 0100  |.|...|.d.......
+00000160: 5700 710c 0400 7402 7933 0100 7d05 0100  W.q...t.y3..}...
+00000170: 7a0d 7c03 a003 6404 7c04 6901 a101 0100  z.|...d.|.i.....
+00000180: 5700 5900 6400 7d05 7e05 710c 6400 7d05  W.Y.d.}.~.q.d.}.
+00000190: 7e05 7701 7700 6405 7c03 6901 5300 2906  ~.w.w.d.|.i.S.).
+000001a0: 4eda 1476 656e 7475 7265 735f 6d61 705f  N..ventures_map_
+000001b0: 6272 6163 6b65 74da 0876 656e 7475 7265  bracket..venture
+000001c0: 7329 02da 0776 656e 7475 7265 7207 0000  s)...venturer...
+000001d0: 00da 046e 616d 65da 0a75 6e66 696e 6973  ...name..unfinis
+000001e0: 6865 6429 0472 0600 0000 7204 0000 00da  hed).r....r.....
+000001f0: 0945 7863 6570 7469 6f6e da06 6170 7065  .Exception..appe
+00000200: 6e64 2906 da06 7061 636b 6574 7207 0000  nd)...packetr...
+00000210: 0072 0800 0000 720b 0000 0072 0a00 0000  .r....r....r....
+00000220: da01 45a9 0072 1000 0000 fa31 2f68 6162  ..E..r.....1/hab
+00000230: 6974 6174 2f76 656e 7565 732f 7374 6167  itat/venues/stag
+00000240: 6573 2f76 656e 7475 7265 732f 706c 6179  es/ventures/play
+00000250: 732f 7475 726e 5f6f 6666 2e70 79da 0874  s/turn_off.py..t
+00000260: 7572 6e5f 6f66 6620 0000 0073 2200 0000  urn_off ...s"...
+00000270: 0801 0801 0402 0801 0201 0201 0801 0201  ................
+00000280: 0cfe 0e04 0401 0401 12ff 0880 02ff 0406  ................
+00000290: 04ff 7212 0000 0029 11da 075f 5f64 6f63  ..r....)...__doc
+000002a0: 5f5f da1b 7665 6e74 7572 6573 2e75 7469  __..ventures.uti
+000002b0: 6c69 7469 6573 2e6d 6170 2e65 7463 6872  lities.map.etchr
+000002c0: 0200 0000 da1b 7665 6e74 7572 6573 2e75  ......ventures.u
+000002d0: 7469 6c69 7469 6573 2e6d 6170 2e73 6361  tilities.map.sca
+000002e0: 6e72 0300 0000 da28 7665 6e74 7572 6573  nr.....(ventures
+000002f0: 2e75 7469 6c69 7469 6573 2e76 656e 7475  .utilities.ventu
+00000300: 7265 732e 6669 6e64 5f76 656e 7475 7265  res.find_venture
+00000310: 7204 0000 00da 2676 656e 7475 7265 732e  r.....&ventures.
+00000320: 7574 696c 6974 6965 732e 7072 6f63 6573  utilities.proces
+00000330: 732e 6368 6563 6b5f 6973 5f6f 6e72 0500  s.check_is_onr..
+00000340: 0000 da1f 7665 6e74 7572 6573 2e70 6c61  ....ventures.pla
+00000350: 7973 5f76 656e 7475 7265 2e74 7572 6e5f  ys_venture.turn_
+00000360: 6f66 6672 0600 0000 da04 7269 6368 da04  offr......rich..
+00000370: 6a73 6f6e da06 7369 676e 616c da02 6f73  json..signal..os
+00000380: da04 7469 6d65 7212 0000 0072 1000 0000  ..timer....r....
+00000390: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+000003a0: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
+000003b0: 0000 0402 0c0a 0c01 0c01 0c01 0c02 0803  ................
+000003c0: 0803 0801 0801 0801 0c05                 ..........
```

### Comparing `ventures-1.4.1/venues/stages/ventures/plays/is_on.py` & `ventures-1.5.0/venues/stages/ventures/plays/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays/turn_off.py` & `ventures-1.5.0/venues/stages/ventures/plays/turn_off.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,17 +29,27 @@
 #++++
 
 
 def turn_off (packet):
 	ventures_map_bracket = packet ["ventures_map_bracket"]
 	ventures = packet ["ventures"]
 	
+	unfinished = []
 	for name in ventures_map_bracket:
-		turn_off_venture ({
-			"venture": find_venture (ventures, name),
-			"ventures_map_bracket": ventures_map_bracket
-		})
+		try:
+			turn_off_venture ({
+				"venture": find_venture (ventures, name),
+				"ventures_map_bracket": ventures_map_bracket
+			})
+		except Exception as E:
+			unfinished.append ({
+				"name": name
+			})
+			
+	return {
+		"unfinished": unfinished
+	}
```

### Comparing `ventures-1.4.1/venues/stages/ventures/plays/turn_off_v1.py` & `ventures-1.5.0/venues/stages/ventures/plays/turn_off_v1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays/turn_on.py` & `ventures-1.5.0/venues/stages/ventures/plays/turn_on.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,19 +42,25 @@
 "'''
 
 
 def turn_on (packet):
 	ventures = packet ["ventures"]
 	ventures_map_bracket = packet ["ventures_map_bracket"]
 	
-	for adventure in ventures:
-		turn_on_venture ({
-			"venture": adventure,
-			"ventures_map_bracket": ventures_map_bracket
-		})
-		
-		continue;
 	
+	unfinished = []
+	for adventure in ventures:
+		try:
+			turn_on_venture ({
+				"venture": adventure,
+				"ventures_map_bracket": ventures_map_bracket
+			})
+		except Exception as E:
+			unfinished.append ({
+				"name": name
+			})
+			
 	return {
-		"ventures_map_bracket": ventures_map_bracket
+		"unfinished": unfinished
 	}
 	
+
```

### Comparing `ventures-1.4.1/venues/stages/ventures/plays/turn_on_v1.py` & `ventures-1.5.0/venues/stages/ventures/plays/turn_on_v1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays_venture/is_on.py` & `ventures-1.5.0/venues/stages/ventures/plays_venture/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays_venture/turn_off/__init__.py` & `ventures-1.5.0/venues/stages/ventures/plays_venture/turn_off/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays_venture/turn_on/__init__.py` & `ventures-1.5.0/venues/stages/ventures/plays_venture/turn_on/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/readme.md` & `ventures-1.5.0/venues/stages/ventures/readme.md`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.5.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.5.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.5.0/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.5.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.5.0/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.4.1/PKG-INFO` & `ventures-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.4.1
+Version: 1.5.0
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

