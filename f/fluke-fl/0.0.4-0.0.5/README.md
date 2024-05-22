# Comparing `tmp/fluke_fl-0.0.4.tar.gz` & `tmp/fluke_fl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluke_fl-0.0.4.tar", last modified: Mon May 20 16:20:03 2024, max compression
+gzip compressed data, was "fluke_fl-0.0.5.tar", last modified: Wed May 22 10:15:37 2024, max compression
```

## Comparing `fluke_fl-0.0.4.tar` & `fluke_fl-0.0.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 16:20:03.129289 fluke_fl-0.0.4/
--rw-r--r--   0 mirko      (501) staff       (20)    26083 2024-05-16 12:16:36.000000 fluke_fl-0.0.4/LICENSE
--rw-r--r--   0 mirko      (501) staff       (20)    34816 2024-05-20 16:20:03.128904 fluke_fl-0.0.4/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)     3585 2024-05-20 06:05:54.000000 fluke_fl-0.0.4/README.md
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 16:20:03.112962 fluke_fl-0.0.4/fluke/
--rw-r--r--   0 mirko      (501) staff       (20)     8686 2024-05-20 12:55:54.000000 fluke_fl-0.0.4/fluke/__init__.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 16:20:03.119082 fluke_fl-0.0.4/fluke/algorithms/
--rw-r--r--   0 mirko      (501) staff       (20)     9448 2024-05-16 13:37:43.000000 fluke_fl-0.0.4/fluke/algorithms/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)     3711 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/apfl.py
--rw-r--r--   0 mirko      (501) staff       (20)     5907 2024-05-17 07:28:01.000000 fluke_fl-0.0.4/fluke/algorithms/ccvr.py
--rw-r--r--   0 mirko      (501) staff       (20)     3250 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/ditto.py
--rw-r--r--   0 mirko      (501) staff       (20)     5018 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedamp.py
--rw-r--r--   0 mirko      (501) staff       (20)      496 2024-04-23 11:33:36.000000 fluke_fl-0.0.4/fluke/algorithms/fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     1893 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedavgm.py
--rw-r--r--   0 mirko      (501) staff       (20)     4089 2024-05-17 07:29:44.000000 fluke_fl-0.0.4/fluke/algorithms/fedbabu.py
--rw-r--r--   0 mirko      (501) staff       (20)     1333 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedbn.py
--rwxr-xr-x   0 mirko      (501) staff       (20)     7466 2024-05-17 07:32:27.000000 fluke_fl-0.0.4/fluke/algorithms/feddyn.py
--rw-r--r--   0 mirko      (501) staff       (20)     1914 2024-05-19 10:47:03.000000 fluke_fl-0.0.4/fluke/algorithms/fedexp.py
--rw-r--r--   0 mirko      (501) staff       (20)     6855 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedhp.py
--rw-r--r--   0 mirko      (501) staff       (20)     1746 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedlc.py
--rw-r--r--   0 mirko      (501) staff       (20)     9164 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fednh.py
--rw-r--r--   0 mirko      (501) staff       (20)     2723 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fednova.py
--rw-r--r--   0 mirko      (501) staff       (20)     3536 2024-05-16 12:28:24.000000 fluke_fl-0.0.4/fluke/algorithms/fedopt.py
--rw-r--r--   0 mirko      (501) staff       (20)     1968 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedper.py
--rw-r--r--   0 mirko      (501) staff       (20)     7053 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedproto.py
--rw-r--r--   0 mirko      (501) staff       (20)     2075 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedprox.py
--rw-r--r--   0 mirko      (501) staff       (20)     4047 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedrep.py
--rw-r--r--   0 mirko      (501) staff       (20)      870 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/fedsgd.py
--rw-r--r--   0 mirko      (501) staff       (20)     2235 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/lg_fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     3233 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/moon.py
--rw-r--r--   0 mirko      (501) staff       (20)     5686 2024-05-17 10:05:44.000000 fluke_fl-0.0.4/fluke/algorithms/per_fedavg.py
--rw-r--r--   0 mirko      (501) staff       (20)     5090 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/pfedme.py
--rw-r--r--   0 mirko      (501) staff       (20)     7374 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/scaffold.py
--rw-r--r--   0 mirko      (501) staff       (20)     5580 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/algorithms/superfed.py
--rw-r--r--   0 mirko      (501) staff       (20)    11592 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/client.py
--rw-r--r--   0 mirko      (501) staff       (20)    10376 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/comm.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 16:20:03.119684 fluke_fl-0.0.4/fluke/data/
--rw-r--r--   0 mirko      (501) staff       (20)    34120 2024-05-16 12:25:40.000000 fluke_fl-0.0.4/fluke/data/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)    32234 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/data/datasets.py
--rw-r--r--   0 mirko      (501) staff       (20)     6875 2024-05-17 12:07:25.000000 fluke_fl-0.0.4/fluke/data/support.py
--rw-r--r--   0 mirko      (501) staff       (20)     7167 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/evaluation.py
--rw-r--r--   0 mirko      (501) staff       (20)     1765 2024-05-20 12:55:54.000000 fluke_fl-0.0.4/fluke/get.py
--rw-r--r--   0 mirko      (501) staff       (20)    42854 2024-05-20 15:03:29.000000 fluke_fl-0.0.4/fluke/nets.py
--rw-r--r--   0 mirko      (501) staff       (20)     7223 2024-05-20 13:46:11.000000 fluke_fl-0.0.4/fluke/run.py
--rw-r--r--   0 mirko      (501) staff       (20)    15016 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/fluke/server.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 16:20:03.120116 fluke_fl-0.0.4/fluke/utils/
--rw-r--r--   0 mirko      (501) staff       (20)    22022 2024-05-17 07:33:13.000000 fluke_fl-0.0.4/fluke/utils/__init__.py
--rw-r--r--   0 mirko      (501) staff       (20)    23035 2024-05-17 12:17:19.000000 fluke_fl-0.0.4/fluke/utils/model.py
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 16:20:03.128272 fluke_fl-0.0.4/fluke_fl.egg-info/
--rw-r--r--   0 mirko      (501) staff       (20)    34816 2024-05-20 16:20:03.000000 fluke_fl-0.0.4/fluke_fl.egg-info/PKG-INFO
--rw-r--r--   0 mirko      (501) staff       (20)     1398 2024-05-20 16:20:03.000000 fluke_fl-0.0.4/fluke_fl.egg-info/SOURCES.txt
--rw-r--r--   0 mirko      (501) staff       (20)        1 2024-05-20 16:20:03.000000 fluke_fl-0.0.4/fluke_fl.egg-info/dependency_links.txt
--rw-r--r--   0 mirko      (501) staff       (20)       68 2024-05-20 16:20:03.000000 fluke_fl-0.0.4/fluke_fl.egg-info/entry_points.txt
--rw-r--r--   0 mirko      (501) staff       (20)       96 2024-05-20 16:20:03.000000 fluke_fl-0.0.4/fluke_fl.egg-info/requires.txt
--rw-r--r--   0 mirko      (501) staff       (20)        6 2024-05-20 16:20:03.000000 fluke_fl-0.0.4/fluke_fl.egg-info/top_level.txt
--rw-r--r--   0 mirko      (501) staff       (20)     1752 2024-05-20 12:59:44.000000 fluke_fl-0.0.4/pyproject.toml
--rw-r--r--   0 mirko      (501) staff       (20)       38 2024-05-20 16:20:03.129359 fluke_fl-0.0.4/setup.cfg
-drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-20 16:20:03.127671 fluke_fl-0.0.4/tests/
--rw-r--r--   0 mirko      (501) staff       (20)    10293 2024-05-17 10:06:41.000000 fluke_fl-0.0.4/tests/test_alg.py
--rw-r--r--   0 mirko      (501) staff       (20)     4397 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/tests/test_client.py
--rw-r--r--   0 mirko      (501) staff       (20)     3331 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/tests/test_comm.py
--rw-r--r--   0 mirko      (501) staff       (20)     2130 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/tests/test_core.py
--rw-r--r--   0 mirko      (501) staff       (20)    11108 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/tests/test_data.py
--rw-r--r--   0 mirko      (501) staff       (20)    12738 2024-05-17 12:09:41.000000 fluke_fl-0.0.4/tests/test_datasets.py
--rw-r--r--   0 mirko      (501) staff       (20)     2895 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/tests/test_eval.py
--rw-r--r--   0 mirko      (501) staff       (20)     4620 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/tests/test_nets.py
--rw-r--r--   0 mirko      (501) staff       (20)     3716 2024-05-16 11:01:26.000000 fluke_fl-0.0.4/tests/test_server.py
--rw-r--r--   0 mirko      (501) staff       (20)    13910 2024-05-17 12:13:40.000000 fluke_fl-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.134829 fluke_fl-0.0.5/
+-rw-r--r--   0 mirko      (501) staff       (20)    26083 2024-05-16 12:16:36.000000 fluke_fl-0.0.5/LICENSE
+-rw-r--r--   0 mirko      (501) staff       (20)    34816 2024-05-22 10:15:37.134522 fluke_fl-0.0.5/PKG-INFO
+-rw-r--r--   0 mirko      (501) staff       (20)     3585 2024-05-20 06:05:54.000000 fluke_fl-0.0.5/README.md
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.119082 fluke_fl-0.0.5/fluke/
+-rw-r--r--   0 mirko      (501) staff       (20)     8686 2024-05-20 12:55:54.000000 fluke_fl-0.0.5/fluke/__init__.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.124249 fluke_fl-0.0.5/fluke/algorithms/
+-rw-r--r--   0 mirko      (501) staff       (20)     9464 2024-05-21 10:25:58.000000 fluke_fl-0.0.5/fluke/algorithms/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4190 2024-05-22 09:54:10.000000 fluke_fl-0.0.5/fluke/algorithms/apfl.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6799 2024-05-22 10:05:38.000000 fluke_fl-0.0.5/fluke/algorithms/ccvr.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3525 2024-05-22 09:23:04.000000 fluke_fl-0.0.5/fluke/algorithms/ditto.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5320 2024-05-22 09:23:10.000000 fluke_fl-0.0.5/fluke/algorithms/fedamp.py
+-rw-r--r--   0 mirko      (501) staff       (20)      469 2024-05-22 09:24:56.000000 fluke_fl-0.0.5/fluke/algorithms/fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3271 2024-05-22 09:23:25.000000 fluke_fl-0.0.5/fluke/algorithms/fedavgm.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4353 2024-05-22 09:23:33.000000 fluke_fl-0.0.5/fluke/algorithms/fedbabu.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1637 2024-05-22 09:29:52.000000 fluke_fl-0.0.5/fluke/algorithms/fedbn.py
+-rwxr-xr-x   0 mirko      (501) staff       (20)     7778 2024-05-22 09:30:25.000000 fluke_fl-0.0.5/fluke/algorithms/feddyn.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2180 2024-05-22 09:32:13.000000 fluke_fl-0.0.5/fluke/algorithms/fedexp.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7055 2024-05-22 09:32:36.000000 fluke_fl-0.0.5/fluke/algorithms/fedhp.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2043 2024-05-22 09:33:04.000000 fluke_fl-0.0.5/fluke/algorithms/fedlc.py
+-rw-r--r--   0 mirko      (501) staff       (20)     9460 2024-05-22 09:33:37.000000 fluke_fl-0.0.5/fluke/algorithms/fednh.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3035 2024-05-22 09:34:16.000000 fluke_fl-0.0.5/fluke/algorithms/fednova.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3857 2024-05-22 09:34:46.000000 fluke_fl-0.0.5/fluke/algorithms/fedopt.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2252 2024-05-22 09:35:13.000000 fluke_fl-0.0.5/fluke/algorithms/fedper.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7361 2024-05-22 09:35:49.000000 fluke_fl-0.0.5/fluke/algorithms/fedproto.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2404 2024-05-22 09:36:25.000000 fluke_fl-0.0.5/fluke/algorithms/fedprox.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4338 2024-05-22 09:37:49.000000 fluke_fl-0.0.5/fluke/algorithms/fedrep.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1189 2024-05-22 09:37:52.000000 fluke_fl-0.0.5/fluke/algorithms/fedsgd.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2625 2024-05-22 09:38:31.000000 fluke_fl-0.0.5/fluke/algorithms/lg_fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3452 2024-05-22 09:39:06.000000 fluke_fl-0.0.5/fluke/algorithms/moon.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6000 2024-05-22 09:39:47.000000 fluke_fl-0.0.5/fluke/algorithms/per_fedavg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5345 2024-05-22 09:40:21.000000 fluke_fl-0.0.5/fluke/algorithms/pfedme.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7712 2024-05-22 10:07:02.000000 fluke_fl-0.0.5/fluke/algorithms/scaffold.py
+-rw-r--r--   0 mirko      (501) staff       (20)     5841 2024-05-22 10:00:13.000000 fluke_fl-0.0.5/fluke/algorithms/superfed.py
+-rw-r--r--   0 mirko      (501) staff       (20)    11606 2024-05-20 18:17:39.000000 fluke_fl-0.0.5/fluke/client.py
+-rw-r--r--   0 mirko      (501) staff       (20)    10376 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/fluke/comm.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.124797 fluke_fl-0.0.5/fluke/data/
+-rw-r--r--   0 mirko      (501) staff       (20)    34115 2024-05-20 18:13:10.000000 fluke_fl-0.0.5/fluke/data/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)    32705 2024-05-22 09:08:12.000000 fluke_fl-0.0.5/fluke/data/datasets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     6875 2024-05-17 12:07:25.000000 fluke_fl-0.0.5/fluke/data/support.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7167 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/fluke/evaluation.py
+-rw-r--r--   0 mirko      (501) staff       (20)     1842 2024-05-22 07:24:47.000000 fluke_fl-0.0.5/fluke/get.py
+-rw-r--r--   0 mirko      (501) staff       (20)    42854 2024-05-20 15:03:29.000000 fluke_fl-0.0.5/fluke/nets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     7923 2024-05-21 09:55:17.000000 fluke_fl-0.0.5/fluke/run.py
+-rw-r--r--   0 mirko      (501) staff       (20)    15723 2024-05-20 18:19:27.000000 fluke_fl-0.0.5/fluke/server.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.125165 fluke_fl-0.0.5/fluke/utils/
+-rw-r--r--   0 mirko      (501) staff       (20)    22022 2024-05-17 07:33:13.000000 fluke_fl-0.0.5/fluke/utils/__init__.py
+-rw-r--r--   0 mirko      (501) staff       (20)    23035 2024-05-17 12:17:19.000000 fluke_fl-0.0.5/fluke/utils/model.py
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.134107 fluke_fl-0.0.5/fluke_fl.egg-info/
+-rw-r--r--   0 mirko      (501) staff       (20)    34816 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/PKG-INFO
+-rw-r--r--   0 mirko      (501) staff       (20)     1398 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/SOURCES.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        1 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/dependency_links.txt
+-rw-r--r--   0 mirko      (501) staff       (20)       68 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/entry_points.txt
+-rw-r--r--   0 mirko      (501) staff       (20)       96 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/requires.txt
+-rw-r--r--   0 mirko      (501) staff       (20)        6 2024-05-22 10:15:37.000000 fluke_fl-0.0.5/fluke_fl.egg-info/top_level.txt
+-rw-r--r--   0 mirko      (501) staff       (20)     1752 2024-05-22 08:49:06.000000 fluke_fl-0.0.5/pyproject.toml
+-rw-r--r--   0 mirko      (501) staff       (20)       38 2024-05-22 10:15:37.135011 fluke_fl-0.0.5/setup.cfg
+drwxr-xr-x   0 mirko      (501) staff       (20)        0 2024-05-22 10:15:37.133548 fluke_fl-0.0.5/tests/
+-rw-r--r--   0 mirko      (501) staff       (20)    10293 2024-05-17 10:06:41.000000 fluke_fl-0.0.5/tests/test_alg.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4397 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_client.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3331 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_comm.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2130 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_core.py
+-rw-r--r--   0 mirko      (501) staff       (20)    11108 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_data.py
+-rw-r--r--   0 mirko      (501) staff       (20)    12738 2024-05-17 12:09:41.000000 fluke_fl-0.0.5/tests/test_datasets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     2895 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_eval.py
+-rw-r--r--   0 mirko      (501) staff       (20)     4620 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_nets.py
+-rw-r--r--   0 mirko      (501) staff       (20)     3716 2024-05-16 11:01:26.000000 fluke_fl-0.0.5/tests/test_server.py
+-rw-r--r--   0 mirko      (501) staff       (20)    13910 2024-05-17 12:13:40.000000 fluke_fl-0.0.5/tests/test_utils.py
```

### Comparing `fluke_fl-0.0.4/LICENSE` & `fluke_fl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/PKG-INFO` & `fluke_fl-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-fl
-Version: 0.0.4
+Version: 0.0.5
 Summary: Federated Learning Utility framework for Experimentation and research.
 Author-email: Mirko Polato <mirko.polato@unito.it>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
