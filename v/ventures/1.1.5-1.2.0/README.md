# Comparing `tmp/ventures-1.1.5.tar.gz` & `tmp/ventures-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.1.5.tar", max compression
+gzip compressed data, was "ventures-1.2.0.tar", max compression
```

## Comparing `ventures-1.1.5.tar` & `ventures-1.2.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rwxr-xr-x   0        0        0      567 2024-05-20 03:47:11.426543 ventures-1.1.5/pyproject.toml
--rwxr-xr-x   0        0        0     1120 2024-05-18 18:56:41.459616 ventures-1.1.5/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.1.5/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.1.5/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.1.5/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.1.5/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.1.5/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.1.5/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   197026 2024-05-20 03:44:27.204359 ventures-1.1.5/venues/stages/ventures/_status/DB/records.json
--rwxr-xr-x   0        0        0     1217 2024-05-20 03:37:43.477222 ventures-1.1.5/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1133 2024-05-20 03:37:22.901492 ventures-1.1.5/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-20 03:44:24.108394 ventures-1.1.5/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1283 2024-05-19 23:18:17.298859 ventures-1.1.5/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1428 2024-05-18 02:01:33.088701 ventures-1.1.5/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-20 03:44:26.144371 ventures-1.1.5/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rwxr-xr-x   0        0        0      964 2024-05-20 01:26:25.762311 ventures-1.1.5/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      767 2024-05-20 01:26:19.954331 ventures-1.1.5/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-20 03:44:24.408390 ventures-1.1.5/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.1.5/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.1.5/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.1.5/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.1.5/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      463 2024-05-18 01:29:56.857560 ventures-1.1.5/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.1.5/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.1.5/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1133 2024-05-18 18:53:30.969670 ventures-1.1.5/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1755 2024-05-20 00:56:07.601346 ventures-1.1.5/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1716 2024-05-20 00:59:57.187843 ventures-1.1.5/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1200 2024-05-18 18:45:09.731099 ventures-1.1.5/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0     2439 2024-05-20 00:56:04.745365 ventures-1.1.5/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     2835 2024-05-20 00:59:51.107883 ventures-1.1.5/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.1.5/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:56.689210 ventures-1.1.5/venues/stages/ventures/plays_venture/turn_off.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:52.973247 ventures-1.1.5/venues/stages/ventures/plays_venture/turn_on.py
--rwxr-xr-x   0        0        0     1377 2024-05-20 03:44:44.816161 ventures-1.1.5/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.1.5/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2190 2024-05-20 03:35:10.195306 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive/__init__.py
--rwxr-xr-x   0        0        0     1709 2024-05-20 03:35:20.863155 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.1.5/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      486 2024-05-17 22:53:36.062918 ventures-1.1.5/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.1.5/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      230 2024-05-17 22:53:33.130949 ventures-1.1.5/venues/stages/ventures/utilities/map/scan.py
--rwxr-xr-x   0        0        0      919 2024-05-20 00:48:43.604121 ventures-1.1.5/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      676 2024-05-20 00:48:36.716162 ventures-1.1.5/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.1.5/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      381 2024-05-18 03:46:35.268323 ventures-1.1.5/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      181 2024-05-18 03:46:08.652619 ventures-1.1.5/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.1.5/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 ventures-1.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2024-05-21 20:28:19.492089 ventures-1.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1120 2024-05-18 18:56:41.459616 ventures-1.2.0/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.2.0/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.2.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.2.0/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.2.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.2.0/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.2.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   199523 2024-05-21 20:28:06.460223 ventures-1.2.0/venues/stages/ventures/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1217 2024-05-20 03:37:43.477222 ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1133 2024-05-20 03:37:22.901492 ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-21 20:28:04.452244 ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1283 2024-05-19 23:18:17.298859 ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1428 2024-05-18 02:01:33.088701 ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-21 20:28:05.504233 ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rwxr-xr-x   0        0        0      964 2024-05-20 01:26:25.762311 ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      767 2024-05-20 01:26:19.954331 ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-21 20:28:04.836240 ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rwxr-xr-x   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.2.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.2.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.2.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.2.0/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      463 2024-05-18 01:29:56.857560 ventures-1.2.0/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.2.0/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.2.0/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1133 2024-05-18 18:53:30.969670 ventures-1.2.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1755 2024-05-20 00:56:07.601346 ventures-1.2.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rw-r--r--   0        0        0     1857 2024-05-21 20:24:20.198551 ventures-1.2.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1200 2024-05-18 18:45:09.731099 ventures-1.2.0/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0     2439 2024-05-20 00:56:04.745365 ventures-1.2.0/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     3140 2024-05-21 20:24:14.846606 ventures-1.2.0/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.2.0/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:56.689210 ventures-1.2.0/venues/stages/ventures/plays_venture/turn_off.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:52.973247 ventures-1.2.0/venues/stages/ventures/plays_venture/turn_on.py
+-rwxr-xr-x   0        0        0     1377 2024-05-20 03:44:44.816161 ventures-1.2.0/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.2.0/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2455 2024-05-21 20:21:09.968507 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rw-r--r--   0        0        0     1911 2024-05-21 20:21:12.308483 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.2.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      486 2024-05-17 22:53:36.062918 ventures-1.2.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.2.0/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      230 2024-05-17 22:53:33.130949 ventures-1.2.0/venues/stages/ventures/utilities/map/scan.py
+-rwxr-xr-x   0        0        0      919 2024-05-20 00:48:43.604121 ventures-1.2.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      676 2024-05-20 00:48:36.716162 ventures-1.2.0/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.2.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      381 2024-05-18 03:46:35.268323 ventures-1.2.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      181 2024-05-18 03:46:08.652619 ventures-1.2.0/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.2.0/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 ventures-1.2.0/PKG-INFO
```

### Comparing `ventures-1.1.5/venues/stages/ventures/__init__.py` & `ventures-1.2.0/venues/stages/ventures/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.2.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/DB/records.json` & `ventures-1.2.0/venues/stages/ventures/_status/DB/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795918367346939%*

 * *Differences: {"'_default'": "{'48': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [4.3299951357766986e-07, 'seconds']), ('passed', "*

 * *               "True)])]), ('empty', False), ('parsed', True), ('path', 'status_1.py'), "*

 * *               "('records', []), ('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), "*

 * *               "OrderedDict([('checks', [OrderedDict([('check', 'check 1'), ('elapsed', "*

 * *               "[6.469999789260328e-07, 'seconds']) […]*

```diff
@@ -5710,14 +5710,244 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "48": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.3299951357766986e-07,
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
+                                6.469999789260328e-07,
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
+                                3.1337444400014647,
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
+                                3.090754388998903,
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
+                                2.103997731999698,
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
+        "49": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.669994713272899e-07,
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
+                                4.130015440750867e-07,
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
+                                3.14988380000068,
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
+                                2.3328633659984916,
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
+                                3.0947805029973097,
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
         "5": {
             "alarms": [],
             "paths": [],
             "stats": {
                 "checks": {
                     "alarms": 0,
                     "passes": 0
```

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.2.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.2.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.2.0/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status.proc.py` & `ventures-1.2.0/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.2.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 20 00:59:51 2024 UTC, .py size: 2835 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,117 @@
-00000000: 6f0d 0d0a 0000 0000 87a0 4a66 130b 0000  o.........Jf....
+00000000: 6f0d 0d0a 0000 0000 ee02 4d66 440c 0000  o.........MfD...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 5a0a 6405 6407 6c0b 5a0b 6405 6407 6c0c  Z.d.d.l.Z.d.d.l.
 00000080: 5a0c 0900 6408 6409 8400 5a0d 6407 5300  Z...d.d...Z.d.S.
 00000090: 290a e902 0000 0029 01da 0c68 696b 655f  )......)...hike_
 000000a0: 7061 7373 6976 6529 01da 0865 7463 685f  passive)...etch_
 000000b0: 6d61 7029 01da 0873 6361 6e5f 6d61 7029  map)...scan_map)
 000000c0: 01da 0c66 696e 645f 7665 6e74 7572 65e9  ...find_venture.
 000000d0: 0000 0000 2901 da0b 6368 6563 6b5f 6973  ....)...check_is
 000000e0: 5f6f 6e4e 6301 0000 0000 0000 0000 0000  _onNc...........
