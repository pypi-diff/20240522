# Comparing `tmp/rvc3python-0.9.0.tar.gz` & `tmp/rvc3python-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rvc3python-0.9.0.tar", last modified: Tue May 16 10:36:08 2023, max compression
+gzip compressed data, was "rvc3python-0.9.1.tar", last modified: Wed May 22 04:54:28 2024, max compression
```

## Comparing `rvc3python-0.9.0.tar` & `rvc3python-0.9.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.948825 rvc3python-0.9.0/
--rw-r--r--   0 corkep     (503) staff       (20)     1068 2022-03-03 04:50:52.000000 rvc3python-0.9.0/LICENSE
--rw-r--r--   0 corkep     (503) staff       (20)      325 2023-05-01 11:27:49.000000 rvc3python-0.9.0/MANIFEST.in
--rw-rw----   0 corkep     (503) staff       (20)    17476 2023-05-16 10:36:08.948134 rvc3python-0.9.0/PKG-INFO
--rw-r--r--   0 corkep     (503) staff       (20)    15779 2023-05-14 01:09:13.000000 rvc3python-0.9.0/README.md
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.837525 rvc3python-0.9.0/RVC3/
--rw-r--r--   0 corkep     (503) staff       (20)      110 2023-01-26 06:28:11.000000 rvc3python-0.9.0/RVC3/__init__.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.839956 rvc3python-0.9.0/RVC3/bin/
--rw-rw----   0 corkep     (503) staff       (20)        0 2023-01-25 00:33:56.000000 rvc3python-0.9.0/RVC3/bin/__init__.py
--rwxr--r--   0 corkep     (503) staff       (20)      170 2023-01-26 06:30:34.000000 rvc3python-0.9.0/RVC3/bin/bdsim_path.py
--rwxr--r--   0 corkep     (503) staff       (20)    10533 2023-05-01 10:34:07.000000 rvc3python-0.9.0/RVC3/bin/rvctool.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.846446 rvc3python-0.9.0/RVC3/examples/
--rw-r--r--   0 corkep     (503) staff       (20)        0 2022-03-27 04:11:07.000000 rvc3python-0.9.0/RVC3/examples/__init__.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.873358 rvc3python-0.9.0/RVC3/examples/hershey/
--rw-r--r--   0 corkep     (503) staff       (20)     3655 2021-07-07 23:37:23.000000 rvc3python-0.9.0/RVC3/examples/hershey/genhershey.py
--rw-r--r--   0 corkep     (503) staff       (20)    22558 2021-07-07 23:37:37.000000 rvc3python-0.9.0/RVC3/examples/hershey/hershey.json
--rw-r--r--   0 corkep     (503) staff       (20)   109512 2021-04-08 10:54:54.000000 rvc3python-0.9.0/RVC3/examples/hershey/hershey.txt
--rw-r--r--   0 corkep     (503) staff       (20)      271 2021-04-08 10:54:54.000000 rvc3python-0.9.0/RVC3/examples/hershey/roman-plain.txt
--rw-r--r--   0 corkep     (503) staff       (20)      277 2021-04-08 10:54:54.000000 rvc3python-0.9.0/RVC3/examples/hershey/roman-simplex.txt
--rw-r--r--   0 corkep     (503) staff       (20)      287 2021-04-08 10:54:54.000000 rvc3python-0.9.0/RVC3/examples/hershey/roman-triplex.txt
--rwxr--r--   0 corkep     (503) staff       (20)     2514 2023-01-07 00:39:10.000000 rvc3python-0.9.0/RVC3/examples/imu_data.py
--rwxr--r--   0 corkep     (503) staff       (20)      986 2023-01-08 14:11:21.000000 rvc3python-0.9.0/RVC3/examples/mosaic.py
--rwxr--r--   0 corkep     (503) staff       (20)     2099 2022-10-04 10:46:02.000000 rvc3python-0.9.0/RVC3/examples/ransac_line.py
--rwxr--r--   0 corkep     (503) staff       (20)     4114 2023-01-08 13:29:36.000000 rvc3python-0.9.0/RVC3/examples/visodom.py
--rwxr--r--   0 corkep     (503) staff       (20)     3443 2022-03-27 04:59:28.000000 rvc3python-0.9.0/RVC3/examples/walking.py
--rwxr--r--   0 corkep     (503) staff       (20)      985 2022-03-13 02:43:06.000000 rvc3python-0.9.0/RVC3/examples/writing.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.941162 rvc3python-0.9.0/RVC3/models/
--rwxr-xr--   0 corkep     (503) staff       (20)      908 2023-04-30 06:30:00.000000 rvc3python-0.9.0/RVC3/models/IBVS-arm-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    43781 2023-05-12 05:09:05.000000 rvc3python-0.9.0/RVC3/models/IBVS-arm.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1155 2023-04-30 06:30:25.000000 rvc3python-0.9.0/RVC3/models/IBVS-holonomic-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    40660 2023-05-12 05:09:30.000000 rvc3python-0.9.0/RVC3/models/IBVS-holonomic.bd
--rwxr-xr--   0 corkep     (503) staff       (20)      586 2023-05-03 10:34:50.000000 rvc3python-0.9.0/RVC3/models/IBVS-main.py
--rwxr-xr--   0 corkep     (503) staff       (20)     1922 2023-04-30 06:43:51.000000 rvc3python-0.9.0/RVC3/models/IBVS-nonholonomic-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    71669 2023-05-12 05:09:39.000000 rvc3python-0.9.0/RVC3/models/IBVS-nonholonomic.bd
--rwxr-xr--   0 corkep     (503) staff       (20)      997 2023-05-03 10:35:10.000000 rvc3python-0.9.0/RVC3/models/IBVS-partitioned-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    47445 2023-05-12 05:09:57.000000 rvc3python-0.9.0/RVC3/models/IBVS-partitioned.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     3614 2023-04-30 22:13:37.000000 rvc3python-0.9.0/RVC3/models/IBVS-quadrotor-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    67100 2023-05-12 05:10:35.000000 rvc3python-0.9.0/RVC3/models/IBVS-quadrotor.bd
--rw-r--r--   0 corkep     (503) staff       (20)    30462 2022-10-04 10:46:18.000000 rvc3python-0.9.0/RVC3/models/IBVS.bd
--rw-r--r--   0 corkep     (503) staff       (20)    11048 2022-10-04 10:46:18.000000 rvc3python-0.9.0/RVC3/models/RRMC.bd
--rwxr-xr--   0 corkep     (503) staff       (20)      940 2023-05-03 10:35:39.000000 rvc3python-0.9.0/RVC3/models/RRMC.py
--rw-r--r--   0 corkep     (503) staff       (20)    19606 2022-10-04 10:46:18.000000 rvc3python-0.9.0/RVC3/models/RRMC2.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1682 2023-05-03 10:35:54.000000 rvc3python-0.9.0/RVC3/models/RRMC2.py
--rwxr-x---   0 corkep     (503) staff       (20)      572 2023-04-30 06:09:05.000000 rvc3python-0.9.0/RVC3/models/SEA-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    43915 2023-04-30 04:14:43.000000 rvc3python-0.9.0/RVC3/models/SEA.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     2602 2023-05-03 10:36:23.000000 rvc3python-0.9.0/RVC3/models/SEA.py
--rwxr-xr--   0 corkep     (503) staff       (20)        0 2022-12-04 09:00:09.000000 rvc3python-0.9.0/RVC3/models/__init__.py
--rw-r--r--   0 corkep     (503) staff       (20)    26126 2023-05-12 05:03:56.000000 rvc3python-0.9.0/RVC3/models/braitenberg.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1639 2023-05-03 10:36:41.000000 rvc3python-0.9.0/RVC3/models/braitenberg.py
--rw-r--r--   0 corkep     (503) staff       (20)     6868 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/cartspace.bd
--rwxr-x---   0 corkep     (503) staff       (20)      541 2023-04-30 06:05:47.000000 rvc3python-0.9.0/RVC3/models/computed-torque-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    26667 2023-04-30 01:25:50.000000 rvc3python-0.9.0/RVC3/models/computed-torque.bd
--rw-r--r--   0 corkep     (503) staff       (20)    47832 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/driveconfig.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     3001 2023-05-03 10:36:53.000000 rvc3python-0.9.0/RVC3/models/driveconfig.py
--rw-r--r--   0 corkep     (503) staff       (20)    24930 2022-10-04 10:46:02.000000 rvc3python-0.9.0/RVC3/models/driveline.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1656 2023-05-03 10:37:05.000000 rvc3python-0.9.0/RVC3/models/driveline.py
--rw-r--r--   0 corkep     (503) staff       (20)    27760 2022-10-04 10:46:18.000000 rvc3python-0.9.0/RVC3/models/drivepoint.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1582 2023-05-03 10:37:14.000000 rvc3python-0.9.0/RVC3/models/drivepoint.py
--rw-r--r--   0 corkep     (503) staff       (20)    23208 2023-04-18 11:09:49.000000 rvc3python-0.9.0/RVC3/models/drivepursuit.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     2593 2023-05-03 10:37:30.000000 rvc3python-0.9.0/RVC3/models/drivepursuit.py
--rwxr-x---   0 corkep     (503) staff       (20)      714 2023-05-07 10:28:12.000000 rvc3python-0.9.0/RVC3/models/feedforward-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    32877 2023-05-12 05:07:32.000000 rvc3python-0.9.0/RVC3/models/feedforward.bd
--rw-r--r--   0 corkep     (503) staff       (20)     8695 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/jointspace.bd
--rwxr-xr--   0 corkep     (503) staff       (20)      619 2023-04-30 23:26:33.000000 rvc3python-0.9.0/RVC3/models/jointspace.py
--rw-r--r--   0 corkep     (503) staff       (20)     5273 2023-04-18 21:48:51.000000 rvc3python-0.9.0/RVC3/models/lanechange.bd
--rwxr-xr--   0 corkep     (503) staff       (20)      609 2023-05-03 10:37:50.000000 rvc3python-0.9.0/RVC3/models/lanechange.py
--rwxr-x---   0 corkep     (503) staff       (20)     1856 2023-05-12 04:59:54.000000 rvc3python-0.9.0/RVC3/models/opspace-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    57493 2023-05-12 04:51:21.000000 rvc3python-0.9.0/RVC3/models/opspace.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     3860 2023-05-12 04:54:29.000000 rvc3python-0.9.0/RVC3/models/opspace.py
--rw-r--r--   0 corkep     (503) staff       (20)    24713 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/ploop.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1980 2023-04-30 06:07:17.000000 rvc3python-0.9.0/RVC3/models/ploop.py
--rw-r--r--   0 corkep     (503) staff       (20)    11860 2022-11-21 10:01:57.000000 rvc3python-0.9.0/RVC3/models/ploop_test.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1206 2023-05-03 10:38:27.000000 rvc3python-0.9.0/RVC3/models/ploop_test.py
--rwxr-x---   0 corkep     (503) staff       (20)     4407 2023-03-13 03:01:39.000000 rvc3python-0.9.0/RVC3/models/quad_model.py
--rwxr-xr--   0 corkep     (503) staff       (20)     2172 2023-05-03 10:38:49.000000 rvc3python-0.9.0/RVC3/models/quadrotor-main.py
--rw-r--r--   0 corkep     (503) staff       (20)    57216 2023-05-12 05:12:18.000000 rvc3python-0.9.0/RVC3/models/quadrotor.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     3760 2023-05-03 10:39:10.000000 rvc3python-0.9.0/RVC3/models/quadrotor.py
--rw-r--r--   0 corkep     (503) staff       (20)    39699 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/vloop.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1290 2023-04-30 06:09:33.000000 rvc3python-0.9.0/RVC3/models/vloop.py
--rw-r--r--   0 corkep     (503) staff       (20)    16230 2022-01-05 20:50:13.000000 rvc3python-0.9.0/RVC3/models/vloop_test.bd
--rwxr-xr--   0 corkep     (503) staff       (20)     1340 2023-05-03 10:39:25.000000 rvc3python-0.9.0/RVC3/models/vloop_test.py
--rw-r--r--   0 corkep     (503) staff       (20)     3690 2022-10-04 10:44:19.000000 rvc3python-0.9.0/RVC3/models/zerotorque.bd
--rwxr-xr--   0 corkep     (503) staff       (20)      662 2023-05-03 10:39:34.000000 rvc3python-0.9.0/RVC3/models/zerotorque.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.943149 rvc3python-0.9.0/RVC3/tools/
--rw-r--r--   0 corkep     (503) staff       (20)        0 2022-12-04 10:32:34.000000 rvc3python-0.9.0/RVC3/tools/__init__.py
--rw-r--r--   0 corkep     (503) staff       (20)     7358 2023-01-15 01:05:41.000000 rvc3python-0.9.0/RVC3/tools/rvcprint.py
--rw-r--r--   0 corkep     (503) staff       (20)       72 2022-12-04 21:35:33.000000 rvc3python-0.9.0/Untitled.ipynb
--rw-rw----   0 corkep     (503) staff       (20)     2646 2023-05-14 01:14:42.000000 rvc3python-0.9.0/pyproject.toml
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-16 10:36:08.947338 rvc3python-0.9.0/rvc3python.egg-info/
--rw-rw----   0 corkep     (503) staff       (20)    17476 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)     2272 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/SOURCES.txt
--rw-rw----   0 corkep     (503) staff       (20)        1 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/dependency_links.txt
--rw-rw----   0 corkep     (503) staff       (20)       88 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/entry_points.txt
--rw-rw----   0 corkep     (503) staff       (20)      129 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/requires.txt
--rw-rw----   0 corkep     (503) staff       (20)        5 2023-05-16 10:36:08.000000 rvc3python-0.9.0/rvc3python.egg-info/top_level.txt
--rw-rw----   0 corkep     (503) staff       (20)       38 2023-05-16 10:36:08.948956 rvc3python-0.9.0/setup.cfg
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-22 04:54:28.477042 rvc3python-0.9.1/
+-rw-r--r--   0 pic        (503) staff       (20)     1068 2022-03-03 04:50:52.000000 rvc3python-0.9.1/LICENSE
+-rw-r--r--   0 pic        (503) staff       (20)      325 2023-05-01 11:27:49.000000 rvc3python-0.9.1/MANIFEST.in
+-rw-r--r--   0 pic        (503) staff       (20)    17941 2024-05-22 04:54:28.476297 rvc3python-0.9.1/PKG-INFO
+-rw-rw----   0 pic        (503) staff       (20)    15901 2024-05-22 04:32:06.000000 rvc3python-0.9.1/README.md
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-22 04:54:28.348565 rvc3python-0.9.1/RVC3/
+-rw-r--r--   0 pic        (503) staff       (20)      110 2023-01-26 06:28:11.000000 rvc3python-0.9.1/RVC3/__init__.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-22 04:54:28.349962 rvc3python-0.9.1/RVC3/bin/
+-rw-rw----   0 pic        (503) staff       (20)        0 2023-01-25 00:33:56.000000 rvc3python-0.9.1/RVC3/bin/__init__.py
+-rwxr--r--   0 pic        (503) staff       (20)      170 2023-01-26 06:30:34.000000 rvc3python-0.9.1/RVC3/bin/bdsim_path.py
+-rwxr--r--   0 pic        (503) staff       (20)    10533 2023-05-01 10:34:07.000000 rvc3python-0.9.1/RVC3/bin/rvctool.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-22 04:54:28.354182 rvc3python-0.9.1/RVC3/examples/
+-rw-r--r--   0 pic        (503) staff       (20)        0 2022-03-27 04:11:07.000000 rvc3python-0.9.1/RVC3/examples/__init__.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-22 04:54:28.358168 rvc3python-0.9.1/RVC3/examples/hershey/
+-rw-r--r--   0 pic        (503) staff       (20)     3655 2021-07-07 23:37:23.000000 rvc3python-0.9.1/RVC3/examples/hershey/genhershey.py
+-rw-r--r--   0 pic        (503) staff       (20)    22558 2021-07-07 23:37:37.000000 rvc3python-0.9.1/RVC3/examples/hershey/hershey.json
+-rw-r--r--   0 pic        (503) staff       (20)   109512 2021-04-08 10:54:54.000000 rvc3python-0.9.1/RVC3/examples/hershey/hershey.txt
+-rw-r--r--   0 pic        (503) staff       (20)      271 2021-04-08 10:54:54.000000 rvc3python-0.9.1/RVC3/examples/hershey/roman-plain.txt
+-rw-r--r--   0 pic        (503) staff       (20)      277 2021-04-08 10:54:54.000000 rvc3python-0.9.1/RVC3/examples/hershey/roman-simplex.txt
+-rw-r--r--   0 pic        (503) staff       (20)      287 2021-04-08 10:54:54.000000 rvc3python-0.9.1/RVC3/examples/hershey/roman-triplex.txt
+-rwxr--r--   0 pic        (503) staff       (20)     2514 2023-01-07 00:39:10.000000 rvc3python-0.9.1/RVC3/examples/imu_data.py
+-rwxr--r--   0 pic        (503) staff       (20)      986 2023-01-08 14:11:21.000000 rvc3python-0.9.1/RVC3/examples/mosaic.py
+-rwxr--r--   0 pic        (503) staff       (20)     2099 2022-10-04 10:46:02.000000 rvc3python-0.9.1/RVC3/examples/ransac_line.py
+-rwxr--r--   0 pic        (503) staff       (20)     4114 2023-01-08 13:29:36.000000 rvc3python-0.9.1/RVC3/examples/visodom.py
+-rwxr--r--   0 pic        (503) staff       (20)     3443 2022-03-27 04:59:28.000000 rvc3python-0.9.1/RVC3/examples/walking.py
+-rwxr--r--   0 pic        (503) staff       (20)      985 2022-03-13 02:43:06.000000 rvc3python-0.9.1/RVC3/examples/writing.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-22 04:54:28.470701 rvc3python-0.9.1/RVC3/models/
+-rwxr-xr--   0 pic        (503) staff       (20)      908 2023-04-30 06:30:00.000000 rvc3python-0.9.1/RVC3/models/IBVS-arm-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    43781 2023-05-12 05:09:05.000000 rvc3python-0.9.1/RVC3/models/IBVS-arm.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1155 2023-04-30 06:30:25.000000 rvc3python-0.9.1/RVC3/models/IBVS-holonomic-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    40660 2023-05-12 05:09:30.000000 rvc3python-0.9.1/RVC3/models/IBVS-holonomic.bd
+-rwxr-xr--   0 pic        (503) staff       (20)      586 2023-05-03 10:34:50.000000 rvc3python-0.9.1/RVC3/models/IBVS-main.py
+-rwxr-xr--   0 pic        (503) staff       (20)     1922 2023-04-30 06:43:51.000000 rvc3python-0.9.1/RVC3/models/IBVS-nonholonomic-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    71669 2023-05-12 05:09:39.000000 rvc3python-0.9.1/RVC3/models/IBVS-nonholonomic.bd
+-rwxr-xr--   0 pic        (503) staff       (20)      997 2023-05-03 10:35:10.000000 rvc3python-0.9.1/RVC3/models/IBVS-partitioned-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    47445 2023-05-12 05:09:57.000000 rvc3python-0.9.1/RVC3/models/IBVS-partitioned.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     3614 2023-04-30 22:13:37.000000 rvc3python-0.9.1/RVC3/models/IBVS-quadrotor-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    67100 2023-05-12 05:10:35.000000 rvc3python-0.9.1/RVC3/models/IBVS-quadrotor.bd
+-rw-r--r--   0 pic        (503) staff       (20)    30462 2022-10-04 10:46:18.000000 rvc3python-0.9.1/RVC3/models/IBVS.bd
+-rw-r--r--   0 pic        (503) staff       (20)    11048 2022-10-04 10:46:18.000000 rvc3python-0.9.1/RVC3/models/RRMC.bd
+-rwxr-xr--   0 pic        (503) staff       (20)      940 2023-05-03 10:35:39.000000 rvc3python-0.9.1/RVC3/models/RRMC.py
+-rw-r--r--   0 pic        (503) staff       (20)    19606 2022-10-04 10:46:18.000000 rvc3python-0.9.1/RVC3/models/RRMC2.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1682 2023-05-03 10:35:54.000000 rvc3python-0.9.1/RVC3/models/RRMC2.py
+-rwxr-x---   0 pic        (503) staff       (20)      572 2023-04-30 06:09:05.000000 rvc3python-0.9.1/RVC3/models/SEA-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    43915 2023-04-30 04:14:43.000000 rvc3python-0.9.1/RVC3/models/SEA.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     2602 2023-05-03 10:36:23.000000 rvc3python-0.9.1/RVC3/models/SEA.py
+-rwxr-xr--   0 pic        (503) staff       (20)        0 2022-12-04 09:00:09.000000 rvc3python-0.9.1/RVC3/models/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)    26126 2023-05-12 05:03:56.000000 rvc3python-0.9.1/RVC3/models/braitenberg.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1639 2023-05-03 10:36:41.000000 rvc3python-0.9.1/RVC3/models/braitenberg.py
+-rw-r--r--   0 pic        (503) staff       (20)     6868 2022-10-04 10:44:19.000000 rvc3python-0.9.1/RVC3/models/cartspace.bd
+-rwxr-x---   0 pic        (503) staff       (20)      541 2023-04-30 06:05:47.000000 rvc3python-0.9.1/RVC3/models/computed-torque-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    26667 2023-04-30 01:25:50.000000 rvc3python-0.9.1/RVC3/models/computed-torque.bd
+-rw-r--r--   0 pic        (503) staff       (20)    47832 2022-10-04 10:44:19.000000 rvc3python-0.9.1/RVC3/models/driveconfig.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     3001 2023-05-03 10:36:53.000000 rvc3python-0.9.1/RVC3/models/driveconfig.py
+-rw-r--r--   0 pic        (503) staff       (20)    24930 2022-10-04 10:46:02.000000 rvc3python-0.9.1/RVC3/models/driveline.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1656 2023-05-03 10:37:05.000000 rvc3python-0.9.1/RVC3/models/driveline.py
+-rw-r--r--   0 pic        (503) staff       (20)    27760 2022-10-04 10:46:18.000000 rvc3python-0.9.1/RVC3/models/drivepoint.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1582 2023-05-03 10:37:14.000000 rvc3python-0.9.1/RVC3/models/drivepoint.py
+-rw-r--r--   0 pic        (503) staff       (20)    23208 2023-04-18 11:09:49.000000 rvc3python-0.9.1/RVC3/models/drivepursuit.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     2593 2023-05-03 10:37:30.000000 rvc3python-0.9.1/RVC3/models/drivepursuit.py
+-rwxr-x---   0 pic        (503) staff       (20)      714 2023-05-07 10:28:12.000000 rvc3python-0.9.1/RVC3/models/feedforward-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    32877 2023-05-12 05:07:32.000000 rvc3python-0.9.1/RVC3/models/feedforward.bd
+-rw-r--r--   0 pic        (503) staff       (20)     8695 2022-10-04 10:44:19.000000 rvc3python-0.9.1/RVC3/models/jointspace.bd
+-rwxr-xr--   0 pic        (503) staff       (20)      619 2023-04-30 23:26:33.000000 rvc3python-0.9.1/RVC3/models/jointspace.py
+-rw-r--r--   0 pic        (503) staff       (20)     5273 2023-04-18 21:48:51.000000 rvc3python-0.9.1/RVC3/models/lanechange.bd
+-rwxr-xr--   0 pic        (503) staff       (20)      609 2023-05-03 10:37:50.000000 rvc3python-0.9.1/RVC3/models/lanechange.py
+-rwxr-x---   0 pic        (503) staff       (20)     1856 2023-05-12 04:59:54.000000 rvc3python-0.9.1/RVC3/models/opspace-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    57493 2023-05-12 04:51:21.000000 rvc3python-0.9.1/RVC3/models/opspace.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     3860 2023-05-12 04:54:29.000000 rvc3python-0.9.1/RVC3/models/opspace.py
+-rw-r--r--   0 pic        (503) staff       (20)    24713 2022-10-04 10:44:19.000000 rvc3python-0.9.1/RVC3/models/ploop.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1980 2023-04-30 06:07:17.000000 rvc3python-0.9.1/RVC3/models/ploop.py
+-rw-r--r--   0 pic        (503) staff       (20)    11860 2022-11-21 10:01:57.000000 rvc3python-0.9.1/RVC3/models/ploop_test.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1206 2023-05-03 10:38:27.000000 rvc3python-0.9.1/RVC3/models/ploop_test.py
+-rwxr-x---   0 pic        (503) staff       (20)     4407 2023-03-13 03:01:39.000000 rvc3python-0.9.1/RVC3/models/quad_model.py
+-rwxr-xr--   0 pic        (503) staff       (20)     2172 2023-05-03 10:38:49.000000 rvc3python-0.9.1/RVC3/models/quadrotor-main.py
+-rw-r--r--   0 pic        (503) staff       (20)    57216 2023-05-12 05:12:18.000000 rvc3python-0.9.1/RVC3/models/quadrotor.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     3760 2023-05-03 10:39:10.000000 rvc3python-0.9.1/RVC3/models/quadrotor.py
+-rw-r--r--   0 pic        (503) staff       (20)    39699 2022-10-04 10:44:19.000000 rvc3python-0.9.1/RVC3/models/vloop.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1290 2023-04-30 06:09:33.000000 rvc3python-0.9.1/RVC3/models/vloop.py
+-rw-r--r--   0 pic        (503) staff       (20)    16230 2022-01-05 20:50:13.000000 rvc3python-0.9.1/RVC3/models/vloop_test.bd
+-rwxr-xr--   0 pic        (503) staff       (20)     1340 2023-05-03 10:39:25.000000 rvc3python-0.9.1/RVC3/models/vloop_test.py
+-rw-r--r--   0 pic        (503) staff       (20)     3690 2022-10-04 10:44:19.000000 rvc3python-0.9.1/RVC3/models/zerotorque.bd
+-rwxr-xr--   0 pic        (503) staff       (20)      662 2023-05-03 10:39:34.000000 rvc3python-0.9.1/RVC3/models/zerotorque.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-22 04:54:28.471701 rvc3python-0.9.1/RVC3/tools/
+-rw-r--r--   0 pic        (503) staff       (20)        0 2022-12-04 10:32:34.000000 rvc3python-0.9.1/RVC3/tools/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)     7358 2023-01-15 01:05:41.000000 rvc3python-0.9.1/RVC3/tools/rvcprint.py
+-rw-r--r--   0 pic        (503) staff       (20)       72 2022-12-04 21:35:33.000000 rvc3python-0.9.1/Untitled.ipynb
+-rw-rw----   0 pic        (503) staff       (20)     2814 2024-05-22 04:22:00.000000 rvc3python-0.9.1/pyproject.toml
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-22 04:54:28.475195 rvc3python-0.9.1/rvc3python.egg-info/
+-rw-r--r--   0 pic        (503) staff       (20)    17941 2024-05-22 04:54:28.000000 rvc3python-0.9.1/rvc3python.egg-info/PKG-INFO
+-rw-rw----   0 pic        (503) staff       (20)     2272 2024-05-22 04:54:28.000000 rvc3python-0.9.1/rvc3python.egg-info/SOURCES.txt
+-rw-rw----   0 pic        (503) staff       (20)        1 2024-05-22 04:54:28.000000 rvc3python-0.9.1/rvc3python.egg-info/dependency_links.txt
+-rw-rw----   0 pic        (503) staff       (20)       88 2024-05-22 04:54:28.000000 rvc3python-0.9.1/rvc3python.egg-info/entry_points.txt
+-rw-rw----   0 pic        (503) staff       (20)      129 2024-05-22 04:54:28.000000 rvc3python-0.9.1/rvc3python.egg-info/requires.txt
+-rw-rw----   0 pic        (503) staff       (20)        5 2024-05-22 04:54:28.000000 rvc3python-0.9.1/rvc3python.egg-info/top_level.txt
+-rw-rw----   0 pic        (503) staff       (20)       38 2024-05-22 04:54:28.477184 rvc3python-0.9.1/setup.cfg
```

### Comparing `rvc3python-0.9.0/LICENSE` & `rvc3python-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/PKG-INFO` & `rvc3python-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: rvc3python
-Version: 0.9.0
+Version: 0.9.1
 Summary: Support for book: Robotics, Vision & Control 3 in Python
 Author-email: Peter Corke <rvc@petercorke.com>
 Project-URL: Homepage, https://github.com/petercorke/RVC3-python
 Project-URL: Bug Tracker, https://github.com/petercorke/RVC3-python/issues
 Project-URL: Source, https://github.com/petercorke/RVC3-python
 Keywords: robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly exploring random tree,probabilistic roadmap planner,force control,kinematics,Jacobian,position control,velocity control,spatial math,SO(2),SE(2),SO(3),SE(3),twist,product of exponential,translation,orientation,angle-axis,Lie group,skew symmetric matrix,pose,translation,rotation matrix,rigid body transform,homogeneous transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-quaternion,computer vision,machine vision,robotic vision,color space,blackbody,image segmentation,blobs,Hough transform,k-means,homography,camera calibration,visual odometry,bundle adjustment,stereo vision,rectification
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: pytorch
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: roboticstoolbox-python>=1
+Requires-Dist: machinevision-toolbox-python
+Requires-Dist: bdsim>=1.1
+Requires-Dist: IPython
+Requires-Dist: sympy
+Requires-Dist: pybullet
+Provides-Extra: pytorch
+Requires-Dist: torch; extra == "pytorch"
+Requires-Dist: torchvision; extra == "pytorch"
 
 # Robotics, Vision & Control: 3rd edition in Python (2023)
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 [![PyPI version](https://badge.fury.io/py/rvc3python.svg)](https://badge.fury.io/py/rvc3python)
@@ -42,15 +52,15 @@
 <li>Peter Corke, published by Springer-Nature 2023.</li>
 <li><b>ISBN</b> 978-3-031-06468-5 (hardcopy), 978-3-031-06469-2 (eBook)</li>
 <li><b>DOI</b> <a href="https://doi.org/10.1007/978-3-031-06469-2">10.1007/978-3-031-06469-2</a></li>
 </ul>
 <br><br>
 <p>Report an issue with the book or its supporting code <a href="https://github.com/petercorke/RVC3-python/issues/new/choose">here</a>.</p>
 
-<p>Knwon errata for the book can be viewed <a href="https://github.com/petercorke/RVC3-python/wiki/Errata">here</a>.</p>
+<p>Known errata for the book can be viewed <a href="https://github.com/petercorke/RVC3-python/wiki/Errata">here</a>.</p>
 </td>
 </tr>
 </table>
 
 
 This book uses many examples based on the following open-source Python packages
 
@@ -102,15 +112,15 @@
 Chapter 11 has some deep learning examples based on PyTorch.  If you don't have 
 PyTorch installed you can use the `pytorch` install option
 ```shell
 pip install rvc3python[pytorch]
 ```
 or
 ```shell
-conda install rvc3python[pytorch]
+conda install rvc3python
 ```
 ## Using the Toolboxes
 
 The simplest way to get going is to use the command line tool
 
 ```shell
 $ rvctool
@@ -233,15 +243,15 @@
 experimentation, but in your own code you can handle the imports as you see
 fit.
 
 ### Cutting and pasting
 
 IPython is very forgiving when it comes to cutting and pasting in blocks of Python
 code.  It will strip off the `>>>` prompt character and ignore indentation.  The normal
-python REPL is not so forgiving.  IPython also allows maintains a command history and
+python REPL is not so forgiving.  IPython also maintains a command history and
 allows command editing.
 ### Simple scripting
 You can write very simple scripts, for example `test.py` is
 
 ```python
 T = puma.fkine(puma.qn)
 sol = puma.ikine_LM(T)
@@ -262,14 +272,18 @@
 array([7.235e-08,  -0.8335,  0.09396,    3.142,   0.8312,   -3.142])
 PyPlot3D backend, t = 0.05, scene:
   robot: Text(0.0, 0.0, 'Puma 560')
 >>>
 ```
 and you are dropped into an IPython session after the script has run.
 
+## Issues running on Apple Silicon
+
+Check out the [wiki page](https://github.com/petercorke/RVC3-python/wiki/Running-on-Apple-Silicon).
+
 ## Using Jupyter and Colab
 
 Graphics and animations are problematic in these environments, some things work
 well, some don't.  As much as possible I've tweaked the Jupyter notebooks to work
 as best they can in these environments.
 
 For local use the [Jupyter plugin for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty decent.  Colab suffers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rvc3python Version: 0.9.0 Summary: Support for
+Metadata-Version: 2.1 Name: rvc3python Version: 0.9.1 Summary: Support for
 book: Robotics, Vision & Control 3 in Python Author-email: Peter Corke
 petercorke.com> Project-URL: Homepage, https://github.com/petercorke/RVC3-
 python Project-URL: Bug Tracker, https://github.com/petercorke/RVC3-python/
 issues Project-URL: Source, https://github.com/petercorke/RVC3-python Keywords:
 robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path
 planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly
 exploring random tree,probabilistic roadmap planner,force
@@ -15,23 +15,27 @@
 space,blackbody,image segmentation,blobs,Hough transform,k-
 means,homography,camera calibration,visual odometry,bundle adjustment,stereo
 vision,rectification Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: pytorch License-File: LICENSE # Robotics, Vision & Control: 3rd
-edition in Python (2023) [![A Python Robotics Package](https://
-raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/
-svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-
-python) [![QUT Centre for Robotics Open Source](https://github.com/qcr/
-qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io) [![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: matplotlib Requires-Dist: roboticstoolbox-python>=1 Requires-Dist:
+machinevision-toolbox-python Requires-Dist: bdsim>=1.1 Requires-Dist: IPython
+Requires-Dist: sympy Requires-Dist: pybullet Provides-Extra: pytorch Requires-
+Dist: torch; extra == "pytorch" Requires-Dist: torchvision; extra == "pytorch"
+# Robotics, Vision & Control: 3rd edition in Python (2023) [![A Python Robotics
+Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/
+master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/
+robotics-toolbox-python) [![QUT Centre for Robotics Open Source](https://
+github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/
 rvc3python.svg)](https://badge.fury.io/py/rvc3python) ![PyPI - Python Version]
 (https://img.shields.io/pypi/pyversions/rvc3python.svg) [![PyPI - Downloads]
 (https://img.shields.io/pypi/dw/rvc3python)](https://pypistats.org/packages/
 rvc3python)
                                      Welcome to the online hub for the book:
                                          # RRoobboottiiccss,, VViissiioonn && CCoonnttrrooll:
@@ -42,15 +46,15 @@
                                          # IISSBBNN 978-3-031-06468-5 (hardcopy),
 [Front cover 978-3-031-06468-5_5208]       978-3-031-06469-2 (eBook)
                                          # DDOOII _1_0_._1_0_0_7_/_9_7_8_-_3_-_0_3_1_-_0_6_4_6_9_-_2
 
 
                                      Report an issue with the book or its
                                      supporting code _h_e_r_e.
-                                     Knwon errata for the book can be viewed
+                                     Known errata for the book can be viewed
                                      _h_e_r_e.
 This book uses many examples based on the following open-source Python packages
 _[_R_o_b_o_t_i_c_s_ _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_M_a_c_h_i_n_e_ _V_i_s_i_o_n_ _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_S_p_a_t_i_a_l_ _M_a_t_h_s
 _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_B_l_o_c_k_ _d_i_a_g_r_a_m_ _s_i_m_u_l_a_t_i_o_n_ _f_o_r_ _P_y_t_h_o_n_]**Robotics Toolbox for
 Python**, **Machine Vision Toolbox for Python**, **Spatial Maths Toolbox for
 Python**, **Block Diagram Simulation for Python**. These in turn have
 dependencies on other packages created by the author and third parties. ##
@@ -69,35 +73,35 @@
 separated from your other Python code and projects. If you've never used
 virtual environments before this might be a good time to start, and it is
 really easy [using Conda](https://conda.io/projects/conda/en/latest/user-guide/
 install/index.html): ```shell conda create -n RVC3 python=3.10 conda activate
 RVC3 pip install rvc3python ``` ### Installing deep learning tools Chapter 11
 has some deep learning examples based on PyTorch. If you don't have PyTorch
 installed you can use the `pytorch` install option ```shell pip install
-rvc3python[pytorch] ``` or ```shell conda install rvc3python[pytorch] ``` ##
-Using the Toolboxes The simplest way to get going is to use the command line
-tool ```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__
-___ | |_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___
-| | |___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \
-/ _ \/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| |
-(__\__ \_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) |
-| ___) | |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_|
-\___/\/ \____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.1.0,
-MVTB==0.9.5, SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1,
-Matplotlib==3.7.1) import math import numpy as np from scipy import linalg,
-optimize import matplotlib.pyplot as plt from spatialmath import * from
-spatialmath.base import * from spatialmath.base import sym from spatialgeometry
-import * from roboticstoolbox import * from machinevisiontoolbox import *
-import machinevisiontoolbox.base as mvb # useful variables from math import pi
-puma = models.DH.Puma560() panda = models.DH.Panda() func/object? - show brief
-help help(func/object) - show detailed help func/object?? - show source code
-Results of assignments will be displayed, use trailing ; to suppress Python
-3.10.9 | packaged by conda-forge | (main, Feb 2 2023, 20:24:27) [Clang 14.0.6 ]
-Type 'copyright', 'credits' or 'license' for more information IPython 8.11.0 -
-- An enhanced Interactive Python. Type '?' for help. >>> ``` This provides an
+rvc3python[pytorch] ``` or ```shell conda install rvc3python ``` ## Using the
+Toolboxes The simplest way to get going is to use the command line tool
+```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__ ___ |
+|_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___ | |
+|___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \ / _
+\/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| | (__\__
+\_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) | | ___)
+| |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_| \___/\/
+\____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.1.0, MVTB==0.9.5,
+SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1, Matplotlib==3.7.1) import
+math import numpy as np from scipy import linalg, optimize import
+matplotlib.pyplot as plt from spatialmath import * from spatialmath.base import
+* from spatialmath.base import sym from spatialgeometry import * from
+roboticstoolbox import * from machinevisiontoolbox import * import
+machinevisiontoolbox.base as mvb # useful variables from math import pi puma =
+models.DH.Puma560() panda = models.DH.Panda() func/object? - show brief help
+help(func/object) - show detailed help func/object?? - show source code Results
+of assignments will be displayed, use trailing ; to suppress Python 3.10.9 |
+packaged by conda-forge | (main, Feb 2 2023, 20:24:27) [Clang 14.0.6 ] Type
+'copyright', 'credits' or 'license' for more information IPython 8.11.0 -- An
+enhanced Interactive Python. Type '?' for help. >>> ``` This provides an
 interactive Python ([IPython](https://ipython.readthedocs.io/en/stable))
 session with all the Toolboxes and supporting packages imported, and ready to
 go. It's a highly capable, convenient, and "MATLAB-like" workbench environment
 for robotics and computer vision. For example to load an ETS model of a Panda
 robot, solve a forward kinematics and inverse kinematics problem, and an
 interactive graphical display is simply: ```python >>> panda = models.ETS.Panda
 () ERobot: Panda (by Franka Emika), 7 joints (RRRRRRR)
@@ -143,50 +147,51 @@
 the book, and prompt characters are ignored The Robotics, Vision & Control book
 uses `rvctool` for all the included examples. `rvctool` imports the all the
 above mentioned packages using `import *` which is not considered best Python
 practice. It is very convenient for interactive experimentation, but in your
 own code you can handle the imports as you see fit. ### Cutting and pasting
 IPython is very forgiving when it comes to cutting and pasting in blocks of
 Python code. It will strip off the `>>>` prompt character and ignore
-indentation. The normal python REPL is not so forgiving. IPython also allows
-maintains a command history and allows command editing. ### Simple scripting
-You can write very simple scripts, for example `test.py` is ```python T =
-puma.fkine(puma.qn) sol = puma.ikine_LM(T) sol.q puma.plot(sol.q); ``` then
-```shell $ rvctool test.py 0 0 1 0.5963 0 1 0 -0.1501 -1 0 0 0.6575 0 0 0 1
-IKSolution(q=array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]),
-success=True, iterations=15, searches=1, residual=1.406125546650288e-07,
-reason='Success') array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142])
-PyPlot3D backend, t = 0.05, scene: robot: Text(0.0, 0.0, 'Puma 560') >>> ```
-and you are dropped into an IPython session after the script has run. ## Using
-Jupyter and Colab Graphics and animations are problematic in these
-environments, some things work well, some don't. As much as possible I've
-tweaked the Jupyter notebooks to work as best they can in these environments.
-For local use the [Jupyter plugin for Visual Studio Code](https://
-marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty
-decent. Colab suffers from old versions of major packages (though they are
-getting better at keeping up to date) and animations can suffer from slow
-update over the network. ## Other command line tools Additional command line
-tools available (from the Robotics Toolbox) include: - `eigdemo`, animation
-showing linear transformation of a rotating unit vector which demonstrates
-eigenvalues and eigenvectors. - `tripleangledemo`, Swift visualization that
-lets you experiment with various triple-angle sequences. - `twistdemo`, Swift
-visualization that lets you experiment with 3D twists. The screw axis is the
-blue rod and you can position and orient it using the sliders, and adjust its
-pitch. Then apply a rotation about the screw using the bottom slider. # Block
-diagram models _[_b_d_s_i_m_ _l_o_g_o_]Block diagram models are key to the pedagogy of the
-RVC3 book and 25 models are included. To simulate these models we use the
-Python package [bdsim](https://github.com/petercorke/bdsim) which can run
-models: - written in Python using [bdsim](https://github.com/petercorke/
-bdsim#getting-started) blocks and wiring. - created graphically using [bdedit]
-(https://github.com/petercorke/bdsim#bdedit-the-graphical-editing-tool) and
-saved as a `.bd` (JSON format) file. The models are included in the `RVC3`
-package when it is installed and `rvctool` adds them to the module search path.
-This means you can invoke them from `rvctool` by ```python >>> %run -
-m vloop_test ``` If you want to directly access the folder containing the
-models, the command line tool ```shell bdsim_path ``` will display the full
+indentation. The normal python REPL is not so forgiving. IPython also maintains
+a command history and allows command editing. ### Simple scripting You can
+write very simple scripts, for example `test.py` is ```python T = puma.fkine
+(puma.qn) sol = puma.ikine_LM(T) sol.q puma.plot(sol.q); ``` then ```shell $
+rvctool test.py 0 0 1 0.5963 0 1 0 -0.1501 -1 0 0 0.6575 0 0 0 1 IKSolution
+(q=array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]), success=True,
+iterations=15, searches=1, residual=1.406125546650288e-07, reason='Success')
+array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]) PyPlot3D backend, t
+= 0.05, scene: robot: Text(0.0, 0.0, 'Puma 560') >>> ``` and you are dropped
+into an IPython session after the script has run. ## Issues running on Apple
+Silicon Check out the [wiki page](https://github.com/petercorke/RVC3-python/
+wiki/Running-on-Apple-Silicon). ## Using Jupyter and Colab Graphics and
+animations are problematic in these environments, some things work well, some
+don't. As much as possible I've tweaked the Jupyter notebooks to work as best
+they can in these environments. For local use the [Jupyter plugin for Visual
+Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-
+toolsai.jupyter) is pretty decent. Colab suffers from old versions of major
+packages (though they are getting better at keeping up to date) and animations
+can suffer from slow update over the network. ## Other command line tools
+Additional command line tools available (from the Robotics Toolbox) include: -
+`eigdemo`, animation showing linear transformation of a rotating unit vector
+which demonstrates eigenvalues and eigenvectors. - `tripleangledemo`, Swift
+visualization that lets you experiment with various triple-angle sequences. -
+`twistdemo`, Swift visualization that lets you experiment with 3D twists. The
+screw axis is the blue rod and you can position and orient it using the
+sliders, and adjust its pitch. Then apply a rotation about the screw using the
+bottom slider. # Block diagram models _[_b_d_s_i_m_ _l_o_g_o_]Block diagram models are key
+to the pedagogy of the RVC3 book and 25 models are included. To simulate these
+models we use the Python package [bdsim](https://github.com/petercorke/bdsim)
+which can run models: - written in Python using [bdsim](https://github.com/
+petercorke/bdsim#getting-started) blocks and wiring. - created graphically
+using [bdedit](https://github.com/petercorke/bdsim#bdedit-the-graphical-
+editing-tool) and saved as a `.bd` (JSON format) file. The models are included
+in the `RVC3` package when it is installed and `rvctool` adds them to the
+module search path. This means you can invoke them from `rvctool` by ```python
+>>> %run -m vloop_test ``` If you want to directly access the folder containing
+the models, the command line tool ```shell bdsim_path ``` will display the full
 path to where they have been installed in the Python package tree. # Additional
 book resources [Front cover 978-3-031-06468-5_5208]This GitHub repo provides
 additional resources for readers including: - Jupyter notebooks containing all
 code lines from each chapter, see the [`notebooks`](notebooks) folder - The
 code to produce every Python/Matplotlib (2D) figure in the book, see the
 [`figures`](figures) folder - 3D points clouds from chapter 14, and the code to
 create them, see the [`pointclouds`](../pointclouds) folder. - 3D figures from
```

