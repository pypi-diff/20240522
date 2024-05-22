# Comparing `tmp/ventures-1.3.3.tar.gz` & `tmp/ventures-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.3.3.tar", max compression
+gzip compressed data, was "ventures-1.4.0.tar", max compression
```

## Comparing `ventures-1.3.3.tar` & `ventures-1.4.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
--rwxr-xr-x   0        0        0      585 2024-05-22 01:39:04.240070 ventures-1.3.3/pyproject.toml
--rwxr-xr-x   0        0        0     3135 2024-05-22 01:19:34.461653 ventures-1.3.3/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.3.3/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.3.3/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.3.3/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.3.3/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.3.3/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.3.3/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   361169 2024-05-22 01:38:55.132171 ventures-1.3.3/venues/stages/ventures/_status/DB/records.json
--rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-22 01:38:51.068217 ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-22 01:38:53.136194 ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-22 01:38:52.244204 ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.3.3/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.3.3/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
--rwxr-xr-x   0        0        0      184 2024-05-22 01:38:54.144183 ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.3.3/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.3.3/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      984 2024-05-21 22:50:00.483641 ventures-1.3.3/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.3.3/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.3.3/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1055 2024-05-22 01:14:22.929696 ventures-1.3.3/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rw-r--r--   0        0        0      846 2024-05-22 01:38:48.876241 ventures-1.3.3/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0      838 2024-05-22 01:28:15.483410 ventures-1.3.3/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1189 2024-05-22 01:14:18.249745 ventures-1.3.3/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0      691 2024-05-22 01:38:30.720444 ventures-1.3.3/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.3.3/venues/stages/ventures/plays/turn_off_v1.py
--rwxr-xr-x   0        0        0      994 2024-05-22 01:26:13.120834 ventures-1.3.3/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.3.3/venues/stages/ventures/plays/turn_on_v1.py
--rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.3.3/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.3.3/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.3.3/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0     2136 2024-05-22 01:37:25.861169 ventures-1.3.3/venues/stages/ventures/plays_venture/turn_off/__init__.py
--rw-r--r--   0        0        0     1686 2024-05-22 01:38:48.876241 ventures-1.3.3/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.3.3/venues/stages/ventures/plays_venture/turn_on/__init__.py
--rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.3.3/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.3.3/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.3.3/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive/__init__.py
--rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.3.3/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.3.3/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.3.3/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.3.3/venues/stages/ventures/utilities/map/scan.py
--rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.3.3/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.3.3/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.3.3/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.3.3/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.3.3/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.3.3/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.3.3/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2024-05-22 02:27:25.345879 ventures-1.4.0/pyproject.toml
+-rwxr-xr-x   0        0        0     2988 2024-05-22 01:50:56.204575 ventures-1.4.0/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.4.0/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.4.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.4.0/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.4.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.4.0/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.4.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   380192 2024-05-22 02:26:21.642724 ventures-1.4.0/venues/stages/ventures/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1227 2024-05-22 00:50:05.015739 ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1153 2024-05-22 00:49:57.459796 ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-22 02:26:17.558779 ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1293 2024-05-22 00:50:05.015739 ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1448 2024-05-22 00:49:57.479796 ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-22 02:26:19.614751 ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rwxr-xr-x   0        0        0      974 2024-05-22 01:32:06.796762 ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      788 2024-05-22 01:30:33.169828 ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-22 02:26:18.686763 ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.4.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.4.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1604 2024-05-22 00:50:05.007739 ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1919 2024-05-22 00:49:57.511796 ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py
+-rwxr-xr-x   0        0        0      184 2024-05-22 02:26:20.654737 ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.4.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.4.0/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0     1450 2024-05-22 01:51:45.688162 ventures-1.4.0/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.4.0/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.4.0/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1043 2024-05-22 02:08:02.966812 ventures-1.4.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      846 2024-05-22 01:38:48.876241 ventures-1.4.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      838 2024-05-22 01:28:15.483410 ventures-1.4.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1370 2024-05-22 02:07:55.802884 ventures-1.4.0/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0      691 2024-05-22 01:38:30.720444 ventures-1.4.0/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     2696 2024-05-22 01:31:54.244904 ventures-1.4.0/venues/stages/ventures/plays/turn_off_v1.py
+-rwxr-xr-x   0        0        0      994 2024-05-22 01:26:13.120834 ventures-1.4.0/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0     3301 2024-05-22 01:25:32.497311 ventures-1.4.0/venues/stages/ventures/plays/turn_on_v1.py
+-rwxr-xr-x   0        0        0      940 2024-05-22 02:10:17.449440 ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1720 2024-05-22 00:50:05.059738 ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1960 2024-05-21 22:11:56.167317 ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      924 2024-05-22 02:10:12.141494 ventures-1.4.0/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0     2136 2024-05-22 01:37:25.861169 ventures-1.4.0/venues/stages/ventures/plays_venture/turn_off/__init__.py
+-rwxr-xr-x   0        0        0     1686 2024-05-22 01:38:48.876241 ventures-1.4.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2756 2024-05-22 01:12:51.670650 ventures-1.4.0/venues/stages/ventures/plays_venture/turn_on/__init__.py
+-rwxr-xr-x   0        0        0     1915 2024-05-22 01:14:22.929696 ventures-1.4.0/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2367 2024-05-22 01:16:23.132122 ventures-1.4.0/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.4.0/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2446 2024-05-21 22:11:00.972030 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rwxr-xr-x   0        0        0     1902 2024-05-21 22:11:03.367998 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.4.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      496 2024-05-22 00:50:05.051739 ventures-1.4.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.4.0/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      245 2024-05-22 00:49:57.599795 ventures-1.4.0/venues/stages/ventures/utilities/map/scan.py
+-rwxr-xr-x   0        0        0      886 2024-05-22 00:23:05.620048 ventures-1.4.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      669 2024-05-22 00:23:03.376080 ventures-1.4.0/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.4.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      499 2024-05-21 21:59:03.306202 ventures-1.4.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-21 21:58:17.698946 ventures-1.4.0/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.4.0/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 ventures-1.4.0/PKG-INFO
```

### Comparing `ventures-1.3.3/pyproject.toml` & `ventures-1.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.3.3"
+version = "1.4.0"
 description = ""
 authors = []
 readme = "venues/stages/ventures/readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "GPL-3.0-only"