```

### Comparing `fluke_fl-0.0.4/README.md` & `fluke_fl-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/fluke/__init__.py` & `fluke_fl-0.0.5/fluke/__init__.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/fluke/algorithms/__init__.py` & `fluke_fl-0.0.5/fluke/algorithms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""This module contains the implementation of several the federated learning algorithms."""
+"""This module contains (as submodules) the implementation of several the federated learning
+algorithms."""
 from __future__ import annotations
 import torch
 from typing import Callable, Union, Any, Iterable
 from copy import deepcopy
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/apfl.py` & `fluke_fl-0.0.5/fluke/algorithms/apfl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Implementation of the [APFL20]_ algorithm.
+
+References:
+    .. [APFL20] Yuyang Deng, Mohammad Mahdi Kamani, and Mehrdad Mahdavi. Adaptive Personalized
+       Federated Learning. In: arXiv (2020). URL: https://arxiv.org/abs/2003.13461
+"""
 from copy import deepcopy
 from torch.nn import Module
 import torch
 from typing import Any, Callable, Iterable
 import sys
 sys.path.append(".")
 sys.path.append("..")
@@ -94,14 +100,20 @@
                  weighted: bool = False,
                  tau: int = 3):
         super().__init__(model, test_data, clients, eval_every, weighted)
         self.hyper_params.update(tau=tau)
 
     @torch.no_grad()
     def aggregate(self, eligible: Iterable[Client]) -> None:
