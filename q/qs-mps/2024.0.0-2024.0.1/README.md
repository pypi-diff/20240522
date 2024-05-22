# Comparing `tmp/qs-mps-2024.0.0.tar.gz` & `tmp/qs-mps-2024.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qs-mps-2024.0.0.tar", last modified: Fri Mar 15 11:17:35 2024, max compression
+gzip compressed data, was "qs-mps-2024.0.1.tar", last modified: Wed May 22 09:01:19 2024, max compression
```

## Comparing `qs-mps-2024.0.0.tar` & `qs-mps-2024.0.1.tar`

### file list

```diff
@@ -1,59 +1,67 @@
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.124861 qs-mps-2024.0.0/
--rw-r--r--   0 fradm98    (504) staff       (20)    11357 2023-09-04 14:16:50.000000 qs-mps-2024.0.0/LICENSE
--rw-r--r--   0 fradm98    (504) staff       (20)    14164 2024-03-15 11:17:35.124364 qs-mps-2024.0.0/PKG-INFO
--rw-r--r--   0 fradm98    (504) staff       (20)      386 2023-11-27 10:16:47.000000 qs-mps-2024.0.0/README.md
--rw-r--r--   0 fradm98    (504) staff       (20)     1141 2024-03-15 11:14:29.000000 qs-mps-2024.0.0/pyproject.toml
--rw-r--r--   0 fradm98    (504) staff       (20)       38 2024-03-15 11:17:35.125023 qs-mps-2024.0.0/setup.cfg
--rw-r--r--   0 fradm98    (504) staff       (20)       38 2023-11-27 10:16:47.000000 qs-mps-2024.0.0/setup.py
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.102930 qs-mps-2024.0.0/src/
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.108666 qs-mps-2024.0.0/src/qs_mps/
--rw-r--r--   0 fradm98    (504) staff       (20)     3014 2023-12-12 17:45:24.000000 qs-mps-2024.0.0/src/qs_mps/Ising_gs_and_time_ev.py
--rw-r--r--   0 fradm98    (504) staff       (20)      787 2024-03-11 09:33:26.000000 qs-mps-2024.0.0/src/qs_mps/TensorMultiplier.py
--rw-r--r--   0 fradm98    (504) staff       (20)        0 2023-11-27 10:16:47.000000 qs-mps-2024.0.0/src/qs_mps/__init__.py
--rw-r--r--   0 fradm98    (504) staff       (20)     1148 2023-11-27 10:16:47.000000 qs-mps-2024.0.0/src/qs_mps/analytical_formulas_TFIC.py
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.110833 qs-mps-2024.0.0/src/qs_mps/applications/
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.111904 qs-mps-2024.0.0/src/qs_mps/applications/ANNNI/
--rw-r--r--   0 fradm98    (504) staff       (20)     9449 2024-03-14 11:40:36.000000 qs-mps-2024.0.0/src/qs_mps/applications/ANNNI/get_gs_DMRG.py
--rw-r--r--   0 fradm98    (504) staff       (20)     4541 2024-02-07 16:07:45.000000 qs-mps-2024.0.0/src/qs_mps/applications/ANNNI/get_observables_MPS.py
--rw-r--r--   0 fradm98    (504) staff       (20)     3004 2024-02-08 17:47:33.000000 qs-mps-2024.0.0/src/qs_mps/applications/ANNNI/ground_state_multiprocessing.py
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.112338 qs-mps-2024.0.0/src/qs_mps/applications/CLUSTER/
--rw-r--r--   0 fradm98    (504) staff       (20)     4691 2024-03-12 17:53:07.000000 qs-mps-2024.0.0/src/qs_mps/applications/CLUSTER/get_observables_MPS.py
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.116138 qs-mps-2024.0.0/src/qs_mps/applications/ISING/
--rw-r--r--   0 fradm98    (504) staff       (20)        0 2024-01-19 14:00:23.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/TEBD_different_chi.py
--rw-r--r--   0 fradm98    (504) staff       (20)     6645 2023-11-27 10:16:57.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/TEBD_different_delta.py
--rw-r--r--   0 fradm98    (504) staff       (20)        0 2023-11-27 10:16:57.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/__init__.py
--rw-r--r--   0 fradm98    (504) staff       (20)     8666 2023-12-12 17:45:24.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/assess_time.py
--rw-r--r--   0 fradm98    (504) staff       (20)     7665 2024-02-12 15:24:30.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/get_gs_DMRG.py
--rw-r--r--   0 fradm98    (504) staff       (20)     3014 2023-12-12 17:45:24.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/get_gs_and_time_ev_EXACT.py
--rw-r--r--   0 fradm98    (504) staff       (20)     3764 2024-02-12 15:40:43.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/get_observables_MPS.py
--rw-r--r--   0 fradm98    (504) staff       (20)     9514 2024-02-02 22:25:10.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/plot_DMRG.py
--rw-r--r--   0 fradm98    (504) staff       (20)     9660 2023-12-12 17:45:24.000000 qs-mps-2024.0.0/src/qs_mps/applications/ISING/plot_TEBD.py
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.123603 qs-mps-2024.0.0/src/qs_mps/applications/Z2/
--rw-r--r--   0 fradm98    (504) staff       (20)        0 2023-11-27 10:16:57.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/__init__.py
--rw-r--r--   0 fradm98    (504) staff       (20)     8812 2024-01-18 18:46:29.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/exact_hamiltonian.py
--rw-r--r--   0 fradm98    (504) staff       (20)     7971 2024-03-11 16:40:29.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/get_gs_DMRG.py
--rw-r--r--   0 fradm98    (504) staff       (20)     5976 2024-01-10 11:17:46.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/get_gs_EXACT.py
--rw-r--r--   0 fradm98    (504) staff       (20)     5034 2024-01-18 16:41:55.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/get_observables_EXACT.py
--rw-r--r--   0 fradm98    (504) staff       (20)     7786 2024-03-07 09:54:44.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/get_observables_MPS.py
--rw-r--r--   0 fradm98    (504) staff       (20)     4919 2024-02-16 04:03:41.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/ground_state_multiprocessing.py
--rw-r--r--   0 fradm98    (504) staff       (20)     9766 2024-01-19 14:00:23.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/multi_run_gs.py
--rw-r--r--   0 fradm98    (504) staff       (20)     7749 2024-01-19 14:00:23.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/multi_run_obs.py
--rw-r--r--   0 fradm98    (504) staff       (20)    13543 2024-03-07 13:52:56.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/plot_DMRG.py
--rw-r--r--   0 fradm98    (504) staff       (20)     5814 2024-03-07 09:42:55.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/plot_animations.py
--rw-r--r--   0 fradm98    (504) staff       (20)    13618 2023-12-12 17:45:24.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/test_sparse_mpo.py
--rw-r--r--   0 fradm98    (504) staff       (20)    14817 2024-03-11 16:47:03.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/time_ev_debug.py
--rw-r--r--   0 fradm98    (504) staff       (20)     3754 2023-12-18 09:05:19.000000 qs-mps-2024.0.0/src/qs_mps/applications/Z2/vacuum_sector.py
--rw-r--r--   0 fradm98    (504) staff       (20)        0 2023-11-27 10:16:57.000000 qs-mps-2024.0.0/src/qs_mps/applications/__init__.py
--rw-r--r--   0 fradm98    (504) staff       (20)     3310 2023-11-27 10:16:47.000000 qs-mps-2024.0.0/src/qs_mps/checks.py
--rw-r--r--   0 fradm98    (504) staff       (20)     2161 2024-02-12 09:54:41.000000 qs-mps-2024.0.0/src/qs_mps/gs_multiprocessing.py
--rw-r--r--   0 fradm98    (504) staff       (20)    15432 2023-12-21 10:53:35.000000 qs-mps-2024.0.0/src/qs_mps/lattice.py
--rw-r--r--   0 fradm98    (504) staff       (20)    20934 2024-03-11 17:51:02.000000 qs-mps-2024.0.0/src/qs_mps/mpo_class.py
--rw-r--r--   0 fradm98    (504) staff       (20)   103698 2024-03-15 11:10:43.000000 qs-mps-2024.0.0/src/qs_mps/mps_class.py
--rw-r--r--   0 fradm98    (504) staff       (20)    10431 2023-12-15 12:34:05.000000 qs-mps-2024.0.0/src/qs_mps/sparse_hamiltonians_and_operators.py
--rw-r--r--   0 fradm98    (504) staff       (20)    38581 2024-03-07 10:12:05.000000 qs-mps-2024.0.0/src/qs_mps/utils.py
-drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-03-15 11:17:35.110512 qs-mps-2024.0.0/src/qs_mps.egg-info/
--rw-r--r--   0 fradm98    (504) staff       (20)    14164 2024-03-15 11:17:35.000000 qs-mps-2024.0.0/src/qs_mps.egg-info/PKG-INFO
--rw-r--r--   0 fradm98    (504) staff       (20)     1856 2024-03-15 11:17:35.000000 qs-mps-2024.0.0/src/qs_mps.egg-info/SOURCES.txt
--rw-r--r--   0 fradm98    (504) staff       (20)        1 2024-03-15 11:17:35.000000 qs-mps-2024.0.0/src/qs_mps.egg-info/dependency_links.txt
--rw-r--r--   0 fradm98    (504) staff       (20)       78 2024-03-15 11:17:35.000000 qs-mps-2024.0.0/src/qs_mps.egg-info/requires.txt
--rw-r--r--   0 fradm98    (504) staff       (20)        7 2024-03-15 11:17:35.000000 qs-mps-2024.0.0/src/qs_mps.egg-info/top_level.txt
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.643178 qs-mps-2024.0.1/
+-rw-r--r--   0 fradm98    (504) staff       (20)    11357 2023-09-04 14:16:50.000000 qs-mps-2024.0.1/LICENSE
+-rw-r--r--   0 fradm98    (504) staff       (20)    14164 2024-05-22 09:01:19.642688 qs-mps-2024.0.1/PKG-INFO
+-rw-r--r--   0 fradm98    (504) staff       (20)      386 2023-11-27 10:16:47.000000 qs-mps-2024.0.1/README.md
+-rw-r--r--   0 fradm98    (504) staff       (20)     1141 2024-05-22 09:00:33.000000 qs-mps-2024.0.1/pyproject.toml
+-rw-r--r--   0 fradm98    (504) staff       (20)       38 2024-05-22 09:01:19.643375 qs-mps-2024.0.1/setup.cfg
+-rw-r--r--   0 fradm98    (504) staff       (20)       38 2023-11-27 10:16:47.000000 qs-mps-2024.0.1/setup.py
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.616187 qs-mps-2024.0.1/src/
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.623268 qs-mps-2024.0.1/src/qs_mps/
+-rw-r--r--   0 fradm98    (504) staff       (20)     3014 2023-12-12 17:45:24.000000 qs-mps-2024.0.1/src/qs_mps/Ising_gs_and_time_ev.py
+-rw-r--r--   0 fradm98    (504) staff       (20)      787 2024-03-11 09:33:26.000000 qs-mps-2024.0.1/src/qs_mps/TensorMultiplier.py
+-rw-r--r--   0 fradm98    (504) staff       (20)        0 2023-11-27 10:16:47.000000 qs-mps-2024.0.1/src/qs_mps/__init__.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     1148 2023-11-27 10:16:47.000000 qs-mps-2024.0.1/src/qs_mps/analytical_formulas_TFIC.py
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.625403 qs-mps-2024.0.1/src/qs_mps/applications/
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.626926 qs-mps-2024.0.1/src/qs_mps/applications/ANNNI/
+-rw-r--r--   0 fradm98    (504) staff       (20)     8788 2024-04-17 15:14:04.000000 qs-mps-2024.0.1/src/qs_mps/applications/ANNNI/get_gs_DMRG.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     4541 2024-02-07 16:07:45.000000 qs-mps-2024.0.1/src/qs_mps/applications/ANNNI/get_observables_MPS.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     3004 2024-02-08 17:47:33.000000 qs-mps-2024.0.1/src/qs_mps/applications/ANNNI/ground_state_multiprocessing.py
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.628325 qs-mps-2024.0.1/src/qs_mps/applications/CLUSTER/
+-rw-r--r--   0 fradm98    (504) staff       (20)     7890 2024-04-16 15:04:15.000000 qs-mps-2024.0.1/src/qs_mps/applications/CLUSTER/get_gs_DMRG-xy.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     8303 2024-05-13 07:21:19.000000 qs-mps-2024.0.1/src/qs_mps/applications/CLUSTER/get_gs_DMRG.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     4691 2024-03-12 17:53:07.000000 qs-mps-2024.0.1/src/qs_mps/applications/CLUSTER/get_observables_MPS.py
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.632598 qs-mps-2024.0.1/src/qs_mps/applications/ISING/
+-rw-r--r--   0 fradm98    (504) staff       (20)        0 2024-01-19 14:00:23.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/TEBD_different_chi.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     6645 2023-11-27 10:16:57.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/TEBD_different_delta.py
+-rw-r--r--   0 fradm98    (504) staff       (20)        0 2023-11-27 10:16:57.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/__init__.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     8666 2023-12-12 17:45:24.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/assess_time.py
+-rw-r--r--   0 fradm98    (504) staff       (20)    10290 2024-04-18 14:46:03.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/get_gs_DMRG.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     3014 2023-12-12 17:45:24.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/get_gs_and_time_ev_EXACT.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     3764 2024-02-12 15:40:43.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/get_observables_MPS.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     9514 2024-02-02 22:25:10.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/plot_DMRG.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     9660 2023-12-12 17:45:24.000000 qs-mps-2024.0.1/src/qs_mps/applications/ISING/plot_TEBD.py
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.633057 qs-mps-2024.0.1/src/qs_mps/applications/XXZ/
+-rw-r--r--   0 fradm98    (504) staff       (20)     7924 2024-04-18 10:35:31.000000 qs-mps-2024.0.1/src/qs_mps/applications/XXZ/get_gs_DMRG.py
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.641437 qs-mps-2024.0.1/src/qs_mps/applications/Z2/
+-rw-r--r--   0 fradm98    (504) staff       (20)        0 2023-11-27 10:16:57.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/__init__.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     8812 2024-01-18 18:46:29.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/exact_hamiltonian.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     8765 2024-04-26 14:18:55.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/get_gs_DMRG.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     5982 2024-04-19 09:49:53.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/get_gs_EXACT.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     5034 2024-01-18 16:41:55.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/get_observables_EXACT.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     8637 2024-04-26 14:42:11.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/get_observables_MPS.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     6434 2024-04-24 11:32:08.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/ground_state_multiprocessing.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     9766 2024-01-19 14:00:23.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/multi_run_gs.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     7749 2024-01-19 14:00:23.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/multi_run_obs.py
+-rw-r--r--   0 fradm98    (504) staff       (20)    13543 2024-03-07 13:52:56.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/plot_DMRG.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     5814 2024-03-07 09:42:55.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/plot_animations.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     2703 2024-03-25 17:38:52.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/string_energy_density_debug.py
+-rw-r--r--   0 fradm98    (504) staff       (20)    13618 2023-12-12 17:45:24.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/test_sparse_mpo.py
+-rw-r--r--   0 fradm98    (504) staff       (20)    15759 2024-03-22 14:04:36.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/time_ev_debug.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     3978 2024-04-15 15:11:04.000000 qs-mps-2024.0.1/src/qs_mps/applications/Z2/vacuum_sector.py
+-rw-r--r--   0 fradm98    (504) staff       (20)        0 2023-11-27 10:16:57.000000 qs-mps-2024.0.1/src/qs_mps/applications/__init__.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     3310 2023-11-27 10:16:47.000000 qs-mps-2024.0.1/src/qs_mps/checks.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     5209 2024-04-18 10:35:31.000000 qs-mps-2024.0.1/src/qs_mps/get_rdms.py
+-rw-r--r--   0 fradm98    (504) staff       (20)     2161 2024-02-12 09:54:41.000000 qs-mps-2024.0.1/src/qs_mps/gs_multiprocessing.py
+-rw-r--r--   0 fradm98    (504) staff       (20)    15432 2023-12-21 10:53:35.000000 qs-mps-2024.0.1/src/qs_mps/lattice.py
+-rw-r--r--   0 fradm98    (504) staff       (20)    21007 2024-04-25 13:33:14.000000 qs-mps-2024.0.1/src/qs_mps/mpo_class.py
+-rw-r--r--   0 fradm98    (504) staff       (20)   115029 2024-05-13 07:24:17.000000 qs-mps-2024.0.1/src/qs_mps/mps_class.py
+-rw-r--r--   0 fradm98    (504) staff       (20)    20428 2024-04-16 08:06:48.000000 qs-mps-2024.0.1/src/qs_mps/sparse_hamiltonians_and_operators.py
+-rw-r--r--   0 fradm98    (504) staff       (20)    39334 2024-05-13 07:25:37.000000 qs-mps-2024.0.1/src/qs_mps/utils.py
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.625062 qs-mps-2024.0.1/src/qs_mps.egg-info/
+-rw-r--r--   0 fradm98    (504) staff       (20)    14164 2024-05-22 09:01:19.000000 qs-mps-2024.0.1/src/qs_mps.egg-info/PKG-INFO
+-rw-r--r--   0 fradm98    (504) staff       (20)     2096 2024-05-22 09:01:19.000000 qs-mps-2024.0.1/src/qs_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 fradm98    (504) staff       (20)        1 2024-05-22 09:01:19.000000 qs-mps-2024.0.1/src/qs_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 fradm98    (504) staff       (20)       78 2024-05-22 09:01:19.000000 qs-mps-2024.0.1/src/qs_mps.egg-info/requires.txt
+-rw-r--r--   0 fradm98    (504) staff       (20)        7 2024-05-22 09:01:19.000000 qs-mps-2024.0.1/src/qs_mps.egg-info/top_level.txt
+drwxr-xr-x   0 fradm98    (504) staff       (20)        0 2024-05-22 09:01:19.641962 qs-mps-2024.0.1/tests/
+-rw-r--r--   0 fradm98    (504) staff       (20)      480 2024-04-10 13:19:11.000000 qs-mps-2024.0.1/tests/test_rdms.py
```

### Comparing `qs-mps-2024.0.0/LICENSE` & `qs-mps-2024.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/PKG-INFO` & `qs-mps-2024.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qs-mps
-Version: 2024.0.0
+Version: 2024.0.1
 Summary: Quantum Simulation with Matrix Product State, a Tensor network method for the study of Quantum Systems
 Author-email: Francesco Di Marcantonio <francesco.di.marcantonio@cern.ch>
 Maintainer-email: Francesco Di Marcantonio <francesco.di.marcantonio@cern.ch>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `qs-mps-2024.0.0/pyproject.toml` & `qs-mps-2024.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qs-mps"
-version = "2024.0.0"
+version = "2024.0.1"
 description = "Quantum Simulation with Matrix Product State, a Tensor network method for the study of Quantum Systems"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
     {name="Francesco Di Marcantonio", email="francesco.di.marcantonio@cern.ch"},
 ]
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/Ising_gs_and_time_ev.py` & `qs-mps-2024.0.1/src/qs_mps/Ising_gs_and_time_ev.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/TensorMultiplier.py` & `qs-mps-2024.0.1/src/qs_mps/TensorMultiplier.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/analytical_formulas_TFIC.py` & `qs-mps-2024.0.1/src/qs_mps/analytical_formulas_TFIC.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ANNNI/get_gs_DMRG.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ISING/get_gs_DMRG.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import argparse
 import numpy as np
 from qs_mps.mps_class import MPS
-from qs_mps.utils import get_precision, save_list_of_lists, access_txt, tensor_shapes
-from qs_mps.applications.ANNNI.ground_state_multiprocessing import ground_state_ANNNI
-from scipy.sparse.linalg._eigen.arpack.arpack import ArpackNoConvergence
+from qs_mps.utils import get_precision, save_list_of_lists, access_txt, swap_rows
+from qs_mps.gs_multiprocessing import ground_state_ising
 
-# DENSITY MATRIX RENORMALIZATION GROUP to find ground states of the Z2 Pure Gauge Theory 
-# changing the transverse field parameters in its dual formulation
+import signal
+import time
 
-parser = argparse.ArgumentParser(prog="gs_search_ANNNI")
+# Define a function to handle the timeout
+def timeout_handler(signum, frame):
+    raise TimeoutError("Algorithm took too long to execute")
+
+# Set the signal handler
+signal.signal(signal.SIGALRM, timeout_handler)
+
+# DENSITY MATRIX RENORMALIZATION GROUP to find ground states of the 
+# 1D Ising Transverse Field model changing the transverse field parameters
+
+parser = argparse.ArgumentParser(prog="gs_search_Ising")
 parser.add_argument(
     "npoints",
     help="Number of points in an interval of transverse field values",
     type=int,
 )
 parser.add_argument(
-    "h_i", help="Starting value of h external transverse field", type=float
-)
-parser.add_argument(
-    "h_f", help="Final value of h external transverse field", type=float
-)
-parser.add_argument(
-    "k_i", help="Starting value of J2 next nearest interaction coefficient", type=float
+    "h_i", help="Starting value of h (external transverse field)", type=float
 )
 parser.add_argument(
-    "k_f", help="Final value of J2 next nearest interaction coefficient", type=float
+    "h_f", help="Final value of h (external transverse field)", type=float
 )
 parser.add_argument(
     "path",
     help="Path to the drive depending on the device used. Available are 'pc', 'mac', 'marcos'",
     type=str,
 )
 parser.add_argument("-L", "--Ls", help="Spin chain lengths", nargs="*", type=int)
 parser.add_argument("-D", "--chis", help="Simulated bond dimensions", nargs="+", type=int)
 parser.add_argument("-d","--dimension", help="Physical dimension. By default 2", default=2, type=int)
 parser.add_argument(
-    "-ty", "--type_shape", help="Type of shape of the bond dimension. Available are: 'trapezoidal', 'pyramidal', 'rectangular'", default="rectangular", type=str
-)
-parser.add_argument(
-    "-m", "--model", help="Model to simulate", default="ANNNI", type=str
+    "-ty", "--type_shape", help="Type of shape of the bond dimension. Available are: 'trapezoidal', 'pyramidal', 'rectangular'", default="trapezoidal", type=str
 )
 parser.add_argument(
-    "-mu", "--multpr", help="If True computes ground states with multiprocessing. By default False", action="store_true"
+    "-m", "--model", help="Model to simulate", default="Ising", type=str
 )
 parser.add_argument(
     "-s",
     "--number_sweeps",
     help="Number of sweeps during the compression algorithm for each trotter step",
     default=8,
     type=int,
@@ -54,183 +54,208 @@
     "-cv",
     "--conv_tol",
     help="Convergence tolerance of the compression algorithm",
     default=1e-10,
     type=float,
 )
 parser.add_argument(
+    "-fid",
+    "--fidelity",
+    help="Fidelity with exact solution. Doable only for small Ising chains",
+    action="store_true",
+)
+parser.add_argument(
     "-b",
     "--bond",
     help="Save the schmidt values for one bond. If False save for each bond. By default True",
     action="store_false",
 )
 parser.add_argument(
     "-w",
     "--where",
     help="Bond where we want to observe the Schmidt values, should be between 1 and (L-1)",
     default=-1,
     type=int,
 )
 parser.add_argument(
-    "-v",
-    "--save",
-    help="Save the tensors. By default True",
-    action="store_false",
-)
-parser.add_argument(
     "-tr",
     "--training",
-    help="Save all the energies also the ones during the variational optimization. By default False",
-    action="store_true",
+    help="Save all the energies during the variational optimization. By default True",
+    action="store_false",
 )
 
 args = parser.parse_args()
 
 # define the interval of equally spaced values of external field
-interval_h = np.linspace(args.h_i, args.h_f, args.npoints)
-interval_k = np.linspace(args.k_i, args.k_f, args.npoints)
+interval_hx = np.linspace(args.h_i, args.h_f, args.npoints).tolist()
+interval_hy = np.linspace(args.h_i, args.h_f, args.npoints)
+interval_hx.reverse()
 
 # take the path and precision to save files
 # if we want to save the tensors we save them locally because they occupy a lot of memory
 if args.path == "pc":
-    parent_path = "G:/My Drive/projects/2_ANNNI"
-    path_tensor = "D:/code/projects/2_ANNNI"
+    parent_path = "G:/My Drive/projects/0_ISING"
+    path_tensor = "D:/code/projects/0_ISING"
 elif args.path == "mac":
-    parent_path = "/Users/fradm98/Google Drive/My Drive/projects/2_ANNNI"
-    path_tensor = "/Users/fradm98/Desktop/projects/2_ANNNI"
+    parent_path = "/Users/fradm98/Google Drive/My Drive/projects/0_ISING"
+    path_tensor = "/Users/fradm98/Desktop/projects/0_ISING"
 elif args.path == "marcos":
-    parent_path = "/Users/fradm/Google Drive/My Drive/projects/2_ANNNI"
-    path_tensor = "/Users/fradm/Desktop/projects/2_ANNNI"
+    parent_path = "/Users/fradm/Google Drive/My Drive/projects/0_ISING"
+    path_tensor = "/Users/fradm/Desktop/projects/0_ISING"
 else:
     raise SyntaxError("Path not valid. Choose among 'pc', 'mac', 'marcos'")
 
+path = f"{parent_path}/results/tensors"
 num = (args.h_f - args.h_i) / args.npoints
 precision = get_precision(num)
 
-Z = np.array([[1, 0], [0, -1]])
+
 # ---------------------------------------------------------
 # DMRG
 # ---------------------------------------------------------
 for L in args.Ls:
     if args.where == -1:
         args.where = L // 2
     elif args.where == -2:
         args.bond = False
     for chi in args.chis:  # L // 2 + 1
-        args_mps = {
-            "L": L,
-            "d": args.dimension,
-            "chi": chi,
-            "type_shape": args.type_shape,
-            "model": args.model,
-            "trunc_tol": False,
-            "trunc_chi": True,
-            "where": args.where,
-            "bond": args.bond,
-            "path": path_tensor,
-            "save": args.save,
-            "precision": precision,
-            "eps": 0,
-        }
-        if __name__ == "__main__":
-            energy_chi = []
-            entropy_chi = []
-            schmidt_vals_chi = []
-            for h in interval_h:
-                # init_tensor = MPS(
-                #         L=args_mps["L"],
-                #         d=args_mps["d"],
-                #         model="Ising",
-                #         chi=args_mps["chi"],
-                #         h=h,
-                #         J=1,
-                #         eps=args_mps["eps"],
-                #         )
-                # init_tensor.load_sites(path=path_tensor.rsplit("/", 1)[:-1][0]+"0_ISING", precision=args_mps["precision"])
-                # init = init_tensor.sites.copy()
-                for k in interval_k:
-                    precision = args_mps["precision"]
-                    chain = MPS(
-                        L=args_mps["L"],
-                        d=args_mps["d"],
-                        model=args_mps["model"],
-                        chi=args_mps["chi"],
-                        h=h,
-                        k=k,
-                        J=1,
-                        eps=args_mps["eps"],
-                    )
-                    chain._random_state(seed=3,type_shape="rectangular", chi=chi)
-                    # chain._random_state(seed=7, chi=args_mps["chi"], type_shape=args_mps["type_shape"])
+        # init_state = np.zeros((1, 2, 1))
+        # init_state[0, 0, 0] = 1
+        # init_tensor = [init_state for _ in range(L)]
+        energy_chi = []
+        entropy_chi = []
+        schmidt_vals_chi = []
+        time_chi = []
+        exceptions_chi = np.zeros((len(interval_hy),len(interval_hx)))
+        for idx0, J in enumerate(interval_hy):
+            energy_J = []
+            entropy_J = []
+            schmidt_vals_J = []
+            t_slice = []
+            new_timeout_secs = 5
+            for idx1, h in enumerate(interval_hx):
+                chain = MPS(
+                    L=L,
+                    d=2,
+                    model="Ising",
+                    chi=chi,
+                    h=h,
+                    J=J,
+                    eps=1e-5,
+                )                
+                if h == interval_hx[0]:
+                    # init_tensor = [init_state for _ in range(L)]
+                    # chain.sites = init_tensor.copy()
+                    # chain.enlarge_chi(type_shape="rectangular", prnt=False)
+                    chain._random_state(3, chi=chi)
                     chain.canonical_form(trunc_chi=False, trunc_tol=True)
-                    # # total
-                    # chain.order_param(op=Z)
-                    # mag = np.real(chain.mpo_first_moment())
-                    # if mag < 0:
-                    #     chain.flipping_all()
-
-                    try:
-                        energy, entropy, schmidt_vals = chain.DMRG(
-                            trunc_tol=args_mps["trunc_tol"],
-                            trunc_chi=args_mps["trunc_chi"],
-                            where=args_mps["where"],
-                            bond=args_mps["bond"],
-                        )
-
-                        print(f"energy of h:{h:.{precision}f}, k:{k:.{precision}f} is:\n {energy}")
-                        print(f"Schmidt values in the middle of the chain:\n {schmidt_vals}")
-
-                        chain.save_sites(path=args_mps["path"], precision=args_mps["precision"])
-                        
-                    except ArpackNoConvergence:
-                        energy = np.nan
-                        entropy = np.nan
-                        schmidt_vals = np.nan
-                        
-                    energy_chi.append(energy)
-                    entropy_chi.append(entropy)
-                    schmidt_vals_chi.append(schmidt_vals)
-        # energy_chi, entropy_chi, schmidt_vals_chi = ground_state_ANNNI(
-        #     args_mps=args_mps, multpr=args.multpr, param=[interval_h,interval_k]
+                else:
+                    chain.sites = init_tensor.copy()
+
+                # Set the timeout period (in seconds)
+                timeout_secs = new_timeout_secs # You can change this value according to your requirement
+
+                # Set the alarm
+                signal.alarm(int(timeout_secs+1))
+                print(f"New timeout seconds: {int(timeout_secs+1)}")
+                try:
+                    # Call your algorithm function with the initial parameter
+                    print("Running with guess state:")
+                    energy, entropy, schmidt_vals, t_dmrg = chain.DMRG(
+                        trunc_tol=False,
+                        trunc_chi=True,
+                        where=args.where,
+                        bond=args.bond,
+                    )
+                except TimeoutError as e:
+                    print(e)
+                    # Modify the parameter and call the algorithm again
+                    chain._random_state(seed=7, type_shape="rectangular", chi=chi)
+                    chain.canonical_form()
+                    print("Running with random state:")
+                    energy, entropy, schmidt_vals, t_dmrg = chain.DMRG(
+                        trunc_tol=False,
+                        trunc_chi=True,
+                        where=args.where,
+                        bond=args.bond,
+                    )
+                    exceptions_chi[idx0,idx1] = 1
+                else:
+                    # Cancel the alarm if the algorithm finishes before the timeout
+                    signal.alarm(0)
+
+                t_slice.append(t_dmrg)
+                t_mean = np.mean(t_slice)
+                t_std = np.std(t_slice)
+                new_timeout_secs = t_mean + 3*t_std
+                
+                print(f"energy of h:{h:.{precision}f}, J:{J:.{precision}f} is:\n {energy}")
+                print(f"Schmidt values in the middle of the chain:\n {schmidt_vals}")
+
+                chain.save_sites(path=path_tensor, precision=precision)
+                if args.training:
+                    energy_J.append(energy)
+                else:
+                    energy_J.append(energy[-1])
+                entropy_J.append(entropy)
+                schmidt_vals_J.append(schmidt_vals)
+
+                if h == interval_hx[0]:
+                    init_tensor_J = chain.sites.copy()
+                init_tensor = chain.sites.copy()
+            
+            init_tensor = init_tensor_J.copy()
+
+            time_chi.append(t_slice)
+            energy_chi.append(energy_J)
+            entropy_chi.append(entropy_J)
+            schmidt_vals_chi.append(schmidt_vals_J)
+        # energy_chi, entropy_chi, schmidt_vals_chi = ground_state_ising(
+        #     args_mps=args_mps, multpr=False, param=interval
         # )
 
         if args.bond == False:
             args.where = "all"
 
+        np.save(f"{parent_path}/results/energy_data/", exceptions_chi)
+
         if args.training:
-            save_list_of_lists(
-                f"{parent_path}/results/energy_data/energies_{args.model}_spin_{L}_h_{args.h_i}-{args.h_f}_k_{args.k_i}-{args.k_f}_delta_{args.npoints}_chi_{chi}",
+            energy_chi = np.swapaxes(swap_rows(np.asarray(energy_chi)), axis1=0, axis2=1)
+            np.save(
+                f"{parent_path}/results/energy_data/energies_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_J_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
                 energy_chi,
             )
-            energy_gs = access_txt(
-                    f"{parent_path}/results/energy_data/energies_{args.model}_spin_{L}_h_{args.h_i}-{args.h_f}_k_{args.k_i}-{args.k_f}_delta_{args.npoints}_chi_{chi}",
-                    -1,
-                )
-            np.savetxt(
-                f"{parent_path}/results/energy_data/energies_{args.model}_spin_{L}_h_{args.h_i}-{args.h_f}_k_{args.k_i}-{args.k_f}_delta_{args.npoints}_chi_{chi}",
-                energy_gs,
-            )
+            energy_min = []
+            for i in range(len(interval_hx)):
+                energy_min_i = []
+                for j in range(len(interval_hy)):
+                    energy_min_i.append(energy_chi[i][j][-1])
+                energy_min.append(energy_min_i)
+            np.save(f"{parent_path}/results/energy_data/energy_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_J_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}", energy_min)
         else:
-            np.savetxt(
-                f"{parent_path}/results/energy_data/energies_{args.model}_spin_{L}_h_{args.h_i}-{args.h_f}_k_{args.k_i}-{args.k_f}_delta_{args.npoints}_chi_{chi}",
+            energy_chi = np.array(energy_chi)
+            energy_chi = np.array_split(energy_chi, args.npoints)
+            save_list_of_lists(
+                f"{parent_path}/results/energy_data/energies_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
                 energy_chi,
             )
-             
+        entropy_chi = np.array(entropy_chi)
+        entropy_chi = np.array_split(entropy_chi, args.npoints)
         save_list_of_lists(
-            f"{parent_path}/results/entropy_data/{args.where}_bond_entropy_{args.model}_spin_{L}_h_{args.h_i}-{args.h_f}_k_{args.k_i}-{args.k_f}_delta_{args.npoints}_chi_{chi}",
+            f"{parent_path}/results/entropy/{args.where}_bond_entropy_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
             entropy_chi,
         )
-
+        schmidt_vals_chi = np.array(schmidt_vals_chi)
+        schmidt_vals_chi = np.array_split(schmidt_vals_chi, args.npoints)
         save_list_of_lists(
-            f"{parent_path}/results/entropy_data/{args.where}_schmidt_vals_{args.model}_spin_{L}_h_{args.h_i}-{args.h_f}_k_{args.k_i}-{args.k_f}_delta_{args.npoints}_chi_{chi}",
+            f"{parent_path}/results/entropy/{args.where}_schmidt_values_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
             schmidt_vals_chi,
         )
-
         if args.where == "all":
             entropy_mid = access_txt(
-                f"{parent_path}/results/entropy_data/{args.where}_bond_entropy_{args.model}_spin_{L}_h_{args.h_i}-{args.h_f}_k_{args.k_i}-{args.k_f}_delta_{args.npoints}_chi_{chi}",
-                (L-1) // 2,
+                f"{parent_path}/results/entropy/{args.where}_bond_entropy_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
+                L // 2,
             )
             np.savetxt(
-                f"{parent_path}/results/entropy_data/{L // 2}_bond_entropy_{args.model}_spin_{L}_h_{args.h_i}-{args.h_f}_k_{args.k_i}-{args.k_f}_delta_{args.npoints}_chi_{chi}",
+                f"{parent_path}/results/entropy/{L // 2}_bond_entropy_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
                 entropy_mid,
-            )
+            )
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ANNNI/get_observables_MPS.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ANNNI/get_observables_MPS.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ANNNI/ground_state_multiprocessing.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ANNNI/ground_state_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/CLUSTER/get_observables_MPS.py` & `qs-mps-2024.0.1/src/qs_mps/applications/CLUSTER/get_observables_MPS.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ISING/TEBD_different_delta.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ISING/TEBD_different_delta.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ISING/assess_time.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ISING/assess_time.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ISING/get_gs_DMRG.py` & `qs-mps-2024.0.1/src/qs_mps/applications/XXZ/get_gs_DMRG.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,198 +1,210 @@
 import argparse
 import numpy as np
 from qs_mps.mps_class import MPS
-from qs_mps.utils import get_precision, save_list_of_lists, access_txt
-from qs_mps.gs_multiprocessing import ground_state_ising
+from qs_mps.utils import get_precision, save_list_of_lists, access_txt, swap_rows
 
-# DENSITY MATRIX RENORMALIZATION GROUP to find ground states of the 
-# 1D Ising Transverse Field model changing the transverse field parameters
+# DENSITY MATRIX RENORMALIZATION GROUP to find ground states of the Cluster Theory 
+# changing the transverse field parameters
 
-parser = argparse.ArgumentParser(prog="gs_search_Ising")
+parser = argparse.ArgumentParser(prog="gs_search_Cluster")
 parser.add_argument(
     "npoints",
     help="Number of points in an interval of transverse field values",
     type=int,
 )
 parser.add_argument(
-    "h_i", help="Starting value of h (external transverse field)", type=float
+    "hx_i", help="Starting value of h (external transverse field)", type=float
 )
 parser.add_argument(
-    "h_f", help="Final value of h (external transverse field)", type=float
+    "hx_f", help="Final value of h (external transverse field)", type=float
+)
+parser.add_argument(
+    "hy_i", help="Starting value of h (external transverse field)", type=float
+)
+parser.add_argument(
+    "hy_f", help="Final value of h (external transverse field)", type=float
 )
 parser.add_argument(
     "path",
     help="Path to the drive depending on the device used. Available are 'pc', 'mac', 'marcos'",
     type=str,
 )
-parser.add_argument("-L", "--Ls", help="Spin chain lengths", nargs="*", type=int)
+parser.add_argument("-L", "--Ls", help="Number of sites in the chain", nargs="+", type=int)
 parser.add_argument("-D", "--chis", help="Simulated bond dimensions", nargs="+", type=int)
-parser.add_argument("-d","--dimension", help="Physical dimension. By default 2", default=2, type=int)
 parser.add_argument(
-    "-ty", "--type_shape", help="Type of shape of the bond dimension. Available are: 'trapezoidal', 'pyramidal', 'rectangular'", default="trapezoidal", type=str
+    "-ty", "--type_shape", help="Type of shape of the bond dimension. Available are: 'trapezoidal', 'pyramidal', 'rectangular'", default="rectangular", type=str
+)
+parser.add_argument(
+    "-m", "--model", help="Model to simulate. By default XXZ", default="XXZ", type=str
 )
 parser.add_argument(
-    "-m", "--model", help="Model to simulate", default="Ising", type=str
+    "-mu", "--multpr", help="If True computes ground states with multiprocessing. By default False", action="store_true"
 )
 parser.add_argument(
     "-s",
     "--number_sweeps",
     help="Number of sweeps during the compression algorithm for each trotter step",
     default=8,
     type=int,
 )
 parser.add_argument(
     "-cv",
     "--conv_tol",
     help="Convergence tolerance of the compression algorithm",
-    default=1e-10,
+    default=1e-12,
     type=float,
 )
 parser.add_argument(
-    "-fid",
-    "--fidelity",
-    help="Fidelity with exact solution. Doable only for small Ising chains",
-    action="store_true",
-)
-parser.add_argument(
     "-b",
     "--bond",
     help="Save the schmidt values for one bond. If False save for each bond. By default True",
     action="store_false",
 )
 parser.add_argument(
     "-w",
     "--where",
     help="Bond where we want to observe the Schmidt values, should be between 1 and (L-1)",
     default=-1,
     type=int,
 )
+parser.add_argument(
+    "-v",
+    "--save",
+    help="Save the tensors. By default True",
+    action="store_false",
+)
+parser.add_argument(
+    "-tr",
+    "--training",
+    help="Save all the energies during the variational optimization. By default True",
+    action="store_false",
+)
+parser.add_argument(
+    "-i",
+    "--interval",
+    help="Type of interval spacing. Available are 'log', 'lin'",
+    default="lin",
+    type=str
+)
 
 args = parser.parse_args()
 
+# define the physical dimension
+d = int(2)
+
 # define the interval of equally spaced values of external field
-interval = np.linspace(args.h_i, args.h_f, args.npoints)
+if args.interval == "lin":
+    interval = np.linspace(args.hx_i, args.hx_f, args.npoints)
+    num = (args.hx_f - args.hx_i) / args.npoints
+    precision = get_precision(num)
+elif args.interval == "log":
+    interval = np.logspace(args.hx_i, args.hx_f, args.npoints)
+    num = (interval[-1]-interval[0]) / args.npoints
+    precision = get_precision(num)
+
+interval_d = np.linspace(args.hx_i, args.hx_f, args.npoints).tolist()
+interval_h = np.linspace(args.hy_i, args.hy_f, args.npoints)
+interval_d.reverse()
 
 # take the path and precision to save files
 # if we want to save the tensors we save them locally because they occupy a lot of memory
 if args.path == "pc":
-    parent_path = "G:/My Drive/projects/0_ISING"
-    path_tensor = "D:/code/projects/0_ISING"
+    parent_path = "G:/My Drive/projects/4_XXZ"
+    path_tensor = "D:/code/projects/4_XXZ"
 elif args.path == "mac":
-    parent_path = "/Users/fradm98/Google Drive/My Drive/projects/0_ISING"
-    path_tensor = "/Users/fradm98/Desktop/projects/0_ISING"
+    parent_path = "/Users/fradm98/Google Drive/My Drive/projects/4_XXZ"
+    path_tensor = "/Users/fradm98/Desktop/projects/4_XXZ"
 elif args.path == "marcos":
-    parent_path = "/Users/fradm/Google Drive/My Drive/projects/0_ISING"
-    path_tensor = "/Users/fradm/Desktop/projects/0_ISING"
+    parent_path = "/Users/fradm/Google Drive/My Drive/projects/4_XXZ"
+    path_tensor = "/Users/fradm/Desktop/projects/4_XXZ"
 else:
     raise SyntaxError("Path not valid. Choose among 'pc', 'mac', 'marcos'")
 
-path = f"{parent_path}/results/tensors"
-num = (args.h_f - args.h_i) / args.npoints
-precision = get_precision(num)
 
-Z = np.array([[1, 0], [0, -1]])
+
 
 # ---------------------------------------------------------
 # DMRG
 # ---------------------------------------------------------
 for L in args.Ls:
+    # where to look at for the entropy
     if args.where == -1:
         args.where = L // 2
     elif args.where == -2:
         args.bond = False
     for chi in args.chis:  # L // 2 + 1
-        args_mps = {
-            "L": L,
-            "d": args.dimension,
-            "model": args.model,
-            "chi": chi,
-            "path": path_tensor,
-            "type_shape": args.type_shape,
-            "precision": precision,
-            "trunc_chi": True,
-            "trunc_tol": False,
-            "where": args.where,
-            "bond": args.bond,
-            "J": 1,
-            "eps": 0,
-        }
-        if __name__ == "__main__":
-            
+        up = np.array([[[1],[0]]])
+        init_tensor = [up for _ in range(L)]
+
+        energy_chi = []
+        entropy_chi = []
+        schmidt_vals_chi = []
+        for h in interval_h:
+            energy_h = []
+            entropy_h = []
+            schmidt_vals_h = []
+            for delta in interval_d:
+                chain = MPS(L=L, d=d, chi=chi, model=args.model, eps=1e-5, h=h, J=1, k=delta)
+                chain.sites = init_tensor.copy()
+                chain.enlarge_chi()
+                energy, entropy, schmidt_vals, _ = chain.DMRG(trunc_tol=False, trunc_chi=True, where=L//2)
+                print(f"energy of h:{h:.{precision}f}, delta:{delta:.{precision}f} is:\n {energy}")
+                print(f"Schmidt values in the middle of the chain:\n {schmidt_vals}")
+                print(f"Entropy: {entropy}")
+                
+                if args.training:
+                    energy_h.append(energy)
+                else:
+                    energy_h.append(energy[-1])
+                entropy_h.append(entropy)
+                schmidt_vals_h.append(schmidt_vals)
+                chain.save_sites(path=path_tensor, precision=precision)
+                if h == interval_h[0]:
+                    init_tensor_h = chain.sites.copy()
+                init_tensor = chain.sites.copy()
             
-            energy_chi = []
-            entropy_chi = []
-            schmidt_vals_chi = []
-            for J in interval:
-                init_state = np.zeros((1, 2, 1))
-                init_state[0, 0, 0] = 1
-                init_tensor = [init_state for _ in range(L)]
-                for h in interval:
-                    precision = args_mps["precision"]
-                    chain = MPS(
-                        L=args_mps["L"],
-                        d=args_mps["d"],
-                        model=args_mps["model"],
-                        chi=args_mps["chi"],
-                        h=h,
-                        J=J,
-                        eps=args_mps["eps"],
-                    )
-                    chain.sites = init_tensor
-                    chain.enlarge_chi(type_shape="rectangular", prnt=False)
-                    # chain._random_state(seed=7, chi=args_mps["chi"], type_shape=args_mps["type_shape"])
-                    chain.canonical_form(trunc_chi=False, trunc_tol=True)
-                    # total
-                    chain.order_param(op=Z)
-                    mag = np.real(chain.mpo_first_moment())
-                    if mag < 0:
-                        chain.flipping_all()
-
-                    energy, entropy, schmidt_vals = chain.DMRG(
-                        trunc_tol=args_mps["trunc_tol"],
-                        trunc_chi=args_mps["trunc_chi"],
-                        where=args_mps["where"],
-                        bond=args_mps["bond"],
-                    )
-
-                    print(f"energy of h:{h:.{precision}f}, J:{J:.{precision}f} is:\n {energy}")
-                    print(f"Schmidt values in the middle of the chain:\n {schmidt_vals}")
-
-                    chain.save_sites(path=args_mps["path"], precision=args_mps["precision"])
-                    energy_chi.append(energy)
-                    entropy_chi.append(entropy)
-                    schmidt_vals_chi.append(schmidt_vals)
-
-            # energy_chi, entropy_chi, schmidt_vals_chi = ground_state_ising(
-            #     args_mps=args_mps, multpr=False, param=interval
-            # )
-
-            if args.bond == False:
-                args.where = "all"
-
-            energy_chi = np.array(energy_chi)
-            energy_chi = np.array_split(energy_chi, args.npoints)
-            save_list_of_lists(
-                f"{parent_path}/results/energy_data/energies_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
+            init_tensor = init_tensor_h.copy()
+
+            # energy_h.reverse()
+            # entropy_h.reverse()
+            # schmidt_vals_h.reverse()
+            energy_chi.append(energy_h)
+            entropy_chi.append(entropy_h)
+            schmidt_vals_chi.append(schmidt_vals_h)
+
+        if args.bond == False:
+            args.where = "all"
+
+        if args.training:
+            energy_chi = np.swapaxes(swap_rows(np.asarray(energy_chi)), axis1=0, axis2=1)
+            np.save(
+                f"{parent_path}/results/energy_data/energies_{args.model}_L_{L}_d_{args.hx_i}-{args.hx_f}_h_{args.hy_i}-{args.hy_f}_delta_{args.npoints}_chi_{chi}",
                 energy_chi,
             )
-            entropy_chi = np.array(entropy_chi)
-            entropy_chi = np.array_split(entropy_chi, args.npoints)
-            save_list_of_lists(
-                f"{parent_path}/results/entropy/{args.where}_bond_entropy_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
-                entropy_chi,
+            for i in range(len(interval_h)):
+                for j in range(len(interval_d)):
+                    np.save(f"{parent_path}/results/energy_data/energy_{args.model}_L_{L}_d_{args.hx_i}-{args.hx_f}_h_{args.hy_i}-{args.hy_f}_delta_{args.npoints}_chi_{chi}", energy_chi[i][j][-1])
+
+        else:
+            np.save(
+                f"{parent_path}/results/energy_data/energy_{args.model}_L_{L}_d_{args.hx_i}-{args.hx_f}_h_{args.hy_i}-{args.hy_f}_delta_{args.npoints}_chi_{chi}",
+                energy_chi,
             )
-            schmidt_vals_chi = np.array(schmidt_vals_chi)
-            schmidt_vals_chi = np.array_split(schmidt_vals_chi, args.npoints)
-            save_list_of_lists(
-                f"{parent_path}/results/entropy/{args.where}_schmidt_values_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
-                schmidt_vals_chi,
+            
+        save_list_of_lists(
+            f"{parent_path}/results/entropy_data/{args.where}_bond_entropy_{args.model}_L_{L}_d_{args.hx_i}-{args.hx_f}_h_{args.hy_i}-{args.hy_f}_delta_{args.npoints}_chi_{chi}",
+            entropy_chi,
+        )
+        save_list_of_lists(
+            f"{parent_path}/results/entropy_data/{args.where}_schmidt_vals_{args.model}_L_{L}_d_{args.hx_i}-{args.hx_f}_h_{args.hy_i}-{args.hy_f}_delta_{args.npoints}_chi_{chi}",
+            schmidt_vals_chi,
+        )
+        if args.where == "all":
+            entropy_mid = access_txt(
+                f"{parent_path}/results/entropy_data/{args.where}_bond_entropy_{args.model}_L_{L}_d_{args.hx_i}-{args.hx_f}_h_{args.hy_i}-{args.hy_f}_delta_{args.npoints}_chi_{chi}",
+                (L-1) // 2,
             )
-            if args.where == "all":
-                entropy_mid = access_txt(
-                    f"{parent_path}/results/entropy/{args.where}_bond_entropy_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
-                    L // 2,
-                )
-                np.savetxt(
-                    f"{parent_path}/results/entropy/{L // 2}_bond_entropy_{args.model}_L_{L}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
-                    entropy_mid,
-                )
+            np.savetxt(
+                f"{parent_path}/results/entropy_data/{args.L // 2}_bond_entropy_{args.model}_L_{L}_d_{args.hx_i}-{args.hx_f}_h_{args.hy_i}-{args.hy_f}_delta_{args.npoints}_chi_{chi}",
+                entropy_mid,
+            )
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ISING/get_gs_and_time_ev_EXACT.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ISING/get_gs_and_time_ev_EXACT.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ISING/get_observables_MPS.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ISING/get_observables_MPS.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ISING/plot_DMRG.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ISING/plot_DMRG.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/ISING/plot_TEBD.py` & `qs-mps-2024.0.1/src/qs_mps/applications/ISING/plot_TEBD.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/exact_hamiltonian.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/exact_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/get_gs_DMRG.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/get_gs_DMRG.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 parser.add_argument(
     "-mu", "--multpr", help="If True computes ground states with multiprocessing. By default False", action="store_true"
 )
 parser.add_argument(
     "-s",
     "--number_sweeps",
     help="Number of sweeps during the compression algorithm for each trotter step",
-    default=8,
+    default=10,
     type=int,
 )
 parser.add_argument(
     "-cv",
     "--conv_tol",
     help="Convergence tolerance of the compression algorithm",
     default=1e-12,
@@ -70,16 +70,16 @@
     "--save",
     help="Save the tensors. By default True",
     action="store_false",
 )
 parser.add_argument(
     "-tr",
     "--training",
-    help="Save all the energies during the variational optimization. By default False",
-    action="store_true",
+    help="Save all the energies during the variational optimization. By default True",
+    action="store_false",
 )
 parser.add_argument(
     "-i",
     "--interval",
     help="Type of interval spacing. Available are 'log', 'lin'",
     default="lin",
     type=str
@@ -93,16 +93,15 @@
 # define the interval of equally spaced values of external field
 if args.interval == "lin":
     interval = np.linspace(args.h_i, args.h_f, args.npoints)
     num = (interval[-1] - interval[0]) / args.npoints
     precision = get_precision(num)
 elif args.interval == "log":
     interval = np.logspace(args.h_i, args.h_f, args.npoints)
-    num = (args.h_f - args.h_i) / args.npoints
-    precision = get_precision(num)
+    precision = int(np.max([np.abs(args.h_f),np.abs(args.h_i)]))
 
 # take the path and precision to save files
 # if we want to save the tensors we save them locally because they occupy a lot of memory
 if args.path == "pc":
     parent_path = "G:/My Drive/projects/1_Z2"
     path_tensor = "D:/code/projects/1_Z2"
 elif args.path == "mac":
@@ -124,20 +123,25 @@
         sector = "vacuum_sector"
         charges_x = None
         charges_y = None
     else:
         sector = f"{len(args.charges_x)}_particle(s)_sector"
         charges_x = args.charges_x
         charges_y = args.charges_y
-
     # where to look at for the entropy
     if args.where == -1:
         args.where = L // 2
     elif args.where == -2:
         args.bond = False
+
+    # init_state = np.zeros((d))
+    # init_state[0] = 1
+    # init_state = init_state.reshape((1,d,1))
+    # init_tensor = [init_state for _ in range(L-1)]
+    init_tensor = []
     for chi in args.chis:  # L // 2 + 1
         args_mps = {
             "L": L,
             "d": d,
             "chi": chi,
             "type_shape": args.type_shape,
             "model": args.model,
@@ -149,48 +153,63 @@
             "save": args.save,
             "precision": precision,
             "sector": sector,
             "charges_x": charges_x,
             "charges_y": charges_y,
             "n_sweeps": args.number_sweeps,
             "conv_tol": args.conv_tol,
+            "training": args.training,
+            "guess": init_tensor,
         }
         if __name__ == "__main__":
-            energy_chi, entropy_chi, schmidt_vals_chi = ground_state_Z2(
+            energy_chi, entropy_chi, schmidt_vals_chi, t_chi = ground_state_Z2(
                 args_mps=args_mps, multpr=args.multpr, param=interval
             )
 
+            t_final = np.sum(t_chi)
+            if t_final < 60:
+                t_unit = "sec(s)"
+            elif t_final > 60 and t_final < 3600:
+                t_unit = "min(s)"
+                t_final = t_final/60
+            elif t_final > 3600:
+                t_unit = "hour(s)"
+                t_final = t_final/3600
+
+            print(f"time of the whole search for chi={chi} is: {t_final} {t_unit}")
             if args.bond == False:
                 args.where = "all"
 
             if args.training:
-                save_list_of_lists(
+                energy_chi = np.asarray(energy_chi)
+                energy_chi = energy_chi.reshape((len(interval),len(energy_chi[0])))
+                print(energy_chi.shape)
+                np.save(
                     f"{parent_path}/results/energy_data/energies_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
                     energy_chi,
                 )
-                energy_gs = access_txt(
-                        f"{parent_path}/results/energy_data/energies_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
-                        -1,
-                    )
-                np.savetxt(
-                    f"{parent_path}/results/energy_data/energies_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
-                    energy_gs,
-                )
+                for i in range(len(interval)):
+                    np.save(f"{parent_path}/results/energy_data/energy_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}", energy_chi[i,-1])
+
             else:
-                np.savetxt(
-                    f"{parent_path}/results/energy_data/energies_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
+                np.save(
+                    f"{parent_path}/results/energy_data/energy_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
                     energy_chi,
                 )
-                
+
             save_list_of_lists(
                 f"{parent_path}/results/entropy_data/{args.where}_bond_entropy_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
                 entropy_chi,
             )
-            save_list_of_lists(
-                f"{parent_path}/results/entropy_data/{args.where}_schmidt_vals_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
+            # save_list_of_lists(
+            #     f"{parent_path}/results/entropy_data/{args.where}_schmidt_vals_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
+            #     schmidt_vals_chi,
+            # )
+            np.save(
+                f"{parent_path}/results/entropy_data/{args.where}_schmidt_vals_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}.npy",
                 schmidt_vals_chi,
             )
             if args.where == "all":
                 entropy_mid = access_txt(
                     f"{parent_path}/results/entropy_data/{args.where}_bond_entropy_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
                     (L-1) // 2,
                 )
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/get_gs_EXACT.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/get_gs_EXACT.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 # define the initial guess state
 dof_direct = (2*args.l*args.L - args.l - args.L)
 # constant without sparse method (if we start from h=0)
 c = (1/np.sqrt(2))**dof_direct
 
 print("finding guess for the sparse computation...")
-v0 = [c]*(2**dof_direct)
+v0 = np.full(2**dof_direct, c)
 v0 = np.array(v0, dtype=complex)
 print(v0)
 
 # choose how many eigenvalues to compute
 if args.spectrum == -1:
     spectrum = "gs"
 elif args.spectrum == 0:
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/get_observables_EXACT.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/get_observables_EXACT.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/get_observables_MPS.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/get_observables_MPS.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     "h_f", help="Final value of h (external transverse field on the dual lattice)", type=float
 )
 parser.add_argument(
     "path",
     help="Path to the drive depending on the device used. Available are 'pc', 'mac', 'marcos'",
     type=str,
 )
-parser.add_argument("-o", "--obs", help="Observable we want to compute. Available are 'wl', 'el', 'thooft'", type=str)
+parser.add_argument("-o", "--obs", help="Observable we want to compute. Available are 'wl', 'el', 'thooft', 'mag', 'corr'", type=str)
 parser.add_argument("-L", "--Ls", help="Number of rungs per ladder", nargs="+", type=int)
 parser.add_argument("-D", "--chis", help="Simulated bond dimensions", nargs="+", type=int)
 parser.add_argument("-cx", "--charges_x", help="a list of the first index of the charges", nargs="*", type=int)
 parser.add_argument("-cy", "--charges_y", help="a list of the second index of the charges", nargs="*", type=int)
-parser.add_argument("-lx", "--sites", help="Number of sites in the wilson loop", nargs="*", type=int)
-parser.add_argument("-ly", "--ladders", help="Number of ladders in the wilson loop", nargs="*", type=int)
+parser.add_argument("-lx", "--sites", help="coordinates of sites", nargs="*", type=int)
+parser.add_argument("-ly", "--ladders", help="coordinates of ladders", nargs="*", type=int)
 parser.add_argument(
     "-d", "--direction", help="Direction of the string", default="hor", type=str
 )
 parser.add_argument(
     "-m", "--model", help="Model to simulate", default="Z2_dual", type=str
 )
 parser.add_argument(
@@ -49,16 +49,19 @@
 
 # define the physical dimension
 d = int(2**(args.l))
 
 # define the interval of equally spaced values of external field
 if args.interval == "lin":
     interval = np.linspace(args.h_i, args.h_f, args.npoints)
+    num = (interval[-1] - interval[0]) / args.npoints
+    precision = get_precision(num)
 elif args.interval == "log":
     interval = np.logspace(args.h_i, args.h_f, args.npoints)
+    precision = int(np.max([np.abs(args.h_f),np.abs(args.h_i)]))
 
 # take the path and precision to save files
 # if we want to save the tensors we save them locally because they occupy a lot of memory
 if args.path == "pc":
     parent_path = "G:/My Drive/projects/1_Z2"
     path_tensor = "D:/code/projects/1_Z2"
 elif args.path == "mac":
@@ -66,22 +69,14 @@
     path_tensor = "/Users/fradm98/Desktop/projects/1_Z2"
 elif args.path == "marcos":
     parent_path = "/Users/fradm/Google Drive/My Drive/projects/1_Z2"
     path_tensor = "/Users/fradm/Desktop/projects/1_Z2"
 else:
     raise SyntaxError("Path not valid. Choose among 'pc', 'mac', 'marcos'")
 
-num = (args.h_f - args.h_i) / args.npoints
-precision = get_precision(num)
-
-# # for the wilson loop
-# if args.sites == 1:
-#     sites = 0
-# if args.ladders == 1:
-#     ladders = 1
 
 # define the direction
 if args.direction == "ver":
     direction = "vertical"
 elif args.direction == "hor":
     direction = "horizontal"    
 
@@ -109,75 +104,86 @@
         charges_y = args.charges_y
 
     for chi in args.chis:
         W = []
         E = []
         S = []
         M = []
+        C = []
         for h in interval:
             lattice_mps = MPS(L=L, d=d, model=args.model, chi=chi, h=h)
             lattice_mps.L = lattice_mps.L - 1
 
             lattice_mps.load_sites(path=path_tensor, precision=precision, cx=charges_x, cy=charges_y)
             if sector != "vacuum_sector":
                 lattice_mps.Z2.add_charges(charges_x, charges_y)
             
             if args.obs == "wl":
-                print(f"wilson loop for h:{h:.{precision}f}, L:{L}")
+                print(f"wilson loop for h:{h:.{precision}f}, direct lattice lxL:{args.l}x{L-1}, chi:{chi}")
                 lattice_mps.Z2.wilson_Z2_dual(mpo_sites=args.sites, ls=args.ladders) #list(range(s))
                 lattice_mps.w = lattice_mps.Z2.mpo.copy()
                 if args.moment == 1:
                     print(lattice_mps.mpo_first_moment().real)
                     W.append(lattice_mps.mpo_first_moment().real)
                 elif args.moment == 2:
                     print(lattice_mps.mpo_second_moment().real)
                     W.append(lattice_mps.mpo_second_moment().real)
                 elif args.moment == 4:
                     print(lattice_mps.mpo_fourth_moment().real)
                     W.append(lattice_mps.mpo_fourth_moment().real)
 
             elif args.obs == "el":
-                print(f"electric field for h:{h:.{precision}f}, L:{L}")
+                print(f"electric field for h:{h:.{precision}f}, direct lattice lxL:{args.l}x{L-1}, chi:{chi}")
                 E_h = np.zeros((2*args.l+1,2*L-1))
                 E_h[:] = np.nan
                 E_h = lattice_mps.electric_field_Z2(E_h)
                 E.append(E_h)
             
             elif args.obs == "thooft":
-                print(f"'t Hooft string for h:{h:.{precision}f}, L:{L}")
+                print(f"'t Hooft string for h:{h:.{precision}f}, direct lattice lxL:{args.l}x{L-1}, chi:{chi}")
                 lattice_mps.Z2.thooft(site=args.sites, l=args.ladders, direction=direction)
                 lattice_mps.w = lattice_mps.Z2.mpo.copy()
                 S.append(lattice_mps.mpo_first_moment().real)
 
             elif args.obs == "mag":
-                print(f"Magnetization for h:{h:.{precision}f}, L:{L}")
+                print(f"Magnetization for h:{h:.{precision}f}, direct lattice lxL:{args.l}x{L-1}, chi:{chi}")
                 lattice_mps.order_param()
                 if args.moment == 1:
                     print(lattice_mps.mpo_first_moment().real, (len(lattice_mps.Z2.latt.plaquettes())-(2*(L-3)+2*(args.l))))
                     M.append(lattice_mps.mpo_first_moment().real/(len(lattice_mps.Z2.latt.plaquettes())-(2*(L-3)+2*(args.l))))
                 elif args.moment == 2:
                     M.append(lattice_mps.mpo_second_moment().real/(len(lattice_mps.Z2.latt.plaquettes())-(2*(L-3)+2*(args.l)))**2)
                 elif args.moment == 4:
                     M.append(lattice_mps.mpo_fourth_moment().real/(len(lattice_mps.Z2.latt.plaquettes())-(2*(L-3)+2*(args.l)))**4)
 
-
-
-    if args.obs == "wl":
-        np.savetxt(
-                    f"{parent_path}/results/wilson_loops/wilson_loop_{moment}_moment_{args.model}_direct_lattice_{args.l}x{L-1}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
-                    W,
-                )
-    if args.obs == "el":
-        np.save(
-                    f"{parent_path}/results/electric_field/electric_field_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{args.charges_x}-{args.charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}.npy",
-                    E,
-                )
-    if args.obs == "thooft":
-        np.save(
-                    f"{parent_path}/results/thooft/thooft_string_{moment}_moment_{args.sites[0]}-{args.ladders[0]}_{direction}_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{args.charges_x}-{args.charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}.npy",
-                    S,
-                )
-    if args.obs == "mag":
-        np.save(
-                    f"{parent_path}/results/mag_data/dual_mag_{moment}_moment_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{args.charges_x}-{args.charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}.npy",
-                    M,
-                )
+            elif args.obs == "corr":
+                print(f"Correlator for h:{h:.{precision}f}, direct lattice lxL:{args.l}x{L-1}, chi:{chi}")
+                c = lattice_mps.connected_correlator(site=args.sites[0], lad=args.ladders[0])
+                C.append(c)
+
+
+        if args.obs == "wl":
+            np.savetxt(
+                        f"{parent_path}/results/wilson_loops/wilson_loop_{moment}_moment_{args.model}_direct_lattice_{args.l}x{L-1}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}",
+                        W,
+                    )
+        if args.obs == "el":
+            np.save(
+                        f"{parent_path}/results/electric_field/electric_field_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}.npy",
+                        E,
+                    )
+        if args.obs == "thooft":
+            np.save(
+                        f"{parent_path}/results/thooft/thooft_string_{moment}_moment_{args.sites[0]}-{args.ladders[0]}_{direction}_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}.npy",
+                        S,
+                    )
+        if args.obs == "mag":
+            np.save(
+                        f"{parent_path}/results/mag_data/dual_mag_{moment}_moment_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}.npy",
+                        M,
+                    )
+        if args.obs == "corr":
+            C = np.array_split(C, args.npoints)
+            np.save(
+                        f"{parent_path}/results/mag_data/connected_correlator_s_{args.sites[0]}_l_{args.ladders[0]}_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_{args.h_i}-{args.h_f}_delta_{args.npoints}_chi_{chi}.npy",
+                        C,
+                    )
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/multi_run_gs.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/multi_run_gs.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/multi_run_obs.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/multi_run_obs.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/plot_DMRG.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/plot_DMRG.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/plot_animations.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/plot_animations.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/test_sparse_mpo.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/test_sparse_mpo.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/time_ev_debug.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/time_ev_debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 parser.add_argument(
     "path",
     help="Path to the drive depending on the device used. Available are 'pc', 'mac', 'marcos'",
     type=str,
 )
 parser.add_argument("-L", "--Ls", help="Number of rungs per ladder", nargs="+", type=int)
 parser.add_argument("-D", "--chis", help="Simulated bond dimensions", nargs="+", type=int)
-parser.add_argument("-o", "--obs", help="Observable we want to compute. Available are 'wl', 'el', 'thooft', 'mag'", nargs="*", type=str)
+parser.add_argument("-o", "--obs", help="Observable we want to compute. Available are 'wl', 'el', 'thooft', 'mag', 'eed'", nargs="*", type=str)
 parser.add_argument("-cx", "--charges_x", help="a list of the first index of the charges", nargs="*", type=int)
 parser.add_argument("-cy", "--charges_y", help="a list of the second index of the charges", nargs="*", type=int)
 parser.add_argument("-lx", "--sites", help="Number of sites in the wilson loop", nargs="*", type=int)
 parser.add_argument("-ly", "--ladders", help="Number of ladders in the wilson loop", nargs="*", type=int)
 parser.add_argument(
     "-d", "--direction", help="Direction of the string", default="hor", type=str
 )
@@ -132,18 +132,19 @@
     if args.where == -1:
         args.where = L // 2
     elif args.where == -2:
         args.bond = False
 
     for chi in args.chis:
         W = []
-        E = []
+        El = []
         S = []
         M = []
         C = []
+        Ed = []
 
         # initialize the tensor
         lattice_mps = MPS(L=L, d=d, model=args.model, chi=chi, h=args.h_i)
         lattice_mps.L = lattice_mps.L - 1
         
         # load the mps
         lattice_mps.load_sites(path=path_tensor, precision=precision, cx=charges_x, cy=charges_y)
@@ -172,15 +173,15 @@
                 W.append(lattice_mps.mpo_fourth_moment().real)
 
         if  "el" in args.obs:
             print(f"electric field before trotter - L:{L}, chi:{chi}")
             E_h = np.zeros((2*args.l+1,2*L-1))
             E_h[:] = np.nan
             E_h = lattice_mps.electric_field_Z2(E_h)
-            E.append(E_h)
+            El.append(E_h)
         
         if "thooft" in args.obs:
             print(f"'t Hooft string before trotter - L:{L}, chi:{chi}")
             lattice_mps.Z2.thooft(site=args.sites, l=args.ladders, direction=direction)
             lattice_mps.w = lattice_mps.Z2.mpo.copy()
             S.append(lattice_mps.mpo_first_moment().real)
 
@@ -196,14 +197,21 @@
 
         if "corr" in args.obs:
             s = (charges_x[0]+charges_x[1]) //2
             lad = np.min(charges_y)
             print(f"connected correlator before trotter - L:{L}, chi:{chi}")
             corr = lattice_mps.connected_correlator(site=s, lad=lad)
             C.append(corr)
+        
+        if "eed" in args.obs:
+            s = (charges_x[0]+charges_x[1]) //2
+            print(f"electric energy density before trotter - L:{L}, chi:{chi}")
+            ed = lattice_mps.electric_energy_density_Z2(site=s)
+            Ed.append(ed)
+
         # ---------------------------------------------------------
         # Trotter Evolution
         # ---------------------------------------------------------        
         lattice_mps.enlarge_chi()
         lattice_mps.ancilla_sites = lattice_mps.sites.copy()
         for t in range(args.npoints):
             
@@ -224,15 +232,15 @@
                     W.append(lattice_mps.mpo_fourth_moment().real)
 
             if  "el" in args.obs:
                 print(f"electric field for trotter step:{t}, L:{L}, chi:{chi}")
                 E_h = np.zeros((2*args.l+1,2*L-1))
                 E_h[:] = np.nan
                 E_h = lattice_mps.electric_field_Z2(E_h)
-                E.append(E_h)
+                El.append(E_h)
             
             if "thooft" in args.obs:
                 print(f"'t Hooft string for trotter step:{t}, L:{L}, chi:{chi}")
                 lattice_mps.Z2.thooft(site=args.sites, l=args.ladders, direction=direction)
                 lattice_mps.w = lattice_mps.Z2.mpo.copy()
                 S.append(lattice_mps.mpo_first_moment().real)
 
@@ -246,14 +254,20 @@
                 elif args.moment == 4:
                     M.append(lattice_mps.mpo_fourth_moment().real/(len(lattice_mps.Z2.latt.plaquettes())-(2*(L-3)+2*(args.l)))**4)
 
             if "corr" in args.obs:
                 print(f"connected correlator for trotter step:{t}, L:{L}, chi:{chi}")
                 corr = lattice_mps.connected_correlator(site=s, lad=lad)
                 C.append(corr)
+            
+            if "eed" in args.obs:
+                s = (charges_x[0]+charges_x[1]) //2
+                print(f"electric energy density before trotter - L:{L}, chi:{chi}")
+                ed = lattice_mps.electric_energy_density_Z2(site=s)
+                Ed.append(ed)
 
             print(f"\nError at trotter step: {t} is: {error}\n")
             errors_tr.append(error)
             errors.append(error[-1])
             entropies.append(entropy)
             schmidt_vals.append(schmidt_values)
 
@@ -261,15 +275,15 @@
             np.save(
                         f"{parent_path}/results/wilson_loops/wilson_loop_{moment}_moment_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{args.charges_x}-{args.charges_y}_h_i_{args.h_i}_h_ev_{args.h_ev}_delta_{args.delta}_trotter_steps_{args.npoints}_chi_{chi}.npy",
                         W,
                     )
         if "el" in args.obs:
             np.save(
                         f"{parent_path}/results/electric_field/electric_field_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{args.charges_x}-{args.charges_y}_h_i_{args.h_i}_h_ev_{args.h_ev}_delta_{args.delta}_trotter_steps_{args.npoints}_chi_{chi}.npy",
-                        E,
+                        El,
                     )
         if "thooft" in args.obs:
             np.save(
                         f"{parent_path}/results/thooft/thooft_string_{moment}_moment_{args.sites[0]}-{args.ladders[0]}_{direction}_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{args.charges_x}-{args.charges_y}_h_i_{args.h_i}_h_ev_{args.h_ev}_delta_{args.delta}_trotter_steps_{args.npoints}_chi_{chi}.npy",
                         S,
                     )
         if "mag" in args.obs:
@@ -278,14 +292,19 @@
                         M,
                     )
         if "corr" in args.obs:
             np.save(
                         f"{parent_path}/results/mag_data/connected_correlator_s_{s}_l_{lad}_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{args.charges_x}-{args.charges_y}_h_i_{args.h_i}_h_ev_{args.h_ev}_delta_{args.delta}_trotter_steps_{args.npoints}_chi_{chi}.npy",
                         C,
                     )
+        if "eed" in args.obs:
+            np.save(
+                        f"{parent_path}/results/electric_field/electric_energy_density_s_{s}_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{args.charges_x}-{args.charges_y}_h_i_{args.h_i}_h_ev_{args.h_ev}_delta_{args.delta}_trotter_steps_{args.npoints}_chi_{chi}.npy",
+                        Ed,
+                    )
             
         if args.bond == False:
             args.where = "all"
 
         if args.training:
             save_list_of_lists(
                 f"{parent_path}/results/error_data/errors_tr_quench_dynamics_{args.model}_direct_lattice_{args.l}x{L-1}_{sector}_{charges_x}-{charges_y}_h_i_{args.h_i}_h_ev_{args.h_ev}_delta_{args.delta}_trotter_steps_{args.npoints}_chi_{chi}",
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/applications/Z2/vacuum_sector.py` & `qs-mps-2024.0.1/src/qs_mps/applications/Z2/vacuum_sector.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import time
 
 
 # finding the ground state of the vacuum sector
 L = 5
 l = 2
 d = int(2**l)
-chi = 4  # this is interpreted as d**(int(log2(chi))) --> e.g. chi=8 == 4**3=64
-type_shape = "trapezoidal"
-array = np.linspace(0, 10, 100)
+chi = 16  # this is interpreted as d**(int(log2(chi))) --> e.g. chi=8 == 4**3=64
+type_shape = "rectangular"
+array = np.linspace(0.001, 10, 100)
 hs = [h for h in array]
 model = "Z2_dual"
 path = "/Users/fradm98/Desktop/projects/1_Z2"
 multpr = False
 param = hs
 
 if __name__ == "__main__":
@@ -32,17 +32,25 @@
         "chi": chi,
         "type_shape": type_shape,
         "model": model,
         "trunc_tol": False,
         "trunc_chi": True,
         "where": L // 2,
         "path": path,
+        "save": True,
+        "precision": 2,
+        "sector": "vacuum_sector",
+        "bond": True,
+        "n_sweeps": 2,
+        "conv_tol": 1e-10,
+        "charges_x": None,
+        "charges_y": None,
     }
 
-    energies_h, entropy_h = ground_state_Z2(
+    energies_h, entropy_h, schmidt_vals = ground_state_Z2(
         args_mps=args_mps, multpr=multpr, param=param
     )
 
 
 # exact
 eig_exact = []
 eig_first = []
@@ -55,15 +63,15 @@
 dof = (2*l*L - l - L)
 print(dof)
 v0 = np.array([-0.25 for _ in range(2**dof)])
 for s in range(L-1):
     W = []
     W_exact = []
     for h in hs:
-        # print(f"h: {h}")
+        print(f"h: {h}")
         ladder = MPS(L=L, d=d, model=model, h=h, eps=0, J=1, chi=chi)
         ladder.L = ladder.L - 1
 
         ladder.load_sites(path=path)
         ladder.Z2.wilson_Z2_dual(mpo_sites=[s], ls=[1]) #list(range(s))
         ladder.w = ladder.Z2.mpo
         W.append(ladder.mpo_first_moment().real)
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/checks.py` & `qs-mps-2024.0.1/src/qs_mps/checks.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/gs_multiprocessing.py` & `qs-mps-2024.0.1/src/qs_mps/gs_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/lattice.py` & `qs-mps-2024.0.1/src/qs_mps/lattice.py`

 * *Files identical despite different names*