### Comparing `rvc3python-0.9.0/README.md` & `rvc3python-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 <li>Peter Corke, published by Springer-Nature 2023.</li>
 <li><b>ISBN</b> 978-3-031-06468-5 (hardcopy), 978-3-031-06469-2 (eBook)</li>
 <li><b>DOI</b> <a href="https://doi.org/10.1007/978-3-031-06469-2">10.1007/978-3-031-06469-2</a></li>
 </ul>
 <br><br>
 <p>Report an issue with the book or its supporting code <a href="https://github.com/petercorke/RVC3-python/issues/new/choose">here</a>.</p>
 
-<p>Knwon errata for the book can be viewed <a href="https://github.com/petercorke/RVC3-python/wiki/Errata">here</a>.</p>
+<p>Known errata for the book can be viewed <a href="https://github.com/petercorke/RVC3-python/wiki/Errata">here</a>.</p>
 </td>
 </tr>
 </table>
 
 
 This book uses many examples based on the following open-source Python packages
 
@@ -79,15 +79,15 @@
 Chapter 11 has some deep learning examples based on PyTorch.  If you don't have 
 PyTorch installed you can use the `pytorch` install option
 ```shell
 pip install rvc3python[pytorch]
 ```
 or
 ```shell
-conda install rvc3python[pytorch]
+conda install rvc3python
 ```
 ## Using the Toolboxes
 
 The simplest way to get going is to use the command line tool
 
 ```shell
 $ rvctool
@@ -210,15 +210,15 @@
 experimentation, but in your own code you can handle the imports as you see
 fit.
 
 ### Cutting and pasting
 
 IPython is very forgiving when it comes to cutting and pasting in blocks of Python
 code.  It will strip off the `>>>` prompt character and ignore indentation.  The normal
-python REPL is not so forgiving.  IPython also allows maintains a command history and
+python REPL is not so forgiving.  IPython also maintains a command history and
 allows command editing.
 ### Simple scripting
 You can write very simple scripts, for example `test.py` is
 
 ```python
 T = puma.fkine(puma.qn)
 sol = puma.ikine_LM(T)