+        """Aggregate the models of the eligible clients every `hyper_params.tau` rounds.
+
+        Args:
+            eligible (Iterable[Client]): The clients that are eligible to participate in the
+                aggregation.
+        """
         if self.rounds % self.hyper_params.tau != 0:
             # Ignore the sent models and clear the channel's cache
             self.channel.clear(self)
         else:
             super().aggregate(eligible)
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/ccvr.py` & `fluke_fl-0.0.5/fluke/algorithms/ccvr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [CCVR21]_ algorithm.
+
+References:
+    .. [CCVR21] Mi Luo, Fei Chen, Dapeng Hu, Yifan Zhang, Jian Liang, Jiashi Feng. No Fear of
+       Heterogeneity: Classifier Calibration for Federated Learning with Non-IID Data. In: NeurIPS
+       (2021). URL: https://arxiv.org/abs/2106.05001
+"""
 import torch
 import numpy as np
 import sys
 from typing import Sequence
 
 from torch.nn.modules import Module
 
@@ -13,15 +20,19 @@
 from ..comm import Message  # NOQA
 from ..data import FastDataLoader  # NOQA
 from . import CentralizedFL  # NOQA
 
 
 class CCVRClient(Client):
     @torch.no_grad()
-    def compute_mean_cov(self):
+    def compute_mean_cov(self) -> None:
+        """Computes the label-wise mean and covariance of the data. After the computation, the
+        client send (through the channel) a message to the server containing the computed values and
+        the number of examples per class.
+        """
         list_z, list_y = [], []
         for _, (X, y) in enumerate(self.train_set):
             X, y = X.to(self.device), y.to(self.device)
             Z = self.model.forward_encoder(X)
             list_z.append(Z)
             list_y.append(y)
 
@@ -65,15 +76,15 @@
         super().__init__(model, test_data, clients, eval_every, weighted)
         self.hyper_params.update(
             lr=lr,
             batch_size=batch_size,
             sample_per_class=sample_per_class
         )
 
-    def _compute_mean_cov(self):
+    def _compute_mean_cov(self) -> tuple[list[torch.Tensor], list[torch.Tensor]]:
         means, covs, ns = [], [], []
         for client in self.clients:
             client.receive_model()
             client.compute_mean_cov()
             mean, cov, n = self.channel.receive(self, client, msg_type="mean_cov").payload
             means.append(mean)
             covs.append(cov)
@@ -104,16 +115,17 @@
                 classes_cov[c] -= (ex_x_class[c] / (ex_x_class[c] - 1)) * (
                     torch.outer(classes_mean[c], classes_mean[c])
                 )
 
         return classes_mean, classes_cov
 
     def _generate_virtual_repr(self,
-                               classes_mean: Sequence[torch.tensor],
-                               classes_cov: Sequence[torch.tensor]):
+                               classes_mean: Sequence[torch.Tensor],
+                               classes_cov: Sequence[torch.Tensor]) -> tuple[torch.Tensor,
+                                                                             torch.Tensor]:
         data, targets = [], []
         for c, (mean, cov) in enumerate(zip(classes_mean, classes_cov)):
             if mean is not None and cov is not None:
                 samples = np.random.multivariate_normal(
                     mean.cpu().numpy(),
                     cov.cpu().numpy(),
                     self.hyper_params.sample_per_class,
@@ -126,15 +138,15 @@
                     ) * c
                 )
 
         data = torch.cat(data)
         targets = torch.cat(targets)
         return data, targets
 
-    def _calibrate(self, Z_train: torch.FloatTensor, y_train: torch.LongTensor):
+    def _calibrate(self, Z_train: torch.FloatTensor, y_train: torch.LongTensor) -> None:
         self.model.train()
         self.model.to(self.device)
 
         # FIXME: loss, optimizer and scheduler are fixed for now
         optimizer = torch.optim.SGD(self.model.head.parameters(), lr=self.hyper_params.lr)
         loss_fn = torch.nn.CrossEntropyLoss()
         train_set = FastDataLoader(Z_train,
@@ -149,14 +161,17 @@
             y_hat = self.model.forward_head(Z)
             loss = loss_fn(y_hat, y)
             loss.backward()
             optimizer.step()
         self.model.to("cpu")
 
     def finalize(self) -> None:
+        """In the CCVR Server, at the end of the learning the model is calibrated according to the
+        data distributions of the clients.
+        """
         self.broadcast_model(self.clients)
         classes_mean, classes_cov = self._compute_mean_cov()
         Z, y = self._generate_virtual_repr(classes_mean, classes_cov)
         self._calibrate(Z, y)
         super().finalize()
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/ditto.py` & `fluke_fl-0.0.5/fluke/algorithms/ditto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [Ditto21]_ algorithm.
+
+References:
+    .. [Ditto21] Tian Li, Shengyuan Hu, Ahmad Beirami, and Virginia Smith. Ditto: Fair and Robust
+       Federated Learning Through Personalization. In: ICML (2021).
+       URL: https://arxiv.org/abs/2012.04221
+"""
 from copy import deepcopy
 import torch
 from typing import Any, Callable
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedamp.py` & `fluke_fl-0.0.5/fluke/algorithms/fedamp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedAMP21]_ algorithm.
+
+References:
+    .. [FedAMP21] Yutao Huang, Lingyang Chu, Zirui Zhou, Lanjun Wang, Jiangchuan Liu, Jian Pei, Yong
+       Zhang. Personalized Cross-Silo Federated Learning on Non-IID Data. In: AAAI (2021).
+       URL: https://arxiv.org/abs/2007.03797
+"""
 from torch.nn import Module
 import torch
 from typing import Callable, Sequence
 from copy import deepcopy
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedavgm.py` & `fluke_fl-0.0.5/fluke/algorithms/fedexp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,61 @@
-from torch.nn import Module
-import torch
+"""Implementation of the [FedExP23]_ algorithm.
+
+References:
+    .. [FedExP23] Divyansh Jhunjhunwala, Shiqiang Wang, and Gauri Joshi.
+       FedExP: Speeding Up Federated Averaging via Extrapolation. In: ICLR (2023).
+       URL: https://arxiv.org/abs/2301.09604
+"""
 from collections import OrderedDict
 from typing import Iterable
+import torch
 import sys
 sys.path.append(".")
 sys.path.append("..")
 
-from ..data import FastDataLoader  # NOQA
 from ..algorithms import CentralizedFL  # NOQA
 from ..utils.model import diff_model, STATE_DICT_KEYS_TO_IGNORE  # NOQA
 from ..server import Server  # NOQA
 from ..client import Client  # NOQA
 
 
-class FedAVGMServer(Server):
-    def __init__(self,
-                 model: Module,
-                 test_data: FastDataLoader,
-                 clients: Iterable[Client],
-                 eval_every: int = 1,
-                 weighted: bool = True,
-                 momentum: float = 0.9):
-        super().__init__(model, test_data, clients, eval_every, weighted)
-        self.hyper_params.update(momentum=momentum)
+class FedExPServer(Server):
 
     @torch.no_grad()
     def aggregate(self, eligible: Iterable[Client]) -> None:
-        avg_model_sd = OrderedDict()
         clients_sd = self.get_client_models(eligible)
         clients_diff = [diff_model(self.model.state_dict(), client_model)
                         for client_model in clients_sd]
-        weights = self._get_client_weights(eligible)
+        eta, mu_diff = self._compute_eta(clients_diff)
 
+        avg_model_sd = OrderedDict()
+        w = self.model.state_dict()
         for key in self.model.state_dict().keys():
             if key.endswith(STATE_DICT_KEYS_TO_IGNORE):
+                # avg_model_sd[key] = clients_sd[0][key].clone()
                 avg_model_sd[key] = self.model.state_dict()[key].clone()
                 continue
-            for i, client_diff in enumerate(clients_diff):
-                if key not in avg_model_sd:
-                    avg_model_sd[key] = weights[i] * client_diff[key]
-                else:
-                    avg_model_sd[key] += weights[i] * client_diff[key]
+            avg_model_sd[key] = w[key] - eta[key] * mu_diff[key]
+        self.model.load_state_dict(avg_model_sd)
+
+    def _compute_eta(self, clients_diff: Iterable[dict], eps: float = 1e-4) -> float:
+        num = {}
+        den = {}
+        mu_diff = {}
+        eta = {}
+        M = len(clients_diff)
+
+        for key in clients_diff[0].keys():
+            if key.endswith(STATE_DICT_KEYS_TO_IGNORE):
+                continue
+            num[key] = torch.sum(torch.FloatTensor([torch.norm(c[key])**2 for c in clients_diff]))
+            mu_diff[key] = torch.mean(torch.stack([c[key] for c in clients_diff]), dim=0)
+            den[key] = 2 * M * (torch.norm(mu_diff[key])**2 + eps)
+            eta[key] = torch.max(num[key] / den[key], torch.FloatTensor([1.0]))
 
-        for key, param in self.model.named_parameters():
-            param.data = self.hyper_params.momentum * param.data - avg_model_sd[key].data
+        return eta, mu_diff
 
 
-class FedAVGM(CentralizedFL):
+class FedExP(CentralizedFL):
 
     def get_server_class(self) -> Server:
-        return FedAVGMServer
+        return FedExPServer
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedbabu.py` & `fluke_fl-0.0.5/fluke/algorithms/fedbabu.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Implementation of the [FedBABU22]_ algorithm.
+
+References:
+    .. [FedBABU22] Jaehoon Oh, Sangmook Kim, Se-Young Yun. FedBABU: Towards Enhanced Representation
+       for Federated Image Classification. In: ICLR (2022). URL: https://arxiv.org/abs/2106.06042
+"""
 from rich.progress import Progress
 from typing import Any, Callable, Sequence
 from torch.nn import Module
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedbn.py` & `fluke_fl-0.0.5/fluke/algorithms/fedbn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedBN21]_ algorithm.
+
+References:
+    .. [FedBN21] Xiaoxiao Li, Meirui JIANG, Xiaofei Zhang, Michael Kamp, and Qi Dou. FedBN:
+       Federated Learning on Non-IID Features via Local Batch Normalization. In: ICLR (2021).
+       URL: https://openreview.net/pdf?id=6YEQUn0QICG
+"""
 import torch
 import sys
 sys.path.append(".")
 sys.path.append("..")
 
 from ..algorithms import CentralizedFL  # NOQA
 from ..client import Client  # NOQA
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/feddyn.py` & `fluke_fl-0.0.5/fluke/algorithms/feddyn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedDyn21]_ algorithm.
+
+References:
+    .. [FedDyn21] Durmus Alp Emre Acar, Yue Zhao, Ramon Matas, Matthew Mattina, Paul Whatmough,
+       and Venkatesh Saligrama. Federated Learning with Dynamic Regularization.
+       In: ICLR (2021). URL: https://openreview.net/pdf?id=B7v4QMR6Z9w
+"""
 from torch.nn import Module
 import numpy as np
 import torch
 from typing import Callable, Iterable
 from collections import OrderedDict
 from copy import deepcopy
 import sys
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedhp.py` & `fluke_fl-0.0.5/fluke/algorithms/fedhp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Implementation of the [FedHP24]_ algorithm.
+
+References:
+    .. [FedHP24] Samuele Fonio, Mirko Polato, Roberto Esposito. Federated Hyperbolic Prototype
+       Learning. Submitted to ESANN 2024
+"""
 from typing import Sequence, Callable
 import torch
 from torch import nn
 # from torch.optim import Adam
 from rich.progress import track
 import sys
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedlc.py` & `fluke_fl-0.0.5/fluke/algorithms/fedlc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedLC22]_ algorithm.
+
+References:
+    .. [FedLC22] Jie Zhang, Zhiqi Li, Bo Li, Jianghe Xu, Shuang Wu, Shouhong Ding, Chao Wu.
+       Federated Learning with Label Distribution Skew via Logits Calibration. In: ICML (2022).
+       URL: https://arxiv.org/abs/2209.00189
+"""
 from collections import Counter
 from typing import Callable
 import torch
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fednh.py` & `fluke_fl-0.0.5/fluke/algorithms/fednh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedNH23]_ algorithm.
+
+References:
+    .. [FedNH23] Yutong Dai, Zeyuan Chen, Junnan Li, Shelby Heinecke, Lichao Sun, Ran Xu.
+       Tackling Data Heterogeneity in Federated Learning with Class Prototypes. In: AAAI (2023).
+       URL: https://arxiv.org/abs/2212.02758
+"""
 from collections import OrderedDict
 import torch
 from torch.nn import Module, Parameter, CrossEntropyLoss
 from typing import Sequence, Callable
 from collections import defaultdict
 import sys
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fednova.py` & `fluke_fl-0.0.5/fluke/algorithms/fednova.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedNova21]_ algorithm.
+
+References:
+    .. [FedNova21] Jianyu Wang, Qinghua Liu, Hao Liang, Gauri Joshi, and H. Vincent Poor.
+       Tackling the Objective Inconsistency Problem in Heterogeneous Federated Optimization.
+       In: NeurIPS 2020. URL: https://arxiv.org/abs/2007.07481
+"""
 import torch
 from typing import Callable, Iterable
 from copy import deepcopy
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedopt.py` & `fluke_fl-0.0.5/fluke/algorithms/fedopt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedOpt21]_ algorithm.
+
+References:
+    .. [FedOpt21] Sashank Reddi, Zachary Charles, Manzil Zaheer, Zachary Garrett, Keith Rush,
+       Jakub Konečný, Sanjiv Kumar, H. Brendan McMahan. Adaptive Federated Optimization.
+       In: ICLR (2021). URL: https://openreview.net/pdf?id=LkFG3lB13U5
+"""
 from torch.nn import Module
 import torch
 from collections import OrderedDict
 from typing import Iterable
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedper.py` & `fluke_fl-0.0.5/fluke/algorithms/fedper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedPer19]_ algorithm.
+
+References:
+    .. [FedPer19] Manoj Ghuhan Arivazhagan, Vinay Aggarwal, Aaditya Kumar Singh, and
+       Sunav Choudhary. Federated learning with personalization layers.
+       In: arXiv (2019). URL:https://arxiv.org/abs/1912.00818
+"""
 from typing import Sequence, Callable
 from copy import deepcopy
 import torch
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedproto.py` & `fluke_fl-0.0.5/fluke/algorithms/fedproto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedProto22]_ algorithm.
+
+References:
+    .. [FedProto22] Yue Tan, Guodong Long, Lu Liu, Tianyi Zhou, Qinghua Lu, Jing Jiang, Chengqi
+       Zhang. FedProto: Federated Prototype Learning across Heterogeneous Clients. In: AAAI (2022).
+       URL: https://arxiv.org/abs/2105.00243
+"""
 import torch
 from torch.nn import Module
 from typing import Sequence, Callable
 from collections import defaultdict
 from copy import deepcopy
 import sys
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedprox.py` & `fluke_fl-0.0.5/fluke/algorithms/fedprox.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedProx18]_ algorithm.
+
+References:
+    .. [FedProx18] Tian Li, Anit Kumar Sahu, Manzil Zaheer, Maziar Sanjabi, Ameet Talwalkar,
+       and Virginia Smith. Federated Optimization in Heterogeneous Networks. Adaptive & Multitask
+       Learning Workshop. URL: https://openreview.net/pdf?id=SkgwE5Ss3N
+"""
 from typing import Callable
 from copy import deepcopy
 import torch
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/fedrep.py` & `fluke_fl-0.0.5/fluke/algorithms/fedrep.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [FedRep21]_ algorithm.
+
+References:
+    .. [FedRep21] Liam Collins, Hamed Hassani, Aryan Mokhtari, and Sanjay Shakkottai.
+       Exploiting shared representations for personalized federated learning. In: ICML (2021).
+       URL: https://arxiv.org/abs/2102.07078
+"""
 import torch
 from typing import Any, Callable, Sequence
 import sys
 sys.path.append(".")
 sys.path.append("..")
 
 from ..algorithms import PersonalizedFL  # NOQA
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/moon.py` & `fluke_fl-0.0.5/fluke/algorithms/moon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Implementation of the [Moon21]_ algorithm.
+
+References:
+    .. [Moon21] Qinbin Li, Bingsheng He, and Dawn Song. Model-Contrastive Federated Learning.
+       In: CVPR (2021). URL: https://arxiv.org/abs/2103.16257
+"""
 from torch.nn import CosineSimilarity
 import torch
 from typing import Callable
 from copy import deepcopy
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/per_fedavg.py` & `fluke_fl-0.0.5/fluke/algorithms/per_fedavg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [Per-FedAVG20]_ algorithm.
+
+References:
+    .. [Per-FedAVG20] Alireza Fallah, Aryan Mokhtari, Asuman Ozdaglar. Personalized Federated
+       Learning with Theoretical Guarantees: A Model-Agnostic Meta-Learning Approach.
+       In: NeurIPS (2020). URL: https://arxiv.org/abs/2002.07948
+"""
 from torch.optim import Optimizer
 import torch
 from typing import Callable, Union
 from collections import OrderedDict
 from copy import deepcopy
 import sys
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/pfedme.py` & `fluke_fl-0.0.5/fluke/algorithms/pfedme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Implementation of the [pFedMe20]_ algorithm.
+
+References:
+    .. [pFedMe20] Canh T. Dinh, Nguyen H. Tran, and Tuan Dung Nguyen. Personalized Federated
+       Learning with Moreau Envelopes. In: NeurIPS (2020). URL: https://arxiv.org/abs/2006.08848
+"""
 from torch.optim import Optimizer
 from torch.nn import Module
 import torch
 from typing import Callable, Sequence
 from collections import OrderedDict
 from copy import deepcopy
 import sys
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/scaffold.py` & `fluke_fl-0.0.5/fluke/algorithms/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Implementation of the [SCAFFOLD20]_ algorithm.
+
+References:
+    .. [SCAFFOLD20] Sai Praneeth Karimireddy, Satyen Kale, Mehryar Mohri, Sashank J. Reddi,
+       Sebastian U. Stich, Ananda Theertha Suresh. SCAFFOLD: Stochastic Controlled Averaging for
+       Federated Learning. In: ICML (2020). URL: https://arxiv.org/abs/1910.06378
+"""
 from torch.optim import Optimizer
 from torch.nn import Module
 import torch
 from typing import Callable, Iterable
 from copy import deepcopy
 import sys
 sys.path.append(".")
```

### Comparing `fluke_fl-0.0.4/fluke/algorithms/superfed.py` & `fluke_fl-0.0.5/fluke/algorithms/superfed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Implementation of the [SuPerFed22]_ algorithm.
+
+References:
+    .. [SuPerFed22] Seok-Ju Hahn, Minwoo Jeong, and Junghye Lee. Connecting Low-Loss Subspace
+       for Personalized Federated Learning. In: KDD (2022). URL: https://arxiv.org/abs/2109.07628v3
+"""
 from torch.nn.modules import Module
 from typing import Any, Callable
 import numpy as np
 from copy import deepcopy
 import sys
 sys.path.append(".")
 sys.path.append("..")