-000000f0: 000c 0000 0008 0000 0043 0000 0073 e401  .........C...s..
+000000f0: 000d 0000 0008 0000 0043 0000 0073 2a02  .........C...s*.
 00000100: 0000 7c00 6401 1900 7d01 7c00 6402 1900  ..|.d...}.|.d...
 00000110: 7d02 6900 7d03 7400 6a01 a002 7c02 a101  }.i.}.t.j...|...
 00000120: 7216 7403 6403 7c02 6901 8301 7d03 7c01  r.t.d.|.i...}.|.
-00000130: 4400 5dd0 7d04 7c04 6404 1900 6405 1900  D.].}.|.d...d...
+00000130: 4400 5df3 7d04 7c04 6404 1900 6405 1900  D.].}.|.d...d...
 00000140: 7d05 7c04 6406 1900 7d06 7c04 6407 1900  }.|.d...}.|.d...
 00000150: 7d07 7c07 7c03 7600 7258 7c06 6408 6b02  }.|.|.v.rX|.d.k.
 00000160: 7245 7c03 7c07 1900 6408 1900 6409 6b03  rE|.|...d...d.k.
 00000170: 7245 7404 7c03 7c07 1900 6408 1900 8301  rEt.|.|...d.....
 00000180: 7d08 7c08 640a 6b02 7245 7118 7c06 640b  }.|.d.k.rEq.|.d.
 00000190: 6b02 7258 7405 7c01 7c07 8302 7d09 7c09  k.rXt.|.|...}.|.
 000001a0: 640c 1900 8300 7d08 7c08 640a 6b02 7258  d.....}.|.d.k.rX