@@ -239,14 +239,18 @@
 array([7.235e-08,  -0.8335,  0.09396,    3.142,   0.8312,   -3.142])
 PyPlot3D backend, t = 0.05, scene:
   robot: Text(0.0, 0.0, 'Puma 560')
 >>>
 ```
 and you are dropped into an IPython session after the script has run.
 
+## Issues running on Apple Silicon
+
+Check out the [wiki page](https://github.com/petercorke/RVC3-python/wiki/Running-on-Apple-Silicon).
+
 ## Using Jupyter and Colab
 
 Graphics and animations are problematic in these environments, some things work
 well, some don't.  As much as possible I've tweaked the Jupyter notebooks to work
 as best they can in these environments.
 
 For local use the [Jupyter plugin for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty decent.  Colab suffers
@@ -307,8 +311,8 @@
 - 3D figures from chapters 2-3, 7-9, and the code to create them, see the [`3dfigures`](../3dfigures) folder.
 - All example scripts, see the [`examples`](examples) folder.
 - To run the visual odometry example in Sect. 14.8.3 you need to download two image sequence, each over 100MB, [see the instructions here](https://github.com/petercorke/machinevision-toolbox-python/blob/master/mvtb-data/README.md#install-big-image-files). 
 
 To get that material you must clone the repo
 ```shell
 git clone https://github.com/petercorke/RVC3-python.git