```

### Comparing `fluke_fl-0.0.4/fluke/client.py` & `fluke_fl-0.0.5/fluke/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         return self.train_set.size
 
     @property
     def channel(self) -> Channel:
         """The communication channel.
 
         Attention:
-            Use this channel to communicate with the server.
+            Use this channel to exchange data/information with the server.
 
         Returns:
             Channel: The communication channel.
         """
         return self._channel
 
     @property
```

### Comparing `fluke_fl-0.0.4/fluke/comm.py` & `fluke_fl-0.0.5/fluke/comm.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/fluke/data/__init__.py` & `fluke_fl-0.0.5/fluke/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,16 +312,16 @@
         """Assign the data to the clients and the server according to the configuration.
         Specifically, we can have the following scenarios:
 
         1. ``server_test = True`` and ``keep_test = True``: The server has a test set that
            corresponds to the test set of the dataset. The clients have a training set and,
            if ``client_split > 0``, a test set.
         2. ``server_test = True`` and ``keep_test = False``: The server has a test set that
-           is sampled from the test set of whole dataset (training set and test set are merged). The
-           sampling is done according to the ``server_split`` parameter. The clients have a training
+           is sampled from the whole dataset (training set and test set are merged). The server's
+           sample size is indicated by the ``server_split`` parameter. The clients have a training
            set and, if ``client_split > 0``, a test set.
         3. ``server_test = False`` and ``keep_test = True``: The server does not have a test set.
            The clients have a training set and a test set that corresponds to the test set of the
            dataset distributed uniformly across the clients. In this case the ``client_split`` is
            ignored.
         4. ``server_test = False`` and ``keep_test = False``: The server does not have a test set.
            The clients have a training set and, if ``client_split > 0``, a test set.
```

### Comparing `fluke_fl-0.0.4/fluke/data/datasets.py` & `fluke_fl-0.0.5/fluke/data/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import json
 import os
 import sys
 sys.path.append(".")
 sys.path.append("..")
 
 from . import DataContainer, FastDataLoader, support  # NOQA
+from ..utils import get_class_from_qualified_name  # NOQA
 
 
 def _apply_transforms(dataset: VisionDataset, transforms: Optional[Callable]) -> VisionDataset:
     if transforms is not None:
         new_data = []
         for i in range(len(dataset)):
             new_data.append(transforms(dataset[i][0]))
@@ -39,29 +40,35 @@
     """
 
     @classmethod
     def get(cls, name: str, **kwargs) -> DataContainer | tuple:
         """Get a dataset by name initialized with the provided arguments.
         Supported datasets are: ``mnist``, ``mnistm``, ``svhn``, ``femnist``, ``emnist``,
         ``cifar10``, ``cifar100``, ``tiny_imagenet``, ``shakespeare``, ``fashion_mnist``, and
-        ``cinic10``.
+        ``cinic10``. If `name` is not in the supported datasets, it is assumed to be a fully
+        qualified name of a custom dataset function (``Callable[..., DataContainer]``).
 
         Args:
-            name (str): The name of the dataset to load.
+            name (str): The name of the dataset to load or the fully qualified name of a custom
+              dataset function.
             **kwargs: Additional arguments to pass to construct the dataset.
 
         Returns:
             DataContainer: The ``DataContainer`` object containing the dataset.
 
         Raises:
             ValueError: If the dataset is not supported or the name is wrong.
         """
         if name not in Datasets._DATASET_MAP:
