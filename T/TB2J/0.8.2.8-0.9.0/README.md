# Comparing `tmp/TB2J-0.8.2.8.tar.gz` & `tmp/TB2J-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TB2J-0.8.2.8.tar", last modified: Tue Apr  9 08:56:21 2024, max compression
+gzip compressed data, was "TB2J-0.9.0.tar", last modified: Wed May 22 13:11:16 2024, max compression
```

## Comparing `TB2J-0.8.2.8.tar` & `TB2J-0.9.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1332 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/LICENSE
--rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     2089 2024-03-08 15:04:05.000000 TB2J-0.8.2.8/README.md
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/TB2J/
--rw-r--r--   0 hexu      (1032) phythema   (500)     6980 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/Jdownfolder.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3179 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/Jtensor.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3383 2024-04-07 10:46:54.000000 TB2J-0.8.2.8/TB2J/Oiju.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6809 2024-04-07 10:46:54.000000 TB2J-0.8.2.8/TB2J/Oiju_epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       24 2024-04-09 08:56:13.000000 TB2J-0.8.2.8/TB2J/__init__.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/TB2J/abacus/
--rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-03-04 09:41:08.000000 TB2J-0.8.2.8/TB2J/abacus/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-03-04 09:41:08.000000 TB2J-0.8.2.8/TB2J/abacus/abacus_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8492 2024-03-08 15:04:05.000000 TB2J-0.8.2.8/TB2J/abacus/abacus_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2973 2024-03-04 09:41:08.000000 TB2J-0.8.2.8/TB2J/abacus/gen_exchange_abacus.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-03-04 09:41:08.000000 TB2J-0.8.2.8/TB2J/abacus/orbital_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-03-08 12:59:31.000000 TB2J-0.8.2.8/TB2J/abacus/stru_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-03-04 09:41:08.000000 TB2J-0.8.2.8/TB2J/abacus/test_read_HRSR.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-03-04 09:41:08.000000 TB2J-0.8.2.8/TB2J/abacus/test_read_stru.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1558 2024-03-04 09:41:08.000000 TB2J-0.8.2.8/TB2J/basis.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2891 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/citation.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2633 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/contour.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1514 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/density_matrix.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3474 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    29570 2024-04-07 10:46:54.000000 TB2J-0.8.2.8/TB2J/exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    10985 2024-04-07 14:47:26.000000 TB2J-0.8.2.8/TB2J/exchangeCL2.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8523 2024-04-07 10:46:54.000000 TB2J-0.8.2.8/TB2J/exchange_pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8436 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/exchange_qspace.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/TB2J/external/
--rw-r--r--   0 hexu      (1032) phythema   (500)      137 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/external/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5831 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/external/p_tqdm.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6890 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/gpaw_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    13377 2024-04-09 08:55:41.000000 TB2J-0.8.2.8/TB2J/green.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1603 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/greentest.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/TB2J/io_exchange/
--rw-r--r--   0 hexu      (1032) phythema   (500)       32 2024-02-28 11:09:31.000000 TB2J-0.8.2.8/TB2J/io_exchange/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    19354 2024-03-27 09:14:31.000000 TB2J-0.8.2.8/TB2J/io_exchange/io_exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6739 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/io_exchange/io_multibinit.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4173 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/io_exchange/io_tomsasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    10547 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/io_exchange/io_txt.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3301 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/io_exchange/io_uppasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5583 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/io_exchange/io_vampire.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    15265 2024-03-08 15:04:05.000000 TB2J-0.8.2.8/TB2J/io_merge.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      532 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/kpoints.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    15372 2024-04-07 10:46:54.000000 TB2J-0.8.2.8/TB2J/manager.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      300 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/mathutils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    17721 2024-03-04 10:09:47.000000 TB2J-0.8.2.8/TB2J/myTB.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6669 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/orbmap.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4120 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/pauli.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1192 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4104 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/plot.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3031 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/rotate_atoms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    14823 2024-03-18 09:10:54.000000 TB2J-0.8.2.8/TB2J/sisl_wrapper.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/TB2J/spinham/
--rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.8.2.8/TB2J/spinham/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2196 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/base_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      762 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/constants.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2784 2024-04-08 08:59:38.000000 TB2J-0.8.2.8/TB2J/spinham/h_matrix.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    16607 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/hamiltonian.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9714 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/hamiltonian_terms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2401 2024-04-08 09:13:15.000000 TB2J-0.8.2.8/TB2J/spinham/obtain_J.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6599 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/plot.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4986 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/qsolver.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2219 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/spin_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    11033 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/spin_xml.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    12217 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/spinham/supercell.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8083 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/tensor_rotate.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3897 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/utest.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9880 2024-03-18 09:04:29.000000 TB2J-0.8.2.8/TB2J/utils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      337 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/TB2J/versioninfo.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/TB2J/wannier/
--rw-r--r--   0 hexu      (1032) phythema   (500)       80 2024-03-04 10:09:47.000000 TB2J-0.8.2.8/TB2J/wannier/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4620 2024-03-14 08:56:01.000000 TB2J-0.8.2.8/TB2J/wannier/w90_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-03-04 10:09:47.000000 TB2J-0.8.2.8/TB2J/wannier/w90_tb_parser.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/TB2J.egg-info/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-04-09 08:56:21.000000 TB2J-0.8.2.8/TB2J.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     1797 2024-04-09 08:56:21.000000 TB2J-0.8.2.8/TB2J.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-04-09 08:56:21.000000 TB2J-0.8.2.8/TB2J.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)       79 2024-04-09 08:56:21.000000 TB2J-0.8.2.8/TB2J.egg-info/requires.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        5 2024-04-09 08:56:21.000000 TB2J-0.8.2.8/TB2J.egg-info/top_level.txt
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/scripts/
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/scripts/TB2J_downfold.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1142 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/scripts/TB2J_eigen.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3115 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/scripts/TB2J_magnon.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      124 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/scripts/TB2J_magnon_dos.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1636 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/scripts/TB2J_merge.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      648 2024-02-28 11:18:04.000000 TB2J-0.8.2.8/scripts/TB2J_rotate.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     4422 2024-03-04 09:41:08.000000 TB2J-0.8.2.8/scripts/abacus2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     4317 2024-04-07 10:46:54.000000 TB2J-0.8.2.8/scripts/siesta2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     5728 2024-04-07 10:46:54.000000 TB2J-0.8.2.8/scripts/wann2J.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-04-09 08:56:21.801303 TB2J-0.8.2.8/setup.cfg
--rw-r--r--   0 hexu      (1032) phythema   (500)     1952 2024-04-09 08:56:14.000000 TB2J-0.8.2.8/setup.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1332 2024-02-28 11:18:04.000000 TB2J-0.9.0/LICENSE
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-05-22 13:11:16.087083 TB2J-0.9.0/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2089 2024-03-08 15:04:05.000000 TB2J-0.9.0/README.md
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.083083 TB2J-0.9.0/TB2J/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6980 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/Jdownfolder.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3179 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/Jtensor.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3383 2024-04-07 10:46:54.000000 TB2J-0.9.0/TB2J/Oiju.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6809 2024-04-07 10:46:54.000000 TB2J-0.9.0/TB2J/Oiju_epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       22 2024-05-22 12:10:06.000000 TB2J-0.9.0/TB2J/__init__.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.083083 TB2J-0.9.0/TB2J/abacus/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/abacus_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8461 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/abacus/abacus_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2973 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/gen_exchange_abacus.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/orbital_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-03-08 12:59:31.000000 TB2J-0.9.0/TB2J/abacus/stru_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/test_read_HRSR.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/abacus/test_read_stru.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1558 2024-03-04 09:41:08.000000 TB2J-0.9.0/TB2J/basis.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2891 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/citation.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2633 2024-04-18 09:51:34.000000 TB2J-0.9.0/TB2J/contour.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1514 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/density_matrix.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3474 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    29586 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10985 2024-05-22 12:05:07.000000 TB2J-0.9.0/TB2J/exchangeCL2.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8523 2024-04-07 10:46:54.000000 TB2J-0.9.0/TB2J/exchange_pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8436 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/exchange_qspace.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.083083 TB2J-0.9.0/TB2J/external/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      137 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/external/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5831 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/external/p_tqdm.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6890 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/gpaw_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    13377 2024-05-22 12:05:07.000000 TB2J-0.9.0/TB2J/green.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1603 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/greentest.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/TB2J/io_exchange/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       32 2024-02-28 11:09:31.000000 TB2J-0.9.0/TB2J/io_exchange/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    19354 2024-04-13 21:06:36.000000 TB2J-0.9.0/TB2J/io_exchange/io_exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6739 2024-05-22 12:05:07.000000 TB2J-0.9.0/TB2J/io_exchange/io_multibinit.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4173 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/io_exchange/io_tomsasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10547 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/io_exchange/io_txt.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3301 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/io_exchange/io_uppasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5583 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/io_exchange/io_vampire.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6825 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/io_merge.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      532 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/kpoints.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    15372 2024-04-07 10:46:54.000000 TB2J-0.9.0/TB2J/manager.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      300 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/mathutils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    17659 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/myTB.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6669 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/orbmap.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4120 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/pauli.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1192 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4104 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/plot.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3277 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/rotate_atoms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1070 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/rotate_siestaDM.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    14792 2024-05-22 12:05:11.000000 TB2J-0.9.0/TB2J/sisl_wrapper.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/TB2J/spinham/
+-rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.9.0/TB2J/spinham/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2196 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/base_parser.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      762 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/constants.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16607 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/hamiltonian.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9714 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/hamiltonian_terms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6599 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/plot.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4986 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/qsolver.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2219 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/spin_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11033 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/spin_xml.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    12217 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/spinham/supercell.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8083 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/tensor_rotate.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3897 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/utest.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9880 2024-05-22 12:05:07.000000 TB2J-0.9.0/TB2J/utils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      337 2024-02-28 11:18:04.000000 TB2J-0.9.0/TB2J/versioninfo.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/TB2J/wannier/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       80 2024-03-04 10:09:47.000000 TB2J-0.9.0/TB2J/wannier/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4620 2024-03-14 08:56:01.000000 TB2J-0.9.0/TB2J/wannier/w90_parser.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-03-04 10:09:47.000000 TB2J-0.9.0/TB2J/wannier/w90_tb_parser.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.083083 TB2J-0.9.0/TB2J.egg-info/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1796 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)       79 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        5 2024-05-22 13:11:16.000000 TB2J-0.9.0/TB2J.egg-info/top_level.txt
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-22 13:11:16.087083 TB2J-0.9.0/scripts/
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-02-28 11:18:04.000000 TB2J-0.9.0/scripts/TB2J_downfold.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1142 2024-02-28 11:18:04.000000 TB2J-0.9.0/scripts/TB2J_eigen.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3115 2024-02-28 11:18:04.000000 TB2J-0.9.0/scripts/TB2J_magnon.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      124 2024-02-28 11:18:04.000000 TB2J-0.9.0/scripts/TB2J_magnon_dos.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-05-22 12:05:11.000000 TB2J-0.9.0/scripts/TB2J_merge.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      887 2024-05-22 12:05:11.000000 TB2J-0.9.0/scripts/TB2J_rotate.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      581 2024-05-22 12:05:11.000000 TB2J-0.9.0/scripts/TB2J_rotateDM.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     4422 2024-03-04 09:41:08.000000 TB2J-0.9.0/scripts/abacus2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     4317 2024-04-07 10:46:54.000000 TB2J-0.9.0/scripts/siesta2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     5728 2024-04-07 10:46:54.000000 TB2J-0.9.0/scripts/wann2J.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-05-22 13:11:16.087083 TB2J-0.9.0/setup.cfg
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1986 2024-05-22 12:09:56.000000 TB2J-0.9.0/setup.py
```

### Comparing `TB2J-0.8.2.8/LICENSE` & `TB2J-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/PKG-INFO` & `TB2J-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.8.2.8
+Version: 0.9.0
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.8.2.8/README.md` & `TB2J-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/Jdownfolder.py` & `TB2J-0.9.0/TB2J/Jdownfolder.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/Jtensor.py` & `TB2J-0.9.0/TB2J/Jtensor.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/Oiju.py` & `TB2J-0.9.0/TB2J/Oiju.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/Oiju_epc.py` & `TB2J-0.9.0/TB2J/Oiju_epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/abacus/abacus_api.py` & `TB2J-0.9.0/TB2J/abacus/abacus_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/abacus/abacus_wrapper.py` & `TB2J-0.9.0/TB2J/abacus/abacus_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 from TB2J.abacus.stru_api import read_abacus, read_abacus_out
 
 
 class AbacusWrapper(AbstractTB):
     def __init__(self, HR, SR, Rlist, nbasis, nspin=1):
         self.R2kfactor = -2j * np.pi
         self.is_orthogonal = False