-```
+```
```

#### html2text {}

```diff
@@ -18,15 +18,15 @@
                                          # IISSBBNN 978-3-031-06468-5 (hardcopy),
 [Front cover 978-3-031-06468-5_5208]       978-3-031-06469-2 (eBook)
                                          # DDOOII _1_0_._1_0_0_7_/_9_7_8_-_3_-_0_3_1_-_0_6_4_6_9_-_2
 
 
                                      Report an issue with the book or its
                                      supporting code _h_e_r_e.
-                                     Knwon errata for the book can be viewed
+                                     Known errata for the book can be viewed
                                      _h_e_r_e.
 This book uses many examples based on the following open-source Python packages
 _[_R_o_b_o_t_i_c_s_ _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_M_a_c_h_i_n_e_ _V_i_s_i_o_n_ _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_S_p_a_t_i_a_l_ _M_a_t_h_s
 _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_B_l_o_c_k_ _d_i_a_g_r_a_m_ _s_i_m_u_l_a_t_i_o_n_ _f_o_r_ _P_y_t_h_o_n_]**Robotics Toolbox for
 Python**, **Machine Vision Toolbox for Python**, **Spatial Maths Toolbox for
 Python**, **Block Diagram Simulation for Python**. These in turn have
 dependencies on other packages created by the author and third parties. ##