-            raise ValueError(f"Dataset {name} not found. The supported datasets are: " +
-                             ", ".join(Datasets._DATASET_MAP.keys()) + ".")
+            try:
+                data_fun = get_class_from_qualified_name(name)
+                return data_fun(**kwargs)
+            except ModuleNotFoundError | TypeError:
+                raise ValueError(f"Dataset {name} not found. The supported datasets are: " +
+                                 ", ".join(Datasets._DATASET_MAP.keys()) + ".")
 
         return Datasets._DATASET_MAP[name](**kwargs)
 
     @classmethod
     def MNIST(cls,
               path: str = "../data",
               transforms: Optional[Callable] = None,
```

### Comparing `fluke_fl-0.0.4/fluke/data/support.py` & `fluke_fl-0.0.5/fluke/data/support.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/fluke/evaluation.py` & `fluke_fl-0.0.5/fluke/evaluation.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/fluke/nets.py` & `fluke_fl-0.0.5/fluke/nets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/fluke/run.py` & `fluke_fl-0.0.5/fluke/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""`fluke` command line interface."""
 from rich.pretty import Pretty
 from rich.panel import Panel
 from rich.progress import track
 import rich
 from typing import Any
 import typer
 import pandas as pd
@@ -22,15 +23,21 @@
 # CONST
 CONFIG_FNAME = ""
 
 
 @app.command()
 def centralized(alg_cfg: str = typer.Argument(..., help='Config file for the algorithm to run'),
                 epochs: int = typer.Option(0, help='Number of epochs to run')) -> None:
+    """Run a centralized learning experiment.
 
+    Args:
+        alg_cfg (str): Configuration file for the algorithm to run.
+        epochs (int, optional): Number of learning epochs. If set to 0, the number of epochs
+            is computed as `n_rounds * eligible_perc`. Defaults to 0.
+    """
     cfg = Configuration(CONFIG_FNAME, alg_cfg)
     GlobalSettings().set_seed(cfg.exp.seed)
     GlobalSettings().set_device(cfg.exp.device)
     data_container = Datasets.get(**cfg.data.dataset)
 
     device = GlobalSettings().get_device()
 
@@ -41,18 +48,16 @@
     test_loader = FastDataLoader(*data_container.test,
                                  batch_size=10,
                                  num_labels=data_container.num_classes,
                                  shuffle=False)
 
     # , **cfg.method.hyperparameters.net_args)
     model = get_model(mname=cfg.method.hyperparameters.model)
-    sch_args = cfg.method.hyperparameters.client.scheduler
-    cfg.method.hyperparameters.client.optimizer.name = torch.optim.SGD
     optimizer_cfg = OptimizerConfigurator(optimizer_cfg=cfg.method.hyperparameters.client.optimizer,
-                                          scheduler_cfg=sch_args)
+                                          scheduler_cfg=cfg.method.hyperparameters.client.scheduler)
     optimizer, scheduler = optimizer_cfg(model)
     criterion = get_loss(cfg.method.hyperparameters.client.loss)
     evaluator = ClassificationEval(criterion, data_container.num_classes, device)
     history = []
 
     model.to(device)
     epochs = epochs if epochs > 0 else int(
@@ -76,15 +81,19 @@
         rich.print()
     model.to("cpu")
 
 
 @app.command()
 def federation(alg_cfg: str = typer.Argument(...,
                                              help='Config file for the algorithm to run')) -> None:
+    """Run a federated learning experiment.
 
+    Args:
+        alg_cfg (str): Configuration file for the algorithm to run.
+    """
     cfg = Configuration(CONFIG_FNAME, alg_cfg)
     GlobalSettings().set_seed(cfg.exp.seed)
     GlobalSettings().set_device(cfg.exp.device)
     data_container = Datasets.get(**cfg.data.dataset)
     data_splitter = DataSplitter(dataset=data_container,
                                  distribution=cfg.data.distribution.name,
                                  dist_args=cfg.data.distribution.exclude("name"),
@@ -103,15 +112,21 @@
 
 
 @app.command()
 def clients_only(alg_cfg: str = typer.Argument(...,
                                                help='Config file for \
                                                 the algorithm to run'),
                  epochs: int = typer.Option(0, help='Number of epochs to run')) -> None:
+    """Run a local training (for all clients) experiment.
 
+    Args:
+        alg_cfg (str): Configuration file for the algorithm to run.
+        epochs (int, optional): Number of learning epochs. If set to 0, the number of epochs
+            is computed as `max(100, n_rounds * eligible_perc * local_epochs)`. Defaults to 0.
+    """
     cfg = Configuration(CONFIG_FNAME, alg_cfg)
     GlobalSettings().set_seed(cfg.exp.seed)
     GlobalSettings().set_device(cfg.exp.device)
 
     data_container = Datasets.get(**cfg.data.dataset)
     data_splitter = DataSplitter(dataset=data_container,
                                  distribution=cfg.data.distribution.name,
```

### Comparing `fluke_fl-0.0.4/fluke/server.py` & `fluke_fl-0.0.5/fluke/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
           When a new server class inherits from this class, it must add all its hyper-parameters
           to this dictionary.
         device (torch.device): The device where the server runs.
         model (torch.nn.Module): The federated model to be trained.
         clients (Sequence[Client]): The clients that will participate in the federated learning
           process.
-        channel (Channel): The channel to communicate with the clients.
         rounds (int): The number of rounds that have been executed.
         test_data (FastDataLoader): The test data to evaluate the model. If None, the model
           will not be evaluated server-side.
 
     Args:
         model (torch.nn.Module): The federated model to be trained.
         test_data (FastDataLoader): The test data to evaluate the model.
@@ -81,14 +80,18 @@
         for client in self.clients:
             client.set_server(self)
 
     @property
     def channel(self) -> Channel:
         """The channel to communicate with the clients.
 
+        Important:
+            Always use this channel to exchange data/information with the clients.
+            The server should directly call the clients' methods only to trigger specific actions.
+
         Returns:
             Channel: The channel to communicate with the clients.
         """
         return self._channel
 
     @property
     def has_test(self) -> bool:
@@ -262,18 +265,29 @@
             return [1. / len(eligible)] * len(eligible)
 
     @torch.no_grad()
     def aggregate(self, eligible: Sequence[Client]) -> None:
         """Aggregate the models of the clients.
         The aggregation is done by averaging the models of the clients. If the hyperparameter
         ``weighted`` is True, the clients are weighted by their number of samples.
-        The method directly updates the model of the server.
+        The method directly updates the model of the server. Formally, let :math:`\\theta` be the
+        model of the server, :math:`\\theta_i` the model of client :math:`i`, and :math:`w_i` the
+        weight of client :math:`i` such that :math:`\\sum_{i=1}^{N} w_i = 1`. The aggregation is
+        done as follows [FedAVG]_:
+
+        .. math::
+            \\theta = \\sum_{i=1}^{N} w_i \\theta_i
 
         Args:
             eligible (Sequence[Client]): The clients that will participate in the aggregation.
+
+        References:
+            .. [FedAVG] H. B. McMahan, E. Moore, D. Ramage, S. Hampson, and B. A. y Arcas,
+               "Communication-Efficient Learning of Deep Networks from Decentralized Data".
+               In: AISTATS (2017).
         """
         avg_model_sd = OrderedDict()
         clients_sd = self.get_client_models(eligible)
         weights = self._get_client_weights(eligible)
         for key in self.model.state_dict().keys():
             if key.endswith(STATE_DICT_KEYS_TO_IGNORE):
                 avg_model_sd[key] = self.model.state_dict()[key].clone()
```

### Comparing `fluke_fl-0.0.4/fluke/utils/__init__.py` & `fluke_fl-0.0.5/fluke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/fluke/utils/model.py` & `fluke_fl-0.0.5/fluke/utils/model.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/fluke_fl.egg-info/PKG-INFO` & `fluke_fl-0.0.5/fluke_fl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-fl
-Version: 0.0.4
+Version: 0.0.5
 Summary: Federated Learning Utility framework for Experimentation and research.
 Author-email: Mirko Polato <mirko.polato@unito.it>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
```

### Comparing `fluke_fl-0.0.4/fluke_fl.egg-info/SOURCES.txt` & `fluke_fl-0.0.5/fluke_fl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/pyproject.toml` & `fluke_fl-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 where = ["."]  # list of folders that contain the packages (["."] by default)
 include = ["fluke", "fluke.data", "fluke.utils", "fluke.algorithms"]  # package names should match these glob patterns (["*"] by default)
 exclude = []  # exclude packages matching these glob patterns (empty by default)
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [project]
 name = "fluke-fl"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Mirko Polato", email="mirko.polato@unito.it" },
 ]
 description = "Federated Learning Utility framework for Experimentation and research."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `fluke_fl-0.0.4/tests/test_alg.py` & `fluke_fl-0.0.5/tests/test_alg.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_client.py` & `fluke_fl-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_comm.py` & `fluke_fl-0.0.5/tests/test_comm.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_core.py` & `fluke_fl-0.0.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_data.py` & `fluke_fl-0.0.5/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_datasets.py` & `fluke_fl-0.0.5/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_eval.py` & `fluke_fl-0.0.5/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_nets.py` & `fluke_fl-0.0.5/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_server.py` & `fluke_fl-0.0.5/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `fluke_fl-0.0.4/tests/test_utils.py` & `fluke_fl-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