-        self.is_siesta = False
-        self._name = "Abacus"
+        self._name = "ABACUS"
         self.HR = HR
         self.SR = SR
         self.Rlist = Rlist
         self.nbasis = nbasis
         self.nspin = nspin
         self.norb = nbasis * nspin
         self._build_Rdict()
```

### Comparing `TB2J-0.8.2.8/TB2J/abacus/gen_exchange_abacus.py` & `TB2J-0.9.0/TB2J/abacus/gen_exchange_abacus.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/abacus/orbital_api.py` & `TB2J-0.9.0/TB2J/abacus/orbital_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/abacus/stru_api.py` & `TB2J-0.9.0/TB2J/abacus/stru_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/abacus/test_read_HRSR.py` & `TB2J-0.9.0/TB2J/abacus/test_read_HRSR.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/abacus/test_read_stru.py` & `TB2J-0.9.0/TB2J/abacus/test_read_stru.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/basis.py` & `TB2J-0.9.0/TB2J/basis.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/citation.py` & `TB2J-0.9.0/TB2J/citation.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/contour.py` & `TB2J-0.9.0/TB2J/contour.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/density_matrix.py` & `TB2J-0.9.0/TB2J/density_matrix.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/epc.py` & `TB2J-0.9.0/TB2J/epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/exchange.py` & `TB2J-0.9.0/TB2J/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
         self._prepare_orb_mmat()
 
     def _prepare_orb_mmat(self):
         self.mmats = {}
         self.orbital_names = {}
         self.norb_reduced = {}