```

### Comparing `ventures-1.3.3/venues/stages/ventures/__init__.py` & `ventures-1.4.0/venues/stages/ventures/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,39 +71,37 @@
 		ventures_map_bracket = scan_map ({
 			"path": the_map_path
 		})
 
 	def turn_on_move (packet = {}):
 		print ('turn on move', packet)
 	
-		if (type (packet) == dict):
-			if ("name" in packet):
-				name = packet ["name"]
+		if (type (packet) == dict and "name" in packet):
+			name = packet ["name"]
+		
+			venture = find_venture (ventures, name)
+			rich.print_json (data = {
+				"venture": venture
+			})
+		
+			the_venture_packet = turn_on_venture ({
+				"venture": venture,
+				"ventures_map_bracket": ventures_map_bracket
+			})
 			
-				venture = find_venture (ventures, name)
-				rich.print_json (data = {
-					"venture": venture
-				})
+			etch_map ({
+				"path": the_map_path,
+				"bracket": ventures_map_bracket
+			})
+			status = is_on ({
+				"ventures": ventures,
+				"ventures_map_bracket": ventures_map_bracket
+			});
 			
-				the_venture_packet = turn_on_venture ({
-					"venture": venture,
-					"ventures_map_bracket": ventures_map_bracket
-				})
-				
-				etch_map ({
-					"path": the_map_path,
-					"bracket": ventures_map_bracket
-				})
-						
-				status = is_on ({
-					"ventures": ventures,
-					"ventures_map_bracket": ventures_map_bracket
-				});
-				
-				return;
+			return;
 	
 		ventures_packet = turn_on ({
 			"ventures": ventures,
 			"ventures_map_bracket": ventures_map_bracket
 		})
 		
 		rich.print_json (data = {
@@ -126,50 +124,43 @@
 		});
 	
 		return;
 		
 	def turn_off_move (packet = {}):
 		print ("turn_off_move:", turn_off_move)
 	
-		if (type (packet) == dict):
-			if ("name" in packet):
-				name = packet ["name"]
+		if (type (packet) == dict and "name" in packet):
+			name = packet ["name"]
+		
+			turn_off_venture ({
+				"venture": find_venture (ventures, name),
+				"ventures_map_bracket": ventures_map_bracket
+			})
 			
-				venture = find_venture (ventures, name)
-				rich.print_json (data = {
-					"venture": venture
-				})
+			etch_map ({
+				"path": the_map_path,
+				"bracket": ventures_map_bracket
+			})
 			