@@ -45,35 +45,35 @@
 separated from your other Python code and projects. If you've never used
 virtual environments before this might be a good time to start, and it is
 really easy [using Conda](https://conda.io/projects/conda/en/latest/user-guide/
 install/index.html): ```shell conda create -n RVC3 python=3.10 conda activate
 RVC3 pip install rvc3python ``` ### Installing deep learning tools Chapter 11
 has some deep learning examples based on PyTorch. If you don't have PyTorch
 installed you can use the `pytorch` install option ```shell pip install
-rvc3python[pytorch] ``` or ```shell conda install rvc3python[pytorch] ``` ##
-Using the Toolboxes The simplest way to get going is to use the command line
-tool ```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__
-___ | |_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___
-| | |___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \
-/ _ \/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| |
-(__\__ \_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) |
-| ___) | |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_|
-\___/\/ \____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.1.0,
-MVTB==0.9.5, SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1,
-Matplotlib==3.7.1) import math import numpy as np from scipy import linalg,
-optimize import matplotlib.pyplot as plt from spatialmath import * from
-spatialmath.base import * from spatialmath.base import sym from spatialgeometry
-import * from roboticstoolbox import * from machinevisiontoolbox import *
-import machinevisiontoolbox.base as mvb # useful variables from math import pi
-puma = models.DH.Puma560() panda = models.DH.Panda() func/object? - show brief
-help help(func/object) - show detailed help func/object?? - show source code
-Results of assignments will be displayed, use trailing ; to suppress Python
-3.10.9 | packaged by conda-forge | (main, Feb 2 2023, 20:24:27) [Clang 14.0.6 ]
-Type 'copyright', 'credits' or 'license' for more information IPython 8.11.0 -
-- An enhanced Interactive Python. Type '?' for help. >>> ``` This provides an
+rvc3python[pytorch] ``` or ```shell conda install rvc3python ``` ## Using the
+Toolboxes The simplest way to get going is to use the command line tool
+```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__ ___ |
+|_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___ | |
+|___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \ / _
+\/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| | (__\__
+\_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) | | ___)
+| |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_| \___/\/
+\____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.1.0, MVTB==0.9.5,
+SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1, Matplotlib==3.7.1) import
+math import numpy as np from scipy import linalg, optimize import
+matplotlib.pyplot as plt from spatialmath import * from spatialmath.base import
+* from spatialmath.base import sym from spatialgeometry import * from
+roboticstoolbox import * from machinevisiontoolbox import * import
+machinevisiontoolbox.base as mvb # useful variables from math import pi puma =
+models.DH.Puma560() panda = models.DH.Panda() func/object? - show brief help
+help(func/object) - show detailed help func/object?? - show source code Results
+of assignments will be displayed, use trailing ; to suppress Python 3.10.9 |
+packaged by conda-forge | (main, Feb 2 2023, 20:24:27) [Clang 14.0.6 ] Type
+'copyright', 'credits' or 'license' for more information IPython 8.11.0 -- An
+enhanced Interactive Python. Type '?' for help. >>> ``` This provides an
 interactive Python ([IPython](https://ipython.readthedocs.io/en/stable))
 session with all the Toolboxes and supporting packages imported, and ready to
 go. It's a highly capable, convenient, and "MATLAB-like" workbench environment
 for robotics and computer vision. For example to load an ETS model of a Panda
 robot, solve a forward kinematics and inverse kinematics problem, and an
 interactive graphical display is simply: ```python >>> panda = models.ETS.Panda
 () ERobot: Panda (by Franka Emika), 7 joints (RRRRRRR)
@@ -119,50 +119,51 @@
 the book, and prompt characters are ignored The Robotics, Vision & Control book
 uses `rvctool` for all the included examples. `rvctool` imports the all the
 above mentioned packages using `import *` which is not considered best Python
 practice. It is very convenient for interactive experimentation, but in your
 own code you can handle the imports as you see fit. ### Cutting and pasting
 IPython is very forgiving when it comes to cutting and pasting in blocks of
 Python code. It will strip off the `>>>` prompt character and ignore