-        if self.backend_name == "SIESTA":
+        if self.backend_name.upper() == "SIESTA":
             syms = self.atoms.get_chemical_symbols()
             for iatom, orbs in self.labels.items():
                 if (self.include_orbs is not None) and syms[iatom] in self.include_orbs:
                     mmat, reduced_orbs = map_orbs_matrix(
                         orbs,
                         spinor=not (self._is_collinear),
                         include_only=self.include_orbs[syms[iatom]],
@@ -301,15 +301,15 @@
         """
         return np.array(self.orb_dict[iatom], dtype=int)
 
     def simplify_orbital_contributions(self, Jorbij, iatom, jatom):
         """
         sum up the contribution of all the orbitals with same (n,l,m)
         """
-        if self.backend_name == "SIESTA":
+        if self.backend_name.upper() == "SIESTA":
             mmat_i = self.mmats[iatom]
             mmat_j = self.mmats[jatom]
             Jorbij = mmat_i.T @ Jorbij @ mmat_j
         return Jorbij
 
     def calculate_all(self):
         raise NotImplementedError(
```

### Comparing `TB2J-0.8.2.8/TB2J/exchangeCL2.py` & `TB2J-0.9.0/TB2J/exchangeCL2.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/exchange_pert.py` & `TB2J-0.9.0/TB2J/exchange_pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/exchange_qspace.py` & `TB2J-0.9.0/TB2J/exchange_qspace.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/external/p_tqdm.py` & `TB2J-0.9.0/TB2J/external/p_tqdm.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/gpaw_wrapper.py` & `TB2J-0.9.0/TB2J/gpaw_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/green.py` & `TB2J-0.9.0/TB2J/green.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/greentest.py` & `TB2J-0.9.0/TB2J/greentest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/io_exchange/io_exchange.py` & `TB2J-0.9.0/TB2J/io_exchange/io_exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/io_exchange/io_multibinit.py` & `TB2J-0.9.0/TB2J/io_exchange/io_multibinit.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/io_exchange/io_tomsasd.py` & `TB2J-0.9.0/TB2J/io_exchange/io_tomsasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/io_exchange/io_txt.py` & `TB2J-0.9.0/TB2J/io_exchange/io_txt.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/io_exchange/io_uppasd.py` & `TB2J-0.9.0/TB2J/io_exchange/io_uppasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/io_exchange/io_vampire.py` & `TB2J-0.9.0/TB2J/io_exchange/io_vampire.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/kpoints.py` & `TB2J-0.9.0/TB2J/kpoints.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/manager.py` & `TB2J-0.9.0/TB2J/manager.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/myTB.py` & `TB2J-0.9.0/TB2J/myTB.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from TB2J.wannier import parse_ham, parse_xyz, parse_atoms, parse_tb
 
 
 class AbstractTB:
     def __init__(self, R2kfactor, nspin, norb):
         #: :math:`\alpha` used in :math:`H(k)=\sum_R  H(R) \exp( \alpha k \cdot R)`,
         #: Should be :math:`2\pi i` or :math:`-2\pi i`
-        self.is_siesta = False
         self.is_orthogonal = True
         self.R2kfactor = R2kfactor
 
         #: number of spin. 1 for collinear, 2 for spinor.
         self.nspin = nspin
 
         #:number of orbitals. Each orbital can have two spins.
@@ -121,15 +120,14 @@
         self.sparse = sparse
         self.double_site_energy = double_site_energy
         if sparse:
             self._matrix = csr_matrix
         self.atoms = None
         self.R2kfactor = 2.0j * np.pi
         self.k2Rfactor = -2.0j * np.pi
-        self.is_siesta = False
         self.is_orthogonal = True
         self._name = "Wannier"
 
     def set_atoms(self, atoms):
         self.atoms = atoms
 
     @property
```

### Comparing `TB2J-0.8.2.8/TB2J/orbmap.py` & `TB2J-0.9.0/TB2J/orbmap.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/pauli.py` & `TB2J-0.9.0/TB2J/pauli.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/pert.py` & `TB2J-0.9.0/TB2J/pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/plot.py` & `TB2J-0.9.0/TB2J/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/rotate_atoms.py` & `TB2J-0.9.0/TB2J/rotate_atoms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 #!/usr/bin/env python3
 import copy
 from ase.io import read, write
 import numpy as np
 from TB2J.tensor_rotate import Rxx, Rxy, Rxz, Ryx, Ryy, Ryz, Rzx, Rzy, Rzz
 
 
-def rotate_atom_xyz(atoms):
+def rotate_atom_xyz(atoms, noncollinear=False):
     """
-    given a atoms, return:
-    - 'z'->'x'
-    - 'z'->'y'
-    - 'z'->'z'
-    """
-    atoms_x = copy.deepcopy(atoms)
-    atoms_x.rotate(90, "y", rotate_cell=True)
-    atoms_y = copy.deepcopy(atoms)
-    atoms_y.rotate(90, "x", rotate_cell=True)
-    atoms_z = atoms
-    return atoms_x, atoms_y, atoms_z
+    given a atoms, return rotated atoms:
+    atoms_1, ..., atoms_n,
+    where we considered n diffeerent roation axes.
+
+    When noncollinear == True, more rotated structures
+    will be generated.
+    """
+
+    rotation_axes = [(1, 0, 0), (0, 1, 0)]
+    if noncollinear:
+        rotation_axes += [(1, 1, 0), (1, 0, 1), (0, 1, 1)]
+    
+    for axis in rotation_axes:
+        rotated_atoms = copy.deepcopy(atoms)
+        rotated_atoms.rotate(90, axis, rotate_cell=True)
+        yield rotated_atoms
 
 
 def rotate_atom_spin_one_rotation(atoms, Rotation):
     """
     roate the spin of atoms with one rotation operator
     """
     magmoms = np.array(atoms.get_initial_magnetic_moments())
@@ -92,22 +97,19 @@
         print("WARNING!!!!!")
         print(
             f"{ftype} type does not contains the cell matrix explicitly. Therefore the outputted files does not give the rotation properly. Please use another format."
         )
         print("=" * 40)
 
 
-def rotate_xyz(fname, ftype="xyz"):
+def rotate_xyz(fname, ftype="xyz", noncollinear=False):
     check_ftype(ftype)
     atoms = read(fname)
     atoms.set_pbc(True)
 
-    atoms_x, atoms_y, atoms_z = rotate_atom_xyz(atoms)
+    rotated = rotate_atom_xyz(atoms, noncollinear=noncollinear)
+
+    for i, rotated_atoms in enumerate(rotated):
+        write(f"atoms_{i+1}.{ftype}", rotated_atoms)
+    write(f"atoms_0.{ftype}", atoms)
 
-    fname_x = f"atoms_x.{ftype}"
-    fname_y = f"atoms_y.{ftype}"
-    fname_z = f"atoms_z.{ftype}"
-
-    write(fname_x, atoms_x)
-    write(fname_y, atoms_y)
-    write(fname_z, atoms_z)
-    print(f"The output has been written to {fname_x}, {fname_y}, {fname_z}")
+    print(f"The output has been written to the atoms_i.{ftype} files. atoms_0.{ftype} contains the reference structure.")
```

### Comparing `TB2J-0.8.2.8/TB2J/sisl_wrapper.py` & `TB2J-0.9.0/TB2J/sisl_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from scipy.linalg import eigh
 from TB2J.myTB import AbstractTB
 from TB2J.mathutils import Lowdin
 
 
 class SislWrapper(AbstractTB):
     def __init__(self, sisl_hamiltonian, geom=None, spin=None):
-        self.is_siesta = False
         self.is_orthogonal = False
         self.ham = sisl_hamiltonian
         # k2Rfactor : H(k) = \int_R H(R) * e^(k2Rfactor * k.R)
         self.R2kfactor = 2.0j * np.pi  #
         if spin == "up":
             spin = 0
         elif spin == "down":
```

### Comparing `TB2J-0.8.2.8/TB2J/spinham/base_parser.py` & `TB2J-0.9.0/TB2J/spinham/base_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/spinham/constants.py` & `TB2J-0.9.0/TB2J/spinham/constants.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/spinham/hamiltonian.py` & `TB2J-0.9.0/TB2J/spinham/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/spinham/hamiltonian_terms.py` & `TB2J-0.9.0/TB2J/spinham/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/spinham/plot.py` & `TB2J-0.9.0/TB2J/spinham/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/spinham/qsolver.py` & `TB2J-0.9.0/TB2J/spinham/qsolver.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/spinham/spin_api.py` & `TB2J-0.9.0/TB2J/spinham/spin_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/spinham/spin_xml.py` & `TB2J-0.9.0/TB2J/spinham/spin_xml.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/spinham/supercell.py` & `TB2J-0.9.0/TB2J/spinham/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/tensor_rotate.py` & `TB2J-0.9.0/TB2J/tensor_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/utest.py` & `TB2J-0.9.0/TB2J/utest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/utils.py` & `TB2J-0.9.0/TB2J/utils.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/wannier/w90_parser.py` & `TB2J-0.9.0/TB2J/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J/wannier/w90_tb_parser.py` & `TB2J-0.9.0/TB2J/wannier/w90_tb_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/TB2J.egg-info/PKG-INFO` & `TB2J-0.9.0/TB2J.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.8.2.8
+Version: 0.9.0
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.8.2.8/TB2J.egg-info/SOURCES.txt` & `TB2J-0.9.0/TB2J.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 TB2J/mathutils.py
 TB2J/myTB.py
 TB2J/orbmap.py
 TB2J/pauli.py
 TB2J/pert.py
 TB2J/plot.py
 TB2J/rotate_atoms.py
+TB2J/rotate_siestaDM.py
 TB2J/sisl_wrapper.py
 TB2J/tensor_rotate.py
 TB2J/utest.py
 TB2J/utils.py
 TB2J/versioninfo.py
 TB2J.egg-info/PKG-INFO
 TB2J.egg-info/SOURCES.txt
@@ -54,28 +55,27 @@
 TB2J/io_exchange/io_tomsasd.py
 TB2J/io_exchange/io_txt.py
 TB2J/io_exchange/io_uppasd.py
 TB2J/io_exchange/io_vampire.py
 TB2J/spinham/__init__.py
 TB2J/spinham/base_parser.py
 TB2J/spinham/constants.py
-TB2J/spinham/h_matrix.py
 TB2J/spinham/hamiltonian.py
 TB2J/spinham/hamiltonian_terms.py
-TB2J/spinham/obtain_J.py
 TB2J/spinham/plot.py
 TB2J/spinham/qsolver.py
 TB2J/spinham/spin_api.py
 TB2J/spinham/spin_xml.py
 TB2J/spinham/supercell.py
 TB2J/wannier/__init__.py
 TB2J/wannier/w90_parser.py
 TB2J/wannier/w90_tb_parser.py
 scripts/TB2J_downfold.py
 scripts/TB2J_eigen.py
 scripts/TB2J_magnon.py
 scripts/TB2J_magnon_dos.py
 scripts/TB2J_merge.py
 scripts/TB2J_rotate.py
+scripts/TB2J_rotateDM.py
 scripts/abacus2J.py
 scripts/siesta2J.py
 scripts/wann2J.py
```

### Comparing `TB2J-0.8.2.8/scripts/TB2J_downfold.py` & `TB2J-0.9.0/scripts/TB2J_downfold.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/scripts/TB2J_eigen.py` & `TB2J-0.9.0/scripts/TB2J_eigen.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/scripts/TB2J_magnon.py` & `TB2J-0.9.0/scripts/TB2J_magnon.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/scripts/TB2J_merge.py` & `TB2J-0.9.0/scripts/TB2J_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import argparse
 import os
 import sys
-from TB2J.io_merge import merge, merge2
+from TB2J.io_merge import merge
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="TB2J_merge: merge the exchange parameters calculated from different directions. It can accept two types of calculations, first, the lattice structures are rotated from the original structure, from z to x, y, and z, respectively. The structures could be generated using the TB2J_rotate.py command. The second type is the three calculations have the spins along the x, y, and z axis, respectively."
     )
     parser.add_argument(
@@ -24,15 +24,22 @@
     )
     parser.add_argument(
         "--output_path",
         help="The path of the output directory, default is TB2J_results",
         type=str,
         default="TB2J_results",
     )