### Comparing `qs-mps-2024.0.0/src/qs_mps/mpo_class.py` & `qs-mps-2024.0.1/src/qs_mps/mpo_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,16 +332,16 @@
         """
         thooft
 
         This function finds the 't Hooft string for the Z2 dual lattice.
         It gives us vertical and horizontal strings from a specific dual lattice
         site and going, conventionally, up and left, respectively (to vertical and horizontal).
         
-        site: list - the first element is the mps site of the interested dual lattice site
-        l: list - the first element is the ladder of the interested dual lattice site
+        site: list - the first element is the mps site of the interested dual lattice site, starts from 0
+        l: list - the first element is the ladder of the interested dual lattice site, starts from 0
         direction: str - indicates in the direction of the string. We use the convention:
                 hor -> from left to 'site' at a specific 'l'
                 ver -> from up to 'l' at a specific 'site'
 
         """
         self.mpo_skeleton(aux_dim=2)
 
@@ -504,25 +504,25 @@
 
             mpo_tot.append(self.mpo)
             self.mpo_skeleton(aux_dim=2)
 
         self.mpo = mpo_tot
         return self
 
-    def zz_observable_Z2_dual(self, mpo_site, l, direction):
+    def zz_observable_Z2_dual(self, mpo_site: int, l: int, direction: str, aux_dim: int=2):
         """
         zz_observable_Z2_dual
 
         This function finds the mpo representing the interacting observales in the
         dual lattice of the Z2 theory. We make a distinction in the direction of
         the interaction because in our mps formalism the vertical interaction falls
         back into a local one.
 
         """