-000001b0: 7118 7c06 6408 6b02 72a0 7406 640d 7c05  q.|.d.k.r.t.d.|.
-000001c0: 6901 8301 7d0a 640e 7d0b 0900 7404 7c0a  i...}.d.}...t.|.
-000001d0: 6408 1900 8301 7d08 7407 6a08 6410 6411  d.....}.t.j.d.d.
-000001e0: 7c0b 7c07 7c08 6412 9c04 6901 6413 8d01  |.|.|.d...i.d...
-000001f0: 0100 7c08 640a 6b02 727d 6e19 7409 a00a  ..|.d.k.r}n.t...
-00000200: 6414 a101 0100 7c0b 6414 3700 7d0b 7c0b  d.....|.d.7.}.|.
-00000210: 6415 6b02 7295 740b 6416 7c0b 9b00 6417  d.k.r.t.d.|...d.
-00000220: 7c07 9b00 6418 9d05 8301 8201 7165 7c06  |...d.......qe|.
-00000230: 7c0a 6408 1900 6419 9c02 7c03 7c07 3c00  |.d...d...|.|.<.
-00000240: 7118 7c06 640b 6b02 72e1 7c05 8300 0100  q.|.d.k.r.|.....
-00000250: 640e 7d0b 0900 7c04 640c 1900 8300 7d08  d.}...|.d.....}.
-00000260: 7407 6a08 6410 6411 7c0b 7c07 7c08 6412  t.j.d.d.|.|.|.d.
-00000270: 9c04 6901 6413 8d01 0100 7c08 640a 6b02  ..i.d.....|.d.k.
-00000280: 72c1 6e19 7409 a00a 6414 a101 0100 7c0b  r.n.t...d.....|.
-00000290: 6414 3700 7d0b 7c0b 6415 6b02 72d9 740b  d.7.}.|.d.k.r.t.
-000002a0: 6416 7c0b 9b00 6417 7c07 9b00 6418 9d05  d.|...d.|...d...
-000002b0: 8301 8201 71aa 6406 7c06 6901 7c03 7c07  ....q.d.|.i.|.|.
-000002c0: 3c00 7118 740b 641a 7c06 9b00 641b 9d03  <.q.t.d.|...d...
-000002d0: 8301 8201 740c 7c02 7c03 641c 9c02 8301  ....t.|.|.d.....
-000002e0: 0100 7c03 5300 291d 4eda 0876 656e 7475  ..|.S.).N..ventu
-000002f0: 7265 73da 036d 6170 da04 7061 7468 7a07  res..map..pathz.
-00000300: 7475 726e 206f 6eda 0961 6476 656e 7475  turn on..adventu
-00000310: 7265 da04 6b69 6e64 da04 6e61 6d65 da10  re..kind..name..
-00000320: 7072 6f63 6573 735f 6964 656e 7469 7479  process_identity
-00000330: da00 da02 6f6e da04 7461 736b 7a05 6973  ....on..taskz.is
-00000340: 206f 6eda 0673 6372 6970 7472 0600 0000   on..scriptr....
-00000350: 547a 1976 656e 7475 7265 2073 7461 7475  Tz.venture statu
-00000360: 7320 6368 6563 6b20 6c6f 6f70 7a16 6166  s check loopz.af
-00000370: 7465 7220 7475 726e 206f 6e20 7761 7320  ter turn on was 
-00000380: 7365 6e74 2904 da04 7768 656e da04 6c6f  sent)...when..lo
-00000390: 6f70 720d 0000 00da 0673 7461 7475 7329  opr......status)
-000003a0: 01da 0464 6174 61e9 0100 0000 e90a 0000  ...data.........
-000003b0: 007a 0641 6674 6572 207a 0820 6c6f 6f70  .z.After z. loop
-000003c0: 732c 207a 1120 6469 6420 6e6f 7420 7475  s, z. did not tu
-000003d0: 726e 206f 6e2e 2902 720c 0000 0072 0e00  rn on.).r....r..
-000003e0: 0000 7a06 4b69 6e64 2022 7a0f 2077 6173  ..z.Kind "z. was
-000003f0: 206e 6f74 2066 6f75 6e64 2e29 0272 0a00   not found.).r..
-00000400: 0000 da07 6272 6163 6b65 7429 0dda 026f  ....bracket)...o
-00000410: 7372 0a00 0000 da06 6578 6973 7473 7204  sr......existsr.
-00000420: 0000 0072 0700 0000 7205 0000 0072 0200  ...r....r....r..
-00000430: 0000 da04 7269 6368 da0a 7072 696e 745f  ....rich..print_
-00000440: 6a73 6f6e da04 7469 6d65 da05 736c 6565  json..time..slee
-00000450: 70da 0945 7863 6570 7469 6f6e 7203 0000  p..Exceptionr...
-00000460: 0029 0cda 0670 6163 6b65 7472 0800 0000  .)...packetr....
-00000470: da0c 7468 655f 6d61 705f 7061 7468 da14  ..the_map_path..
-00000480: 7665 6e74 7572 6573 5f6d 6170 5f62 7261  ventures_map_bra
-00000490: 636b 6574 720b 0000 00da 1061 6476 656e  cketr......adven
-000004a0: 7475 7265 5f73 6372 6970 7472 0c00 0000  ture_scriptr....
-000004b0: 720d 0000 0072 1500 0000 da07 7665 6e74  r....r......vent
-000004c0: 7572 65da 0770 726f 6365 7373 7214 0000  ure..processr...
-000004d0: 00a9 0072 2700 0000 fa30 2f68 6162 6974  ...r'....0/habit
-000004e0: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
-000004f0: 2f76 656e 7475 7265 732f 706c 6179 732f  /ventures/plays/
-00000500: 7475 726e 5f6f 6e2e 7079 da07 7475 726e  turn_on.py..turn
-00000510: 5f6f 6e27 0000 0073 a000 0000 0801 0801  _on'...s........
-00000520: 0402 0c01 0201 0401 06ff 0804 0c01 0801  ................
-00000530: 0801 0807 0801 1001 1001 0801 0202 0802  ................
-00000540: 0a01 0a01 0801 0201 0804 0201 0401 06ff  ................
-00000550: 0404 0201 0c01 0401 0201 0201 0201 0201  ................
-00000560: 0201 04fc 08ff 0809 0201 0a02 0802 0801  ................
-00000570: 0201 1001 04ff 02ee 0217 0601 0afe 0205  ................
-00000580: 0802 0601 0402 0201 0a01 0401 0201 0201  ................
-00000590: 0201 0201 0201 04fc 08ff 0809 0201 0a02  ................
-000005a0: 0802 0801 0201 1001 04ff 02ee 0417 0aff  ................
-000005b0: 1006 0203 0201 0201 08fe 0405 7229 0000  ............r)..
-000005c0: 0029 0eda 1675 7469 6c69 7469 6573 2e68  .)...utilities.h
-000005d0: 696b 655f 7061 7373 6976 6572 0200 0000  ike_passiver....
-000005e0: da12 7574 696c 6974 6965 732e 6d61 702e  ..utilities.map.
-000005f0: 6574 6368 7203 0000 00da 1275 7469 6c69  etchr......utili
-00000600: 7469 6573 2e6d 6170 2e73 6361 6e72 0400  ties.map.scanr..
-00000610: 0000 da1f 7574 696c 6974 6965 732e 7665  ....utilities.ve
-00000620: 6e74 7572 6573 2e66 696e 645f 7665 6e74  ntures.find_vent
-00000630: 7572 6572 0500 0000 da26 7665 6e74 7572  urer.....&ventur
-00000640: 6573 2e75 7469 6c69 7469 6573 2e70 726f  es.utilities.pro
-00000650: 6365 7373 2e63 6865 636b 5f69 735f 6f6e  cess.check_is_on
-00000660: 7207 0000 0072 1c00 0000 721a 0000 0072  r....r....r....r
-00000670: 1e00 0000 7229 0000 0072 2700 0000 7227  ....r)...r'...r'
-00000680: 0000 0072 2700 0000 7228 0000 00da 083c  ...r'...r(.....<
-00000690: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
-000006a0: 0c03 0c01 0c01 0c01 0c02 0803 0803 0801  ................
-000006b0: 0204 0c13                                ....
+000001b0: 7118 7c06 6408 6b02 72c2 7406 640d 7c04  q.|.d.k.r.t.d.|.
+000001c0: 8302 0100 6900 7d0a 6404 7c04 7600 727d  ....i.}.d.|.v.r}
+000001d0: 640e 7c04 6404 1900 7600 727d 7407 7c04  d.|.d...v.r}t.|.
+000001e0: 6404 1900 640e 1900 8301 7408 6b02 727d  d...d.....t.k.r}
+000001f0: 7c04 6404 1900 640e 1900 7d0a 7409 7c05  |.d...d...}.t.|.
+00000200: 7c0a 640f 9c02 8301 7d0b 6410 7d0c 0900  |.d.....}.d.}...
+00000210: 7404 7c0b 6408 1900 8301 7d08 740a 6a0b  t.|.d.....}.t.j.
+00000220: 6412 6413 7c0c 7c07 7c08 6414 9c04 6901  d.d.|.|.|.d...i.
+00000230: 6415 8d01 0100 7c08 640a 6b02 729f 6e19  d.....|.d.k.r.n.
+00000240: 740c a00d 6416 a101 0100 7c0c 6416 3700  t...d.....|.d.7.
+00000250: 7d0c 7c0c 6417 6b02 72b7 740e 6418 7c0c  }.|.d.k.r.t.d.|.
+00000260: 9b00 6419 7c07 9b00 641a 9d05 8301 8201  ..d.|...d.......
+00000270: 7187 7c06 7c0b 6408 1900 641b 9c02 7c03  q.|.|.d...d...|.
+00000280: 7c07 3c00 7118 7c06 640b 6b02 9001 7204  |.<.q.|.d.k...r.
+00000290: 7c05 8300 0100 6410 7d0c 0900 7c04 640c  |.....d.}...|.d.
+000002a0: 1900 8300 7d08 740a 6a0b 6412 6413 7c0c  ....}.t.j.d.d.|.
+000002b0: 7c07 7c08 6414 9c04 6901 6415 8d01 0100  |.|.d...i.d.....
+000002c0: 7c08 640a 6b02 72e4 6e19 740c a00d 6416  |.d.k.r.n.t...d.
+000002d0: a101 0100 7c0c 6416 3700 7d0c 7c0c 6417  ....|.d.7.}.|.d.
+000002e0: 6b02 72fc 740e 6418 7c0c 9b00 6419 7c07  k.r.t.d.|...d.|.
+000002f0: 9b00 641a 9d05 8301 8201 71cd 6406 7c06  ..d.......q.d.|.
+00000300: 6901 7c03 7c07 3c00 7118 740e 641c 7c06  i.|.|.<.q.t.d.|.
+00000310: 9b00 641d 9d03 8301 8201 740f 7c02 7c03  ..d.......t.|.|.
+00000320: 641e 9c02 8301 0100 7c03 5300 291f 4eda  d.......|.S.).N.
+00000330: 0876 656e 7475 7265 73da 036d 6170 da04  .ventures..map..
+00000340: 7061 7468 7a07 7475 726e 206f 6eda 0961  pathz.turn on..a
+00000350: 6476 656e 7475 7265 da04 6b69 6e64 da04  dventure..kind..
+00000360: 6e61 6d65 da10 7072 6f63 6573 735f 6964  name..process_id
+00000370: 656e 7469 7479 da00 da02 6f6e da04 7461  entity....on..ta
+00000380: 736b 7a05 6973 206f 6e7a 0a61 6476 656e  skz.is onz.adven
+00000390: 7475 7265 3ada 0550 6f70 656e 2902 da06  ture:..Popen)...
+000003a0: 7363 7269 7074 7212 0000 0072 0600 0000  scriptr....r....
+000003b0: 547a 1976 656e 7475 7265 2073 7461 7475  Tz.venture statu
+000003c0: 7320 6368 6563 6b20 6c6f 6f70 7a16 6166  s check loopz.af
+000003d0: 7465 7220 7475 726e 206f 6e20 7761 7320  ter turn on was 
+000003e0: 7365 6e74 2904 da04 7768 656e da04 6c6f  sent)...when..lo
+000003f0: 6f70 720d 0000 00da 0673 7461 7475 7329  opr......status)
+00000400: 01da 0464 6174 61e9 0100 0000 e90a 0000  ...data.........
+00000410: 007a 0641 6674 6572 207a 0820 6c6f 6f70  .z.After z. loop
+00000420: 732c 207a 1120 6469 6420 6e6f 7420 7475  s, z. did not tu
+00000430: 726e 206f 6e2e 2902 720c 0000 0072 0e00  rn on.).r....r..
+00000440: 0000 7a06 4b69 6e64 2022 7a0f 2077 6173  ..z.Kind "z. was
+00000450: 206e 6f74 2066 6f75 6e64 2e29 0272 0a00   not found.).r..
+00000460: 0000 da07 6272 6163 6b65 7429 10da 026f  ....bracket)...o
+00000470: 7372 0a00 0000 da06 6578 6973 7473 7204  sr......existsr.
+00000480: 0000 0072 0700 0000 7205 0000 00da 0570  ...r....r......p
+00000490: 7269 6e74 da04 7479 7065 da04 6469 6374  rint..type..dict
+000004a0: 7202 0000 00da 0472 6963 68da 0a70 7269  r......rich..pri
+000004b0: 6e74 5f6a 736f 6eda 0474 696d 65da 0573  nt_json..time..s
+000004c0: 6c65 6570 da09 4578 6365 7074 696f 6e72  leep..Exceptionr
+000004d0: 0300 0000 290d da06 7061 636b 6574 7208  ....)...packetr.
+000004e0: 0000 00da 0c74 6865 5f6d 6170 5f70 6174  .....the_map_pat
+000004f0: 68da 1476 656e 7475 7265 735f 6d61 705f  h..ventures_map_
+00000500: 6272 6163 6b65 7472 0b00 0000 da10 6164  bracketr......ad
+00000510: 7665 6e74 7572 655f 7363 7269 7074 720c  venture_scriptr.
+00000520: 0000 0072 0d00 0000 7216 0000 00da 0776  ...r....r......v
+00000530: 656e 7475 7265 da0a 506f 7065 6e5f 6b65  enture..Popen_ke
+00000540: 7973 da07 7072 6f63 6573 7372 1500 0000  ys..processr....
+00000550: a900 722c 0000 00fa 302f 6861 6269 7461  ..r,....0/habita
+00000560: 742f 7665 6e75 6573 2f73 7461 6765 732f  t/venues/stages/
+00000570: 7665 6e74 7572 6573 2f70 6c61 7973 2f74  ventures/plays/t
+00000580: 7572 6e5f 6f6e 2e70 79da 0774 7572 6e5f  urn_on.py..turn_
+00000590: 6f6e 2a00 0000 73ae 0000 0008 0108 0104  on*...s.........
+000005a0: 040c 0102 0104 0106 ff08 040c 0108 0108  ................
+000005b0: 0108 0708 0110 0110 0108 0102 0208 020a  ................
+000005c0: 010a 0108 0102 0108 040a 0104 0208 010c  ................
+000005d0: 0114 010c 0102 0202 0102 0108 fe04 0502  ................
+000005e0: 010c 0104 0102 0102 0102 0102 0102 0104  ................
+000005f0: fc08 ff08 0902 010a 0208 0208 0102 0110  ................
+00000600: 0104 ff02 ee02 1706 010a fe02 050a 0206  ................
+00000610: 0104 0202 010a 0104 0102 0102 0102 0102  ................
+00000620: 0102 0104 fc08 ff08 0902 010a 0208 0208  ................
+00000630: 0102 0110 0104 ff02 ee04 170a ff10 0602  ................
+00000640: 0302 0102 0108 fe04 0572 2e00 0000 290e  .........r....).
+00000650: da16 7574 696c 6974 6965 732e 6869 6b65  ..utilities.hike
+00000660: 5f70 6173 7369 7665 7202 0000 00da 1275  _passiver......u
+00000670: 7469 6c69 7469 6573 2e6d 6170 2e65 7463  tilities.map.etc
+00000680: 6872 0300 0000 da12 7574 696c 6974 6965  hr......utilitie
+00000690: 732e 6d61 702e 7363 616e 7204 0000 00da  s.map.scanr.....
+000006a0: 1f75 7469 6c69 7469 6573 2e76 656e 7475  .utilities.ventu
+000006b0: 7265 732e 6669 6e64 5f76 656e 7475 7265  res.find_venture
+000006c0: 7205 0000 00da 2676 656e 7475 7265 732e  r.....&ventures.
+000006d0: 7574 696c 6974 6965 732e 7072 6f63 6573  utilities.proces
+000006e0: 732e 6368 6563 6b5f 6973 5f6f 6e72 0700  s.check_is_onr..
+000006f0: 0000 7220 0000 0072 1b00 0000 7222 0000  ..r ...r....r"..
+00000700: 0072 2e00 0000 722c 0000 0072 2c00 0000  .r....r,...r,...
+00000710: 722c 0000 0072 2d00 0000 da08 3c6d 6f64  r,...r-.....<mod
+00000720: 756c 653e 0100 0000 7314 0000 000c 030c  ule>....s.......
+00000730: 010c 010c 010c 0208 0308 0308 0102 040c  ................
+00000740: 16                                       .
```

### Comparing `ventures-1.1.5/venues/stages/ventures/plays/is_on.py` & `ventures-1.2.0/venues/stages/ventures/plays/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/plays/turn_off.py` & `ventures-1.2.0/venues/stages/ventures/plays/turn_off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/plays/turn_on.py` & `ventures-1.2.0/venues/stages/ventures/plays/turn_on.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 #++++
 
 '''
 	{
 		"name": "adventure_1",
 		"turn on": {
 			"adventure": "python3 -m http.server 8080",
-			"kind": "process_identity"
+			"kind": "process_identity",
+			"Popen": {
+				"CWD": 
+			},
 		}
 	}
 	
 	{
 		"name": "adventure_2",
 		"turn on": {
 			"adventure": turn_on,
@@ -36,14 +39,16 @@
 '''
 
 
 def turn_on (packet):
 	ventures = packet ["ventures"]
 	the_map_path = packet ["map"]
 	