-indentation. The normal python REPL is not so forgiving. IPython also allows
-maintains a command history and allows command editing. ### Simple scripting
-You can write very simple scripts, for example `test.py` is ```python T =
-puma.fkine(puma.qn) sol = puma.ikine_LM(T) sol.q puma.plot(sol.q); ``` then
-```shell $ rvctool test.py 0 0 1 0.5963 0 1 0 -0.1501 -1 0 0 0.6575 0 0 0 1
-IKSolution(q=array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]),
-success=True, iterations=15, searches=1, residual=1.406125546650288e-07,
-reason='Success') array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142])
-PyPlot3D backend, t = 0.05, scene: robot: Text(0.0, 0.0, 'Puma 560') >>> ```
-and you are dropped into an IPython session after the script has run. ## Using
-Jupyter and Colab Graphics and animations are problematic in these
-environments, some things work well, some don't. As much as possible I've
-tweaked the Jupyter notebooks to work as best they can in these environments.
-For local use the [Jupyter plugin for Visual Studio Code](https://
-marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty
-decent. Colab suffers from old versions of major packages (though they are
-getting better at keeping up to date) and animations can suffer from slow
-update over the network. ## Other command line tools Additional command line
-tools available (from the Robotics Toolbox) include: - `eigdemo`, animation
-showing linear transformation of a rotating unit vector which demonstrates
-eigenvalues and eigenvectors. - `tripleangledemo`, Swift visualization that
-lets you experiment with various triple-angle sequences. - `twistdemo`, Swift
-visualization that lets you experiment with 3D twists. The screw axis is the
-blue rod and you can position and orient it using the sliders, and adjust its
-pitch. Then apply a rotation about the screw using the bottom slider. # Block
-diagram models _[_b_d_s_i_m_ _l_o_g_o_]Block diagram models are key to the pedagogy of the
-RVC3 book and 25 models are included. To simulate these models we use the
-Python package [bdsim](https://github.com/petercorke/bdsim) which can run
-models: - written in Python using [bdsim](https://github.com/petercorke/
-bdsim#getting-started) blocks and wiring. - created graphically using [bdedit]
-(https://github.com/petercorke/bdsim#bdedit-the-graphical-editing-tool) and
-saved as a `.bd` (JSON format) file. The models are included in the `RVC3`
-package when it is installed and `rvctool` adds them to the module search path.
-This means you can invoke them from `rvctool` by ```python >>> %run -
-m vloop_test ``` If you want to directly access the folder containing the
-models, the command line tool ```shell bdsim_path ``` will display the full
+indentation. The normal python REPL is not so forgiving. IPython also maintains
+a command history and allows command editing. ### Simple scripting You can
+write very simple scripts, for example `test.py` is ```python T = puma.fkine
+(puma.qn) sol = puma.ikine_LM(T) sol.q puma.plot(sol.q); ``` then ```shell $
+rvctool test.py 0 0 1 0.5963 0 1 0 -0.1501 -1 0 0 0.6575 0 0 0 1 IKSolution
+(q=array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]), success=True,
+iterations=15, searches=1, residual=1.406125546650288e-07, reason='Success')
+array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]) PyPlot3D backend, t
+= 0.05, scene: robot: Text(0.0, 0.0, 'Puma 560') >>> ``` and you are dropped
+into an IPython session after the script has run. ## Issues running on Apple
+Silicon Check out the [wiki page](https://github.com/petercorke/RVC3-python/
+wiki/Running-on-Apple-Silicon). ## Using Jupyter and Colab Graphics and
+animations are problematic in these environments, some things work well, some
+don't. As much as possible I've tweaked the Jupyter notebooks to work as best
+they can in these environments. For local use the [Jupyter plugin for Visual
+Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-
+toolsai.jupyter) is pretty decent. Colab suffers from old versions of major
+packages (though they are getting better at keeping up to date) and animations
+can suffer from slow update over the network. ## Other command line tools
+Additional command line tools available (from the Robotics Toolbox) include: -
+`eigdemo`, animation showing linear transformation of a rotating unit vector
+which demonstrates eigenvalues and eigenvectors. - `tripleangledemo`, Swift
+visualization that lets you experiment with various triple-angle sequences. -
+`twistdemo`, Swift visualization that lets you experiment with 3D twists. The
+screw axis is the blue rod and you can position and orient it using the
+sliders, and adjust its pitch. Then apply a rotation about the screw using the
+bottom slider. # Block diagram models _[_b_d_s_i_m_ _l_o_g_o_]Block diagram models are key
+to the pedagogy of the RVC3 book and 25 models are included. To simulate these
+models we use the Python package [bdsim](https://github.com/petercorke/bdsim)
+which can run models: - written in Python using [bdsim](https://github.com/
+petercorke/bdsim#getting-started) blocks and wiring. - created graphically
+using [bdedit](https://github.com/petercorke/bdsim#bdedit-the-graphical-
+editing-tool) and saved as a `.bd` (JSON format) file. The models are included
+in the `RVC3` package when it is installed and `rvctool` adds them to the
+module search path. This means you can invoke them from `rvctool` by ```python
+>>> %run -m vloop_test ``` If you want to directly access the folder containing
+the models, the command line tool ```shell bdsim_path ``` will display the full
 path to where they have been installed in the Python package tree. # Additional
 book resources [Front cover 978-3-031-06468-5_5208]This GitHub repo provides
 additional resources for readers including: - Jupyter notebooks containing all
 code lines from each chapter, see the [`notebooks`](notebooks) folder - The
 code to produce every Python/Matplotlib (2D) figure in the book, see the
 [`figures`](figures) folder - 3D points clouds from chapter 14, and the code to
 create them, see the [`pointclouds`](../pointclouds) folder. - 3D figures from
```

### Comparing `rvc3python-0.9.0/RVC3/bin/rvctool.py` & `rvc3python-0.9.1/RVC3/bin/rvctool.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/hershey/genhershey.py` & `rvc3python-0.9.1/RVC3/examples/hershey/genhershey.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/hershey/hershey.json` & `rvc3python-0.9.1/RVC3/examples/hershey/hershey.json`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/hershey/hershey.txt` & `rvc3python-0.9.1/RVC3/examples/hershey/hershey.txt`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/imu_data.py` & `rvc3python-0.9.1/RVC3/examples/imu_data.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/mosaic.py` & `rvc3python-0.9.1/RVC3/examples/mosaic.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/ransac_line.py` & `rvc3python-0.9.1/RVC3/examples/ransac_line.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/visodom.py` & `rvc3python-0.9.1/RVC3/examples/visodom.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/walking.py` & `rvc3python-0.9.1/RVC3/examples/walking.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/examples/writing.py` & `rvc3python-0.9.1/RVC3/examples/writing.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-arm-main.py` & `rvc3python-0.9.1/RVC3/models/IBVS-arm-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-arm.bd` & `rvc3python-0.9.1/RVC3/models/IBVS-arm.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-holonomic-main.py` & `rvc3python-0.9.1/RVC3/models/IBVS-holonomic-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-holonomic.bd` & `rvc3python-0.9.1/RVC3/models/IBVS-holonomic.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-main.py` & `rvc3python-0.9.1/RVC3/models/IBVS-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-nonholonomic-main.py` & `rvc3python-0.9.1/RVC3/models/IBVS-nonholonomic-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-nonholonomic.bd` & `rvc3python-0.9.1/RVC3/models/IBVS-nonholonomic.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-partitioned-main.py` & `rvc3python-0.9.1/RVC3/models/IBVS-partitioned-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-partitioned.bd` & `rvc3python-0.9.1/RVC3/models/IBVS-partitioned.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-quadrotor-main.py` & `rvc3python-0.9.1/RVC3/models/IBVS-quadrotor-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS-quadrotor.bd` & `rvc3python-0.9.1/RVC3/models/IBVS-quadrotor.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/IBVS.bd` & `rvc3python-0.9.1/RVC3/models/IBVS.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/RRMC.bd` & `rvc3python-0.9.1/RVC3/models/RRMC.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/RRMC.py` & `rvc3python-0.9.1/RVC3/models/RRMC.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/RRMC2.bd` & `rvc3python-0.9.1/RVC3/models/RRMC2.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/RRMC2.py` & `rvc3python-0.9.1/RVC3/models/RRMC2.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/SEA-main.py` & `rvc3python-0.9.1/RVC3/models/SEA-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/SEA.bd` & `rvc3python-0.9.1/RVC3/models/SEA.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/SEA.py` & `rvc3python-0.9.1/RVC3/models/SEA.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/braitenberg.bd` & `rvc3python-0.9.1/RVC3/models/braitenberg.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/braitenberg.py` & `rvc3python-0.9.1/RVC3/models/braitenberg.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/cartspace.bd` & `rvc3python-0.9.1/RVC3/models/cartspace.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/computed-torque-main.py` & `rvc3python-0.9.1/RVC3/models/computed-torque-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/computed-torque.bd` & `rvc3python-0.9.1/RVC3/models/computed-torque.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/driveconfig.bd` & `rvc3python-0.9.1/RVC3/models/driveconfig.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/driveconfig.py` & `rvc3python-0.9.1/RVC3/models/driveconfig.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/driveline.bd` & `rvc3python-0.9.1/RVC3/models/driveline.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/driveline.py` & `rvc3python-0.9.1/RVC3/models/driveline.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/drivepoint.bd` & `rvc3python-0.9.1/RVC3/models/drivepoint.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/drivepoint.py` & `rvc3python-0.9.1/RVC3/models/drivepoint.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/drivepursuit.bd` & `rvc3python-0.9.1/RVC3/models/drivepursuit.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/drivepursuit.py` & `rvc3python-0.9.1/RVC3/models/drivepursuit.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/feedforward-main.py` & `rvc3python-0.9.1/RVC3/models/feedforward-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/feedforward.bd` & `rvc3python-0.9.1/RVC3/models/feedforward.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/jointspace.bd` & `rvc3python-0.9.1/RVC3/models/jointspace.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/jointspace.py` & `rvc3python-0.9.1/RVC3/models/jointspace.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/lanechange.bd` & `rvc3python-0.9.1/RVC3/models/lanechange.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/lanechange.py` & `rvc3python-0.9.1/RVC3/models/lanechange.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/opspace-main.py` & `rvc3python-0.9.1/RVC3/models/opspace-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/opspace.bd` & `rvc3python-0.9.1/RVC3/models/opspace.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/opspace.py` & `rvc3python-0.9.1/RVC3/models/opspace.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/ploop.bd` & `rvc3python-0.9.1/RVC3/models/ploop.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/ploop.py` & `rvc3python-0.9.1/RVC3/models/ploop.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/ploop_test.bd` & `rvc3python-0.9.1/RVC3/models/ploop_test.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/ploop_test.py` & `rvc3python-0.9.1/RVC3/models/ploop_test.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/quad_model.py` & `rvc3python-0.9.1/RVC3/models/quad_model.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/quadrotor-main.py` & `rvc3python-0.9.1/RVC3/models/quadrotor-main.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/quadrotor.bd` & `rvc3python-0.9.1/RVC3/models/quadrotor.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/quadrotor.py` & `rvc3python-0.9.1/RVC3/models/quadrotor.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/vloop.bd` & `rvc3python-0.9.1/RVC3/models/vloop.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/vloop.py` & `rvc3python-0.9.1/RVC3/models/vloop.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/vloop_test.bd` & `rvc3python-0.9.1/RVC3/models/vloop_test.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/vloop_test.py` & `rvc3python-0.9.1/RVC3/models/vloop_test.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/zerotorque.bd` & `rvc3python-0.9.1/RVC3/models/zerotorque.bd`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/models/zerotorque.py` & `rvc3python-0.9.1/RVC3/models/zerotorque.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/RVC3/tools/rvcprint.py` & `rvc3python-0.9.1/RVC3/tools/rvcprint.py`

 * *Files identical despite different names*

### Comparing `rvc3python-0.9.0/pyproject.toml` & `rvc3python-0.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,86 @@
 [project]
 name = "rvc3python"
-version = "0.9.0"
-authors = [
-  { name="Peter Corke", email="rvc@petercorke.com" },
-]
+version = "0.9.1"
+authors = [{ name = "Peter Corke", email = "rvc@petercorke.com" }]
 description = "Support for book: Robotics, Vision & Control 3 in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     # Indicate who your project is intended for
     "Intended Audience :: Developers",
     # Specify the Python versions you support here.
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = [
-    "robotics", "robot", "manipulator", "robot arm", 
-    "mobile robot", "mobile manipulation",
-    "path planning", "SLAM", "pose graph", 
-    "Dubins", "Reeds-Shepp", "lattice planner", "RRT", "PRM",
-    "rapidly exploring random tree", "probabilistic roadmap planner",
-    "force control", "kinematics", "Jacobian", "position control", "velocity control",
-    "spatial math", 
-    "SO(2)", "SE(2)", "SO(3)", "SE(3)",
-    "twist", "product of exponential", "translation", "orientation",
-    "angle-axis", "Lie group", "skew symmetric matrix",
-    "pose", "translation", "rotation matrix", "rigid body transform", "homogeneous transformation",
-    "Euler angles", "roll-pitch-yaw angles", "quaternion", "unit-quaternion",
-    "computer vision", "machine vision", "robotic vision",
-    "color space", "blackbody", "image segmentation", "blobs",
-    "Hough transform", "k-means", "homography", "camera calibration", "visual odometry",
-    "bundle adjustment",  "stereo vision", "rectification",
+    "robotics",
+    "robot",
+    "manipulator",
+    "robot arm",
+    "mobile robot",
+    "mobile manipulation",
+    "path planning",
+    "SLAM",
+    "pose graph",
+    "Dubins",
+    "Reeds-Shepp",
+    "lattice planner",
+    "RRT",
+    "PRM",
+    "rapidly exploring random tree",
+    "probabilistic roadmap planner",
+    "force control",
+    "kinematics",
+    "Jacobian",
+    "position control",
+    "velocity control",
+    "spatial math",
+    "SO(2)",
+    "SE(2)",
+    "SO(3)",
+    "SE(3)",
+    "twist",
+    "product of exponential",
+    "translation",
+    "orientation",
+    "angle-axis",
+    "Lie group",
+    "skew symmetric matrix",
+    "pose",
+    "translation",
+    "rotation matrix",
+    "rigid body transform",
+    "homogeneous transformation",
+    "Euler angles",
+    "roll-pitch-yaw angles",
+    "quaternion",
+    "unit-quaternion",
+    "computer vision",
+    "machine vision",
+    "robotic vision",
+    "color space",
+    "blackbody",
+    "image segmentation",
+    "blobs",
+    "Hough transform",
+    "k-means",
+    "homography",
+    "camera calibration",
+    "visual odometry",
+    "bundle adjustment",
+    "stereo vision",
+    "rectification",
 ]
 
 dependencies = [
     "matplotlib",
     "roboticstoolbox-python >= 1",
     "machinevision-toolbox-python",
     "bdsim >= 1.1",
@@ -53,18 +92,15 @@
 [project.urls]
 "Homepage" = "https://github.com/petercorke/RVC3-python"
 "Bug Tracker" = "https://github.com/petercorke/RVC3-python/issues"
 "Source" = "https://github.com/petercorke/RVC3-python"
 
 [project.optional-dependencies]
 
-pytorch = [
-    "torch",
-    "torchvision",
-]
+pytorch = ["torch", "torchvision"]
 
 [project.scripts]
 
 rvctool = "RVC3.bin.rvctool:main"
 bdsim_path = "RVC3.bin.bdsim_path:main"
 
 
@@ -76,16 +112,9 @@
 # [tool.setuptools.packages.find]
 # where = ["."]
 
 [tool.setuptools.package-data]
 models = ["*.bd"]
 
 [tool.setuptools]
- 
-packages = [
-    "RVC3",
-    "RVC3.examples",
-    "RVC3.tools",
-    "RVC3.bin",
-    "RVC3.models",
-]
 
+packages = ["RVC3", "RVC3.examples", "RVC3.tools", "RVC3.bin", "RVC3.models"]
```

### Comparing `rvc3python-0.9.0/rvc3python.egg-info/PKG-INFO` & `rvc3python-0.9.1/rvc3python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: rvc3python
-Version: 0.9.0
+Version: 0.9.1
 Summary: Support for book: Robotics, Vision & Control 3 in Python
 Author-email: Peter Corke <rvc@petercorke.com>
 Project-URL: Homepage, https://github.com/petercorke/RVC3-python
 Project-URL: Bug Tracker, https://github.com/petercorke/RVC3-python/issues
 Project-URL: Source, https://github.com/petercorke/RVC3-python
 Keywords: robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly exploring random tree,probabilistic roadmap planner,force control,kinematics,Jacobian,position control,velocity control,spatial math,SO(2),SE(2),SO(3),SE(3),twist,product of exponential,translation,orientation,angle-axis,Lie group,skew symmetric matrix,pose,translation,rotation matrix,rigid body transform,homogeneous transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-quaternion,computer vision,machine vision,robotic vision,color space,blackbody,image segmentation,blobs,Hough transform,k-means,homography,camera calibration,visual odometry,bundle adjustment,stereo vision,rectification
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: pytorch
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: roboticstoolbox-python>=1
+Requires-Dist: machinevision-toolbox-python
+Requires-Dist: bdsim>=1.1
+Requires-Dist: IPython
+Requires-Dist: sympy
+Requires-Dist: pybullet
+Provides-Extra: pytorch
+Requires-Dist: torch; extra == "pytorch"
+Requires-Dist: torchvision; extra == "pytorch"
 
 # Robotics, Vision & Control: 3rd edition in Python (2023)
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 [![PyPI version](https://badge.fury.io/py/rvc3python.svg)](https://badge.fury.io/py/rvc3python)
@@ -42,15 +52,15 @@
 <li>Peter Corke, published by Springer-Nature 2023.</li>
 <li><b>ISBN</b> 978-3-031-06468-5 (hardcopy), 978-3-031-06469-2 (eBook)</li>
 <li><b>DOI</b> <a href="https://doi.org/10.1007/978-3-031-06469-2">10.1007/978-3-031-06469-2</a></li>
 </ul>
 <br><br>
 <p>Report an issue with the book or its supporting code <a href="https://github.com/petercorke/RVC3-python/issues/new/choose">here</a>.</p>
 
-<p>Knwon errata for the book can be viewed <a href="https://github.com/petercorke/RVC3-python/wiki/Errata">here</a>.</p>
+<p>Known errata for the book can be viewed <a href="https://github.com/petercorke/RVC3-python/wiki/Errata">here</a>.</p>
 </td>
 </tr>
 </table>
 
 
 This book uses many examples based on the following open-source Python packages
 
@@ -102,15 +112,15 @@
 Chapter 11 has some deep learning examples based on PyTorch.  If you don't have 
 PyTorch installed you can use the `pytorch` install option
 ```shell
 pip install rvc3python[pytorch]
 ```
 or
 ```shell
-conda install rvc3python[pytorch]
+conda install rvc3python
 ```
 ## Using the Toolboxes
 
 The simplest way to get going is to use the command line tool
 
 ```shell
 $ rvctool
@@ -233,15 +243,15 @@
 experimentation, but in your own code you can handle the imports as you see
 fit.
 
 ### Cutting and pasting
 
 IPython is very forgiving when it comes to cutting and pasting in blocks of Python
 code.  It will strip off the `>>>` prompt character and ignore indentation.  The normal
-python REPL is not so forgiving.  IPython also allows maintains a command history and
+python REPL is not so forgiving.  IPython also maintains a command history and
 allows command editing.
 ### Simple scripting
 You can write very simple scripts, for example `test.py` is
 
 ```python
 T = puma.fkine(puma.qn)
 sol = puma.ikine_LM(T)
@@ -262,14 +272,18 @@
 array([7.235e-08,  -0.8335,  0.09396,    3.142,   0.8312,   -3.142])
 PyPlot3D backend, t = 0.05, scene:
   robot: Text(0.0, 0.0, 'Puma 560')
 >>>
 ```
 and you are dropped into an IPython session after the script has run.
 
+## Issues running on Apple Silicon
+
+Check out the [wiki page](https://github.com/petercorke/RVC3-python/wiki/Running-on-Apple-Silicon).
+
 ## Using Jupyter and Colab
 
 Graphics and animations are problematic in these environments, some things work
 well, some don't.  As much as possible I've tweaked the Jupyter notebooks to work
 as best they can in these environments.
 
 For local use the [Jupyter plugin for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty decent.  Colab suffers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rvc3python Version: 0.9.0 Summary: Support for
+Metadata-Version: 2.1 Name: rvc3python Version: 0.9.1 Summary: Support for
 book: Robotics, Vision & Control 3 in Python Author-email: Peter Corke
 petercorke.com> Project-URL: Homepage, https://github.com/petercorke/RVC3-
 python Project-URL: Bug Tracker, https://github.com/petercorke/RVC3-python/
 issues Project-URL: Source, https://github.com/petercorke/RVC3-python Keywords:
 robotics,robot,manipulator,robot arm,mobile robot,mobile manipulation,path
 planning,SLAM,pose graph,Dubins,Reeds-Shepp,lattice planner,RRT,PRM,rapidly
 exploring random tree,probabilistic roadmap planner,force
@@ -15,23 +15,27 @@
 space,blackbody,image segmentation,blobs,Hough transform,k-
 means,homography,camera calibration,visual odometry,bundle adjustment,stereo
 vision,rectification Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: pytorch License-File: LICENSE # Robotics, Vision & Control: 3rd
-edition in Python (2023) [![A Python Robotics Package](https://
-raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/
-svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-
-python) [![QUT Centre for Robotics Open Source](https://github.com/qcr/
-qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io) [![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: matplotlib Requires-Dist: roboticstoolbox-python>=1 Requires-Dist:
+machinevision-toolbox-python Requires-Dist: bdsim>=1.1 Requires-Dist: IPython
+Requires-Dist: sympy Requires-Dist: pybullet Provides-Extra: pytorch Requires-
+Dist: torch; extra == "pytorch" Requires-Dist: torchvision; extra == "pytorch"
+# Robotics, Vision & Control: 3rd edition in Python (2023) [![A Python Robotics
+Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/
+master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/
+robotics-toolbox-python) [![QUT Centre for Robotics Open Source](https://
+github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/
 rvc3python.svg)](https://badge.fury.io/py/rvc3python) ![PyPI - Python Version]
 (https://img.shields.io/pypi/pyversions/rvc3python.svg) [![PyPI - Downloads]
 (https://img.shields.io/pypi/dw/rvc3python)](https://pypistats.org/packages/
 rvc3python)
                                      Welcome to the online hub for the book:
                                          # RRoobboottiiccss,, VViissiioonn && CCoonnttrrooll:
@@ -42,15 +46,15 @@
                                          # IISSBBNN 978-3-031-06468-5 (hardcopy),
 [Front cover 978-3-031-06468-5_5208]       978-3-031-06469-2 (eBook)
                                          # DDOOII _1_0_._1_0_0_7_/_9_7_8_-_3_-_0_3_1_-_0_6_4_6_9_-_2
 
 
                                      Report an issue with the book or its
                                      supporting code _h_e_r_e.
-                                     Knwon errata for the book can be viewed
+                                     Known errata for the book can be viewed
                                      _h_e_r_e.
 This book uses many examples based on the following open-source Python packages
 _[_R_o_b_o_t_i_c_s_ _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_M_a_c_h_i_n_e_ _V_i_s_i_o_n_ _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_S_p_a_t_i_a_l_ _M_a_t_h_s
 _T_o_o_l_b_o_x_ _f_o_r_ _P_y_t_h_o_n_]_[_B_l_o_c_k_ _d_i_a_g_r_a_m_ _s_i_m_u_l_a_t_i_o_n_ _f_o_r_ _P_y_t_h_o_n_]**Robotics Toolbox for
 Python**, **Machine Vision Toolbox for Python**, **Spatial Maths Toolbox for
 Python**, **Block Diagram Simulation for Python**. These in turn have
 dependencies on other packages created by the author and third parties. ##
@@ -69,35 +73,35 @@
 separated from your other Python code and projects. If you've never used
 virtual environments before this might be a good time to start, and it is
 really easy [using Conda](https://conda.io/projects/conda/en/latest/user-guide/
 install/index.html): ```shell conda create -n RVC3 python=3.10 conda activate
 RVC3 pip install rvc3python ``` ### Installing deep learning tools Chapter 11
 has some deep learning examples based on PyTorch. If you don't have PyTorch
 installed you can use the `pytorch` install option ```shell pip install
-rvc3python[pytorch] ``` or ```shell conda install rvc3python[pytorch] ``` ##
-Using the Toolboxes The simplest way to get going is to use the command line
-tool ```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__
-___ | |_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___
-| | |___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \
-/ _ \/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| |
-(__\__ \_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) |
-| ___) | |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_|
-\___/\/ \____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.1.0,
-MVTB==0.9.5, SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1,
-Matplotlib==3.7.1) import math import numpy as np from scipy import linalg,
-optimize import matplotlib.pyplot as plt from spatialmath import * from
-spatialmath.base import * from spatialmath.base import sym from spatialgeometry
-import * from roboticstoolbox import * from machinevisiontoolbox import *
-import machinevisiontoolbox.base as mvb # useful variables from math import pi
-puma = models.DH.Puma560() panda = models.DH.Panda() func/object? - show brief
-help help(func/object) - show detailed help func/object?? - show source code
-Results of assignments will be displayed, use trailing ; to suppress Python
-3.10.9 | packaged by conda-forge | (main, Feb 2 2023, 20:24:27) [Clang 14.0.6 ]
-Type 'copyright', 'credits' or 'license' for more information IPython 8.11.0 -
-- An enhanced Interactive Python. Type '?' for help. >>> ``` This provides an
+rvc3python[pytorch] ``` or ```shell conda install rvc3python ``` ## Using the
+Toolboxes The simplest way to get going is to use the command line tool
+```shell $ rvctool ____ _ _ _ __ ___ _ ___ ____ _ _ _____ | _ \ ___ | |__ ___ |
+|_(_) ___ ___ \ \ / (_)___(_) ___ _ __ ( _ ) / ___|___ _ __ | |_ _ __ ___ | |
+|___ / | |_) / _ \| '_ \ / _ \| __| |/ __/ __| \ \ / /| / __| |/ _ \| '_ \ / _
+\/\ | | / _ \| '_ \| __| '__/ _ \| | |_ \ | _ < (_) | |_) | (_) | |_| | (__\__
+\_ \ V / | \__ \ | (_) | | | | | (_> < | |__| (_) | | | | |_| | | (_) | | ___)
+| |_| \_\___/|_.__/ \___/ \__|_|\___|___( ) \_/ |_|___/_|\___/|_| |_| \___/\/
+\____\___/|_| |_|\__|_| \___/|_| |____/ |/ for Python (RTB==1.1.0, MVTB==0.9.5,
+SG==1.1.7, SMTB==1.1.7, NumPy==1.24.2, SciPy==1.10.1, Matplotlib==3.7.1) import
+math import numpy as np from scipy import linalg, optimize import
+matplotlib.pyplot as plt from spatialmath import * from spatialmath.base import
+* from spatialmath.base import sym from spatialgeometry import * from
+roboticstoolbox import * from machinevisiontoolbox import * import
+machinevisiontoolbox.base as mvb # useful variables from math import pi puma =
+models.DH.Puma560() panda = models.DH.Panda() func/object? - show brief help
+help(func/object) - show detailed help func/object?? - show source code Results
+of assignments will be displayed, use trailing ; to suppress Python 3.10.9 |
+packaged by conda-forge | (main, Feb 2 2023, 20:24:27) [Clang 14.0.6 ] Type
+'copyright', 'credits' or 'license' for more information IPython 8.11.0 -- An
+enhanced Interactive Python. Type '?' for help. >>> ``` This provides an
 interactive Python ([IPython](https://ipython.readthedocs.io/en/stable))
 session with all the Toolboxes and supporting packages imported, and ready to
 go. It's a highly capable, convenient, and "MATLAB-like" workbench environment
 for robotics and computer vision. For example to load an ETS model of a Panda
 robot, solve a forward kinematics and inverse kinematics problem, and an
 interactive graphical display is simply: ```python >>> panda = models.ETS.Panda
 () ERobot: Panda (by Franka Emika), 7 joints (RRRRRRR)
@@ -143,50 +147,51 @@
 the book, and prompt characters are ignored The Robotics, Vision & Control book
 uses `rvctool` for all the included examples. `rvctool` imports the all the
 above mentioned packages using `import *` which is not considered best Python
 practice. It is very convenient for interactive experimentation, but in your
 own code you can handle the imports as you see fit. ### Cutting and pasting
 IPython is very forgiving when it comes to cutting and pasting in blocks of
 Python code. It will strip off the `>>>` prompt character and ignore
-indentation. The normal python REPL is not so forgiving. IPython also allows
-maintains a command history and allows command editing. ### Simple scripting
-You can write very simple scripts, for example `test.py` is ```python T =
-puma.fkine(puma.qn) sol = puma.ikine_LM(T) sol.q puma.plot(sol.q); ``` then
-```shell $ rvctool test.py 0 0 1 0.5963 0 1 0 -0.1501 -1 0 0 0.6575 0 0 0 1
-IKSolution(q=array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]),
-success=True, iterations=15, searches=1, residual=1.406125546650288e-07,
-reason='Success') array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142])
-PyPlot3D backend, t = 0.05, scene: robot: Text(0.0, 0.0, 'Puma 560') >>> ```
-and you are dropped into an IPython session after the script has run. ## Using
-Jupyter and Colab Graphics and animations are problematic in these
-environments, some things work well, some don't. As much as possible I've
-tweaked the Jupyter notebooks to work as best they can in these environments.
-For local use the [Jupyter plugin for Visual Studio Code](https://
-marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) is pretty
-decent. Colab suffers from old versions of major packages (though they are
-getting better at keeping up to date) and animations can suffer from slow
-update over the network. ## Other command line tools Additional command line
-tools available (from the Robotics Toolbox) include: - `eigdemo`, animation
-showing linear transformation of a rotating unit vector which demonstrates
-eigenvalues and eigenvectors. - `tripleangledemo`, Swift visualization that
-lets you experiment with various triple-angle sequences. - `twistdemo`, Swift
-visualization that lets you experiment with 3D twists. The screw axis is the
-blue rod and you can position and orient it using the sliders, and adjust its
-pitch. Then apply a rotation about the screw using the bottom slider. # Block
-diagram models _[_b_d_s_i_m_ _l_o_g_o_]Block diagram models are key to the pedagogy of the
-RVC3 book and 25 models are included. To simulate these models we use the
-Python package [bdsim](https://github.com/petercorke/bdsim) which can run
-models: - written in Python using [bdsim](https://github.com/petercorke/
-bdsim#getting-started) blocks and wiring. - created graphically using [bdedit]
-(https://github.com/petercorke/bdsim#bdedit-the-graphical-editing-tool) and
-saved as a `.bd` (JSON format) file. The models are included in the `RVC3`
-package when it is installed and `rvctool` adds them to the module search path.
-This means you can invoke them from `rvctool` by ```python >>> %run -
-m vloop_test ``` If you want to directly access the folder containing the
-models, the command line tool ```shell bdsim_path ``` will display the full
+indentation. The normal python REPL is not so forgiving. IPython also maintains
+a command history and allows command editing. ### Simple scripting You can
+write very simple scripts, for example `test.py` is ```python T = puma.fkine
+(puma.qn) sol = puma.ikine_LM(T) sol.q puma.plot(sol.q); ``` then ```shell $
+rvctool test.py 0 0 1 0.5963 0 1 0 -0.1501 -1 0 0 0.6575 0 0 0 1 IKSolution
+(q=array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]), success=True,
+iterations=15, searches=1, residual=1.406125546650288e-07, reason='Success')
+array([7.235e-08, -0.8335, 0.09396, 3.142, 0.8312, -3.142]) PyPlot3D backend, t
+= 0.05, scene: robot: Text(0.0, 0.0, 'Puma 560') >>> ``` and you are dropped
+into an IPython session after the script has run. ## Issues running on Apple
+Silicon Check out the [wiki page](https://github.com/petercorke/RVC3-python/
+wiki/Running-on-Apple-Silicon). ## Using Jupyter and Colab Graphics and
+animations are problematic in these environments, some things work well, some
+don't. As much as possible I've tweaked the Jupyter notebooks to work as best
+they can in these environments. For local use the [Jupyter plugin for Visual
+Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-
+toolsai.jupyter) is pretty decent. Colab suffers from old versions of major
+packages (though they are getting better at keeping up to date) and animations
+can suffer from slow update over the network. ## Other command line tools
+Additional command line tools available (from the Robotics Toolbox) include: -
+`eigdemo`, animation showing linear transformation of a rotating unit vector
+which demonstrates eigenvalues and eigenvectors. - `tripleangledemo`, Swift
+visualization that lets you experiment with various triple-angle sequences. -
+`twistdemo`, Swift visualization that lets you experiment with 3D twists. The
+screw axis is the blue rod and you can position and orient it using the
+sliders, and adjust its pitch. Then apply a rotation about the screw using the
+bottom slider. # Block diagram models _[_b_d_s_i_m_ _l_o_g_o_]Block diagram models are key
+to the pedagogy of the RVC3 book and 25 models are included. To simulate these
+models we use the Python package [bdsim](https://github.com/petercorke/bdsim)
+which can run models: - written in Python using [bdsim](https://github.com/
+petercorke/bdsim#getting-started) blocks and wiring. - created graphically
+using [bdedit](https://github.com/petercorke/bdsim#bdedit-the-graphical-
+editing-tool) and saved as a `.bd` (JSON format) file. The models are included
+in the `RVC3` package when it is installed and `rvctool` adds them to the
+module search path. This means you can invoke them from `rvctool` by ```python
+>>> %run -m vloop_test ``` If you want to directly access the folder containing
+the models, the command line tool ```shell bdsim_path ``` will display the full
 path to where they have been installed in the Python package tree. # Additional
 book resources [Front cover 978-3-031-06468-5_5208]This GitHub repo provides
 additional resources for readers including: - Jupyter notebooks containing all
 code lines from each chapter, see the [`notebooks`](notebooks) folder - The
 code to produce every Python/Matplotlib (2D) figure in the book, see the
 [`figures`](figures) folder - 3D points clouds from chapter 14, and the code to
 create them, see the [`pointclouds`](../pointclouds) folder. - 3D figures from
```

### Comparing `rvc3python-0.9.0/rvc3python.egg-info/SOURCES.txt` & `rvc3python-0.9.1/rvc3python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