-        self.mpo_skeleton(aux_dim=2)
+        self.mpo_skeleton(aux_dim=aux_dim)
 
         mpo_tot = []
         i = 0
 
         for site in range(self.L - 1):
             if direction == "horizontal":
                 assert (0 <= mpo_site < self.L-2), "The mpo site is out of bound. Choose it 0 <= site < L-2"
@@ -537,11 +537,11 @@
                 if mpo_site == site:
                     self.mpo[0, -1] = (
                         sparse_pauli_z(n=l, L=self.l).toarray()
                         @ sparse_pauli_z(n=l + 1, L=self.l).toarray()
                     )
 
             mpo_tot.append(self.mpo)
-            self.mpo_skeleton(aux_dim=2)
+            self.mpo_skeleton(aux_dim=aux_dim)
 
         self.mpo = mpo_tot
         return self
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/mps_class.py` & `qs-mps-2024.0.1/src/qs_mps/mps_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import numpy as np
-from ncon import ncon
-from scipy.sparse.linalg import eigsh, eigs
+
 from scipy.sparse import csr_matrix, csr_array, identity
 from scipy.linalg import expm, solve
+import scipy.linalg as la
+import scipy.sparse.linalg as spla
+
+from ncon import ncon
+
+import time 
 from qs_mps.utils import *
 from qs_mps.checks import check_matrix
 from qs_mps.sparse_hamiltonians_and_operators import (
     exact_evolution_sparse,
     sparse_ising_ground_state,
     U_evolution_sparse,
     sparse_pauli_x,
+    sparse_pauli_y,
     sparse_pauli_z
 )
 from qs_mps.mpo_class import MPO_ladder