-				turn_off_venture ({
-					"venture": venture,
-					"ventures_map_bracket": ventures_map_bracket
-				})
-				
-				etch_map ({
-					"path": the_map_path,
-					"bracket": ventures_map_bracket
-				})
-				
-				status = is_on ({
-					"ventures": ventures,
-					"ventures_map_bracket": ventures_map_bracket
-				});
-				
-				return;
+			status = is_on ({
+				"ventures": ventures,
+				"ventures_map_bracket": ventures_map_bracket
+			});
+			
+			return;
 	
 		turn_off ({
 			"ventures": ventures,
 			"ventures_map_bracket": ventures_map_bracket
 		});
 		
 		etch_map ({
 			"path": the_map_path,
 			"bracket": ventures_map_bracket
 		})
-		
 		status = is_on ({
 			"ventures": ventures,
 			"ventures_map_bracket": ventures_map_bracket
 		});
 	
 		return;
```

### Comparing `ventures-1.3.3/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.4.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/DB/records.json` & `ventures-1.4.0/venues/stages/ventures/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9556962025316456%*

 * *Differences: {"'_default'": "{'73': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [5.409965524449944e-07, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'status_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), OrderedDict([('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('elapsed', [1.14399881567806e-06, "*

 * *               "'seconds']),  […]*

```diff
@@ -11225,14 +11225,1124 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "73": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.409965524449944e-07,
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
+                                1.14399881567806e-06,
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
+                                4.1483647220011335,
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
+                                2.400527425998007,
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
+                                3.0932925040033297,
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
+                                5.189346084000135,
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
+        "74": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.210029823705554e-07,
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
+                                6.449990905821323e-07,
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
+                                4.162233161005133,
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
+                                3.04073802199855,
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
+                                3.08954870699381,
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
+                                4.204773526005738,
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
+        "75": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'adventure_details' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 115, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 37, in is_on",
+                                "    status = venture_is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/is_on.py\", line 34, in venture_is_on",
+                                "    process_identity = adventure_details [\"process_identity\"]",
+                                "NameError: name 'adventure_details' is not defined"
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
+                            "exception": "NameError(\"name 'adventure_details' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 115, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 37, in is_on",
+                                "    status = venture_is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/is_on.py\", line 34, in venture_is_on",
+                                "    process_identity = adventure_details [\"process_identity\"]",
+                                "NameError: name 'adventure_details' is not defined"
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
+                            "exception": "NameError(\"name 'adventure_details' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 115, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 37, in is_on",
+                                "    status = venture_is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/is_on.py\", line 34, in venture_is_on",
+                                "    process_identity = adventure_details [\"process_identity\"]",
+                                "NameError: name 'adventure_details' is not defined"
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
+                                5.300025804899633e-07,
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
+                                4.62001480627805e-07,
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
+                            "exception": "NameError(\"name 'adventure_details' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 115, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 37, in is_on",
+                                "    status = venture_is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/is_on.py\", line 34, in venture_is_on",
+                                "    process_identity = adventure_details [\"process_identity\"]",
+                                "NameError: name 'adventure_details' is not defined"
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
+                                2.3408403560024453,
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
+                            "exception": "NameError(\"name 'adventure_details' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 115, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 37, in is_on",
+                                "    status = venture_is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/is_on.py\", line 34, in venture_is_on",
+                                "    process_identity = adventure_details [\"process_identity\"]",
+                                "NameError: name 'adventure_details' is not defined"
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
+                            "exception": "NameError(\"name 'adventure_details' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py\", line 70, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 115, in turn_on_move",
+                                "    status = is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/is_on.py\", line 37, in is_on",
+                                "    status = venture_is_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/is_on.py\", line 34, in venture_is_on",
+                                "    process_identity = adventure_details [\"process_identity\"]",
+                                "NameError: name 'adventure_details' is not defined"
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
+        "76": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.3399708122015e-07,
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
+                                5.860056262463331e-07,
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
+                                4.149047748003795,
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
+                                2.3629852300000493,
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
+                                3.099560520997329,
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
+                                5.224868472003436,
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
+        "77": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.630055627785623e-07,
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
+                                1.2239979696460068e-06,
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
+                                4.152783249999629,
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
+                                2.334193463997508,
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
+                                3.0944456870056456,
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
+                                5.168792040996777,
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
+        "78": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1_sanique did not turn on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 102, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 50, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 129, in turn_on_venture",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1_sanique did not turn on."
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
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.2160016922280192e-06,
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
+                                7.179987733252347e-07,
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
+                                4.141366172996641,
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
+                            "exception": "Exception('After 10 loops, adventure_1_sanique did not turn on.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task/status_1.py\", line 39, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 102, in turn_on_move",
+                                "    ventures_packet = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 50, in turn_on",
+                                "    turn_on_venture ({",
+                                "  File \"/habitat/venues/stages/ventures/plays_venture/turn_on/__init__.py\", line 129, in turn_on_venture",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1_sanique did not turn on."
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
+                            "elapsed": [
+                                5.197218222005176,
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
+                    "alarms": 2,
+                    "passes": 4
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "79": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.149995558895171e-07,
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
+                                6.140035111457109e-07,
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
+                                4.14887592800369,
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
+                                3.04479723800614,
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
+                                3.0920879550030804,
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
+                                5.182255684994743,
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

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/5_refresh_1/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status.proc.py` & `ventures-1.4.0/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.4.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/clique.py` & `ventures-1.4.0/venues/stages/ventures/clique.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,16 +56,38 @@
 				"name": name
 			})
 			return;
 	
 		ventures ["turn off"] ()
 		
 		
+	@group.command ("refresh")
+	@click.option ('--name', help = 'venture name')
+	def off (name):
+		if (type (name) == str and len (name) >= 1):
+			ventures ["turn off"] ({
+				"name": name
+			})
+			ventures ["turn on"] ({
+				"name": name
+			})
+			return;
+	
+		ventures ["turn off"] ()
+		ventures ["turn on"] ()
+		
+		
 	@group.command ("status")
-	def status ():
+	@click.option ('--name', help = 'venture name')
+	def status (name):
+		if (type (name) == str and len (name) >= 1):
+			ventures ["is on"] ({
+				"name": name
+			})
+			
 		ventures ["is on"] ()
 		
 
 	return group
 
 #
```

### Comparing `ventures-1.3.3/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/is_on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 22 01:14:18 2024 UTC, .py size: 1189 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,59 @@
-00000000: 6f0d 0d0a 0000 0000 ea46 4d66 a504 0000  o........FMf....
+00000000: 6f0d 0d0a 0000 0000 0454 4d66 9c03 0000  o........TMf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
+00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
-00000060: 6405 8400 5a07 6406 6407 8400 5a08 6402  d...Z.d.d...Z.d.
-00000070: 5300 2908 7a05 270a 090a 22e9 0000 0000  S.).z.'...".....
-00000080: 4e29 01da 0b63 6865 636b 5f69 735f 6f6e  N)...check_is_on
-00000090: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000000a0: 0004 0000 0043 0000 0073 2e00 0000 7c00  .....C...s....|.
-000000b0: 4400 5d0c 7d02 7c01 7c02 6401 1900 6b02  D.].}.|.|.d...k.
-000000c0: 720e 7c02 0200 0100 5300 7102 7400 6402  r.|.....S.q.t.d.
-000000d0: 7c01 9b00 6403 9d03 8301 8201 2904 4eda  |...d.......).N.
-000000e0: 046e 616d 657a 1356 656e 7475 7265 2077  .namez.Venture w
-000000f0: 6974 6820 6e61 6d65 2027 7a0c 2720 6e6f  ith name 'z.' no
-00000100: 7420 666f 756e 642e 2901 da09 4578 6365  t found.)...Exce
-00000110: 7074 696f 6e29 03da 0876 656e 7475 7265  ption)...venture
-00000120: 7372 0300 0000 da07 7665 6e74 7572 65a9  sr......venture.
-00000130: 0072 0700 0000 fa2e 2f68 6162 6974 6174  .r....../habitat
-00000140: 2f76 656e 7565 732f 7374 6167 6573 2f76  /venues/stages/v
-00000150: 656e 7475 7265 732f 706c 6179 732f 6973  entures/plays/is
-00000160: 5f6f 6e2e 7079 da0c 6669 6e64 5f76 656e  _on.py..find_ven
-00000170: 7475 7265 1400 0000 730a 0000 0008 010c  ture....s.......
-00000180: 0108 0102 ff10 0372 0900 0000 6301 0000  .......r....c...
-00000190: 0000 0000 0000 0000 000a 0000 0005 0000  ................
-000001a0: 0043 0000 0073 a200 0000 7c00 6401 1900  .C...s....|.d...
-000001b0: 7d01 7c00 6402 1900 7d02 6900 7d03 7c01  }.|.d...}.i.}.|.
-000001c0: 4400 5d3a 7d04 7c01 7c04 1900 7d05 7c05  D.]:}.|.|...}.|.
-000001d0: 6403 1900 7d06 7c06 6404 6b02 722a 7c05  d...}.|.d.k.r*|.
-000001e0: 6404 1900 7d07 7400 7c07 8301 7d08 7c07  d...}.t.|...}.|.
-000001f0: 7c08 6405 9c02 7c03 7c04 3c00 710c 7c06  |.d...|.|.<.q.|.
-00000200: 6406 6b02 723f 7401 7c02 7c04 8302 7d09  d.k.r?t.|.|...}.
-00000210: 7c09 6407 1900 8300 7d08 6408 7c08 6901  |.d.....}.d.|.i.
-00000220: 7c03 7c04 3c00 710c 7402 6409 7c06 9b00  |.|.<.q.t.d.|...
-00000230: 640a 9d03 8301 8201 7403 6a04 640b 7c03  d.......t.j.d.|.
-00000240: 6901 640c 8d01 0100 6400 5300 290d 4eda  i.d.....d.S.).N.
-00000250: 1476 656e 7475 7265 735f 6d61 705f 6272  .ventures_map_br
-00000260: 6163 6b65 7472 0500 0000 da04 6b69 6e64  acketr......kind
-00000270: da10 7072 6f63 6573 735f 6964 656e 7469  ..process_identi
-00000280: 7479 2902 720c 0000 00da 0673 7461 7475  ty).r......statu
-00000290: 73da 0474 6173 6b7a 0569 7320 6f6e 720d  s..taskz.is onr.
-000002a0: 0000 007a 064b 696e 6420 227a 0c22 206e  ...z.Kind "z." n
-000002b0: 6f74 2066 6f75 6e64 2eda 0873 7461 7475  ot found...statu
-000002c0: 7365 7329 01da 0464 6174 6129 0572 0200  ses)...data).r..
-000002d0: 0000 7209 0000 0072 0400 0000 da04 7269  ..r....r......ri
-000002e0: 6368 da0a 7072 696e 745f 6a73 6f6e 290a  ch..print_json).
-000002f0: da06 7061 636b 6574 720a 0000 0072 0500  ..packetr....r..
-00000300: 0000 720f 0000 00da 0961 6476 656e 7475  ..r......adventu
-00000310: 7265 da11 6164 7665 6e74 7572 655f 6465  re..adventure_de
-00000320: 7461 696c 7372 0b00 0000 720c 0000 0072  tailsr....r....r
-00000330: 0d00 0000 7206 0000 0072 0700 0000 7207  ....r....r....r.
-00000340: 0000 0072 0800 0000 da05 6973 5f6f 6e1c  ...r......is_on.
-00000350: 0000 0073 3000 0000 0801 0801 0403 0801  ...s0...........
-00000360: 0801 0801 0803 0801 0801 0203 0201 0afe  ................
-00000370: 0205 0802 0a01 0a01 0403 08ff 0204 1002  ................
-00000380: 0402 0401 08ff 0404 7216 0000 0029 09da  ........r....)..
-00000390: 075f 5f64 6f63 5f5f da06 7073 7574 696c  .__doc__..psutil
-000003a0: da04 7469 6d65 da04 6a73 6f6e 7211 0000  ..time..jsonr...
-000003b0: 00da 2676 656e 7475 7265 732e 7574 696c  ..&ventures.util
-000003c0: 6974 6965 732e 7072 6f63 6573 732e 6368  ities.process.ch
-000003d0: 6563 6b5f 6973 5f6f 6e72 0200 0000 7209  eck_is_onr....r.
-000003e0: 0000 0072 1600 0000 7207 0000 0072 0700  ...r....r....r..
-000003f0: 0000 7207 0000 0072 0800 0000 da08 3c6d  ..r....r......<m
-00000400: 6f64 756c 653e 0100 0000 7310 0000 0004  odule>....s.....
-00000410: 0108 0608 0108 0108 030c 0308 040c 08    ...............
+00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
+00000060: 6404 6c07 6d08 5a08 0100 6405 6406 8400  d.l.m.Z...d.d...
+00000070: 5a09 6402 5300 2907 7a7d 0a09 6672 6f6d  Z.d.S.).z}..from
+00000080: 2076 656e 7475 7265 732e 706c 6179 735f   ventures.plays_
+00000090: 7665 6e74 7572 652e 6973 5f6f 6e20 696d  venture.is_on im
+000000a0: 706f 7274 2076 656e 7475 7265 5f69 735f  port venture_is_
+000000b0: 6f6e 0a09 7665 6e74 7572 655f 6973 5f6f  on..venture_is_o
+000000c0: 6e20 287b 0a09 0922 7665 6e74 7572 6522  n ({..."venture"
+000000d0: 3a20 7b7d 2c0a 0909 2276 656e 7475 7265  : {},..."venture
+000000e0: 735f 6d61 705f 6272 6163 6b65 7422 3a20  s_map_bracket": 
+000000f0: 7b7d 0a09 7d29 0ae9 0000 0000 4e29 01da  {}..})......N)..
+00000100: 0b63 6865 636b 5f69 735f 6f6e 2901 da0c  .check_is_on)...
+00000110: 6669 6e64 5f76 656e 7475 7265 6301 0000  find_venturec...
+00000120: 0000 0000 0000 0000 0008 0000 0004 0000  ................
+00000130: 0043 0000 0073 7600 0000 7c00 6401 1900  .C...sv...|.d...
+00000140: 7d01 7c00 6402 1900 7d02 7c00 6403 1900  }.|.d...}.|.d...
+00000150: 7d03 7c03 6404 1900 7d04 7c04 6405 6b02  }.|.d...}.|.d.k.
+00000160: 7221 7c03 6405 1900 7d05 7400 7c05 8301  r!|.d...}.t.|...
+00000170: 7d06 7c05 7c06 6406 9c02 5300 7c04 6407  }.|.|.d...S.|.d.
+00000180: 6b02 7233 7401 7c02 7c01 8302 7d07 7c07  k.r3t.|.|...}.|.
+00000190: 6408 1900 8300 7d06 6409 7c06 6901 5300  d.....}.d.|.i.S.
+000001a0: 7402 640a 7c04 9b00 640b 9d03 8301 8201  t.d.|...d.......
+000001b0: 290c 4eda 046e 616d 65da 0876 656e 7475  ).N..name..ventu
+000001c0: 7265 73da 1376 656e 7475 7265 5f6d 6170  res..venture_map
+000001d0: 5f64 6574 6169 6c73 da04 6b69 6e64 da10  _details..kind..
+000001e0: 7072 6f63 6573 735f 6964 656e 7469 7479  process_identity
+000001f0: 2902 7208 0000 00da 0673 7461 7475 73da  ).r......status.
+00000200: 0474 6173 6b7a 0569 7320 6f6e 7209 0000  .taskz.is onr...
+00000210: 007a 064b 696e 6420 277a 1027 2077 6173  .z.Kind 'z.' was
+00000220: 206e 6f74 2066 6f75 6e64 2e29 0372 0200   not found.).r..
+00000230: 0000 7203 0000 00da 0945 7863 6570 7469  ..r......Excepti
+00000240: 6f6e 2908 da06 7061 636b 6574 7204 0000  on)...packetr...
+00000250: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
+00000260: 7208 0000 0072 0900 0000 da07 7665 6e74  r....r......vent
+00000270: 7572 65a9 0072 0e00 0000 fa36 2f68 6162  ure..r.....6/hab
+00000280: 6974 6174 2f76 656e 7565 732f 7374 6167  itat/venues/stag
+00000290: 6573 2f76 656e 7475 7265 732f 706c 6179  es/ventures/play
+000002a0: 735f 7665 6e74 7572 652f 6973 5f6f 6e2e  s_venture/is_on.
+000002b0: 7079 da0d 7665 6e74 7572 655f 6973 5f6f  py..venture_is_o
+000002c0: 6e1a 0000 0073 2000 0000 0801 0801 0801  n....s .........
+000002d0: 0802 0802 0801 0801 0202 0201 06fe 0805  ................
+000002e0: 0a01 0a01 0402 04ff 1004 7210 0000 0029  ..........r....)
+000002f0: 0ada 075f 5f64 6f63 5f5f da06 7073 7574  ...__doc__..psut
+00000300: 696c da04 7469 6d65 da04 6a73 6f6e da04  il..time..json..
+00000310: 7269 6368 da26 7665 6e74 7572 6573 2e75  rich.&ventures.u
+00000320: 7469 6c69 7469 6573 2e70 726f 6365 7373  tilities.process
+00000330: 2e63 6865 636b 5f69 735f 6f6e 7202 0000  .check_is_onr...
+00000340: 00da 2876 656e 7475 7265 732e 7574 696c  ..(ventures.util
+00000350: 6974 6965 732e 7665 6e74 7572 6573 2e66  ities.ventures.f
+00000360: 696e 645f 7665 6e74 7572 6572 0300 0000  ind_venturer....
+00000370: 7210 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000380: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
+00000390: 6c65 3e01 0000 0073 1000 0000 0402 080a  le>....s........
+000003a0: 0801 0801 0803 0c03 0c01 0c04            ............
```

### Comparing `ventures-1.3.3/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays/is_on.py` & `ventures-1.4.0/venues/stages/ventures/plays_venture/is_on.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,48 @@
 
-''''
-	
-"'''
+
+'''
+	from ventures.plays_venture.is_on import venture_is_on
+	venture_is_on ({
+		"venture": {},
+		"ventures_map_bracket": {}
+	})
+'''
 
 #++++
 #
 import psutil
 import time
 import json
 #
 #
 import rich
 #
 #
 from ventures.utilities.process.check_is_on import check_is_on
+from ventures.utilities.ventures.find_venture import find_venture
 #
 #++++
 
-def find_venture (ventures, name):
-	for venture in ventures:
-		if (name == venture ["name"]):
-			return venture;
-			
-	raise Exception (f"Venture with name '{ name }' not found.")
-	
-	
-def is_on (packet):
-	ventures_map_bracket = packet ["ventures_map_bracket"]
+def venture_is_on (packet):
+	name = packet ["name"]
 	ventures = packet ["ventures"]
-
+	venture_map_details = packet ["venture_map_details"]
+	
+	kind = venture_map_details ["kind"]
 	
-	statuses = {}
-	for adventure in ventures_map_bracket:
-		adventure_details = ventures_map_bracket [ adventure ]
-		kind = adventure_details ["kind"]
-		#print (ventures)
+	if (kind == "process_identity"):
+		process_identity = venture_map_details ["process_identity"]
+		status = check_is_on (process_identity)
+		return {
+			"process_identity": process_identity,
+			"status": status
+		}
 		
-		if (kind == "process_identity"):
-			process_identity = adventure_details ["process_identity"]
-			status = check_is_on (process_identity)
-			
-			statuses [ adventure ] = {
-				"process_identity": process_identity,
-				"status": status
-			}
-			
-			continue;
-			
-		if (kind == "task"):	
-			venture = find_venture (ventures, adventure)
-			status = venture ["is on"] ()
-				
-			statuses [ adventure ] = {
-				"status": status
-			}	
-				
-			continue;
-			
-		raise Exception (f'Kind "{ kind }" not found.')
-				
-	rich.print_json (data = {
-		"statuses": statuses
-	})
-
-	return;	
+	if (kind == "task"):	
+		venture = find_venture (ventures, name)
+		status = venture ["is on"] ()			
+		return {
+			"status": status
+		}	
 
+	raise Exception (f"Kind '{ kind }' was not found.")
```

### Comparing `ventures-1.3.3/venues/stages/ventures/plays/turn_off.py` & `ventures-1.4.0/venues/stages/ventures/plays/turn_off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays/turn_off_v1.py` & `ventures-1.4.0/venues/stages/ventures/plays/turn_off_v1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays/turn_on.py` & `ventures-1.4.0/venues/stages/ventures/plays/turn_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays/turn_on_v1.py` & `ventures-1.4.0/venues/stages/ventures/plays/turn_on_v1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/plays_venture/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays_venture/turn_off/__init__.py` & `ventures-1.4.0/venues/stages/ventures/plays_venture/turn_off/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/plays_venture/turn_off/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays_venture/turn_on/__init__.py` & `ventures-1.4.0/venues/stages/ventures/plays_venture/turn_on/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/plays_venture/turn_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/readme.md` & `ventures-1.4.0/venues/stages/ventures/readme.md`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.4.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.4.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.4.0/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.4.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.4.0/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.3.3/PKG-INFO` & `ventures-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.3.3
+Version: 1.4.0
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