+    parser.add_argument(
+        "--main_path",
+        help="The path containning the reference structure.",
+        type=str,
+        default=None
+    )
 
     args = parser.parse_args()
     # merge(*(args.directories), args.type.strip().lower(), path=args.output_path)
     # merge(*(args.directories), method=args.type.strip().lower(), path=args.output_path)
-    merge2(args.directories, args.type.strip().lower(), path=args.output_path)
+    #merge2(args.directories, args.type.strip().lower(), path=args.output_path)
+    merge(*args.directories, main_path=args.main_path, write_path=args.output_path)
 
 
 main()
```

### Comparing `TB2J-0.8.2.8/scripts/abacus2J.py` & `TB2J-0.9.0/scripts/abacus2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/scripts/siesta2J.py` & `TB2J-0.9.0/scripts/siesta2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/scripts/wann2J.py` & `TB2J-0.9.0/scripts/wann2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.8/setup.py` & `TB2J-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-__version__ = "0.8.2.8"
+__version__ = "0.9.0"
 
 long_description = """TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. """
 
 setup(
     name="TB2J",
     version=__version__,
     description="TB2J: First principle to Heisenberg exchange J using tight-binding Green function method",
@@ -15,14 +15,15 @@
     license="BSD-2-clause",
     packages=find_packages(),
     scripts=[
         "scripts/wann2J.py",
         "scripts/siesta2J.py",
         "scripts/abacus2J.py",
         "scripts/TB2J_rotate.py",
+        "scripts/TB2J_rotateDM.py",
         "scripts/TB2J_merge.py",
         "scripts/TB2J_magnon.py",
         "scripts/TB2J_magnon_dos.py",
         "scripts/TB2J_downfold.py",
         "scripts/TB2J_eigen.py",
     ],
     install_requires=[
```