-import time
 from qs_mps.TensorMultiplier import TensorMultiplierOperator
 
 class MPS:
     def __init__(
-        self, L, d, model=str, chi=None, w=None, h=None, eps=None, J=None, k=None, charges=None
+        self, L, d, model=str, chi=None, w=None, h=None, lx=None, ly=None, eps=None, J=None, k=None, charges=None
     ):
         self.L = L
         self.d = d
         self.model = model
         self.chi = chi
         self.w = w
         self.w_dag = w
         self.h = h
+        self.lx = lx
+        self.ly = ly
         self.eps = eps
         self.J = J
         self.k = k # (take positive values for annni model)
         self.charges = charges
         self.site = 1
         self.sites = []
         self.bonds = []
@@ -174,31 +181,31 @@
 
             original_matrix = new_site
             scaled_matrix = original_matrix / np.max(np.abs(original_matrix))
             lambda_ = 1e-15
             regularized_matrix = scaled_matrix + lambda_ * np.eye(
                 scaled_matrix.shape[0], scaled_matrix.shape[1]
             )
-            u, s, v = np.linalg.svd(
+            u, s, v = la.svd(
                 regularized_matrix,
                 full_matrices=False,
             )
 
             bond_l = u.shape[0] // self.d
             u = u.reshape(bond_l, self.d, u.shape[1])
             if trunc_chi:
                 if u.shape[0] > self.chi:
                     u = u[:, :, : self.chi]
                     s = s[: self.chi]
                     v = v[: self.chi, :]
-                    s = s / np.linalg.norm(s)
+                    s = s / la.norm(s)
             if trunc_tol:
                 condition = s >= schmidt_tol
                 s_trunc = np.extract(condition, s)
-                s = s_trunc / np.linalg.norm(s_trunc)
+                s = s_trunc / la.norm(s_trunc)
                 u = u[:, :, : len(s)]
                 v = v[: len(s), :]
 
             sites[i] = u
             bonds.append(s)
             psi = ncon(
                 [np.diag(s), v],
@@ -245,31 +252,31 @@
 
             original_matrix = new_site
             scaled_matrix = original_matrix / np.max(np.abs(original_matrix))
             lambda_ = 1e-15
             regularized_matrix = scaled_matrix + lambda_ * np.eye(
                 scaled_matrix.shape[0], scaled_matrix.shape[1]
             )
-            u, s, v = np.linalg.svd(
+            u, s, v = la.svd(
                 regularized_matrix,
                 full_matrices=False,
             )
 
             bond_r = v.shape[1] // self.d
             v = v.reshape((v.shape[0], self.d, bond_r))
             if trunc_chi:
                 if v.shape[0] > self.chi:
                     v = v[: self.chi, :, :]
                     s = s[: self.chi]
                     u = u[:, : self.chi]
-                    s = s / np.linalg.norm(s)
+                    s = s / la.norm(s)
             if trunc_tol:
                 condition = s >= schmidt_tol
                 s_trunc = np.extract(condition, s)
-                s = s_trunc / np.linalg.norm(s_trunc)
+                s = s_trunc / la.norm(s_trunc)
                 v = v[: len(s), :, :]
                 bonds.append(s)
                 u = u[:, : len(s)]
 
             sites[i] = v
             bonds.append(s)
             psi = ncon(
@@ -502,133 +509,292 @@
         env_l = env
         for i in range(sites[0] - 1):
             label_ket = [1, 3, -1]
             label_bra = [2, 3, -2]
             env_l = ncon([env_l, kets[i], bras[i]], [label_env, label_ket, label_bra])
         # right env:
         env_r = env
-        for i in range(self.L - 1, sites[-1], -1):
+        for i in range(self.L - 1, sites[-1]-1, -1):
             label_ket = [-1, 3, 1]
             label_bra = [-2, 3, 2]
             env_r = ncon([env_r, kets[i], bras[i]], [label_env, label_ket, label_bra])
         # central env
-        idx = 0
-        for i in range(sites[0] - 1, sites[-1]):
+        # idx = 0
+        for i in range(len(sites)):
             label_ket = [1, -1 - i, -len(sites) * 100]
             label_bra = [2, -len(sites) - 1 - i, -len(sites) * 100 - 1]
-            env_l = ncon([env_l, kets[i], bras[i]], [label_env, label_ket, label_bra])
-            up = [int(-elem) for elem in np.linspace(1, idx + 1, idx + 1)]
+            env_l = ncon([env_l, kets[sites[i]-1], bras[sites[i]-1]], [label_env, label_ket, label_bra])
+            up = [int(-elem) for elem in np.linspace(1, i + 1, i + 1)]
             down = [
                 int(-elem)
-                for elem in np.linspace(len(sites) + 1, len(sites) + 1 + idx, idx + 1)
+                for elem in np.linspace(len(sites) + 1, len(sites) + 1 + i, i + 1)
             ]
             label_env = up + down + mid_up + mid_down
-            idx += 1
-
-        mps_dm = ncon([env_l, env_r], [[label_env], [1, 2]])
+            # idx += 1
+        mps_dm = ncon([env_l, env_r], [label_env, [1, 2]])
 
         return mps_dm
 
+    def vector_to_mps(self, vec: np.ndarray, trunc_chi: bool=True, trunc_tol: bool=False, chi: int=1, schmidt_tol: float=1e-15):
+        """
+        vector_to_mps
+
+        We decompose the vector with successive svd starting from the right towards the left,
+        hence a left sweep. The final tensors will be in Right Canonical Form (RCF)
+        
+        vec: np.ndarray - vector we want to transform in a MPS
+
+        """
+        vec_legs = int(np.log2(len(vec)))
+        sites = []
+        bonds = []
+        alpha = 1
+        for i in range(vec_legs):
+            matrix = vec.reshape((2**(vec_legs-(i+1)),2*alpha))
+            u,s,v = la.svd(matrix, full_matrices=False)
+            bond_r = v.shape[1] // 2
+            v = truncation(v, threshold=1e-15)
+            s = truncation(s, threshold=1e-15)
+            u = truncation(u, threshold=1e-15)
+            v = v.reshape((v.shape[0], 2, bond_r))
+            if trunc_chi:
+                if v.shape[0] > chi:
+                    v = v[: chi, :, :]
+                    s = s[: chi]
+                    u = u[:, : chi]
+                    s = s / la.norm(s)
+            if trunc_tol:
+                condition = s >= schmidt_tol
+                s_trunc = np.extract(condition, s)
+                s = s_trunc / la.norm(s_trunc)
+                v = v[: len(s), :, :]
+                u = u[:, : len(s)]
+
+            sites.append(v)
+            bonds.append(s)
+            vec = u @ np.diag(s)
+            alpha = vec.shape[1]
+        
+        sites.reverse()
+        bonds.reverse()
+        self.sites = sites.copy()
+        self.bonds = bonds.copy()
+        return self
+
     # -------------------------------------------------
     # Matrix Product Operators, MPOs
     # -------------------------------------------------
-    def mpo(self):
+    def mpo(self, long: str="X", trans: str="Z"):
         """
         mpo
 
         This function selects which MPO to use according to the
         studied model. Here you can add other MPOs that you have
         independently defined in the class.
 
         """
         if self.model == "Ising":
-            self.mpo_Ising()
+            self.mpo_Ising(long=long)
 
         elif self.model == "ANNNI":
-            self.mpo_ANNNI()
+            self.mpo_ANNNI(long=long, deg_method=1)
+        
+        elif self.model == "Cluster":
+            self.mpo_Cluster(long=long)
+        
+        elif self.model == "Cluster-XY":
+            self.mpo_Cluster_xy(long=long)
 
         elif self.model == "Z2_dual":
             self.Z2.mpo_Z2_ladder_generalized()
             self.w = self.Z2.mpo
 
+        elif self.model == "XXZ":
+            self.mpo_xxz(long=long)
+
         return self
 
     # -------------------------------------------------
     # Hamiltonians, time evolution operators
     # -------------------------------------------------
-    def mpo_Ising(self):
+    def mpo_Ising(self, long: str = "Z", trans: str = "X"):
         """
         mpo_Ising
 
         This function defines the MPO for the 1D transverse field Ising model.
         It takes the same MPO for all sites.
 
         """
         I = np.eye(2)
         O = np.zeros((2, 2))
-        X = np.array([[0, 1], [1, 0]])
-        Z = np.array([[1, 0], [0, -1]])
+        if long == "Z":
+            long_op = sparse_pauli_z(n=0, L=1).toarray()
+            trans_op = sparse_pauli_x(n=0, L=1).toarray()
+        elif long == "X":
+            long_op = sparse_pauli_x(n=0, L=1).toarray()
+            trans_op = sparse_pauli_z(n=0, L=1).toarray()
+
         w_tot = []
-        for _ in range(self.L):
+        for i in range(self.L):
+            if i == 0 or i == 1:
+                c = 1
+            else:
+                c = 0
             w = np.array(
-                [[I, -self.J * Z, -self.h * X - self.eps * X], [O, O, Z], [O, O, I]]
+                [[I, -self.J * long_op, -self.h * trans_op - self.eps * c * (long_op - I)], [O, O, long_op], [O, O, I]]
             )
             w_tot.append(w)
         self.w = w_tot
         return self
     
-    def mpo_ANNNI(self):
+    def mpo_ANNNI(self, long: str = "X", trans: str = "Z", deg_method: int = 2):
         """
         mpo_ANNNI
 
         This function defines the MPO for the 1D Axial Next-Nearest Neighbor Interaction model.
-        It takes the same MPO for all sites.
+        It takes the same MPO for all sites apart from a correction term to break degeneracy.
 
         """
         I = identity(2, dtype=complex).toarray()
         O = csc_array((2, 2), dtype=complex).toarray()
-        X = sparse_pauli_x(n=0, L=1).toarray()
-        Z = sparse_pauli_z(n=0, L=1).toarray()
+        if long == "Z":
+            long_op = sparse_pauli_z(n=0, L=1).toarray()
+            trans_op = sparse_pauli_x(n=0, L=1).toarray()
+        elif long == "X":
+            long_op = sparse_pauli_x(n=0, L=1).toarray()
+            trans_op = sparse_pauli_z(n=0, L=1).toarray()
+
         w_tot = []
-        for _ in range(self.L):
+        for i in range(self.L):
+            if deg_method == 1:
+                if i == 0 or i == 1:
+                    c = 1
+                else:
+                    c = 0
+                c_i = c
+            elif deg_method == 2:
+                c = (1 + (-1)**(i // 2))
+                c_i = 1
+
             w = np.array(
-                [[I, X, O, (-self.h * self.J) * Z], 
-                 [O, O, I, -self.J * X], 
-                 [O, O, O, (self.k * self.J) * X], 
+                [[I, long_op, O, - (self.h * self.J) * trans_op - (self.eps * self.J * c) * long_op + (self.eps * self.J * c_i) * I], 
+                 [O, O, I, - (self.J) * long_op], 
+                 [O, O, O, (self.k * self.J) * long_op], 
                  [O, O, O, I]]
             )
             w_tot.append(w)
         self.w = w_tot
         return self
 
-    def mpo_Cluster(self):
+    def mpo_Cluster(self, long: str = "X", trans: str = "Z", eps: float=1e-5):
         """
         mpo_Cluster
 
-        This function defines the MPO for the 1D Axial Next-Nearest Neighbor Interaction model.
+        This function defines the MPO for the 1D Cluster model.
         It takes the same MPO for all sites.
 
         """
         I = identity(2, dtype=complex).toarray()
         O = csc_array((2, 2), dtype=complex).toarray()
-        X = sparse_pauli_x(n=0, L=1).toarray()
-        Z = sparse_pauli_z(n=0, L=1).toarray()
+        if long == "Z":
+            long_op = sparse_pauli_z(n=0, L=1).toarray()
+            trans_op = sparse_pauli_x(n=0, L=1).toarray()
+        elif long == "X":
+            long_op = sparse_pauli_x(n=0, L=1).toarray()
+            trans_op = sparse_pauli_z(n=0, L=1).toarray()
         w_tot = []
-        for _ in range(self.L):
+
+        for i in range(self.L):
+            if i == 0:
+                c = -eps
+            else:
+                c = 0
+
             w = np.array(
-                [[I, Z, O, (-self.h / self.J) * X], 
-                 [O, O, X, O], 
-                 [O, O, O, Z], 
+                [[I, long_op, O, -self.h * trans_op + c * long_op],
+                 [O, O, trans_op, O],
+                 [O, O, O, -self.J * long_op],
                  [O, O, O, I]]
             )
             w_tot.append(w)
         self.w = w_tot
         return self
 
+    def mpo_Cluster_xy(self, long: str="X", eps: float=1e-5):
+        """
+        mpo_Cluster
+
+        This function defines the MPO for the 1D Cluster model.
+        It takes the same MPO for all sites.
+
+        """
+        I = identity(2, dtype=complex).toarray()
+        O = csc_array((2, 2), dtype=complex).toarray()
+        Y = sparse_pauli_y(n=0, L=1).toarray()
+        if long == "Z":
+            long_op = sparse_pauli_z(n=0, L=1).toarray()
+            trans_op = sparse_pauli_x(n=0, L=1).toarray()
+        elif long == "X":
+            long_op = sparse_pauli_x(n=0, L=1).toarray()
+            trans_op = sparse_pauli_z(n=0, L=1).toarray()
+        w_tot = []
+
+        for i in range(self.L):
+            if i == 0:
+                c = -eps
+            else:
+                c = 0
 
+            w = np.array(
+                [[I, long_op, O, Y, -self.h * trans_op + c * long_op],
+                 [O, O, trans_op, O, self.lx * long_op],
+                 [O, O, O, O, -self.J * long_op],
+                 [O, O, O, O, self.ly * Y],
+                 [O, O, O, O, I]]
+            )
+            w_tot.append(w)
+        self.w = w_tot
+        return self
+    
+    def mpo_xxz(self, long: str="X", eps: float=1e-5):
+        """
+        mpo_Cluster
+
+        This function defines the MPO for the 1D Cluster model.
+        It takes the same MPO for all sites.
+
+        """
+        I = identity(2, dtype=complex).toarray()
+        O = csc_array((2, 2), dtype=complex).toarray()
+        Y = sparse_pauli_y(n=0, L=1).toarray()
+        if long == "Z":
+            long_op = sparse_pauli_z(n=0, L=1).toarray()
+            trans_op = sparse_pauli_x(n=0, L=1).toarray()
+        elif long == "X":
+            long_op = sparse_pauli_x(n=0, L=1).toarray()
+            trans_op = sparse_pauli_z(n=0, L=1).toarray()
+        w_tot = []
+
+        for i in range(self.L):
+            if i == 0:
+                c = -eps
+            else:
+                c = 0
+
+            w = np.array(
+                [[I, long_op, Y, trans_op, -self.h * trans_op + c * long_op],
+                 [O, O, O, O, -self.J * long_op],
+                 [O, O, O, O, -self.J * Y],
+                 [O, O, O, O, -self.J * self.k * trans_op],
+                 [O, O, O, O, I]]
+            )
+            w_tot.append(w)
+        self.w = w_tot
+        return self
+    
     def mpo_quench(
         self,
         quench: str,
         delta: float = None,
         h_ev: float = None,
         J_ev: float = 1,
         sites: list = -1,
@@ -815,15 +981,15 @@
                 [
                     [I, O, alpha * X, O],
                     [O, O, O, O],
                     [
                         O,
                         O,
                         beta * X,
-                        gamma * X @ (np.linalg.matrix_power(X, (1 - alpha))),
+                        gamma * X @ (la.matrix_power(X, (1 - alpha))),
                     ],
                     [O, O, O, I],
                 ]
             )
             w_tot.append(w)
         self.w = w_tot
         return self
@@ -865,114 +1031,70 @@
         """
         if self.model == "Ising":
             self.single_operator_Ising(site=site, op=op)
 
         elif self.model == "ANNNI":
             self.single_operator_ANNNI(site=site)
 
-        elif self.model == "Z2_two_ladder":
-            self.sigma_x_Z2_two_ladder()
-
         elif self.model == "Z2_dual":
             self.single_operator_Z2_dual(site=site, l=op)
 
         return self
 
-    def sigma_x_Z2_one_ladder(self, site):
-        I = np.eye(2)
-        O = np.zeros((2, 2))
-        X = np.array([[0, 1], [1, 0]])
-        w_tot = []
-        for i in range(self.L):
-            if i == site - 1:
-                alpha = 1
-            else:
-                alpha = 0
-            w_mag = np.array(
-                [[I, O, O, alpha * X], [O, O, O, O], [O, O, O, O], [O, O, O, I]]
-            )
-            w_tot.append(w_mag)
-        self.w = w_tot
-        return self
-
-    def sigma_x_Z2_two_ladder(self, site, ladder):
-        I = np.eye(2)
-        O = np.zeros((2, 2))
-        X = np.array([[0, 1], [1, 0]])
-        if ladder == 1:
-            X = np.kron(X, I)
-        elif ladder == 2:
-            X = np.kron(I, X)
-        I = np.kron(I, I)
-        O = np.kron(O, O)
-        w_tot = []
-        for i in range(self.L):
-            if i == site - 1:
-                alpha = 1
-            else:
-                alpha = 0
-            w_mag = np.array(
-                [
-                    [I, O, O, O, O, O, alpha * X],
-                    [O, O, O, O, O, O, O],
-                    [O, O, O, O, O, O, O],
-                    [O, O, O, O, O, O, O],
-                    [O, O, O, O, O, O, O],
-                    [O, O, O, O, O, O, O],
-                    [O, O, O, O, O, O, I],
-                ]
-            )
-            w_tot.append(w_mag)
-        self.w = w_tot
-        return self
-
-    def single_operator_Ising(self, site, op: np.ndarray=None):
+    def single_operator_Ising(self, site, long: str="X"):
         """
         single_operator_Ising
 
         This function computes a local operator (op) for the 1D Ising model
         on a certain arbitrary site.
 
         site: int - local site where the operator acts
         op: np.ndarray - operator acting on the local site
 
         """
-        I = np.eye(2)
-        O = np.zeros((2, 2))
+        I = identity(2, dtype=complex).toarray()
+        O = csc_array((2, 2), dtype=complex).toarray()
+        if long == "Z":
+            long_op = sparse_pauli_z(n=0, L=1).toarray()
+        elif long == "X":
+            long_op = sparse_pauli_x(n=0, L=1).toarray()
         w_tot = []
+        w_init = np.array([[I, O], [O, I]])
         for i in range(self.L):
+            w_mag = w_init
             if i == site - 1:
-                alpha = 1
-            else:
-                alpha = 0
-            w_mag = np.array([[I, O, alpha * op], [O, O, O], [O, O, I]])
+                w_mag[0,-1] = long_op
+        
             w_tot.append(w_mag)
         self.w = w_tot
         return self
     
-    def single_operator_ANNNI(self, site):
+    def single_operator_ANNNI(self, site, long: str="X"):
         """
         single_operator_Ising
 
         This function computes a local operator (op) for the 1D Ising model
         on a certain arbitrary site.
 
         site: int - local site where the operator acts
         op: np.ndarray - operator acting on the local site
 
         """
-        I = np.eye(2)
-        O = np.zeros((2, 2))
-        Z = sparse_pauli_z(n=0, L=1).toarray()
+        I = identity(2, dtype=complex).toarray()
+        O = csc_array((2, 2), dtype=complex).toarray()
+        if long == "Z":
+            long_op = sparse_pauli_z(n=0, L=1).toarray()
+        elif long == "X":
+            long_op = sparse_pauli_x(n=0, L=1).toarray()
         w_tot = []
         w_init = np.array([[I, O], [O, I]])
         for i in range(self.L):
             w_mag = w_init
             if i == site - 1:
-                w_mag[0,-1] = Z
+                w_mag[0,-1] = long_op
         
             w_tot.append(w_mag)
         self.w = w_tot
         return self
 
     def single_operator_Z2_dual(self, site, l):
         """
@@ -990,15 +1112,15 @@
         chain = []
         self.clear_envs()
         for i in range(1, self.L + 1):
             self.single_operator_Ising(site=i, op=op)
             self.envs(site=i)
             chain.append(self.braket(site=i))
         self.clear_envs()
-        return chain 
+        return chain
 
     def electric_field_Z2(self, E):
         """
         electric_field_Z2
 
         This function finds the mpo for the electric field in the direct lattice of a Z2 theory.
         To reconstruct the field in the direct lattices we need functions to compute the 
@@ -1045,56 +1167,29 @@
                 coeff = self.Z2.charge_coeff_interaction(n=l+1,mpo_site=mpo_site)
                 self.w = self.Z2.mpo.copy()
                 E_h.append(coeff * self.mpo_first_moment().real)
             E_h.append(E[(l*2+1), -1])
             E[(l*2+1), 2::2] = E_h
         
         return E
-    
-    def corr_test(self, E, mpo_site):
+
+    def connected_correlator(self, site, lad):
         """
-        electric_field_Z2
+        connected_correlator
 
-        This function finds the mpo for the electric field in the direct lattice of a Z2 theory.
-        To reconstruct the field in the direct lattices we need functions to compute the 
-        borders and the bulk fields, weighted for the appropriate charges.
+        This function computes the correlator between a reference link
+        and all the others links in the whole column of our ladder system.
+        The reference link is located at a certain site and ladder.
+        The correlator is connected because we subtract the expecation values
+        of the two links we are referring to. E.g. <E_ref,E_r> - <E_ref><E_r>
 
-        """
-        # let us find the observables for the boudary fields    
-        for l in [0,self.Z2.l-1]:
-            self.Z2.local_observable_Z2_dual(mpo_site=mpo_site, l=l)
-            coeff = self.Z2.charge_coeff_v(mpo_site=mpo_site, l=l)
-            self.w = self.Z2.mpo.copy()
-            E[(l+j)*2,mpo_site*2+1] = coeff * self.mpo_first_moment().real
-            # E[(l+j)*2,mpo_site*2+1] = self.mpo_first_moment().real
-            j = 1
-            
-        # now we can obtain the bulk values given by the zz interactions
-        # vertical
-        for l in range(self.Z2.l-1):
-            E_v = []
-            for mpo_site in range(self.Z2.L-1):
-                self.Z2.zz_observable_Z2_dual(mpo_site=mpo_site, l=l, direction="vertical")
-                self.w = self.Z2.mpo.copy()
-                E_v.append(self.mpo_first_moment().real)
-            E[(l+1)*2, 1::2] = E_v
-        # horizontal
-        for l in range(self.Z2.l):
-            E_h = []
-            for mpo_site in range(self.Z2.L-2):
-                self.Z2.zz_observable_Z2_dual(mpo_site=mpo_site, l=l, direction="horizontal")
-                coeff = self.Z2.charge_coeff_interaction(n=l+1,mpo_site=mpo_site)
-                self.w = self.Z2.mpo.copy()
-                E_h.append(coeff * self.mpo_first_moment().real)
-            E_h.append(E[(l*2+1), -1])
-            E[(l*2+1), 2::2] = E_h
-        
-        return E
+        site: int - site we will use for the vertical section of the ladder system
+        lad: int - It refers to the upper link of a ladder we use as reference
 
-    def connected_correlator(self, site, lad):
+        """
         E_corr = []
         # find the exp val for the reference link
         self.Z2.zz_observable_Z2_dual(mpo_site=site, l=lad-1, direction="vertical")
         self.w = self.Z2.mpo.copy()
         E_lad = self.mpo_first_moment().real
         print(f"E_0: {E_lad}")
         for link in range(self.Z2.l+1):
@@ -1125,14 +1220,75 @@
             E_lad_r = self.mpo_first_moment().real
             print(f"E_0-r: {E_lad_r}")
 
             E_corr.append(E_lad_r - (E_lad * E_r))
             print(E_lad_r - (E_lad * E_r))
 
         return E_corr
+    
+    def electric_energy_density_Z2(self, site):
+        """
+        electric_energy_density_Z2
+
+        This function computes the electric energy density for the Z2 model
+        in the whole column of our ladder system.
+        The column is located at a certain site.
+        We can have a "connected" energy density if we subtract the expecation values
+        of the plaquettes we are referring to with the expectation values of the vacuum state. 
+        E.g. <q,q'|el_en_density|q,q'> - <0|el_en_density|0> (we do not do that here)
+
+        site: int - site we will use for the vertical section of the ladder system
+        lad: int - It refers to the upper link of a ladder we use as reference
+
+        """
+        E_en_density = []
+        for lad in range(self.Z2.l):
+            if lad in [0, self.Z2.l-1]:
+                if lad == 0:
+                    l = lad
+                    # find the sigma_4^x first
+                    self.Z2.zz_observable_Z2_dual(mpo_site=site, l=l, direction="vertical")
+                    self.w += [(self.h / 2) * mpo for mpo in self.Z2.mpo].copy()
+                elif lad == self.Z2.l-1:
+                    l = lad    
+                    # find the sigma_2^x last
+                    self.Z2.zz_observable_Z2_dual(mpo_site=site, l=l-1, direction="vertical")
+                    self.w += [(self.h / 2) * mpo for mpo in self.Z2.mpo].copy()
+                # find the sigma_2^x first or sigma_4^x last
+                self.Z2.local_observable_Z2_dual(mpo_site=site, l=l)
+                coeff = self.Z2.charge_coeff_v(mpo_site=site, l=l)
+                self.w += [(self.h * coeff) * mpo for mpo in self.Z2.mpo].copy() # times 2 because we do not share this link with any other plaquette
+                
+            else:
+                l = lad - 1
+                # find the sigma_2^x
+                self.Z2.zz_observable_Z2_dual(mpo_site=site, l=l, direction="vertical")
+                self.w += [(self.h / 2) * mpo for mpo in self.Z2.mpo].copy()
+                # find the sigma_4^x
+                self.Z2.zz_observable_Z2_dual(mpo_site=site, l=l+1, direction="vertical")
+                self.w += [(self.h / 2) * mpo for mpo in self.Z2.mpo].copy()
+
+
+            # find the sigma_1^x
+            self.Z2.zz_observable_Z2_dual(mpo_site=site, l=lad, direction="horizontal")
+            coeff = self.Z2.charge_coeff_interaction(n=lad+1,mpo_site=site)
+            self.w += [(self.h / 2) * coeff * mpo for mpo in self.Z2.mpo].copy()
+            # find the sigma_3^x
+            self.Z2.zz_observable_Z2_dual(mpo_site=site+1, l=lad, direction="horizontal")
+            coeff = self.Z2.charge_coeff_interaction(n=lad+1,mpo_site=site+1)
+            self.w += [(self.h / 2) * coeff * mpo for mpo in self.Z2.mpo].copy()
+            mpo_split = np.array_split(np.asarray(self.w), self.L)
+            mpo_summed = np.sum(mpo_split, axis=1)
+            self.w = mpo_summed
+            eed = self.mpo_first_moment().real
+            print(f"Electric energy density: {eed}")
+
+            E_en_density.append(eed)
+
+        return E_en_density
 
     # -------------------------------------------------
     # Manipulation of MPOs
     # -------------------------------------------------
     def mpo_dagger(self):
         w_tot = []
         for w in self.w:
@@ -1367,38 +1523,38 @@
 
         This function contracts the left and right environments with the class mpos self.w
         and self.w_2. Then, we reshape the effective Hamiltonian as a matrix.
 
         site: int - site to optimize
 
         """
-        H_eff_time = time.perf_counter()
+        # H_eff_time = time.perf_counter()
         H = ncon(
             [self.env_left[-1], self.w[site - 1]],
             [
                 [-1, 1, -5],
                 [1, -3, -2, -4],
             ]
         )
         H = ncon(
             [H, self.env_right[-1]],
             [
                 [-1, -2, 1, -5, -4],
                 [-3 , 1, -6]
             ]
         )
-        print(f"Time of H_eff contraction: {time.perf_counter()-H_eff_time}")
+        # print(f"Time of H_eff contraction: {time.perf_counter()-H_eff_time}")
 
-        reshape_time = time.perf_counter()
+        # reshape_time = time.perf_counter()
         H = H.reshape(
             self.env_left[-1].shape[0] * self.d * self.env_right[-1].shape[0],
             self.env_left[-1].shape[2] * self.d * self.env_right[-1].shape[2],
         )
-        print(f"Time of H_eff reshaping: {time.perf_counter()-reshape_time}")
-        print(H.shape)
+        # print(f"Time of H_eff reshaping: {time.perf_counter()-reshape_time}")
+        # print(H.shape)
 
         return H
 
     def eigensolver(self, site: int=None, v0: np.ndarray=None, H_eff: np.ndarray=None,):
         """
         eigensolver
 
@@ -1415,29 +1571,31 @@
         """
         # time_eig = time.perf_counter()
         A = TensorMultiplierOperator((
                             self.env_left[-1].shape[0] * self.d * self.env_right[-1].shape[0],
                             self.env_left[-1].shape[2] * self.d * self.env_right[-1].shape[2],
                             ), matvec=self.mv, dtype=np.complex128)
         # print(f"shape of A: {A.shape}")
-        # if A.shape[0] == 2:
-        #     H = self.H_eff(site=site)
-        #     e, v = eigsh(H, k=1, v0=v0)
-        # else:
-        e, v = eigs(A, k=1, v0=v0)
+        if A.shape[0] == 2:
+            H = self.H_eff(site=self.site)
+            e, v = la.eigh(H)
+        else:
+            v0 = self.sites[self.site - 1]
+            # print(f"v0 at site {self.site - 1} has shape: {v0.shape}")
+            e, v = spla.eigsh(A, k=1, v0=v0, which='SA')
         # e, v = eigsh(H_eff, k=1, which="SA", v0=v0)
         # np.savetxt(
         #     f"/Users/fradm/mps/results/times_data/eigsh_eigensolver_site_{site}_h_{self.h:.2f}",
         #     [time.perf_counter() - time_eig],
         # )
         # print(f"Time of eigsh during eigensolver for site {site}: {time.perf_counter()-time_eig}")
         e_min = e[0].real
         eigvec = np.array(v[:,0])
 
-        self.sites[site - 1] = eigvec.reshape(
+        self.sites[self.site - 1] = eigvec.reshape(
             self.env_left[-1].shape[0], self.d, self.env_right[-1].shape[0]
         )
         return e_min
 
     def update_state(
         self,
         sweep: str,
@@ -1462,26 +1620,26 @@
 
         """
         if sweep == "right":
             # we want to write M (left,d,right) in LFC -> (left*d,right)
             m = self.sites[site - 1].reshape(
                 self.env_left[-1].shape[2] * self.d, self.env_right[-1].shape[2]
             )
-            u, s, v = np.linalg.svd(m, full_matrices=False)
+            u, s, v = la.svd(m, full_matrices=False)
             if trunc_tol:
                 condition = s >= schmidt_tol
                 s_trunc = np.extract(condition, s)
-                s = s_trunc / np.linalg.norm(s_trunc)
+                s = s_trunc / la.norm(s_trunc)
                 bond_l = u.shape[0] // self.d
                 u = u.reshape(bond_l, self.d, u.shape[1])
                 u = u[:, :, : len(s)]
                 v = v[: len(s), :]
             elif trunc_chi:
                 s_trunc = s[: self.chi]
-                s = s_trunc / np.linalg.norm(s_trunc)
+                s = s_trunc / la.norm(s_trunc)
                 bond_l = u.shape[0] // self.d
                 u = u.reshape(bond_l, self.d, u.shape[1])
                 u = u[:, :, : len(s)]
                 v = v[: len(s), :]
             else:
                 u = u.reshape(
                     self.env_left[-1].shape[2], self.d, self.env_right[-1].shape[2]
@@ -1498,26 +1656,26 @@
             self.sites[site] = next_site
 
         elif sweep == "left":
             # we want to write M (left,d,right) in RFC -> (left,d*right)
             m = self.sites[site - 1].reshape(
                 self.env_left[-1].shape[2], self.d * self.env_right[-1].shape[2]
             )
-            u, s, v = np.linalg.svd(m, full_matrices=False)
+            u, s, v = la.svd(m, full_matrices=False)
             if trunc_tol:
                 condition = s >= schmidt_tol
                 s_trunc = np.extract(condition, s)
-                s = s_trunc / np.linalg.norm(s_trunc)
+                s = s_trunc / la.norm(s_trunc)
                 bond_r = v.shape[1] // self.d
                 v = v.reshape(v.shape[0], self.d, bond_r)
                 v = v[: len(s), :, :]
                 u = u[:, : len(s)]
             elif trunc_chi:
                 s_trunc = s[: self.chi]
-                s = s_trunc / np.linalg.norm(s_trunc)
+                s = s_trunc / la.norm(s_trunc)
                 bond_r = v.shape[1] // self.d
                 v = v.reshape(v.shape[0], self.d, bond_r)
                 v = v[: len(s), :, :]
                 u = u[:, : len(s)]
             else:
                 v = v.reshape(
                     self.env_left[-1].shape[2], self.d, self.env_right[-1].shape[2]
@@ -1603,43 +1761,47 @@
         res = res.flatten()
         return res
 
     def DMRG(
         self,
         trunc_tol: bool,
         trunc_chi: bool,
+        long: str="X",
+        trans: str="Z",
         schmidt_tol: float = 1e-15,
         conv_tol: float = 1e-10,
         n_sweeps: int = 2,
         bond: bool = True,
         where: int = -1,
     ):
         energies = []
         sweeps = ["right", "left"]
         sites = np.arange(1, self.L + 1).tolist()
 
-        self.mpo()
+        self.mpo(long=long, trans=trans)
         self.envs()
 
         iter = 1
-        
+        H = None
+
         t_start = time.perf_counter()
         for n in range(n_sweeps):
             print(f"Sweep n: {n}\n")
             entropy = []
             schmidt_vals = []
             for i in range(self.L - 1):
                 # print(f"Site: {sites[i]}\n")
-                v0 = self.sites[i].flatten()
                 # t_start = time.perf_counter()
-                # H = self.H_eff(sites[i])
+                if trunc_tol == True:
+                    H = self.H_eff(sites[i])
                 # print(f"Time effective Ham: {abs(time.perf_counter()-t_start)}")
                 # t_start = time.perf_counter()
+                v0 = self.sites[i].flatten()
                 self.site = sites[i]
-                energy = self.eigensolver(site=sites[i], v0=v0) # , v0=v0
+                energy = self.eigensolver(site=sites[i], v0=v0, H_eff=H) # , v0=v0
                 # energy = self.eigensolver(H_eff=H, site=sites[i], v0=v0) # , v0=v0
                 # print(f"Time eigensolver: {abs(time.perf_counter()-t_start)}")
                 energies.append(energy)
                 # t_start = time.perf_counter()
                 s = self.update_state(
                     sweeps[0], sites[i], trunc_tol, trunc_chi, schmidt_tol
                 )
@@ -1656,42 +1818,43 @@
 
                 # t_start = time.perf_counter()
                 self.update_envs(sweeps[0], sites[i])
                 # print(f"Time update envs: {abs(time.perf_counter()-t_start)}")
                 iter += 1
 
             if ((n % 2) - 1) == 0:
-                energy_dist = np.abs(energies[-1] - energies[-2])
+                energy_dist = np.abs(energies[-1] - energies[-2])/energies[-1]
                 if energy_dist < conv_tol:
                     break
             
             # print("reversing the sweep")
             sweeps.reverse()
             sites.reverse()
 
+        t_dmrg = abs(time.perf_counter()-t_start)
         if energy_dist < conv_tol:
             print("##############################")
             print(
                 f"The energy between the two last updated states converged\n"
                 + f"to an order of {conv_tol} after:\n"
                 + f"{n} sweeps at site {sites[i]}\n"
                 + f"total iterations {iter}\n"
-                + f"total time: {abs(time.perf_counter()-t_start)}"
+                + f"total time: {t_dmrg}"
             )
             print("##############################")
         else:
             print("##############################")
             print(
                 f"The energy between the two last updated states converged\n"
                 + f"to an order of {energy_dist}\n"
                 + f"instead of the convergence tolerance {conv_tol}\n"
-                + f"total time: {abs(time.perf_counter()-t_start)}"
+                + f"total time: {t_dmrg}"
             )
             print("##############################")
-        return energies, entropy, schmidt_vals
+        return energies, entropy, schmidt_vals, t_dmrg
 
     def environments_ev(self, site):
         a = np.array([1])
         E_l = ncon([a, a], [[-1], [-2]])
         E_r = E_l
         env_right = []
         env_left = []
@@ -1789,34 +1952,34 @@
         """
         s_mid = 0
         if sweep == "right":
             # we want to write M (left,d,right) in LFC -> (left*d,right)
             m = self.sites[site - 1].reshape(
                 self.sites[site - 1].shape[0] * self.d, self.sites[site - 1].shape[2]
             )
-            u, s, v = np.linalg.svd(m, full_matrices=False)
+            u, s, v = la.svd(m, full_matrices=False)
 
             if trunc_tol:
                 condition = s >= schmidt_tol
                 s_trunc = np.extract(condition, s)
-                s = s_trunc / np.linalg.norm(s_trunc)
+                s = s_trunc / la.norm(s_trunc)
                 bond_l = u.shape[0] // self.d
                 u = u.reshape(bond_l, self.d, u.shape[1])
                 u = u[:, :, : len(s)]
                 v = v[: len(s), :]
                 if site == self.L // 2:
                     # print(f'Schmidt values:\n{s}')
                     s_mid = s
                     # np.savetxt(
                     #     f"/Users/fradm/Google Drive/My Drive/projects/0_ISING/results/bonds_data/schmidt_values_middle_chain_{self.model}_flip_{flip}_L_{self.L}_chi_{self.chi}_trotter_step_{trotter_step}_delta_{delta}",
                     #     s,
                     # )
             elif trunc_chi:
                 s_trunc = s[: self.chi]
-                s = s / np.linalg.norm(s_trunc)
+                s = s / la.norm(s_trunc)
                 bond_l = u.shape[0] // self.d
                 u = u.reshape(bond_l, self.d, u.shape[1])
                 u = u[:, :, : len(s)]
                 v = v[: len(s), :]
                 if site == self.L // 2:
                     s_mid = s
                     # print(f'Schmidt values:\n{s}')
@@ -1842,34 +2005,34 @@
             self.sites[site] = next_site
 
         elif sweep == "left":
             # we want to write M (left,d,right) in RFC -> (left,d*right)
             m = self.sites[site - 1].reshape(
                 self.sites[site - 1].shape[0], self.d * self.sites[site - 1].shape[2]
             )
-            u, s, v = np.linalg.svd(m, full_matrices=False)
+            u, s, v = la.svd(m, full_matrices=False)
 
             if trunc_tol:
                 condition = s >= schmidt_tol
                 s_trunc = np.extract(condition, s)
-                s = s_trunc / np.linalg.norm(s_trunc)
+                s = s_trunc / la.norm(s_trunc)
                 bond_r = v.shape[1] // self.d
                 v = v.reshape(v.shape[0], self.d, bond_r)
                 v = v[: len(s), :, :]
                 u = u[:, : len(s)]
                 if site == self.L // 2:
                     s_mid = s
                     # print(f'Schmidt values:\n{s}')
                     # np.savetxt(
                     #     f"/Users/fradm/Google Drive/My Drive/projects/0_ISING/results/bonds_data/schmidt_values_middle_chain_{self.model}_flip_{flip}_L_{self.L}_chi_{self.chi}_trotter_step_{trotter_step}_delta_{delta}",
                     #     s,
                     # )
             elif trunc_chi:
                 s_trunc = s[: self.chi]
-                s = s / np.linalg.norm(s_trunc)
+                s = s / la.norm(s_trunc)
                 # print(f"Schmidt Values:\n{s}")
                 bond_r = v.shape[1] // self.d
                 v = v.reshape(v.shape[0], self.d, bond_r)
                 v = v[: len(s), :, :]
                 u = u[:, : len(s)]
                 if site == self.L // 2:
                     s_mid = s
@@ -2273,27 +2436,28 @@
         sites = [1,2,3,4]
         ladders = [2,3]
         errors = [[0, 0]]
         entropies = [0]
 
         self.enlarge_chi()
 
+
         # electric field
         E_h = np.zeros((2*self.Z2.l+1,2*self.Z2.L-1))
         E_h[:] = np.nan
         E_h = self.electric_field_Z2(E_h)
 
         # local dual mag
         self.order_param()
         mag = self.mpo_first_moment().real/(len(self.Z2.latt.plaquettes()) - (2 * (self.Z2.L-1) + 2 * (self.Z2.l-2)))
         
-        # # wilson loop
-        # self.Z2.wilson_Z2_dual(mpo_sites=sites, ls=ladders) #list(range(s))
-        # self.w = self.Z2.mpo.copy()
-        # loop = self.mpo_first_moment().real
+        # wilson loop
+        self.Z2.wilson_Z2_dual(mpo_sites=sites, ls=ladders) #list(range(s))
+        self.w = self.Z2.mpo.copy()
+        loop = self.mpo_first_moment().real
 
         # t'hooft string
         self.Z2.thooft(site=[2], l=[2], direction="horizontal")
         self.w = self.Z2.mpo.copy()
         thooft = self.mpo_first_moment().real
 
         E.append(E_h)
@@ -2341,27 +2505,27 @@
             E_h[:] = np.nan
             E_h = self.electric_field_Z2(E_h)
 
             # local dual mag
             self.order_param()
             mag = self.mpo_first_moment().real/(len(self.Z2.latt.plaquettes()) - (2 * (self.Z2.L-1) + 2 * (self.Z2.l-2)))
             
-            # # wilson loop
-            # self.Z2.wilson_Z2_dual(mpo_sites=sites, ls=ladders) #list(range(s))
-            # self.w = self.Z2.mpo.copy()
-            # loop = self.mpo_first_moment().real
+            # wilson loop
+            self.Z2.wilson_Z2_dual(mpo_sites=sites, ls=ladders) #list(range(s))
+            self.w = self.Z2.mpo.copy()
+            loop = self.mpo_first_moment().real
 
             # t'hooft string
             self.Z2.thooft(site=[2], l=[2], direction="horizontal")
             self.w = self.Z2.mpo.copy()
             thooft = self.mpo_first_moment().real
 
             E.append(E_h)
             M.append(mag)
-            # W.append(loop)
+            W.append(loop)
             S.append(thooft)
             errors.append(error)
             entropies.append(entropy)
 
 
         return (
             E,
@@ -2476,17 +2640,15 @@
                 bra[site - 1].conjugate(),
                 env_right[-1],
             ],
             [[1, 4, 7], [1, 3, 2], [4, 5, 3, 6], [7, 6, 8], [2, 5, 8]],
         )
         return sandwich
 
-    def mpo_first_moment(self, site=1, ancilla=False, mixed=False):
-        # self.order_param()
-        # self.sigma_x_Z2(site=site)
+    def mpo_first_moment(self, site: int=1, ancilla: bool=False, mixed: bool=False):
         self.clear_envs()
         self.envs(site, ancilla=ancilla, mixed=mixed)
         sites = self.sites
         ancilla_sites = sites
         if ancilla:
             sites = self.ancilla_sites
             ancilla_sites = sites
@@ -2601,20 +2763,26 @@
 
         This function saves the sites, e.g., the tensors composing our MPS.
         In order to do that we need to flatten the whole list of tensors and save
         their original shapes in order to reshape them in the loading step.
 
         precision: int - indicates the precision of the variable h
         """
-        if "Ising" in self.model:
+        if "Ising" == self.model:
+            self.save_sites_Ising(path=path, precision=precision)
+        elif "Cluster" == self.model:
             self.save_sites_Ising(path=path, precision=precision)
-        elif "ANNNI" in self.model:
+        elif "Cluster-XY" == self.model:
+            self.save_sites_Cluster_xy(path=path, precision=precision)
+        elif "ANNNI" == self.model:
             self.save_sites_ANNNI(path=path, precision=precision)
         elif "Z2" in self.model:
             self.save_sites_Z2(path=path, precision=precision, cx=cx, cy=cy)
+        elif "XXZ" in self.model:
+            self.save_sites_XXZ(path=path, precision=precision)
         else:
             raise ValueError("Choose a correct model")
         return self
     
     def load_sites(self, path: str, precision: int=2, cx: list=None, cy: list=None):
         """
         load_sites
@@ -2622,46 +2790,67 @@
         This function load the tensors into the sites of the MPS.
         We fetch a completely flat list, split it to recover the original tensors
         (but still flat) and reshape each of them accordingly with the saved shapes.
         To initially split the list in the correct index position refer to the auxiliary
         function get_labels().
 
         """
-        if "Ising" in self.model:
+        if "Ising" == self.model:
             self.load_sites_Ising(path=path, precision=precision)
-        elif "ANNNI" in self.model:
+        elif "ANNNI" == self.model:
             self.load_sites_ANNNI(path=path, precision=precision)
-        if "Cluster" in self.model:
+        elif "Cluster" == self.model:
             self.load_sites_Ising(path=path, precision=precision)
+        elif "Cluster-XY" == self.model:
+            self.load_sites_Cluster_xy(path=path, precision=precision)
         elif "Z2" in self.model:
             self.load_sites_Z2(path=path, precision=precision, cx=cx, cy=cy)
+        elif "XXZ" in self.model:
+            self.load_sites_XXZ(path=path, precision=precision)
         else:
             raise ValueError("Choose a correct model")
         return self
 
     def save_sites_Ising(self, path, precision: int=2):
         # shapes of the tensors
-        shapes = tensor_shapes(self.sites)
+        shapes = tensor_shapes(self.sites, False)
         np.savetxt(
             f"{path}/results/tensors/shapes_sites_{self.model}_L_{self.L}_chi_{self.chi}_h_{self.h:.{precision}f}_J_{self.J:.{precision}f}",
             shapes,
             fmt="%1.i",  # , delimiter=','
         )
 
         # flattening of the tensors
         tensor = [element for site in self.sites for element in site.flatten()]
         np.savetxt(
             f"{path}/results/tensors/tensor_sites_{self.model}_L_{self.L}_chi_{self.chi}_h_{self.h:.{precision}f}_J_{self.J:.{precision}f}",
             tensor,
         )
         return self
     
+    def save_sites_Cluster_xy(self, path, precision: int=2):
+        # shapes of the tensors
+        shapes = tensor_shapes(self.sites, False)
+        np.savetxt(
+            f"{path}/results/tensors/shapes_sites_{self.model}_L_{self.L}_chi_{self.chi}_h_{self.h:.{precision}f}_lx_{self.lx:.{precision}f}_ly_{self.ly:.{precision}f}_J_{self.J:.{precision}f}",
+            shapes,
+            fmt="%1.i",  # , delimiter=','
+        )
+
+        # flattening of the tensors
+        tensor = [element for site in self.sites for element in site.flatten()]
+        np.savetxt(
+            f"{path}/results/tensors/tensor_sites_{self.model}_L_{self.L}_chi_{self.chi}_h_{self.h:.{precision}f}_lx_{self.lx:.{precision}f}_ly_{self.ly:.{precision}f}_J_{self.J:.{precision}f}",
+            tensor,
+        )
+        return self
+    
     def save_sites_ANNNI(self, path, precision: int=2):
         # shapes of the tensors
-        shapes = tensor_shapes(self.sites)
+        shapes = tensor_shapes(self.sites, False)
         np.savetxt(
             f"{path}/results/tensors/shapes_sites_{self.model}_L_{self.L}_chi_{self.chi}_h_{self.h:.{precision}f}_k_{self.k:.{precision}f}",
             shapes,
             fmt="%1.i",  # , delimiter=','
         )
 
         # flattening of the tensors
@@ -2684,14 +2873,31 @@
         # flattening of the tensors
         tensor = [element for site in self.sites for element in site.flatten()]
         np.savetxt(
             f"{path}/results/tensors/tensor_sites_{self.model}_direct_lattice_{self.Z2.l}x{self.Z2.L-1}_{cx}-{cy}_chi_{self.chi}_h_{self.h:.{precision}f}",
             tensor,
         )
 
+    def save_sites_XXZ(self, path, precision: int=2):
+        # shapes of the tensors
+        shapes = tensor_shapes(self.sites, False)
+        np.savetxt(
+            f"{path}/results/tensors/shapes_sites_{self.model}_L_{self.L}_chi_{self.chi}_d_{self.k:.{precision}f}_h_{self.h:.{precision}f}",
+            shapes,
+            fmt="%1.i",  # , delimiter=','
+        )
+
+        # flattening of the tensors
+        tensor = [element for site in self.sites for element in site.flatten()]
+        np.savetxt(
+            f"{path}/results/tensors/tensor_sites_{self.model}_L_{self.L}_chi_{self.chi}_d_{self.k:.{precision}f}_h_{self.h:.{precision}f}",
+            tensor,
+        )
+        return self
+
     def load_sites_Ising(self, path, precision: int=2):
         """
         load_sites
 
         This function load the tensors into the sites of the MPS.
         We fetch a completely flat list, split it to recover the original tensors
         (but still flat) and reshape each of them accordingly with the saved shapes.
@@ -2713,14 +2919,43 @@
         flat_tn = np.array_split(filedata, labels)
         flat_tn.pop(-1)
         # reshape the flat tensors and initializing the sites
         self.sites = [site.reshape(shapes[i]) for i, site in enumerate(flat_tn)]
 
         return self
 
+    def load_sites_Cluster_xy(self, path, precision: int=2):
+        """
+        load_sites
+
+        This function load the tensors into the sites of the MPS.
+        We fetch a completely flat list, split it to recover the original tensors
+        (but still flat) and reshape each of them accordingly with the saved shapes.
+        To initially split the list in the correct index position refer to the auxiliary
+        function get_labels().
+
+        """
+        # loading of the shapes
+        shapes = np.loadtxt(
+            f"{path}/results/tensors/shapes_sites_{self.model}_L_{self.L}_chi_{self.chi}_h_{self.h:.{precision}f}_lx_{self.lx:.{precision}f}_ly_{self.ly:.{precision}f}_J_{self.J:.{precision}f}"
+        ).astype(int)
+        # loading of the flat tensors
+        filedata = np.loadtxt(
+            f"{path}/results/tensors/tensor_sites_{self.model}_L_{self.L}_chi_{self.chi}_h_{self.h:.{precision}f}_lx_{self.lx:.{precision}f}_ly_{self.ly:.{precision}f}_J_{self.J:.{precision}f}",
+            dtype=complex,
+        )
+        # auxiliary function to get the indices where to split
+        labels = get_labels(shapes)
+        flat_tn = np.array_split(filedata, labels)
+        flat_tn.pop(-1)
+        # reshape the flat tensors and initializing the sites
+        self.sites = [site.reshape(shapes[i]) for i, site in enumerate(flat_tn)]
+
+        return self
+    
     def load_sites_ANNNI(self, path, precision: int=2):
         """
         load_sites
 
         This function load the tensors into the sites of the MPS.
         We fetch a completely flat list, split it to recover the original tensors
         (but still flat) and reshape each of them accordingly with the saved shapes.
@@ -2772,15 +3007,43 @@
         flat_tn = np.array_split(filedata, labels)
         flat_tn.pop(-1)
         # reshape the flat tensors and initializing the sites
         self.sites = [site.reshape(shapes[i]) for i, site in enumerate(flat_tn)]
 
         return self
 
+    def load_sites_XXZ(self, path, precision: int=2):
+        """
+        load_sites
+
+        This function load the tensors into the sites of the MPS.
+        We fetch a completely flat list, split it to recover the original tensors
+        (but still flat) and reshape each of them accordingly with the saved shapes.
+        To initially split the list in the correct index position refer to the auxiliary
+        function get_labels().
 
+        """
+        # loading of the shapes
+        shapes = np.loadtxt(
+            f"{path}/results/tensors/shapes_sites_{self.model}_L_{self.L}_chi_{self.chi}_d_{self.k:.{precision}f}_h_{self.h:.{precision}f}"
+        ).astype(int)
+        # loading of the flat tensors
+        filedata = np.loadtxt(
+            f"{path}/results/tensors/tensor_sites_{self.model}_L_{self.L}_chi_{self.chi}_d_{self.k:.{precision}f}_h_{self.h:.{precision}f}",
+            dtype=complex,
+        )
+        # auxiliary function to get the indices where to split
+        labels = get_labels(shapes)
+        flat_tn = np.array_split(filedata, labels)
+        flat_tn.pop(-1)
+        # reshape the flat tensors and initializing the sites
+        self.sites = [site.reshape(shapes[i]) for i, site in enumerate(flat_tn)]
+
+        return self
+    
     def save_sites_old(self, path, precision=2):
         """
         save_sites
 
         This function saves the sites, e.g., the tensors composing our MPS.
         In order to do that we need to flatten the whole list of tensors and save
         their original shapes in order to reshape them in the loading step.
```

### Comparing `qs-mps-2024.0.0/src/qs_mps/utils.py` & `qs-mps-2024.0.1/src/qs_mps/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,14 @@
 
     file_path: string - file path
     list: list - list to save
 
     """
     with open(file_path, "w") as file:
         for sublist in list:
-            print(sublist)
             line = " ".join(repr(item) for item in sublist)
             file.write(line + "\n")
 
 
 # ---------------------------------------------------------------------------------------
 # Load list of lists
 # ---------------------------------------------------------------------------------------
@@ -505,14 +504,35 @@
 
     v_r = np.zeros(mpo[0].shape[0])
     v_r[-1] = 1
     d = mpo[0].shape[2]
     matrix = ncon([env, v_r.T], [label_env, mid]).reshape((d**L, d**L))
     return matrix
 
+def swap_columns(matrix, tensor: bool=True):
+    n = len(matrix)
+    for i in range(n // 2):
+        col_to_swap = n - 1 - i
+        if tensor:
+            matrix[i, :, :], matrix[col_to_swap, :, :] = matrix[col_to_swap, :, :], matrix[i, :, :].copy()
+        else:
+            for row in matrix:
+                row[i], row[col_to_swap] = row[col_to_swap], row[i]
+    return matrix
+
+def swap_rows(matrix, tensor: bool=True):
+    n = len(matrix)
+    for i in range(n // 2):
+        row_to_swap = n - 1 - i
+        if tensor:
+            matrix[:, i, :], matrix[:, row_to_swap, :] = matrix[:, row_to_swap, :], matrix[:, i, :].copy()
+        else:
+            for row in matrix:
+                row[i], row[row_to_swap] = row[row_to_swap], row[i]
+    return matrix   
 
 # ---------------------------------------------------------------------------------------
 # ---------------------------------------------------------------------------------------
 # ---------------------------------------------------------------------------------------
 """
 Defining a series of functions to have single and double site operators
 """
@@ -845,15 +865,15 @@
     plt.tight_layout()
     plt.show()
 
 
 # ---------------------------------------------------------------------------------------
 # Create Sequential Colors
 # ---------------------------------------------------------------------------------------
-def create_sequential_colors(num_colors, colormap_name):
+def create_sequential_colors(num_colors, colormap_name: str='viridis'):
     """
     create_sequential_colors
 
     This function creates a sequence of colors extracted from a specified colormap.
 
     num_colors: int - number of colors we want to extract
     colormap_name: string - colormap name we want to use
```

### Comparing `qs-mps-2024.0.0/src/qs_mps.egg-info/PKG-INFO` & `qs-mps-2024.0.1/src/qs_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qs-mps
-Version: 2024.0.0
+Version: 2024.0.1
 Summary: Quantum Simulation with Matrix Product State, a Tensor network method for the study of Quantum Systems
 Author-email: Francesco Di Marcantonio <francesco.di.marcantonio@cern.ch>
 Maintainer-email: Francesco Di Marcantonio <francesco.di.marcantonio@cern.ch>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `qs-mps-2024.0.0/src/qs_mps.egg-info/SOURCES.txt` & `qs-mps-2024.0.1/src/qs_mps.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 src/qs_mps/Ising_gs_and_time_ev.py
 src/qs_mps/TensorMultiplier.py
 src/qs_mps/__init__.py
 src/qs_mps/analytical_formulas_TFIC.py
 src/qs_mps/checks.py
+src/qs_mps/get_rdms.py
 src/qs_mps/gs_multiprocessing.py
 src/qs_mps/lattice.py
 src/qs_mps/mpo_class.py
 src/qs_mps/mps_class.py
 src/qs_mps/sparse_hamiltonians_and_operators.py
 src/qs_mps/utils.py
 src/qs_mps.egg-info/PKG-INFO
@@ -18,31 +19,36 @@
 src/qs_mps.egg-info/dependency_links.txt
 src/qs_mps.egg-info/requires.txt
 src/qs_mps.egg-info/top_level.txt
 src/qs_mps/applications/__init__.py
 src/qs_mps/applications/ANNNI/get_gs_DMRG.py
 src/qs_mps/applications/ANNNI/get_observables_MPS.py
 src/qs_mps/applications/ANNNI/ground_state_multiprocessing.py
+src/qs_mps/applications/CLUSTER/get_gs_DMRG-xy.py
+src/qs_mps/applications/CLUSTER/get_gs_DMRG.py
 src/qs_mps/applications/CLUSTER/get_observables_MPS.py
 src/qs_mps/applications/ISING/TEBD_different_chi.py
 src/qs_mps/applications/ISING/TEBD_different_delta.py
 src/qs_mps/applications/ISING/__init__.py
 src/qs_mps/applications/ISING/assess_time.py
 src/qs_mps/applications/ISING/get_gs_DMRG.py
 src/qs_mps/applications/ISING/get_gs_and_time_ev_EXACT.py
 src/qs_mps/applications/ISING/get_observables_MPS.py
 src/qs_mps/applications/ISING/plot_DMRG.py
 src/qs_mps/applications/ISING/plot_TEBD.py
+src/qs_mps/applications/XXZ/get_gs_DMRG.py
 src/qs_mps/applications/Z2/__init__.py
 src/qs_mps/applications/Z2/exact_hamiltonian.py
 src/qs_mps/applications/Z2/get_gs_DMRG.py
 src/qs_mps/applications/Z2/get_gs_EXACT.py
 src/qs_mps/applications/Z2/get_observables_EXACT.py
 src/qs_mps/applications/Z2/get_observables_MPS.py
 src/qs_mps/applications/Z2/ground_state_multiprocessing.py
 src/qs_mps/applications/Z2/multi_run_gs.py
 src/qs_mps/applications/Z2/multi_run_obs.py
 src/qs_mps/applications/Z2/plot_DMRG.py
 src/qs_mps/applications/Z2/plot_animations.py
+src/qs_mps/applications/Z2/string_energy_density_debug.py
 src/qs_mps/applications/Z2/test_sparse_mpo.py
 src/qs_mps/applications/Z2/time_ev_debug.py
-src/qs_mps/applications/Z2/vacuum_sector.py
+src/qs_mps/applications/Z2/vacuum_sector.py
+tests/test_rdms.py
```