+	
+
 	ventures_map_bracket = {}
 	if os.path.exists (the_map_path):
 		ventures_map_bracket = scan_map ({
 			"path": the_map_path
 		})
 
 	for adventure in ventures:
@@ -69,16 +74,25 @@
 				status = venture ["is on"] ()
 				if (status == "on"):
 					continue;
 
 		
 		
 		if (kind == "process_identity"):
+			print ("adventure:", adventure)
+		
+			Popen_keys = {}
+			if ("turn on" in adventure):
+				if ("Popen" in adventure ["turn on"]):
+					if (type (adventure ["turn on"] ["Popen"]) == dict):
+						Popen_keys = adventure ["turn on"] ["Popen"]
+		
 			process = hike_passive ({
-				"script": adventure_script
+				"script": adventure_script,
+				"Popen": Popen_keys
 			})
 			
 			loop = 0
 			while True:
 				status = check_is_on (process ["process_identity"])	
 				rich.print_json (data = {
 					"venture status check loop": {
```

### Comparing `ventures-1.1.5/venues/stages/ventures/readme.md` & `ventures-1.2.0/venues/stages/ventures/readme.md`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #++++
 #
 from ventures.utilities.hike_passive_p_expect import hike_passive_p_expect
 from ventures.utilities.hike_passive_p_expect_2.implicit import process_on_implicit
 #
 #
 import rich
+from pydash import merge
 #
 #
 from fractions import Fraction
 import multiprocessing
 import subprocess
 import time
 import os
@@ -42,14 +43,19 @@
 #
 #++++
 
 
 def hike_passive (packet):
 	script = packet ["script"]
 
+	Popen_keys = {}
+	if ("Popen" in packet):
+		if (type (packet ["Popen"]) == dict):
+			Popen_keys = packet ["Popen"]
+
 	def daemonize ():
 		# Fork the parent process
 		pid = os.fork ()
 		if pid > 0:
 			# Exit the parent process
 			sys.exit (0)
 
@@ -104,18 +110,24 @@
 			os._exit (0)
 		else:
 			# This is the parent process
 			# Return the PID of the child process
 			return pid
 
 
+	merged_dict = merge ({
+		"close_fds": True
+	}, Popen_keys)
+
+	print ("merged_dict:", merged_dict)
+	print ("packet:", packet)	
 
 	the_process = subprocess.Popen (
 		script,
-		close_fds = True
+		** merged_dict
 	)
 	
 	return {
 		"process_identity": the_process.pid
 	}
 
 	#command_to_execute = the_procedure
```

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 20 03:35:10 2024 UTC, .py size: 2190 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,120 @@
-00000000: 6f0d 0d0a 0000 0000 eec4 4a66 8e08 0000  o.........Jf....
+00000000: 6f0d 0d0a 0000 0000 3502 4d66 9709 0000  o.......5.Mf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
+00000020: 0002 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 0100 6401 6404  d.d.l.m.Z...d.d.
 00000050: 6c05 5a05 6401 6405 6c06 6d07 5a07 0100  l.Z.d.d.l.m.Z...
-00000060: 6401 6404 6c08 5a08 6401 6404 6c09 5a09  d.d.l.Z.d.d.l.Z.
-00000070: 6401 6404 6c0a 5a0a 6401 6404 6c0b 5a0b  d.d.l.Z.d.d.l.Z.
-00000080: 6401 6404 6c0c 5a0c 6401 6404 6c0b 5a0b  d.d.l.Z.d.d.l.Z.
-00000090: 6401 6404 6c0d 5a0d 6401 6404 6c09 5a09  d.d.l.Z.d.d.l.Z.
-000000a0: 6406 6407 8400 5a0e 6404 5300 2908 7a6e  d.d...Z.d.S.).zn
-000000b0: 0a09 6672 6f6d 2076 6163 6369 6e65 732e  ..from vaccines.
-000000c0: 6d69 7865 732e 7665 6e74 7572 6573 5f6d  mixes.ventures_m
-000000d0: 6170 2e68 696b 655f 7061 7373 6976 6520  ap.hike_passive 
-000000e0: 696d 706f 7274 2068 696b 655f 7061 7373  import hike_pass
-000000f0: 6976 650a 0968 696b 655f 7061 7373 6976  ive..hike_passiv
-00000100: 6520 287b 0a09 0922 7363 7269 7074 223a  e ({..."script":
-00000110: 205b 0a09 090a 0909 5d0a 097d 290a e900   [......]..})...
-00000120: 0000 0029 01da 1568 696b 655f 7061 7373  ...)...hike_pass
-00000130: 6976 655f 705f 6578 7065 6374 2901 da13  ive_p_expect)...
-00000140: 7072 6f63 6573 735f 6f6e 5f69 6d70 6c69  process_on_impli
-00000150: 6369 744e 2901 da08 4672 6163 7469 6f6e  citN)...Fraction
-00000160: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-00000170: 0004 0000 0003 0000 0073 3400 0000 7c00  .........s4...|.
-00000180: 6401 1900 7d01 6402 6403 8400 8900 8700  d...}.d.d.......
-00000190: 6601 6404 6405 8408 7d02 7400 6a01 7c01  f.d.d...}.t.j.|.
-000001a0: 6406 6407 8d02 7d03 6408 7c03 6a02 6901  d.d...}.d.|.j.i.
-000001b0: 5300 2909 4eda 0673 6372 6970 7463 0000  S.).N..scriptc..
-000001c0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000001d0: 0000 5300 0000 739c 0000 0074 00a0 01a1  ..S...s....t....
-000001e0: 007d 007c 0064 016b 0472 0d74 02a0 0364  .}.|.d.k.r.t...d
-000001f0: 01a1 0101 0074 00a0 04a1 0001 0074 00a0  .....t.......t..
-00000200: 01a1 007d 007c 0064 016b 0472 1e74 02a0  ...}.|.d.k.r.t..
-00000210: 0364 01a1 0101 0074 00a0 0564 02a1 0101  .d.....t...d....
-00000220: 0074 00a0 0664 01a1 0101 0074 026a 07a0  .t...d.....t.j..
-00000230: 08a1 0001 0074 026a 09a0 08a1 0001 0074  .....t.j.......t
-00000240: 026a 0aa0 08a1 0001 0074 0b74 006a 0c64  .j.......t.t.j.d
-00000250: 0383 0274 025f 0774 0b74 006a 0c64 0483  ...t._.t.t.j.d..
-00000260: 0274 025f 0974 0b74 006a 0c64 0483 0274  .t._.t.t.j.d...t
-00000270: 025f 0a64 0053 0029 054e 7201 0000 00fa  ._.d.S.).Nr.....
-00000280: 012f da01 72da 0177 290d da02 6f73 da04  ./..r..w)...os..
-00000290: 666f 726b da03 7379 73da 0465 7869 74da  fork..sys..exit.
-000002a0: 0673 6574 7369 64da 0563 6864 6972 da05  .setsid..chdir..
-000002b0: 756d 6173 6bda 0573 7464 696e da05 636c  umask..stdin..cl
-000002c0: 6f73 65da 0673 7464 6f75 74da 0673 7464  ose..stdout..std
-000002d0: 6572 72da 046f 7065 6eda 0764 6576 6e75  err..open..devnu
-000002e0: 6c6c 2901 da03 7069 64a9 0072 1700 0000  ll)...pid..r....
-000002f0: fa42 2f68 6162 6974 6174 2f76 656e 7565  .B/habitat/venue
-00000300: 732f 7374 6167 6573 2f76 656e 7475 7265  s/stages/venture
-00000310: 732f 7574 696c 6974 6965 732f 6869 6b65  s/utilities/hike
-00000320: 5f70 6173 7369 7665 2f5f 5f69 6e69 745f  _passive/__init_
-00000330: 5f2e 7079 da09 6461 656d 6f6e 697a 6531  _.py..daemonize1
-00000340: 0000 0073 1e00 0000 0802 0801 0a02 0803  ...s............
-00000350: 0803 0801 0a02 0a03 0a03 0a03 0a01 0a01  ................
-00000360: 0e03 0e01 1201 7a1f 6869 6b65 5f70 6173  ......z.hike_pas
-00000370: 7369 7665 2e3c 6c6f 6361 6c73 3e2e 6461  sive.<locals>.da
-00000380: 656d 6f6e 697a 6563 0100 0000 0000 0000  emonizec........
-00000390: 0000 0000 0400 0000 0400 0000 1300 0000  ................
-000003a0: 734a 0000 007c 0064 0119 007d 0174 00a0  sJ...|.d...}.t..
-000003b0: 01a1 007d 027c 0264 026b 0272 2388 0083  ...}.|.d.k.r#...
-000003c0: 0001 0074 026a 037c 0164 0364 048d 027d  ...t.j.|.d.d...}
-000003d0: 0374 0464 057c 036a 0583 0201 0074 00a0  .t.d.|.j.....t..
-000003e0: 0664 02a1 0101 0064 0053 007c 0253 0029  .d.....d.S.|.S.)
-000003f0: 064e 7205 0000 0072 0100 0000 5429 01da  .Nr....r....T)..
-00000400: 0573 6865 6c6c 7a33 0a09 0909 0a09 0909  .shellz3........
-00000410: 0a09 0909 0963 6869 6c64 2070 726f 6365  .....child proce
-00000420: 7373 2070 6964 3a0a 0909 0909 0a09 0909  ss pid:.........
-00000430: 090a 0909 0909 0a09 0909 0929 0772 0900  ...........).r..
-00000440: 0000 720a 0000 00da 0a73 7562 7072 6f63  ..r......subproc
-00000450: 6573 73da 0550 6f70 656e da05 7072 696e  ess..Popen..prin
-00000460: 7472 1600 0000 da05 5f65 7869 7429 04da  tr......_exit)..
-00000470: 0763 6f6d 6d61 6e64 7205 0000 0072 1600  .commandr....r..
-00000480: 0000 da0b 7468 655f 7072 6f63 6573 73a9  ....the_process.
-00000490: 0172 1900 0000 7217 0000 0072 1800 0000  .r....r....r....
-000004a0: da16 7374 6172 745f 6465 7461 6368 6564  ..start_detached
-000004b0: 5f70 726f 6365 7373 5100 0000 7314 0000  _processQ...s...
-000004c0: 0008 0108 0308 0206 030e 0204 0204 0704  ................
-000004d0: f90e 0a04 047a 2c68 696b 655f 7061 7373  .....z,hike_pass
-000004e0: 6976 652e 3c6c 6f63 616c 733e 2e73 7461  ive.<locals>.sta
-000004f0: 7274 5f64 6574 6163 6865 645f 7072 6f63  rt_detached_proc
-00000500: 6573 7354 2901 da09 636c 6f73 655f 6664  essT)...close_fd
-00000510: 73da 1070 726f 6365 7373 5f69 6465 6e74  s..process_ident
-00000520: 6974 7929 0572 1b00 0000 721c 0000 0072  ity).r....r....r
-00000530: 1600 0000 da04 6a6f 696e 721d 0000 0029  ......joinr....)
-00000540: 05da 0670 6163 6b65 7472 0500 0000 7222  ...packetr....r"
-00000550: 0000 0072 2000 0000 da14 6465 7461 6368  ...r .....detach
-00000560: 6564 5f70 726f 6365 7373 5f70 6964 7217  ed_process_pidr.
-00000570: 0000 0072 2100 0000 7218 0000 00da 0c68  ...r!...r......h
-00000580: 696b 655f 7061 7373 6976 652e 0000 0073  ike_passive....s
-00000590: 1200 0000 0801 0802 0c20 041f 0201 0201  ......... ......
-000005a0: 06fe 0606 04ff 7228 0000 0029 0fda 075f  ......r(...)..._
-000005b0: 5f64 6f63 5f5f da28 7665 6e74 7572 6573  _doc__.(ventures
-000005c0: 2e75 7469 6c69 7469 6573 2e68 696b 655f  .utilities.hike_
-000005d0: 7061 7373 6976 655f 705f 6578 7065 6374  passive_p_expect
-000005e0: 7202 0000 00da 3376 656e 7475 7265 732e  r.....3ventures.
-000005f0: 7574 696c 6974 6965 732e 6869 6b65 5f70  utilities.hike_p
-00000600: 6173 7369 7665 5f70 5f65 7870 6563 745f  assive_p_expect_
-00000610: 322e 696d 706c 6963 6974 7203 0000 00da  2.implicitr.....
-00000620: 0472 6963 68da 0966 7261 6374 696f 6e73  .rich..fractions
-00000630: 7204 0000 00da 0f6d 756c 7469 7072 6f63  r......multiproc
-00000640: 6573 7369 6e67 721b 0000 00da 0474 696d  essingr......tim
-00000650: 6572 0900 0000 da06 6174 6578 6974 720b  er......atexitr.
-00000660: 0000 0072 2800 0000 7217 0000 0072 1700  ...r(...r....r..
-00000670: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
-00000680: 6f64 756c 653e 0100 0000 731e 0000 0004  odule>....s.....
-00000690: 0a02 090c 060c 0108 030c 0308 0108 0108  ................
-000006a0: 0108 0108 0108 0108 0108 010c 05         .............
+00000060: 6401 6406 6c08 6d09 5a09 0100 6401 6404  d.d.l.m.Z...d.d.
+00000070: 6c0a 5a0a 6401 6404 6c0b 5a0b 6401 6404  l.Z.d.d.l.Z.d.d.
+00000080: 6c0c 5a0c 6401 6404 6c0d 5a0d 6401 6404  l.Z.d.d.l.Z.d.d.
+00000090: 6c0e 5a0e 6401 6404 6c0d 5a0d 6401 6404  l.Z.d.d.l.Z.d.d.
+000000a0: 6c0f 5a0f 6401 6404 6c0b 5a0b 6407 6408  l.Z.d.d.l.Z.d.d.
+000000b0: 8400 5a10 6404 5300 2909 7a6e 0a09 6672  ..Z.d.S.).zn..fr
+000000c0: 6f6d 2076 6163 6369 6e65 732e 6d69 7865  om vaccines.mixe
+000000d0: 732e 7665 6e74 7572 6573 5f6d 6170 2e68  s.ventures_map.h
+000000e0: 696b 655f 7061 7373 6976 6520 696d 706f  ike_passive impo
+000000f0: 7274 2068 696b 655f 7061 7373 6976 650a  rt hike_passive.
+00000100: 0968 696b 655f 7061 7373 6976 6520 287b  .hike_passive ({
+00000110: 0a09 0922 7363 7269 7074 223a 205b 0a09  ..."script": [..
+00000120: 090a 0909 5d0a 097d 290a e900 0000 0029  ....]..})......)
+00000130: 01da 1568 696b 655f 7061 7373 6976 655f  ...hike_passive_
+00000140: 705f 6578 7065 6374 2901 da13 7072 6f63  p_expect)...proc
+00000150: 6573 735f 6f6e 5f69 6d70 6c69 6369 744e  ess_on_implicitN
+00000160: 2901 da05 6d65 7267 6529 01da 0846 7261  )...merge)...Fra
+00000170: 6374 696f 6e63 0100 0000 0000 0000 0000  ctionc..........
+00000180: 0000 0700 0000 0400 0000 0300 0000 737e  ..............s~
+00000190: 0000 007c 0064 0119 007d 0169 007d 0264  ...|.d...}.i.}.d
+000001a0: 027c 0076 0072 1674 007c 0064 0219 0083  .|.v.r.t.|.d....
+000001b0: 0174 016b 0272 167c 0064 0219 007d 0264  .t.k.r.|.d...}.d
+000001c0: 0364 0484 0089 0087 0066 0164 0564 0684  .d.......f.d.d..
+000001d0: 087d 0374 0264 0764 0869 017c 0283 027d  .}.t.d.d.i.|...}
+000001e0: 0474 0364 097c 0483 0201 0074 0364 0a7c  .t.d.|.....t.d.|
+000001f0: 0083 0201 0074 046a 057c 0166 0169 007c  .....t.j.|.f.i.|
+00000200: 04a4 018e 017d 0564 0b7c 056a 0669 0153  .....}.d.|.j.i.S
+00000210: 0029 0c4e da06 7363 7269 7074 da05 506f  .).N..script..Po
+00000220: 7065 6e63 0000 0000 0000 0000 0000 0000  penc............
+00000230: 0100 0000 0300 0000 5300 0000 739c 0000  ........S...s...
+00000240: 0074 00a0 01a1 007d 007c 0064 016b 0472  .t.....}.|.d.k.r
+00000250: 0d74 02a0 0364 01a1 0101 0074 00a0 04a1  .t...d.....t....
+00000260: 0001 0074 00a0 01a1 007d 007c 0064 016b  ...t.....}.|.d.k
+00000270: 0472 1e74 02a0 0364 01a1 0101 0074 00a0  .r.t...d.....t..
+00000280: 0564 02a1 0101 0074 00a0 0664 01a1 0101  .d.....t...d....
+00000290: 0074 026a 07a0 08a1 0001 0074 026a 09a0  .t.j.......t.j..
+000002a0: 08a1 0001 0074 026a 0aa0 08a1 0001 0074  .....t.j.......t
+000002b0: 0b74 006a 0c64 0383 0274 025f 0774 0b74  .t.j.d...t._.t.t
+000002c0: 006a 0c64 0483 0274 025f 0974 0b74 006a  .j.d...t._.t.t.j
+000002d0: 0c64 0483 0274 025f 0a64 0053 0029 054e  .d...t._.d.S.).N
+000002e0: 7201 0000 00fa 012f da01 72da 0177 290d  r....../..r..w).
+000002f0: da02 6f73 da04 666f 726b da03 7379 73da  ..os..fork..sys.
+00000300: 0465 7869 74da 0673 6574 7369 64da 0563  .exit..setsid..c
+00000310: 6864 6972 da05 756d 6173 6bda 0573 7464  hdir..umask..std
+00000320: 696e da05 636c 6f73 65da 0673 7464 6f75  in..close..stdou
+00000330: 74da 0673 7464 6572 72da 046f 7065 6eda  t..stderr..open.
+00000340: 0764 6576 6e75 6c6c 2901 da03 7069 64a9  .devnull)...pid.
+00000350: 0072 1900 0000 fa42 2f68 6162 6974 6174  .r.....B/habitat
+00000360: 2f76 656e 7565 732f 7374 6167 6573 2f76  /venues/stages/v
+00000370: 656e 7475 7265 732f 7574 696c 6974 6965  entures/utilitie
+00000380: 732f 6869 6b65 5f70 6173 7369 7665 2f5f  s/hike_passive/_
+00000390: 5f69 6e69 745f 5f2e 7079 da09 6461 656d  _init__.py..daem
+000003a0: 6f6e 697a 6537 0000 0073 1e00 0000 0802  onize7...s......
+000003b0: 0801 0a02 0803 0803 0801 0a02 0a03 0a03  ................
+000003c0: 0a03 0a01 0a01 0e03 0e01 1201 7a1f 6869  ............z.hi
+000003d0: 6b65 5f70 6173 7369 7665 2e3c 6c6f 6361  ke_passive.<loca
+000003e0: 6c73 3e2e 6461 656d 6f6e 697a 6563 0100  ls>.daemonizec..
+000003f0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00000400: 0000 1300 0000 734a 0000 007c 0064 0119  ......sJ...|.d..
+00000410: 007d 0174 00a0 01a1 007d 027c 0264 026b  .}.t.....}.|.d.k
+00000420: 0272 2388 0083 0001 0074 026a 037c 0164  .r#......t.j.|.d
+00000430: 0364 048d 027d 0374 0464 057c 036a 0583  .d...}.t.d.|.j..
+00000440: 0201 0074 00a0 0664 02a1 0101 0064 0053  ...t...d.....d.S
+00000450: 007c 0253 0029 064e 7206 0000 0072 0100  .|.S.).Nr....r..
+00000460: 0000 5429 01da 0573 6865 6c6c 7a33 0a09  ..T)...shellz3..
+00000470: 0909 0a09 0909 0a09 0909 0963 6869 6c64  ...........child
+00000480: 2070 726f 6365 7373 2070 6964 3a0a 0909   process pid:...
+00000490: 0909 0a09 0909 090a 0909 0909 0a09 0909  ................
+000004a0: 0929 0772 0b00 0000 720c 0000 00da 0a73  .).r....r......s
+000004b0: 7562 7072 6f63 6573 7372 0700 0000 da05  ubprocessr......
+000004c0: 7072 696e 7472 1800 0000 da05 5f65 7869  printr......_exi
+000004d0: 7429 04da 0763 6f6d 6d61 6e64 7206 0000  t)...commandr...
+000004e0: 0072 1800 0000 da0b 7468 655f 7072 6f63  .r......the_proc
+000004f0: 6573 73a9 0172 1b00 0000 7219 0000 0072  ess..r....r....r
+00000500: 1a00 0000 da16 7374 6172 745f 6465 7461  ......start_deta
+00000510: 6368 6564 5f70 726f 6365 7373 5700 0000  ched_processW...
+00000520: 7314 0000 0008 0108 0308 0206 030e 0204  s...............
+00000530: 0204 0704 f90e 0a04 047a 2c68 696b 655f  .........z,hike_
+00000540: 7061 7373 6976 652e 3c6c 6f63 616c 733e  passive.<locals>
+00000550: 2e73 7461 7274 5f64 6574 6163 6865 645f  .start_detached_
+00000560: 7072 6f63 6573 73da 0963 6c6f 7365 5f66  process..close_f
+00000570: 6473 547a 0c6d 6572 6765 645f 6469 6374  dsTz.merged_dict
+00000580: 3a7a 0770 6163 6b65 743a da10 7072 6f63  :z.packet:..proc
+00000590: 6573 735f 6964 656e 7469 7479 2908 da04  ess_identity)...
+000005a0: 7479 7065 da04 6469 6374 7204 0000 0072  type..dictr....r
+000005b0: 1e00 0000 721d 0000 0072 0700 0000 7218  ....r....r....r.
+000005c0: 0000 00da 046a 6f69 6e29 07da 0670 6163  .....join)...pac
+000005d0: 6b65 7472 0600 0000 da0a 506f 7065 6e5f  ketr......Popen_
+000005e0: 6b65 7973 7223 0000 00da 0b6d 6572 6765  keysr#.....merge
+000005f0: 645f 6469 6374 7221 0000 00da 1464 6574  d_dictr!.....det
+00000600: 6163 6865 645f 7072 6f63 6573 735f 7069  ached_process_pi
+00000610: 6472 1900 0000 7222 0000 0072 1a00 0000  dr....r"...r....
+00000620: da0c 6869 6b65 5f70 6173 7369 7665 2f00  ..hike_passive/.
+00000630: 0000 732a 0000 0008 0104 0208 0110 0108  ..s*............
+00000640: 0108 020c 2002 1e04 0102 ff02 0204 fe0a  .... ...........
+00000650: 040a 0104 0202 0104 ff02 0206 fe06 0604  ................
+00000660: ff72 2d00 0000 2911 da07 5f5f 646f 635f  .r-...)...__doc_
+00000670: 5fda 2876 656e 7475 7265 732e 7574 696c  _.(ventures.util
+00000680: 6974 6965 732e 6869 6b65 5f70 6173 7369  ities.hike_passi
+00000690: 7665 5f70 5f65 7870 6563 7472 0200 0000  ve_p_expectr....
+000006a0: da33 7665 6e74 7572 6573 2e75 7469 6c69  .3ventures.utili
+000006b0: 7469 6573 2e68 696b 655f 7061 7373 6976  ties.hike_passiv
+000006c0: 655f 705f 6578 7065 6374 5f32 2e69 6d70  e_p_expect_2.imp
+000006d0: 6c69 6369 7472 0300 0000 da04 7269 6368  licitr......rich
+000006e0: da06 7079 6461 7368 7204 0000 00da 0966  ..pydashr......f
+000006f0: 7261 6374 696f 6e73 7205 0000 00da 0f6d  ractionsr......m
+00000700: 756c 7469 7072 6f63 6573 7369 6e67 721d  ultiprocessingr.
+00000710: 0000 00da 0474 696d 6572 0b00 0000 da06  .....timer......
+00000720: 6174 6578 6974 720d 0000 0072 2d00 0000  atexitr....r-...
+00000730: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000740: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000750: 0000 7320 0000 0004 0a02 090c 060c 0108  ..s ............
+00000760: 030c 010c 0308 0108 0108 0108 0108 0108  ................
+00000770: 0108 0108 010c 05                        .......
```

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.2.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.2.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.2.0/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.2.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.2.0/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.1.5/PKG-INFO` & `ventures-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.1.5
+Version: 1.2.0
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: biotech (>=1.1.10,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: pydash (>=8.0.1,<9.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sanic (>=23.12.1,<24.0.0)
 Requires-Dist: sanic-ext (>=23.12.0,<24.0.0)
 Requires-Dist: sanic_limiter (==0.1.3)
 Requires-Dist: setuptools (>=69.5.1,<70.0.0)
 Requires-Dist: somatic (>=3.0.3,<4.0.0)
 Description-Content-Type: text/markdown
```

