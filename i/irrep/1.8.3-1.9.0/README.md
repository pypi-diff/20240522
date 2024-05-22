# Comparing `tmp/irrep-1.8.3.tar.gz` & `tmp/irrep-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irrep-1.8.3.tar", last modified: Thu Aug 31 19:51:01 2023, max compression
+gzip compressed data, was "irrep-1.9.0.tar", last modified: Wed May 22 13:34:57 2024, max compression
```

## Comparing `irrep-1.8.3.tar` & `irrep-1.9.0.tar`

### file list

```diff
@@ -1,499 +1,23 @@
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-08-31 19:51:01.305568 irrep-1.8.3/
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-08-31 19:51:01.249568 irrep-1.8.3/.github/
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-08-31 19:51:01.253568 irrep-1.8.3/.github/workflows/
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      607 2022-04-18 13:41:08.000000 irrep-1.8.3/.github/workflows/tests.yml
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2744 2021-11-23 00:31:37.000000 irrep-1.8.3/.gitignore
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       47 2021-02-02 19:38:10.000000 irrep-1.8.3/INSTALL
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    35148 2021-02-02 19:38:10.000000 irrep-1.8.3/LICENSE
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       47 2023-08-31 19:50:52.000000 irrep-1.8.3/MANIFEST.in
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     8019 2023-08-31 19:51:01.305568 irrep-1.8.3/PKG-INFO
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     7514 2023-08-31 18:23:47.000000 irrep-1.8.3/README.md
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-08-31 19:51:01.253568 irrep-1.8.3/irrep/
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       63 2023-08-31 18:51:53.000000 irrep-1.8.3/irrep/__init__.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    53882 2023-08-31 18:09:30.000000 irrep-1.8.3/irrep/bandstructure.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    14901 2023-08-31 18:09:30.000000 irrep-1.8.3/irrep/cli.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    17184 2022-12-15 09:55:11.000000 irrep-1.8.3/irrep/gvectors.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    56292 2022-12-07 13:24:11.000000 irrep-1.8.3/irrep/kpoint.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     9175 2023-03-06 19:00:22.000000 irrep-1.8.3/irrep/readfiles.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    51880 2023-08-31 18:09:30.000000 irrep-1.8.3/irrep/spacegroup.py
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-08-31 19:51:01.253568 irrep-1.8.3/irrep/tests/
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        0 2021-02-02 19:38:11.000000 irrep-1.8.3/irrep/tests/__init__.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    10397 2021-11-23 00:31:37.000000 irrep-1.8.3/irrep/tests/test_cli.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5289 2022-12-07 13:24:11.000000 irrep-1.8.3/irrep/utility.py
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-08-31 19:51:01.253568 irrep-1.8.3/irrep.egg-info/
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     8019 2023-08-31 19:51:01.000000 irrep-1.8.3/irrep.egg-info/PKG-INFO
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    19699 2023-08-31 19:51:01.000000 irrep-1.8.3/irrep.egg-info/SOURCES.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        1 2023-08-31 19:51:01.000000 irrep-1.8.3/irrep.egg-info/dependency_links.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       40 2023-08-31 19:51:01.000000 irrep-1.8.3/irrep.egg-info/entry_points.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       87 2023-08-31 19:51:01.000000 irrep-1.8.3/irrep.egg-info/requires.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        6 2023-08-31 19:51:01.000000 irrep-1.8.3/irrep.egg-info/top_level.txt
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-08-31 19:51:01.253568 irrep-1.8.3/irreptables/
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      959 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/__convertTab.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)    13012 2021-11-23 00:31:37.000000 irrep-1.8.3/irreptables/__init__.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       20 2022-04-18 13:49:49.000000 irrep-1.8.3/irreptables/_version.py
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-08-31 19:51:01.305568 irrep-1.8.3/irreptables/tables/
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3569 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/README
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      435 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=1-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      488 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=1-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1457 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=10-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2296 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=10-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1991 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=100-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2026 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=100-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2250 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=101-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1683 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=101-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1994 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=102-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2027 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=102-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2249 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=103-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1518 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=103-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2151 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=104-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2026 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=104-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2168 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=105-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1683 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=105-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2152 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=106-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2027 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=106-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1329 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=107-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1292 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=107-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1433 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=108-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1270 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=108-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1320 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=109-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1733 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=109-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1094 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=11-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1609 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=11-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1342 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=110-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1711 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=110-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1852 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=111-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1523 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=111-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2170 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=112-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1687 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=112-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1997 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=113-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2032 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=113-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2157 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=114-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2032 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=114-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1852 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=115-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1523 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=115-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2252 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=116-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1687 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=116-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1996 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=117-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2031 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=117-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1996 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=118-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2031 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=118-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1374 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=119-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1479 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=119-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      977 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=12-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1488 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=12-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1396 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=120-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1457 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=120-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1476 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=121-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1391 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=121-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1502 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=122-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2013 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=122-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5653 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=123-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3726 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=123-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4484 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=124-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4448 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=124-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3847 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=125-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3214 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=125-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3421 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=126-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3534 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=126-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6263 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=127-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4534 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=127-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4791 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=128-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5401 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=128-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3847 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=129-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3214 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=129-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1093 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=13-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1608 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=13-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3825 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=130-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3452 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=130-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4482 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=131-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3051 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=131-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4165 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=132-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3133 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=132-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3424 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=133-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3535 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=133-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3854 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=134-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3215 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=134-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4792 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=135-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3537 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=135-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4474 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=136-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4086 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=136-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3424 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=137-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3535 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=137-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4554 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=138-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3455 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=138-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3630 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=139-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2994 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=139-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1258 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=14-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1445 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=14-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3698 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=140-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2904 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=140-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2702 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=141-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3126 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=141-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2611 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=142-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2954 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=142-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      885 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=143-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1062 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=143-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      896 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=144-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1069 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=144-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      896 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=145-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1069 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=145-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      564 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=146-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      731 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=146-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1698 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=147-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2027 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=147-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1377 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=148-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1696 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=148-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1070 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=149-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1565 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=149-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      795 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=15-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1144 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=15-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1082 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=150-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1693 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=150-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1089 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=151-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1582 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=151-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1101 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=152-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1712 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=152-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1089 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=153-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1582 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=153-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1101 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=154-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1712 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=154-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      748 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=155-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1233 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=155-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1067 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=156-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1562 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=156-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1079 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=157-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1690 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=157-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1151 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=158-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1482 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=158-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1225 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=159-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1552 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=159-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1425 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=16-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      920 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=16-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      745 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=160-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1230 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=160-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      829 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=161-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1150 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=161-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2172 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=162-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3553 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=162-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2051 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=163-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3002 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=163-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2166 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=164-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3547 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=164-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1983 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=165-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3054 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=165-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1832 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=166-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3087 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=166-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1649 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=167-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2594 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=167-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1678 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=168-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2194 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=168-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1782 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=169-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2126 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=169-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1078 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=17-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1609 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=17-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1782 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=170-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2126 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=170-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1698 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=171-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=171-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1698 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=172-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=172-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1765 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=173-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2113 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=173-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2304 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=174-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2956 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=174-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5141 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=175-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6586 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=175-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3800 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=176-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4914 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=176-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2145 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=177-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2314 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=177-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1887 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=178-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2965 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=178-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1887 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=179-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2965 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=179-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1243 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=18-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1610 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=18-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2181 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=180-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2349 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=180-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2181 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=181-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2349 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=181-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1855 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=182-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2930 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=182-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2145 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=183-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2314 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=183-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2527 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=184-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2256 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=184-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2584 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=185-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2437 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=185-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2646 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=186-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2379 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=186-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2756 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=187-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2945 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=187-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2583 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=188-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3682 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=188-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2798 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=189-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2435 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=189-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1326 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=19-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1529 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=19-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2539 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=190-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3737 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=190-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6419 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=191-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5046 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=191-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5691 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=192-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6411 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=192-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4855 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=193-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4906 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=193-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4769 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=194-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5471 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=194-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1878 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=195-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2301 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=195-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1425 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=196-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2030 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=196-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2165 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=197-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2717 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=197-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1809 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=198-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2550 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=198-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2166 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=199-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2920 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=199-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      694 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=2-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      785 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=2-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      806 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=20-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1167 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=20-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5755 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=200-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6048 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=200-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5121 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=201-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6212 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=201-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4008 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=202-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4802 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=202-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3640 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=203-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5102 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=203-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5511 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=204-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6449 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=204-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4944 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=205-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6410 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=205-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5426 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=206-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6485 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=206-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3134 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=207-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3842 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=207-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3141 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=208-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3843 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=208-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2385 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=209-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3431 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=209-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      957 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=21-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      844 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=21-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2338 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=210-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3640 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=210-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3214 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=211-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4037 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=211-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3202 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=212-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4967 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=212-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3201 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=213-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4968 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=213-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3254 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=214-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4276 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=214-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3135 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=215-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3843 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=215-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2426 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=216-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3614 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=216-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3459 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=217-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4122 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=217-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3775 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=218-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4167 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=218-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2488 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=219-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3556 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=219-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      864 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=22-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      704 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=22-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4041 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=220-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5452 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=220-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     9614 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=221-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     9649 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=221-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     7499 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=222-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     9188 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=222-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     7931 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=223-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     8868 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=223-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     8442 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=224-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     8973 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=224-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6583 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=225-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     8131 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=225-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6491 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=226-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     7810 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=226-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     6019 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=227-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     8226 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=227-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     5927 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=228-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     7905 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=228-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     8816 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=229-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     9337 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=229-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      874 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=23-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      871 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=23-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     7632 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=230-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     9934 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=230-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      790 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=24-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1048 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=24-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1423 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=25-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      918 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=25-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1752 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=26-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      919 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=26-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1751 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=27-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      918 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=27-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1075 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=28-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1606 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=28-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1240 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=29-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1443 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=29-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      676 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=3-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      959 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=3-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1239 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=30-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1606 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=30-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1240 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=31-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1607 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=31-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1239 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=32-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1606 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=32-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1322 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=33-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1525 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=33-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1239 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=34-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1606 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=34-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      955 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=35-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      842 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=35-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1142 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=36-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      821 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=36-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1119 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=37-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      842 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=37-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      959 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=38-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      846 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=38-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1003 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=39-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      802 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=39-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      765 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=4-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      872 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=4-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      785 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=40-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1190 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=40-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      829 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=41-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1146 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=41-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      862 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=42-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      702 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=42-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      776 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=43-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1052 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=43-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      789 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=44-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      896 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=44-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      833 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=45-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      852 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=45-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      811 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=46-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      874 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=46-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4035 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=47-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1882 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=47-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2133 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=48-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2374 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=48-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2767 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=49-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=49-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      490 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=5-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      679 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=5-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2133 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=50-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2374 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=50-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2767 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=51-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=51-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1900 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=52-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2923 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=52-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2137 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=53-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3472 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=53-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2297 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=54-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=54-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3399 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=55-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=55-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2613 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=56-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=56-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2297 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=57-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=57-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2453 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=58-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3472 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=58-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2133 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=59-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2374 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=59-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      675 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=6-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      958 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=6-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2064 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=60-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2759 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=60-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2064 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=61-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2443 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=61-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2613 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=62-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2210 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=62-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1792 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=63-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1780 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=63-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1874 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=64-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1698 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=64-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2517 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=65-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1788 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=65-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1883 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=66-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1952 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=66-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2335 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=67-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1444 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=67-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1701 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=68-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1608 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=68-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2277 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=69-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1384 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=69-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      763 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=7-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      870 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=7-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1338 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=70-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1642 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=70-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1909 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=71-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1806 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=71-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1727 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=72-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1462 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=72-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1549 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=73-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1464 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=73-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1731 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=74-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1806 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=74-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1113 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=75-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1575 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=75-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1242 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=76-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1452 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=76-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1118 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=77-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1576 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=77-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1242 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=78-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1456 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=78-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      774 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=79-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1125 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=79-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      489 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=8-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      678 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=8-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      779 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=80-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1128 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=80-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1116 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=81-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1578 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=81-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      900 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=82-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1283 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=82-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3141 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=83-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     4498 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=83-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2196 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=84-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     3315 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=84-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2013 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=85-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2970 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=85-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2014 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=86-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2971 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=86-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2021 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=87-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2946 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=87-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1470 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=88-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2195 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=88-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1850 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=89-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1521 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=89-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      533 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=9-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      634 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=9-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1997 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=90-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2030 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=90-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1496 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=91-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2296 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=91-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1821 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=92-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2379 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=92-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1857 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=93-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1522 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=93-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2000 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=94-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2031 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=94-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1496 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=95-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2294 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=95-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1821 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=96-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     2377 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=96-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1332 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=97-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1295 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=97-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1253 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=98-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1472 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=98-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1846 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=99-scal.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1517 2021-02-02 19:38:11.000000 irrep-1.8.3/irreptables/tables/irreps-SG=99-spin.dat
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       84 2023-08-31 19:51:01.305568 irrep-1.8.3/setup.cfg
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1027 2023-08-31 18:12:49.000000 irrep-1.8.3/setup.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1091 2021-02-02 19:38:11.000000 irrep-1.8.3/setup_tables.py
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      249 2023-08-31 19:38:23.000000 irrep-1.8.3/uploadpypi.sh
+drwxrwxr-x   0 mi2       (1000) mi2       (1000)        0 2024-05-22 13:34:57.716806 irrep-1.9.0/
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)    35148 2023-09-21 13:32:27.000000 irrep-1.9.0/LICENSE
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)       33 2023-09-21 13:57:58.000000 irrep-1.9.0/MANIFEST.in
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)     8057 2024-05-22 13:34:57.716806 irrep-1.9.0/PKG-INFO
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)     7514 2023-09-21 13:57:58.000000 irrep-1.9.0/README.md
+drwxrwxr-x   0 mi2       (1000) mi2       (1000)        0 2024-05-22 13:34:57.716806 irrep-1.9.0/irrep/
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)       64 2024-05-22 12:30:40.000000 irrep-1.9.0/irrep/__init__.py
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)    30357 2024-05-22 12:59:44.000000 irrep-1.9.0/irrep/bandstructure.py
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)    14887 2024-05-22 12:59:23.000000 irrep-1.9.0/irrep/cli.py
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)    17184 2023-09-21 13:32:28.000000 irrep-1.9.0/irrep/gvectors.py
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)    37484 2024-05-22 12:59:08.000000 irrep-1.9.0/irrep/kpoint.py
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)    29755 2024-05-22 12:28:29.000000 irrep-1.9.0/irrep/readfiles.py
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)    50722 2024-05-22 12:28:29.000000 irrep-1.9.0/irrep/spacegroup.py
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)     5976 2024-05-16 12:06:50.000000 irrep-1.9.0/irrep/utility.py
+drwxrwxr-x   0 mi2       (1000) mi2       (1000)        0 2024-05-22 13:34:57.716806 irrep-1.9.0/irrep.egg-info/
+-rw-r--r--   0 mi2       (1000) mi2       (1000)     8057 2024-05-22 13:34:57.000000 irrep-1.9.0/irrep.egg-info/PKG-INFO
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)      368 2024-05-22 13:34:57.000000 irrep-1.9.0/irrep.egg-info/SOURCES.txt
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)        1 2024-05-22 13:34:57.000000 irrep-1.9.0/irrep.egg-info/dependency_links.txt
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)       59 2024-05-22 13:34:57.000000 irrep-1.9.0/irrep.egg-info/entry_points.txt
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)       87 2024-05-22 13:34:57.000000 irrep-1.9.0/irrep.egg-info/requires.txt
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)        6 2024-05-22 13:34:57.000000 irrep-1.9.0/irrep.egg-info/top_level.txt
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)       84 2024-05-22 13:34:57.716806 irrep-1.9.0/setup.cfg
+-rw-rw-r--   0 mi2       (1000) mi2       (1000)     1028 2023-09-21 13:57:58.000000 irrep-1.9.0/setup.py
```

### Comparing `irrep-1.8.3/LICENSE` & `irrep-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `irrep-1.8.3/PKG-INFO` & `irrep-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: irrep
-Version: 1.8.3
+Version: 1.9.0
 Summary: A tool to get symmetry proberties of ab-initio wavefunctions, irreduible representations and more.
 Home-page: https://github.com/stepan-tsirkin/irrep
 Author: Stepan S. Tsirkin
-Author-email: stepan.tsirkin@uzh.ch
+Author-email: stepan.tsirkin@ehu.eus
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IrRep
@@ -149,7 +151,9 @@
    known output.
 7. Make changes to the code as required. The `irrep` command line tool 
    will also be available inside this environment.
 
 You can verify your development environment by opening a Python interpretor 
 (e.g. running `python`) and running `import irrep` and then `print(irrep.__file__)`.
 This should print the path to your local repository containing irrep.
+
+
```

### Comparing `irrep-1.8.3/README.md` & `irrep-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `irrep-1.8.3/irrep/bandstructure.py` & `irrep-1.9.0/irrep/spacegroup.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,1448 +12,1269 @@
 ## see LICENSE file in the                                       #
 ##                                                               #
 ##  Written by Stepan Tsirkin, University of Zurich.             #
 ##  e-mail: stepan.tsirkin@physik.uzh.ch                         #
 ##################################################################
 
 
-import copy
-import functools
-
 import numpy as np
-import numpy.linalg as la
+from math import pi
+from scipy.linalg import expm
+import spglib
+from irreptables import IrrepTable
+from scipy.optimize import minimize
+from .utility import str_
 
-from .utility import str2bool, BOHR
-from .readfiles import AbinitHeader, Hartree_eV
-from .readfiles import WAVECARFILE
-from .kpoint import Kpoint
-from .spacegroup import SpaceGroup
+pauli_sigma = np.array(
+    [[[0, 1], [1, 0]], [[0, -1j], [1j, 0]], [[1, 0], [0, -1]]])
 
 
-class BandStructure:
+class SymmetryOperation():
     """
-    Parses files and organizes info about the whole band structure in 
-    attributes. Contains methods to calculate and write traces (and irreps), 
-    for the separation of the band structure in terms of a symmetry operation 
-    and for the calculation of the Zak phase and wannier charge centers.
+    Contains information to describe a symmetry operation and methods to get 
+    info about the symmetry, transform it to a reference choice of unit cell 
+    and print a description of it.
 
     Parameters
     ----------
-    fWAV : str, default=None
-        Name of file containing wave-functions in VASP (WAVECAR format).
-    fWFK : str, default=None
-        Name of file containing wave-functions in ABINIT (WFK format).
-    prefix : str, default=None
-        Prefix used for Quantum Espresso calculations or seedname of Wannier90 
-        files.
-    fPOS : str, default=None
-        Name of file containing the crystal structure in VASP (POSCAR format).
-    Ecut : float, default=None
-        Plane-wave cutoff in eV to consider in the expansion of wave-functions.
-    IBstart : int, default=None
-        First band to be considered.
-    IBend : int, default=None
-        Last band to be considered.
-    kplist : array, default=None
-        List of indices of k-points to be considered.
-    spinor : bool, default=None
-        `True` if wave functions are spinors, `False` if they are scalars. 
-        Mandatory for VASP.
-    code : str, default='vasp'
-        DFT code used. Set to 'vasp', 'abinit', 'espresso' or 'wannier90'.
-    EF : float, default=None
-        Fermi-energy.
-    onlysym : bool, default=False
-        Exit after printing info about space-group.
-    spin_channel : str, default=None
-        Selection of the spin-channel. 'up' for spin-up, 'dw' for spin-down. 
-        Only applied in the interface to Quantum Espresso.
-    refUC : array, default=None
-        3x3 array describing the transformation of vectors defining the 
-        unit cell to the standard setting.
-    shiftUC : array, default=None
-        Translation taking the origin of the unit cell used in the DFT 
-        calculation to that of the standard setting.
-    search_cell : bool, default=False
-        Whether the transformation to the conventional cell should be computed.
-        It is `True` if kpnames was specified in CLI.
-    _correct_Ecut0 : float
-        In case of VASP, if you get an error like ' computed ncnt=*** != input nplane=*** ', 
-        try to set this parameter to a small positive or negative value (usually of order  +- 1e-7)
-    trans_thresh : float, default=1e-5
-        Threshold to compare translational parts of symmetries.
+    rotation : array, shape=(3,3)
+        Matrix describing the tranformation of basis vectors of the unit cell 
+        under the symmetry operation.
+    translation : array, shape=(3,)
+        Translational part of the symmetry operation, in terms of the basis 
+        vectors of the unit cell.
+    Lattice : array, shape=(3,3) 
+        Each row contains cartesian coordinates of a basis vector forming the 
+        unit-cell in real space.
+    ind : int, default=-1
+        Index of the symmetry operation.
+    spinor : bool, default=true
+        `True` if wave-functions are spinors, `False` if they are scalars.
 
     Attributes
-    ----------
-    spacegroup : class
-        Instance of `SpaceGroup`.
-    spinor : bool
-        `True` if wave functions are spinors, `False` if they are scalars. It 
-        will be read from DFT files.
-    efermi : float
-        Fermi-energy. If user set a number as `EF` in CLI, it will be used. If 
-        `EF` was set to `auto`, it will try to parse it and set to 0.0 if it 
-        could not.
-    Ecut0 : float
-        Plane-wave cutoff (in eV) used in DFT calulations. Always read from 
-        DFT files. Insignificant if `code`='wannier90'.
-    Ecut : float
-        Plane-wave cutoff (in eV) to consider in the expansion of wave-functions.
-        Will be set equal to `Ecut0` if input parameter `Ecut` was not set or 
-        the value of this is negative or larger than `Ecut0`.
+    ---------
+    ind : int
+        Index of the symmetry operation.
+    rotation : array, shape=(3,3)
+        Matrix describing the tranformation of basis vectors of the unit cell 
+        under the symmetry operation.
+    translation : array, shape=(3,)
+        Translational part of the symmetry operation, in terms of the basis 
+        vectors of the unit cell.
     Lattice : array, shape=(3,3) 
         Each row contains cartesian coordinates of a basis vector forming the 
         unit-cell in real space.
-    RecLattice : array, shape=(3,3)
-        Each row contains the cartesian coordinates of a basis vector forming 
-        the unit-cell in reciprocal space.
-    kpoints : list
-        Each element is an instance of `class Kpoint` corresponding to a 
-        k-point specified in input parameter `kpoints`. If this input was not 
-        set, all k-points found in DFT files will be considered.
-    _correct_Ecut0 : float
-        if you get an error like ' computed ncnt=*** != input nplane=*** ', 
-        try to set this parameter to a small positive or negative value (usually of order  +- 1e-7)
+    axis : array, shape=(3,)
+        Rotation axis of the symmetry.
+    angle : float
+        Rotation angle of the symmmetry, in radians.
+    inversion : bool
+        `False` if the symmetry preserves handedness (identity, rotation, 
+        translation or screw rotation), `True` otherwise (inversion, reflection 
+        roto-inversion or glide reflection).
+    angle_str : str
+        String describing the rotation angle in radians.
+    spinor : bool
+        `True` if wave-functions are spinors, `False` if they are scalars.
+    spinor_rotation : array, shape=(2,2)
+        Matrix describing how spinors transform under the symmetry.
+    sign : float
+        Factor needed to match the matrix for the rotation of spinors 
+        to that in tables.
     """
 
-    def __init__(
-        self,
-        fWAV=None,
-        fWFK=None,
-        prefix=None,
-        fPOS=None,
-        Ecut=None,
-        IBstart=None,
-        IBend=None,
-        kplist=None,
-        spinor=None,
-        code="vasp",
-        EF='0.0',
-        onlysym=False,
-        spin_channel=None,
-        refUC = None,
-        shiftUC = None,
-        search_cell = False,
-        trans_thresh=1e-5,
-        _correct_Ecut0 = 0.,
-    ):
-        code = code.lower()
-
-        if spin_channel is not None:
-            spin_channel=spin_channel.lower()
-        if spin_channel=='down' : spin_channel='dw'
+    def __init__(self, rot, trans, Lattice, ind=-1, spinor=True):
+        self.ind = ind
+        self.rotation = rot
+        self.Lattice = Lattice
+        self.translation = trans % 1
+        self.translation[1 - self.translation < 1e-5] = 0
+        self.axis, self.angle, self.inversion = self._get_operation_type()
+        iangle = (round(self.angle / pi * 6) + 6) % 12 - 6
+        if iangle == -6:
+            iangle = 6
+        self.angle = iangle * pi / 6
+        self.angle_str = self.get_angle_str()
+        self.spinor = spinor
+        self.spinor_rotation = expm(-0.5j * self.angle *
+                                    np.einsum('i,ijk->jk', self.axis, pauli_sigma))
+        self.sign = 1  # May be changed later externally
+
+    def get_angle_str(self):
+        """
+        Give str of rotation angle.
+
+        Returns
+        -------
+        str
+            Rotation angle in radians.
         
-        if code == "vasp":
-            self.__init_vasp(
-                fWAV, fPOS, Ecut, IBstart, IBend, kplist, spinor, EF=EF, onlysym=onlysym, refUC=refUC, shiftUC=shiftUC, search_cell=search_cell,
-                _correct_Ecut0=_correct_Ecut0, trans_thresh=trans_thresh
-            )
-        elif code == "abinit":
-            self.__init_abinit(
-                fWFK, Ecut, IBstart, IBend, kplist, EF=EF, onlysym=onlysym, refUC=refUC, shiftUC=shiftUC, search_cell=search_cell, trans_thresh=trans_thresh
-            )
-        elif code == "espresso":
-            self.__init_espresso(
-                prefix, Ecut, IBstart, IBend, kplist, EF=EF, onlysym=onlysym, spin_channel=spin_channel, refUC=refUC, shiftUC=shiftUC, search_cell=search_cell, trans_thresh=trans_thresh
-            )
-        elif code == "wannier90":
-            self.__init_wannier(
-                prefix, Ecut, IBstart, IBend, kplist, EF=EF, onlysym=onlysym, refUC=refUC, shiftUC=shiftUC, search_cell=search_cell, trans_thresh=trans_thresh
-            )
+        Raises
+        ------
+        RuntimeError
+            Angle does not belong to 1, 2, 3, 4 or 6-fold rotation.
+        """
+        accur = 1e-4
+        def is_close_int(x): return abs((x + 0.5) % 1 - 0.5) < accur
+        api = self.angle / np.pi
+        if abs(api) < 0.01:
+            return " 0 "
+        for n in 1, 2, 3, 4, 6:
+            if is_close_int(api * n):
+                return "{0:.0f}{1} pi".format(
+                    round(api * n), "" if n == 1 else "/" + str(n))
+        raise RuntimeError(
+            "{0} pi rotation cannot be in the space group".format(api))
+
+    def _get_operation_type(self):
+        """
+        Calculates the rotation axis and angle of the symmetry and if it 
+        preserves handedness or not.
+
+        Returns
+        -------
+        tuple
+            The first element is an array describing the rotation axis. The 
+            second element describes the rotation angle. The third element is a 
+            boolean, `True` if the symmetry preserves handedness 
+            (determinant -1).
+        """
+        rotxyz = self.Lattice.T.dot(
+            self.rotation).dot(
+            np.linalg.inv(
+                self.Lattice).T)
+#        print ("rotation in real space:\n",rotxyz)
+        E, V = np.linalg.eig(rotxyz)
+        if not np.isclose(abs(E), 1).all():
+            raise RuntimeError(
+                "some eigenvalues of the rotation are not unitary")
+        if E.prod() < 0:
+            inversion = True
+            E *= -1
+        else:
+            inversion = False
+        idx = np.argsort(E.real)
+        E = E[idx]
+        V = V[:, idx]
+        axis = V[:, 2].real
+        if np.isclose(E[:2], 1).all():
+            angle = 0
+        elif np.isclose(E[:2], -1).all():
+            angle = np.pi
         else:
-            raise RuntimeError("Unknown/unsupported code :{}".format(code))
+            angle = np.angle(E[0])
+            v = V[:, 0]
+            s = np.real(np.linalg.det([v, v.conj(), axis]) / 1.j)
+            if np.isclose(s, -1):
+                angle = 2 * np.pi - angle
+            elif not np.isclose(s, 1):
+                raise RuntimeError("the sign of rotation should be +-1")
+        return (axis, angle, inversion)
 
-    def __init_vasp(
-        self,
-        fWAV,
-        fPOS,
-        Ecut=None,
-        IBstart=None,
-        IBend=None,
-        kplist=None,
-        spinor=None,
-        EF='0.0',
-        onlysym=False,
-        refUC=None,
-        shiftUC=None,
-        search_cell=False,
-        trans_thresh=1e-5,
-        _correct_Ecut0=0.,
-    ):
+    def rotation_refUC(self, refUC):
         """
-        Initialization for vasp. Read data and save it in attributes.
+        Calculate the matrix of the symmetry in the reference cell choice.
+        
+        Parameters
+        ----------
+        refUC : array
+            3x3 array describing the transformation of vectors defining the 
+            unit cell to the standard setting.
+
+        Returns
+        -------
+        R1 : array, shape=(3,3)
+            Matrix for the transformation of basis vectors forming the 
+            reference unit cell.
+
+        Raises
+        ------
+        RuntimeError
+            If the matrix contains non-integer elements after the transformation.
+        """
+        R = np.linalg.inv(refUC).dot(self.rotation).dot(refUC)
+        R1 = np.array(R.round(), dtype=int)
+        if (abs(R - R1).max() > 1e-6):
+            raise RuntimeError(
+                "the rotation in the reference UC is not integer. Is that OK? \n{0}".format(R))
+        return R1
+
+    def translation_refUC(self, refUC, shiftUC):
+        """
+        Calculate translation in reference choice of unit cell.
 
         Parameters
         ----------
-        fWAV : str, default=None
-            Filename for wavefunction in VASP WAVECAR format.
-        fPOS : str, default=None
-            Filename for wavefunction in VASP POSCAR format.
-        Ecut : float, default=None
-            Plane-wave cutoff in eV to consider in the expansion of wave-functions.
-        IBstart : int, default=None
-            First band to be considered.
-        IBend : int, default=None
-            Last band to be considered.
-        kplist : , default=None
-            List of indices of k-points to be considered.
-        spinor : bool, default=None
-            `True` if wave functions are spinors, `False` if they are scalars.
-        EF : str, default='0.0'
-            Fermi-energy.
-        onlysym : bool, default=False
-            Exit after printing info about space-group.
-        refUC : array, default=None
+        refUC : array
             3x3 array describing the transformation of vectors defining the 
             unit cell to the standard setting.
-        shiftUC : array, default=None
+        shiftUC : array
             Translation taking the origin of the unit cell used in the DFT 
             calculation to that of the standard setting.
-        search_cell : bool, default=False
-            Whether the transformation to the conventional cell should be computed.
-            It is `True` if kpnames was specified in CLI.
-        trans_thresh : float, default=1e-5
-            Threshold to compare translational parts of symmetries.
-        _correct_Ecut0 : float
-            if you get an error like ' computed ncnt=*** != input nplane=*** ', 
-            try to set this parameter to a small positive or negative value (usually of order +- 1e-7)
+
+        Returns
+        -------
+        array
+            Translation in reference choice of unit cell.
         """
-        if spinor is None:
-            raise RuntimeError(
-                "spinor should be specified in the command line for VASP bandstructure"
-            )
-        self.spacegroup = SpaceGroup(
-                inPOSCAR=fPOS,
-                spinor=spinor,
-                refUC=refUC,
-                shiftUC=shiftUC,
-                search_cell=search_cell,
-                trans_thresh=trans_thresh
-                )
-        self.spinor = spinor
-        if onlysym:
-            return
+        t_ref =  - shiftUC + self.translation + self.rotation.dot(shiftUC)
+        t_ref = np.linalg.inv(refUC).dot(t_ref)
+        return t_ref
 
-        if EF.lower() == "auto":
-            self.efermi = 0.0
-            msg = " (Fermi-energy not found in WAVECAR)"
-        else:
-            try:
-                self.efermi = float(EF)
-                msg = ""
-            except:
-                raise RuntimeError(
-                        ("Invalid value for keyword EF. It must be "
-                         "a number or 'auto'")
-                        )
-        print("Efermi = {:.4f} eV".format(self.efermi) + msg)
-        WCF = WAVECARFILE(fWAV)
-        # RECLENGTH=3 # the length of a record in WAVECAR. It is defined in the
-        # first record, so let it be 3 fo far"
-        WCF.rl, ispin, iprec = [int(x) for x in WCF.record(0)]
-        if iprec != 45200:
-            raise RuntimeError("double precision WAVECAR is not supported")
-        if ispin != 1:
-            raise RuntimeError(
-                "WAVECAR contains spin-polarized non-spinor wavefunctions. "
-                + "ISPIN={0}  this is not supported yet".format(ispin)
-            )
-
-        tmp = WCF.record(1)
-        NK = int(tmp[0])
-        NBin = int(tmp[1])
-        Ecut0 = tmp[2]
-
-        IBstart = 0 if (IBstart is None or IBstart <= 0) else IBstart - 1
-        if IBend is None or IBend <= 0 or IBend > NBin:
-            IBend = NBin
-        NBout = IBend - IBstart
-        if NBout <= 0:
-            raise RuntimeError("No bands to calculate")
-        if Ecut is None or Ecut > Ecut0 or Ecut <= 0:
-            Ecut = Ecut0
-        self.Ecut = Ecut
-        self.Ecut0 = Ecut0
-
-        self.Lattice = np.array(tmp[3:12]).reshape(3, 3)
-        self.RecLattice = (
-            np.array(
-                [
-                    np.cross(self.Lattice[(i + 1) % 3], self.Lattice[(i + 2) % 3])
-                    for i in range(3)
-                ]
-            )
-            * 2
-            * np.pi
-            / np.linalg.det(self.Lattice)
-        )
-
-        print(
-            "WAVECAR contains {0} k-points and {1} bands.\n Saving {2} bands starting from {3} in the output".format(
-                NK, NBin, NBout, IBstart + 1
-            )
-        )
-        print("Energy cutoff in WAVECAR : ", Ecut0)
-        print("Energy cutoff reduced to : ", Ecut)
-        #        print (kplist,NK)
 
-        if kplist is None:
-            kplist = range(NK)
-        else:
-            kplist -= 1
-            kplist = np.array([k for k in kplist if k >= 0 and k < NK])
-        #        print (kplist)
-        self.kpoints = [
-            Kpoint(
-                ik,
-                NBin,
-                IBstart,
-                IBend,
-                Ecut,
-                Ecut0*(1.+_correct_Ecut0),
-                self.RecLattice,
-                symmetries_SG=self.spacegroup.symmetries,
-                spinor=self.spinor,
-                WCF=WCF,
-            )
-            for ik in kplist
-        ]
-
-    def __init_abinit(
-        self,
-        WFKname,
-        Ecut=None,
-        IBstart=None,
-        IBend=None,
-        kplist=None,
-        EF='0.0',
-        onlysym=False,
-        refUC=None,
-        shiftUC=None,
-        search_cell = False,
-        trans_thresh=1e-5
-    ):
+    def show(self, refUC=np.eye(3), shiftUC=np.zeros(3)):
         """
-        Initialization for abinit. Read data and store it in attributes.
-
+        Print description of symmetry operation.
+        
         Parameters
         ----------
-        WFKname : str
-            Filename for wavefunction in ABINIT WFK format.
-        Ecut : float, default=None
-            Plane-wave cutoff in eV to consider in the expansion of wave-functions.
-        IBstart : int, default=None
-            First band to be considered.
-        IBend : int, default=None
-            Last band to be considered.
-        kplist : , default=None
-            List of indices of k-points to be considered.
-        EF : str, default='0.0'
-            Fermi-energy.
-        onlysym : bool, default=False
-            Exit after printing info about space-group.
-        refUC : array, default=None
+        refUC : array, default=np.eye(3)
             3x3 array describing the transformation of vectors defining the 
             unit cell to the standard setting.
-        shiftUC : array, default=None
+        shiftUC : array, default=np.zeros(3)
             Translation taking the origin of the unit cell used in the DFT 
             calculation to that of the standard setting.
-        search_cell : bool, default=False
-            Whether the transformation to the conventional cell should be computed.
-            It is `True` if kpnames was specified in CLI.
-        trans_thresh : float, default=1e-5
-            Threshold to compare translational parts of symmetries.
+            
+        Returns
+        -------
+        json_data : `json` object
+            Object with output structured in `json` format.
         """
-
-        header = AbinitHeader(WFKname)
-        usepaw = header.usepaw
-        self.spinor = header.spinor
-        self.spacegroup = SpaceGroup(
-            cell=(header.rprimd, header.xred, header.typat),
-            spinor=self.spinor,
-            refUC=refUC,
-            shiftUC=shiftUC,
-            search_cell=search_cell,
-            trans_thresh=trans_thresh
-        )
-        if onlysym:
-            return
-        if EF.lower() == "auto":
-            self.efermi = header.efermi * Hartree_eV
+        def parse_row_transform(mrow):
+            s = ""
+            coord = ["kx","ky","kz"]
+            is_first = True
+            for i in range(len(mrow)):
+                b = int(mrow[i]) if np.isclose(mrow[i],int(mrow[i])) else mrow[i]
+                if b == 0:
+                    continue
+                if b == 1:
+                    if is_first:
+                        s += coord[i]
+                    else:
+                        s += "+" + coord[i]
+                elif b == -1:
+                    s += "-" + coord[i]
+                else:
+                    if b > 0:
+                        s += "+" + str(b) + coord[i]
+                    else:
+                        s += str(b) + coord[i]
+                is_first = False
+            return s
+
+        if (not np.allclose(refUC, np.eye(3)) or
+            not np.allclose(shiftUC, np.zeros(3))):
+            write_ref = True  # To avoid writing this huge block again
         else:
-            try:
-                self.efermi = float(EF)
-            except:
-                raise RuntimeError(
-                        ("Invalid value for keyword EF. It must be "
-                         "a number or 'auto'")
-                        )
-        print("Efermi: {:.4f} eV".format(self.efermi))
+            write_ref = False
 
-        #        self.spacegroup.show()
+        # Print header
+        print("\n ### {} \n".format(self.ind))
 
-        #        global fWFK
-        fWFK = header.fWFK
-        Ecut0 = header.ecut
-        NBin = header.nband.min()
-        NK = header.nkpt
-        IBstart = 0 if (IBstart is None or IBstart <= 0) else IBstart - 1
-        if IBend is None or IBend <= 0 or IBend > NBin:
-            IBend = NBin
-        NBout = IBend - IBstart
-        if NBout <= 0:
-            raise RuntimeError("No bands to calculate")
-        if Ecut is None or Ecut > Ecut0 or Ecut <= 0:
-            Ecut = Ecut0
-        self.Ecut = Ecut
-        self.Ecut0 = Ecut0
-
-        self.Lattice = header.rprimd
-        print("lattice vectors:\n", self.Lattice)
-        self.RecLattice = (
-            np.array(
-                [
-                    np.cross(self.Lattice[(i + 1) % 3], self.Lattice[(i + 2) % 3])
-                    for i in range(3)
-                ]
-            )
-            * 2
-            * np.pi
-            / np.linalg.det(self.Lattice)
-        )
-
-        print(
-            "WFK contains {0} k-points and {1} bands.\n Saving {2} bands starting from {3} in the output".format(
-                NK, NBin, NBout, IBstart + 1
-            )
-        )
-        print("Energy cutoff in WFK file : ", Ecut0)
-        print("Energy cutoff reduced to : ", Ecut)
-        if kplist is None:
-            kplist = range(NK)
-        else:
-            kplist -= 1
-            kplist = np.array([k for k in kplist if k >= 0 and k < NK])
-        #        print ("kplist",kplist)
-        self.kpoints = []
-        flag = -1
-        for ik in kplist:
-            kp = Kpoint(
-                ik,
-                header.nband[ik],
-                IBstart,
-                IBend,
-                Ecut,
-                Ecut0,
-                self.RecLattice,
-                symmetries_SG=self.spacegroup.symmetries,
-                spinor=self.spinor,
-                code="abinit",
-                kpt=header.kpt[ik],
-                npw_=header.npwarr[ik],
-                fWFK=fWFK,
-                flag=flag,
-                usepaw=usepaw,
-            )
-            self.kpoints.append(kp)
-            flag = ik
-
-    def __init_wannier(
-        self,
-        prefix,
-        Ecut=None,
-        IBstart=None,
-        IBend=None,
-        kplist=None,
-        EF='0.0',
-        onlysym=False,
-        refUC=None,
-        shiftUC=None,
-        search_cell = False,
-        trans_thresh=1e-5,
-    ):
+        # Print rotation part
+        rotstr = [s +
+                  " ".join("{0:3d}".format(x) for x in row) +
+                  t for s, row, t in zip(["rotation : |", " " *
+                                          11 +
+                                          "|", " " *
+                                          11 +
+                                          "|"], self.rotation, [" |", " |", " |"])]
+        if write_ref:
+            fstr = ("{0:3d}")
+            R = self.rotation_refUC(refUC)
+            rotstr1 = [" " *
+                       5 +
+                       s +
+                       " ".join(fstr.format(x) for x in row) +
+                       t for s, row, t in zip(["rotation : |",
+                                               " (refUC)   |",
+                                               " " * 11 + "|"
+                                               ],
+                                              R,
+                                              [" |", " |", " |"])]
+            rotstr = [r + r1 for r, r1 in zip(rotstr, rotstr1)]
+
+        kstring = "gk = [" + ", ".join(
+                    [parse_row_transform(r) for r in np.transpose(np.linalg.inv(self.rotation))]
+                    ) + "]"
+
+        if write_ref:
+            kstring += "  |   refUC:  gk = ["+", ".join(
+                    [parse_row_transform(r) for r in np.transpose(np.linalg.inv(R))]
+                    )+ "]"
+                
+        print("\n".join(rotstr))
+        print("\n\n",kstring)
+
+        # Print spinor transformation matrix
+        if self.spinor:
+            spinstr = [s +
+                       " ".join("{0:6.3f}{1:+6.3f}j".format(x.real, x.imag) for x in row) +
+                       t 
+                       for s, row, t in zip(["\nspinor rot.         : |",
+                                             " " * 22 + "|",
+                                             ], 
+                                             self.spinor_rotation, 
+                                             [" |", " |"]
+                                           )
+                       ]
+            print("\n".join(spinstr))
+            if write_ref:
+                spinstr = [s +
+                           " ".join("{0:6.3f}{1:+6.3f}j".format(x.real, x.imag) for x in row) +
+                           t 
+                           for s, row, t in zip(["spinor rot. (refUC) : |",
+                                                 " " * 22 + "|",
+                                                 ], 
+                                                 self.spinor_rotation*self.sign, 
+                                                 [" |", " |"]
+                                               )
+                           ]
+                print("\n".join(spinstr))
+
+        # Print translation part
+        trastr = ("\ntranslation         :  [ " 
+                  + " ".join("{0:8.4f}"
+                             .format(x%1) for x in self.translation.round(6)
+                             ) 
+                  + " ] "
+                  )
+        print(trastr)
+
+        if write_ref:
+            _t=self.translation_refUC(refUC,shiftUC)
+            trastr = ("translation (refUC) :  [ " 
+                      + " ".join("{0:8.4f}"
+                                 .format(x%1) for x in _t.round(6)
+                                 )
+                  + " ] "
+                  )
+            print(trastr)
+
+        print("\naxis: {0} ; angle = {1}, inversion : {2}\n".format(
+            self.axis.round(6), self.angle_str, self.inversion))
+
+    def str(self, refUC=np.eye(3), shiftUC=np.zeros(3)):
         """
-        Initialization for wannier90. Read data and store it in attibutes.
+        Construct description of symmetry operation.
 
         Parameters
         ----------
-        prefix : str, default=None
-            Prefix used for Quantum Espresso calculations or seedname of Wannier90 
-            files.
-        Ecut : float, default=None
-            Plane-wave cutoff in eV to consider in the expansion of wave-functions.
-        IBstart : int, default=None
-            First band to be considered.
-        IBend : int, default=None
-            Last band to be considered.
-        kplist : , default=None
-            List of indices of k-points to be considered.
-        EF : str, default='0.0'
-            Fermi-energy.
-        onlysym : bool, default=False
-            Exit after printing info about space-group.
-        refUC : array, default=None
+        refUC : array, default=np.eye(3)
             3x3 array describing the transformation of vectors defining the 
             unit cell to the standard setting.
-        shiftUC : array, default=None
+        shiftUC : array, default=np.zeros(3)
             Translation taking the origin of the unit cell used in the DFT 
             calculation to that of the standard setting.
-        search_cell : bool, default=False
-            Whether the transformation to the conventional cell should be computed.
-            It is `True` if kpnames was specified in CLI.
-        trans_thresh : float, default=1e-5
-            Threshold to compare translational parts of symmetries.
-        """
-        if Ecut is None:
-            raise RuntimeError("Ecut mandatory for Wannier90")
-
-        fwin = [l.strip().lower() for l in open(prefix + ".win").readlines()]
 
-        def split(l):
-            """
-            Determine symbol used for assignment and split accordingly.
+        Returns
+        -------
+        str
+            Description to print.
+        """
+#        print ( "symmetry # ",self.ind )
+        R = self.rotation_refUC(refUC)
+        t = self.translation_refUC(refUC, shiftUC)
+#        np.savetxt(stdout,np.hstack( (R,t[:,None])),fmt="%8.5f" )
+        S = self.spinor_rotation
+        return ("   ".join(" ".join(str(x) for x in r) for r in R) + "     " + " ".join(str_(x) for x in t) + ("      " + \
+                "    ".join("  ".join(str_(x) for x in X) for X in (np.abs(S.reshape(-1)), np.angle(S.reshape(-1)) / np.pi))))
+
+    def str2(self, refUC=np.eye(3), shiftUC=np.zeros(3)):
+        """
+        Print matrix of a symmetry operation in the format: 
+        {{R|t}}-> R11,R12,...,R23,R33,t1,t2,t3 and, when SOC was included, the 
+        elements of the matrix describing the transformation of the spinor in 
+        the format:
+        Re(S11),Im(S11),Re(S12),...,Re(S22),Im(S22).
+        
+        Parameters
+        ----------
+        refUC : array, default=np.eye(3)
+            3x3 array describing the transformation of vectors defining the 
+            unit cell to the standard setting.
+        shiftUC : array, default=np.zeros(3)
+            Translation taking the origin of the unit cell used in the DFT 
+            calculation to that of the standard setting.
 
-            Parameters
-            ---------
-            l : str
-                Part of a line read from .win file.
-            """
-            if "=" in l:
-                return l.split("=")
-            elif ":" in l:
-                return l.split(":")
-            else:
-                return l.split()
-
-        fwin = [
-            [s.strip() for s in split(l)]
-            for l in fwin
-            if len(l) > 0 and l[0] not in ("!", "#")
-        ]
-        ind = np.array([l[0] for l in fwin])
-        # print(fwin) #com
+        Returns
+        -------
+        str
+            Description to print.
+        """
+        if refUC is None:
+            refUC = np.eye(3, dtype=int)
+        if shiftUC is None:
+            shiftUC = np.zeros(3, dtype=float)
+# this method for Bilbao server
+#       refUC - row-vectors, expressing the reference unit cell vectors in terms of the lattice used in calculation
+#        print ( "symmetry # ",self.ind )
+        R = self.rotation
+        t = self.translation
+#        np.savetxt(stdout,np.hstack( (R,t[:,None])),fmt="%8.5f" )
+        S = self.spinor_rotation
+        return ("   ".join(" ".join("{0:2d}".format(x) for x in r) for r in R) + "     " + " ".join("{0:10.6f}".format(x) for x in t) + (
+            ("      " + "    ".join("  ".join("{0:10.6f}".format(x) for x in (X.real, X.imag)) for X in S.reshape(-1))) if S is not None else "") + "\n")
+
+    def json_dict(self, refUC=np.eye(3), shiftUC=np.zeros(3)):
+        '''
+        Prepare dictionary with info of symmetry to save in JSON
 
-        def get_param(key, tp, default=None, join=False):
-            """
-            Return value of a parameter in .win file.
+        Returns
+        -------
+        d : dict
+            Dictionary with info about symmetry
+        '''
 
-            Parameters
-            ----------
-            key : str
-                Wannier90 input parameter.
-            tp : function
-                Function to apply to the value of the parameter, before 
-                returning it.
-            default
-                Default value to return in case parameter `key` is not found.
-            join : bool, default=False
-                If the value of parameter `key` contains more than one element, 
-                they will be concatenated with a blank space if `join` is set 
-                to `True`. Used when the parameter is `mpgrid`.
+        d = {}
+        d["axis"]  = self.axis
+        d["angle_str"] = self.angle_str
+        d["angle_pi"] = self.angle/np.pi
+        d["inversion"] = self.inversion
+        d["sign"] = self.sign
 
-            Returns
-            -------
-            Type(`tp`)
-                Return the value of the parameter, after applying function 
-                passed es keyword `tp`.
-
-            Raises
-            ------
-            RuntimeError
-                The parameter is not found in .win file, it is found more than 
-                once or its value is formed by many elements but it is not
-                `mpgrid`.
-            """
-            i = np.where(ind == key)[0]
-            if len(i) == 0:
-                if default is None:
-                    raise RuntimeError(
-                        "parameter {} was not found in {}.win".format(key, prefix)
-                    )
-                else:
-                    return default
-            if len(i) > 1:
-                raise RuntimeError(
-                    "parameter {} was found {} times in {}.win".format(
-                        key, len(i), prefix
-                    )
-                )
-            x = fwin[i[0]][1:]  # mp_grid should work
-            if len(x) > 1:
-                if join:
-                    x = " ".join(x)
-                else:
-                    raise RuntimeError(
-                        "length {} found for parameter {}, rather than lenght 1 in {}.win".format(
-                            len(x), key, prefix
-                        )
-                    )
-            else:
-                x = fwin[i[0]][1]
-            return tp(x)
-
-        NBin = get_param("num_bands", int)
-        #        print ("nbands=",NBin)
-        self.spinor = str2bool(get_param("spinors", str))
+        d["rotation_matrix"] = self.rotation
+        d["translation"] = self.translation
 
-        if EF.lower() == "auto":
-            try:
-                self.efermi = (
-                    get_param("fermi_energy", float, 0.0)
-                    )
-            except:
-                print("WARNING : fermi-energy not found. Setting it as zero")
-        else:
-            try:
-                self.efermi = float(EF)
-            except:
-                raise RuntimeError(
-                        ("Invalid value for keyword EF. It must be "
-                         "a number or 'auto'")
-                        )
-        print("Efermi = {:.4f} eV".format(self.efermi))
+        R = self.rotation_refUC(refUC)
+        t = self.translation_refUC(refUC, shiftUC)
+        d["rotation_matrix_refUC"] = R
+        d["translation_refUC"]= t
 
-        NK = np.prod(np.array(get_param("mp_grid", str).split(), dtype=int))
+        return d
 
-        self.Lattice = None
-        kpred = None
 
-        if kplist is None:
-            kplist = np.arange(NK) + 1
-        else:
-            # kplist-=1 #files start from 1 in W90
-            kplist = np.array([k for k in kplist if k > 0 and k <= NK])
-        found_atoms = False
-        # todo : use an iterator to avoid double looping over lines between
-        # "begin" and "end"
-        iterwin = iter(fwin)
+class SpaceGroup():
+    """
+    Determine the space-group and save info in attributes. Contains methods to 
+    describe and print info about the space-group.
 
-        def check_end(name):
-            """
-            Check if block in .win file is closed.
+    Parameters
+    ----------
+    inPOSCAR : str, default=None 
+        Name of the POSCAR file from which lattice vectors, atomic species and 
+        positions of ions will be read.
+    cell : tuple, default=None
+        `cell[0]` is a 3x3 array where cartesian coordinates of basis 
+        vectors **a**, **b** and **c** are given in rows. `cell[1]` is an array
+        where each row contains the direct coordinates of an ion's position. 
+        `cell[2]` is an array where each element is a number identifying the 
+        atomic species of an ion. See `cell` parameter of function 
+        `get_symmetry` in 
+        `Spglib <https://spglib.github.io/spglib/python-spglib.html#get-symmetry>`_.
+    spinor : bool, default=True
+        `True` if wave-functions are spinors (SOC), `False` if they are scalars.
+    refUC : array, default=None
+        3x3 array describing the transformation of vectors defining the 
+        unit cell to the standard setting.
+    shiftUC : array, default=None
+        Translation taking the origin of the unit cell used in the DFT 
+        calculation to that of the standard setting.
+    search_cell : bool, default=False
+        Whether the transformation to the conventional cell should be computed.
+        It is `True` if kpnames was specified in CLI.
+    trans_thresh : float, default=1e-5
+        Threshold used to compare translational parts of symmetries.
 
-            Parameters
-            ----------
-            name : str
-                Name of the block in .win file.
-            
-            Raises
-            ------
-            RuntimeError
-                Block is not closed.
-            """
-            s = next(iterwin)
-            if " ".join(s) != "end " + name:
-                raise RuntimeError(
-                    "expected 'end {}, found {}'".format(name, " ".join(s))
-                )
+    Attributes
+    ----------
+    spinor : bool
+        `True` if wave-functions are spinors (SOC), `False` if they are scalars.
+    symmetries : list
+        Each element is an instance of class `SymmetryOperation` corresponding 
+        to a symmetry in the point group of the space-group.
+    symmetries_tables : list
+        Attribute `symmetries` of class `IrrepTable`. Each component is an 
+        instance of class `SymopTable` corresponding to a symmetry operation
+        in the "point-group" of the space-group.
+    name : str 
+        Symbol of the space-group in Hermann-Mauguin notation. 
+    number : int 
+        Number of the space-group.
+    Lattice : array, shape=(3,3) 
+        Each row contains cartesian coordinates of a basis vector forming the 
+        unit-cell in real space.
+    RecLattice : array, shape=(3,3)
+        Each row contains the cartesian coordinates of a basis vector forming 
+        the unit-cell in reciprocal space.
 
-        for l in iterwin:
-            if l[0].startswith("begin"):
-                if l[1] == "unit_cell_cart":
-                    if self.Lattice is not None:
-                        raise RuntimeError(
-                            "'begin unit_cell_cart' found more then once  in {}.win".format(
-                                prefix
-                            )
-                        )
-                    j = 0
-                    l1 = next(iterwin)
-                    if l1[0] in ("bohr", "ang"):
-                        units = l1[0]
-                        L = [next(iterwin) for i in range(3)]
-                    else:
-                        units = "ang"
-                        L = [l1] + [next(iterwin) for i in range(2)]
-                    self.Lattice = np.array(L, dtype=float)
-                    if units == "bohr":
-                        self.Lattice *= BOHR
-                    check_end("unit_cell_cart")
-                elif l[1] == "kpoints":
-                    if kpred is not None:
-                        raise RuntimeError(
-                            "'begin kpoints' found more then once  in {}.win".format(
-                                prefix
-                            )
-                        )
-                    kpred = np.array(
-                        [next(iterwin)[:3] for i in range(NK)], dtype=float
-                    )
-                    #                    kpred=np.array([kpred[j].split()[:3] for j in kplist],dtype=float)
-                    check_end("kpoints")
-                elif l[1].startswith("atoms_"):
-                    if l[1][6:10] not in ("cart", "frac"):
-                        raise RuntimeError("unrecognised block :  '{}' ".format(l[0]))
-                    if found_atoms:
-                        raise RuntimeError(
-                            "'begin atoms_***' found more then once  in {}.win".format(
-                                prefix
-                            )
-                        )
-                    found_atoms = True
-                    xred = []
-                    nameat = []
-                    while True:
-                        l1 = next(iterwin)
-                        if l1[0] == "end":
-                            # if l1[1]!=l[0].split()[1]:
-                            if l1[1] != l[1]:
-                                #                                print (l1[1],l[0].split()[1])
-                                raise RuntimeError(
-                                    "'{}' ended with 'end {}'".format(
-                                        " ".join(l), l1[1]
-                                    )
-                                )
-                            break
-                        nameat.append(l1[0])
-                        xred.append(l1[1:4])
-                    typatdic = {n: i + 1 for i, n in enumerate(set(nameat))}
-                    typat = [typatdic[n] for n in nameat]
-                    xred = np.array(xred, dtype=float)
-                    if l[1][6:10] == "cart":
-                        xred = xred.dot(np.linalg.inv(self.Lattice))
-
-        #        print ("lattice vectors:\n",self.Lattice)
-        self.RecLattice = (
-            np.array(
-                [
-                    np.cross(self.Lattice[(i + 1) % 3], self.Lattice[(i + 2) % 3])
-                    for i in range(3)
-                ]
-            )
-            * 2
-            * np.pi
-            / np.linalg.det(self.Lattice)
-        )
-
-        self.spacegroup = SpaceGroup(
-            cell=(self.Lattice, xred, typat),
-            spinor=self.spinor,
-            refUC=refUC,
-            shiftUC=shiftUC,
-            search_cell=search_cell,
-            trans_thresh=trans_thresh
-        )
-        if onlysym:
-            return
+    Notes
+    -----
+    The symmetry operations to which elements in the attribute `symmetries` 
+    correspond are the operations belonging to the point group of the 
+    space-group :math:`G`, i.e. the coset representations :math:`g_i` 
+    taking part in the coset decomposition of :math:`G` w.r.t the translation 
+    subgroup :math:`T`:
+    ..math:: G=T+ g_1 T + g_2 T +...+ g_N T 
+    """
 
-        feig = prefix + ".eig"
-        eigenval = np.loadtxt(prefix + ".eig")
-        try:
-            if eigenval.shape[0] != NBin * NK:
-                raise RuntimeError("wrong number of entries ")
-            ik = np.array(eigenval[:, 1]).reshape(NK, NBin)
-            if not np.all(
-                ik == np.arange(1, NK + 1)[:, None] * np.ones(NBin, dtype=int)[None, :]
-            ):
-                raise RuntimeError("wrong k-point indices")
-            ib = np.array(eigenval[:, 0]).reshape(NK, NBin)
-            if not np.all(
-                ib == np.arange(1, NBin + 1)[None, :] * np.ones(NK, dtype=int)[:, None]
-            ):
-                raise RuntimeError("wrong band indices")
-            eigenval = eigenval[:, 2].reshape(NK, NBin)
-        except Exception as err:
-            raise RuntimeError(" error reading {} : {}".format(feig,err))
-  
-
-        IBstart = 0 if (IBstart is None or IBstart <= 0) else IBstart - 1
-        if IBend is None or IBend <= 0 or IBend > NBin:
-            IBend = NBin
-        NBout = IBend - IBstart
-        if NBout <= 0:
-            raise RuntimeError("No bands to calculate")
-
-        #        print ("eigenvalues are : ",eigenval)
-        self.kpoints = [
-            Kpoint(
-                ik - 1,
-                NBin,
-                IBstart,
-                IBend,
-                Ecut,
-                None,
-                self.RecLattice,
-                symmetries_SG=self.spacegroup.symmetries,
-                spinor=self.spinor,
-                code="wannier",
-                eigenval=eigenval[ik - 1],
-                kpt=kpred[ik - 1],
-            )
-            for ik in kplist
-        ]
-
-    def __init_espresso(
-        self,
-        prefix,
-        Ecut=None,
-        IBstart=None,
-        IBend=None,
-        kplist=None,
-        EF='0.0',
-        onlysym=False,
-        spin_channel=None,
-        refUC=None,
-        shiftUC=None,
-        search_cell = False,
-        trans_thresh=1e-5
-    ):
+    def _findsym(self, cell):
         """
-        Initialization for Quantum Espresso. Read data and store in attributes.
-
+        Finds the space-group and constructs a list of symmetry operations
+        
         Parameters
         ----------
-        prefix : str, default=None
-            Prefix used for Quantum Espresso calculations or seedname of Wannier90 
-            files.
-        Ecut : float, default=None
-            Plane-wave cutoff in eV to consider in the expansion of wave-functions.
-        IBstart : int, default=None
-            First band to be considered.
-        IBend : int, default=None
-            Last band to be considered.
-        kplist : , default=None
-            List of indices of k-points to be considered.
-        EF : str, default='0.0'
-            Fermi-energy.
-        onlysym : bool, default=False
-            Exit after printing info about space-group.
-        spin_channel : str, default=None
-            Selection of the spin-channel. 'up' for spin-up, 'dw' for spin-down.
-        refUC : array, default=None
+        inPOSCAR : str, default=None 
+            POSCAR file from which lattice vectors, atomic species and positions of
+            ions will be read.
+        cell : list
+            `cell[0]` is a 3x3 array where cartesian coordinates of basis 
+            vectors **a**, **b** and **c** are given in rows. `cell[1]` is an array
+            where each row contains the direct coordinates of an ion's position. 
+            `cell[2]` is an array where each element is a number identifying the 
+            atomic species of an ion. See `cell` parameter of function 
+            `get_symmetry` in 
+            `Spglib <https://spglib.github.io/spglib/python-spglib.html#get-symmetry>`_.
+        
+        Returns
+        -------
+        list
+            Each element is an instance of class `SymmetryOperation` corresponding 
+            to a symmetry in the point group of the space-group.
+        str
+            Symbol of the space-group in Hermann-Mauguin notation. 
+        int
+            Number of the space-group.
+        array
+            3x3 array where cartesian coordinates of basis  vectors **a**, **b** 
+            and **c** are given in rows. 
+        array
             3x3 array describing the transformation of vectors defining the 
-            unit cell to the standard setting.
-        shiftUC : array, default=None
+            unit cell to the convenctional setting.
+        array
             Translation taking the origin of the unit cell used in the DFT 
-            calculation to that of the standard setting.
-        search_cell : bool, default=False
-            Whether the transformation to the conventional cell should be computed.
-            It is `True` if kpnames was specified in CLI.
-        trans_thresh : float, default=1e-5
-            Threshold to compare translational parts of symmetries.
-        """
-        import xml.etree.ElementTree as ET
-
-        mytree = ET.parse(prefix + ".save/data-file-schema.xml")
-        myroot = mytree.getroot()
-
-        inp = myroot.find("input")
-        outp = myroot.find("output")
-        bandstr = outp.find("band_structure")
-        ntyp = int(inp.find("atomic_species").attrib["ntyp"])
-        atnames = [
-            sp.attrib["name"] for sp in inp.find("atomic_species").findall("species")
-        ]
-        assert len(atnames) == ntyp
-        atnumbers = {atn: i + 1 for i, atn in enumerate(atnames)}
-        self.spinor = str2bool(bandstr.find("noncolin").text)
-        #        print ('spinor=',self.spinor)
-        struct = inp.find("atomic_structure")
-        nat = struct.attrib["nat"]
-        self.Lattice = BOHR * np.array(
-            [
-                struct.find("cell").find("a{}".format(i + 1)).text.strip().split()
-                for i in range(3)
-            ],
-            dtype=float,
-        )
-        xcart = []
-        typat = []
-        for at in struct.find("atomic_positions").findall("atom"):
-            typat.append(atnumbers[at.attrib["name"]])
-            xcart.append(at.text.split())
-        xred = (np.array(xcart, dtype=float) * BOHR).dot(np.linalg.inv(self.Lattice))
-        #        print ("xred=",xred)
-        self.spacegroup = SpaceGroup(
-            cell=(self.Lattice, xred, typat),
-            spinor=self.spinor,
-            refUC=refUC,
-            shiftUC=shiftUC,
-            search_cell=search_cell,
-            trans_thresh=trans_thresh
-        )
-        if onlysym:
-            return
-        Ecut0 = float(inp.find("basis").find("ecutwfc").text) * Hartree_eV
+            calculation to that of the standard setting of spglib. It may not be
+            the shift taking to the convenctional cell of tables; indeed, in 
+            centrosymmetric groups they adopt origin choice 1 of ITA, rather 
+            than choice 2 (BCS).
+        """
+        dataset = spglib.get_symmetry_dataset(cell)
+        symmetries = [
+            SymmetryOperation(
+                rot,
+                dataset['translations'][i],
+                cell[0],
+                ind=i + 1,
+                spinor=self.spinor) for i,
+            rot in enumerate(
+                dataset['rotations'])]
+        nsym = len(symmetries)
+
+        return (symmetries, 
+                dataset['international'],
+                dataset['number'], 
+                dataset['transformation_matrix'],
+                dataset['origin_shift']
+                )
 
-        IBstartE=0
+    def __init__(
+            self,
+            cell,
+            spinor=True,
+            refUC=None,
+            shiftUC=None,
+            search_cell=False,
+            trans_thresh=1e-5
+            ):
+        self.spinor = spinor
+        self.Lattice = cell[0]
+        self.positions = cell[1]
+        self.typat = cell[2]
+        (self.symmetries, 
+         self.name, 
+         self.number, 
+         refUC_tmp, 
+         shiftUC_tmp) = self._findsym(cell)
+        self.RecLattice = np.array([np.cross(self.Lattice[(i + 1) %
+                                                          3], self.Lattice[(i + 2) %
+                                                                           3]) for i in range(3)]) * 2 * np.pi / np.linalg.det(self.Lattice)
+        self.order = len(self.symmetries)
+
+        # Determine refUC and shiftUC according to entries in CLI
+        self.symmetries_tables = IrrepTable(self.number, self.spinor).symmetries
+        self.refUC, self.shiftUC = self.determine_basis_transf(
+                                            refUC_cli=refUC, 
+                                            shiftUC_cli=shiftUC,
+                                            refUC_lib=refUC_tmp, 
+                                            shiftUC_lib=shiftUC_tmp,
+                                            search_cell=search_cell,
+                                            trans_thresh=trans_thresh
+                                            )
+
+        # Check matching of symmetries in refUC. If user set transf.
+        # in the CLI and symmetries don't match, raise a warning.
+        # Otherwise, transf. was calculated automatically and 
+        # matching of symmetries was checked in determine_basis_transf
         try:
-            NBin_dw=int(bandstr.find('nbnd_dw').text)
-            NBin_up=int(bandstr.find('nbnd_up').text)
-            spinpol=True
-            print ("spin-polarised bandstructure composed of {} up and {} dw states".format(NBin_dw,NBin_up))
-            NBin_dw+NBin_up
-        except AttributeError as err: 
-            spinpol=False
-            NBin=int(bandstr.find('nbnd').text)
-
-
-        IBstartE=0
-        if self.spinor and spinpol:
-            raise RuntimeError("bandstructure cannot be both noncollinear and spin-polarised. Smth is wrong with the 'data-file-schema.xml'")
-        if spinpol :
-            if spin_channel is None:
-                raise ValueError("Need to select a spin channel for spin-polarised calculations set  'up' or 'dw'")
-            assert (spin_channel in ['dw','up'])
-            if spin_channel=='dw':
-                IBstartE=NBin_up
-                NBin=NBin_dw
-            else : 
-                NBin=NBin_up
-        else :
-            if spin_channel is not None:
-                raise ValueError("Found a non-polarized bandstructure, but spin channel is set to {}".format(spin_channel))
-
-
-        IBstart = 0 if (IBstart is None or IBstart <= 0) else IBstart - 1
-        if IBend is None or IBend <= 0 or IBend > NBin:
-            IBend = NBin
-        NBout = IBend - IBstart
-        if NBout <= 0:
-            raise RuntimeError("No bands to calculate")
-        if Ecut is None or Ecut > Ecut0 or Ecut <= 0:
-            Ecut = Ecut0
-
-        self.Ecut = Ecut
-        self.RecLattice = (
-            np.array(
-                [
-                    np.cross(self.Lattice[(i + 1) % 3], self.Lattice[(i + 2) % 3])
-                    for i in range(3)
-                ]
-            )
-            * 2
-            * np.pi
-            / np.linalg.det(self.Lattice)
-        )
-        
-        if EF.lower() == "auto":
-            try:
-                self.efermi = (
-                               float(bandstr.find("fermi_energy").text) 
-                               * Hartree_eV
-                               )
-            except:
-                print("WARNING : fermi-energy not found. Setting it as zero")
-                self.efermi = 0.0
-        else:
-            try:
-                self.efermi = float(EF)
-            except:
-                raise RuntimeError(
-                        ("Invalid value for keyword EF. It must be "
-                         "a number or 'auto'")
-                        )
-        print("Efermi: {:.4f} eV".format(self.efermi))
+            ind, dt, signs = self.match_symmetries(signs=self.spinor,
+                                                   trans_thresh=trans_thresh
+                                                   )
+            # Sort symmetries like in tables
+            args = np.argsort(ind)
+            for i,i_ind in enumerate(args):
+                self.symmetries[i_ind].ind = i+1
+                self.symmetries[i_ind].sign = signs[i_ind]
+                self.symmetries.append(self.symmetries[i_ind])
+            self.symmetries = self.symmetries[i+1:]
+        except RuntimeError:
+            if search_cell:  # symmetries must match to identify irreps
+                raise RuntimeError((
+                    "refUC and shiftUC don't transform the cellto one where "
+                    "symmetries are identical to those read from tables. "
+                    "Try without specifying refUC and shiftUC."
+                    ))
+            elif refUC is not None or shiftUC is not None:
+                # User specified refUC or shiftUC in CLI. He/She may
+                # want the traces in a cell that is not neither the
+                # one in tables nor the DFT one
+                print(("WARNING: refUC and shiftUC don't transform the cell to "
+                       "one where symmetries are identical to those read from "
+                       "tables. If you want to achieve the same cell as in "
+                       "tables, try not specifying refUC and shiftUC."))
+                pass
+
+    def json(self, symmetries=None):
+        '''
+        Prepare dictionary with info of space group to save in JSON
 
-        kpall = bandstr.findall("ks_energies")
-        NK = len(kpall)
-        if kplist is None:
-            kplist = np.arange(NK)
+        Returns
+        -------
+        d : dict
+            Dictionary with info about space group
+        '''
+
+        d = {}
+
+        if (np.allclose(self.refUC, np.eye(3)) and
+            np.allclose(self.shiftUC, np.zeros(3))):
+            cells_match = True
         else:
-            kplist -= 1
-            kplist = np.array([k for k in kplist if k >= 0 and k < NK])
-        #        print ("kplist",kplist)
-        #        for kp in kpall:
-        #            print(kp.find('k_point').text)
-        self.kpoints = []
-        flag = -1
-        for ik in kplist:
-            kp = Kpoint(
-                ik,
-                NBin,
-                IBstart,
-                IBend,
-                Ecut,
-                Ecut0,
-                self.RecLattice,
-                symmetries_SG=self.spacegroup.symmetries,
-                spinor=self.spinor,
-                code="espresso",
-                kptxml=kpall[ik],
-                prefix=prefix,
-                spin_channel=spin_channel,
-                IBstartE=IBstartE
-            )
-            self.kpoints.append(kp)
-            flag = ik
-
-    #        tagname= mytree.getElementsByTagName('item')[0]
-    #        print(tagname)
-    # If I try to fetch the first ele
-    #        myroot = mytree.getroot()
-    #        print (myroot)
-    #        exit()
-
-    def getNK():
-        """Getter for `self.kpoints`."""
-        return len(self.kpoints)
-
-    NK = property(getNK)
-
-    def write_characters(
-        self,
-        degen_thresh=1e-8,
-        kpnames=None,
-        symmetries=None,
-        preline="",
-        plotFile=None,
-    ):
-        """
-        Calculate irreps, number of band-inversion (if little-group contains 
-        inversion), smallest direct gap and indirect gap and print all of them.
+            cells_match = False
+
+        d = {"name": self.name,
+             "number": self.number,
+             "spinor": self.spinor,
+             "num_symmetries": self.order,
+             "cells_match": cells_match,
+             "symmetries": {}
+             }
+
+        for sym in self.symmetries:
+            if symmetries is None or sym.ind in symmetries:
+                d["symmetries"][sym.ind] = sym.json_dict(self.refUC, self.shiftUC)
+
+        return d
 
+    def show(self, symmetries=None):
+        """
+        Print description of space-group and symmetry operations.
+        
         Parameters
         ----------
-        degen_thresh : float, default=1e-8
-            Threshold energy used to decide whether wave-functions are
-            degenerate in energy.
-        refUC : array, default=None
-            3x3 array describing the transformation of vectors defining the 
-            unit cell to the standard setting.
-        shiftUC : array, default=np.zeros(3)
-            Translation taking the origin of the unit cell used in the DFT 
-            calculation to that of the standard setting.
-        kpnames : list, default=None
-            Labels of maximal k-points at which irreps of bands must be computed. 
-            If it is not specified, only traces will be printed, not irreps.
-        symmetries : list, default=None
+        symmetries : int, default=None
             Index of symmetry operations whose description will be printed. 
-        preline : str, default=''
-            Characters to write before labels of irreps in file `irreps.dat`.
-        plotFile : str, default=None
-            Name of file in which energy-levels and corresponding irreps will be 
-            written to later place irreps in a band structure plot.
+            Run `IrRep` with flag `onlysym` to check the index corresponding 
+            to each symmetry operation.
 
         Returns
         -------
         json_data : `json` object
             Object with output structured in `json` format.
         """
-        #        if refUC is not None:
-        #        self.spacegroup.show(refUC=refUC,shiftUC=shiftUC)
-        #        self.spacegroup.show2(refUC=refUC)
-        kpline = self.KPOINTSline()
-        json_data = {}
-        json_data[ "kpoints_line"] = kpline
-        try:
-            pFile = open(plotFile, "w")
-        except BaseException:
-            pFile = None
-        NBANDINV = 0
-        GAP = np.Inf
-        Low = -np.Inf
-        Up = np.inf
-        json_data["k-points" ] = []
-        if kpnames is not None:
-            for kpname, KP in zip(kpnames, self.kpoints):
-                irreps = self.spacegroup.get_irreps_from_table(kpname, KP.K)
-                ninv, low, up , kdata = KP.write_characters(
-                    degen_thresh,
-                    irreptable=irreps,
-                    symmetries=symmetries,
-                    preline=preline,
-                    efermi=self.efermi,
-                    plotFile=pFile,
-                    kpl=kpline,
-                    symmetries_tables=self.spacegroup.symmetries_tables,
-                    refUC=self.spacegroup.refUC,
-                    shiftUC=self.spacegroup.shiftUC
-                )
-                kdata["kpname"] = kpname
-                json_data["k-points" ].append(kdata)
 
-                NBANDINV += ninv
-                GAP = min(GAP, up - low)
-                Up = min(Up, up)
-                Low = max(Low, low)
-        else:
-            for KP, kpl in zip(self.kpoints, kpline):
-                ninv, low, up , kdata = KP.write_characters(
-                    degen_thresh,
-                    symmetries=symmetries,
-                    preline=preline,
-                    efermi=self.efermi,
-                    plotFile=pFile,
-                    kpl=kpl,
-                    symmetries_tables=self.spacegroup.symmetries_tables,
-                    refUC=self.spacegroup.refUC,
-                    shiftUC=self.spacegroup.shiftUC
-                )
-                kdata["kp in line"] = kpl
-                json_data["k-points" ].append(kdata)
-                NBANDINV += ninv
-                GAP = min(GAP, up - low)
-                Up = min(Up, up)
-                Low = max(Low, low)
 
-        if self.spinor:
-            print(
-                "number of inversions-odd Kramers pairs IN THE LISTED KPOINTS: ",
-                int(NBANDINV / 2),
-                "  Z4= ",
-                int(NBANDINV / 2) % 4,
-            )
-            json_data["number of inversions-odd Kramers pairs"]  = int(NBANDINV / 2)
-            json_data["Z4"] = int(NBANDINV / 2) % 4,
+        if (not np.allclose(self.refUC, np.eye(3)) or
+            not np.allclose(self.shiftUC, np.zeros(3))):
+            write_ref = True  # To avoid writing this huge block again
         else:
-            print("number of inversions-odd states : ", NBANDINV)
-            json_data["number of inversions-odd states"]  = NBANDINV
+            write_ref = False
 
-        #        print ("Total number of inversion-odd Kramers pairs IN THE LISTED KPOINTS: ",NBANDINV,"  Z4= ",NBANDINV%4)
-        print("Minimal direct gap:", GAP, " eV")
-        print("indirect  gap:", Up - Low, " eV")
-        json_data["indirect gap (eV)"] =  Up-Low
-        json_data["Minimal direct gap (eV)"] =  GAP
-       
-        return json_data
+        print('')
+        print("\n ---------- CRYSTAL STRUCTURE ---------- \n")
+        print('')
+
+        # Print cell vectors in DFT and reference cells
+        vecs_refUC = np.dot(self.Lattice, self.refUC).T
+        print('Cell vectors in angstroms:\n')
+        print('{:^32}|{:^32}'.format('Vectors of DFT cell', 'Vectors of REF. cell'))
+        for i in range(3):
+            vec1 = self.Lattice[i]
+            vec2 = vecs_refUC[i]
+            s = 'a{:1d} = {:7.4f}  {:7.4f}  {:7.4f}  '.format(i, vec1[0], vec1[1], vec1[2])
+            s += '|  '
+            s += 'a{:1d} = {:7.4f}  {:7.4f}  {:7.4f}'.format(i, vec2[0], vec2[1], vec2[2])
+            print(s)
+        print()
+
+        # Print atomic positions
+        print('Atomic positions in direct coordinates:\n')
+        print('{:^} | {:^25} | {:^25}'.format('Atom type', 'Position in DFT cell', 'Position in REF cell'))
+        positions_refUC = self.positions.dot(np.linalg.inv(self.refUC.T))
+        for itype, pos1, pos2 in zip(self.typat, self.positions, positions_refUC):
+            s = '{:^9d}'.format(itype)
+            s += ' | '
+            s += '  '.join(['{:7.4f}'.format(x) for x in pos1])
+            s += ' | '
+            s += '  '.join(['{:7.4f}'.format(x) for x in pos2])
+            print(s)
+
+        print()
+        print('\n ---------- SPACE GROUP ----------- \n')
+        print()
+        print('Space group: {} (# {})'.format(self.name, self.number))
+        print('Number of symmetries: {} (mod. lattice translations)'.format(self.order))
+        refUC_print = self.refUC.T  # print following convention in paper
+        print("\nThe transformation from the DFT cell to the reference cell of tables is given by: \n"
+              + "        | {} |\n".format("".join(["{:8.4f}".format(el) for el in refUC_print[0]]))
+              + "refUC = | {} |    shiftUC = {}\n".format("".join(["{:8.4f}".format(el) for el in refUC_print[1]]), np.round(self.shiftUC, 5))
+              + "        | {} |\n".format("".join(["{:8.4f}".format(el) for el in refUC_print[2]]))
+              )
+
+        for symop in self.symmetries:
+            if symmetries is None or symop.ind in symmetries:
+                symop.show(refUC=self.refUC, shiftUC=self.shiftUC)
+
+
+    def write_trace(self):
+        """
+        Construct description of matrices of symmetry operations of the 
+        space-group in the format: 
+        {{R|t}}-> R11,R12,...,R23,R33,t1,t2,t3 and, when SOC was included, the 
+        elements of the matrix describing the transformation of the spinor in 
+        the format:
+        Re(S11),Im(S11),Re(S12),...,Re(S22),Im(S22).
 
-    def getNbands(self):
+        Returns
+        -------
+        str
+            String describing matrices of symmetry operations.
         """
-        Return number of bands (if equal over all k-points), raise RuntimeError 
-        otherwise.
+        res = (" {0} \n"  # Number of Symmetry operations
+               # In the following lines, one symmetry operation for each operation of the point group n"""
+               ).format(len(self.symmetries))
+        for symop in self.symmetries:
+            res += symop.str2(refUC=self.refUC, shiftUC=self.shiftUC)
+        return(res)
+
+    def str(self):
+        """
+        Print description of space-group and its symmetry operations.
 
         Returns
         -------
-        int
-            Number of bands in every k-point.
+        str
+            Description to print.
         """
-        nbarray = [k.Nband for k in self.kpoints]
-        if len(set(nbarray)) > 1:
-            raise RuntimeError(
-                "the numbers of bands differs over k-points:{0} \n cannot write trace.txt \n".format(
-                    nbarray
-                )
-            )
-        if len(nbarray) == 0:
-            raise RuntimeError(
-                "do we have any k-points??? NB={0} \n cannot write trace.txt \n".format(
-                    nbarray
-                )
-            )
-        return nbarray[0]
+        return (
+            "SG={SG}\n name={name} \n nsym= {nsym}\n spinor={spinor}\n".format(
+                SG=self.number,
+                name=self.name,
+                nsym=len(
+                    self.symmetries),
+                spinor=self.spinor) +
+            "symmetries=\n" +
+            "\n".join(
+                s.str(
+                    self.refUC,
+                    self.shiftUC) for s in self.symmetries) +
+            "\n\n")
 
-    def write_trace(
-        self,
-        degen_thresh=1e-8,
-        kpnames=None,
-        symmetries=None,
-    ):
+    def __match_spinor_rotations(self, S1, S2):
         """
-        Generate `trace.txt` file to upload to the program `CheckTopologicalMat` 
-        in `BCS <https://www.cryst.ehu.es/cgi-bin/cryst/programs/topological.pl>`_ .
+        Determine the sign difference between matrices describing the 
+        transformation of spinors found by `spglib` and those read from tables.
 
         Parameters
         ----------
-        degen_thresh : float, default=1e-8
-            Threshold energy used to decide whether wave-functions are
-            degenerate in energy.
-        kpnames : list, default=None
-            Labels of maximal k-points at which irreps of bands must be computed. 
-            If it is not specified, only traces will be printed, not irreps.
-        symmetries : list, default=None
-            Index of symmetry operations whose description will be printed. 
+        S1 : list
+            Contains the matrices for the transformation of spinors 
+            corresponding to symmetry operations found by `spglib`.
+        S2 : list
+            Contains the matrices for the transformation of spinors 
+            corresponding to symmetry operations read from tables.
+
+        Returns
+        -------
+        array
+            The `j`-th element is the matrix to match the `j`-th matrices of 
+            `S1` and `S2`.
         """
-        f = open("trace.txt", "w")
-        f.write(
-            (
-                " {0}  \n"
-                + " {1}  \n"  # Number of bands below the Fermi level  # Spin-orbit coupling. No: 0, Yes: 1
-            ).format(self.getNbands(), 1 if self.spinor else 0)
-        )
+        #        for s1,s2 in zip (S1,S2):
+        #            np.savetxt(stdout,np.hstack( (s1,s2) ),fmt="%8.5f%+8.5fj "*4)
+        n = 2
 
-        f.write(
-                self.spacegroup.write_trace()
-                )
-        # Number of maximal k-vectors in the space group. In the next files
-        # introduce the components of the maximal k-vectors))
-        f.write("  {0}  \n".format(len(self.kpoints)))
-        for KP in self.kpoints:
-            f.write(
-                "   ".join(
-                    "{0:10.6f}".format(x)
-                    for x in KP.K
-                )
-                + "\n"
-            )
-        for KP in self.kpoints:
-            f.write(
-                KP.write_trace(degen_thresh, symmetries=symmetries, efermi=self.efermi)
-            )
+        def RR(x): 
+            """
+            Constructs a 2x2 complex matrix out of a list containing real and 
+            imaginary parts.
 
-    def Separate(self, isymop, degen_thresh=1e-5, groupKramers=True):
+            Parameters
+            ----------
+            x : list, length=8
+                Length is 8. `x[:4]` contains the real parts, `x[4:]` the 
+                imaginary parts.
+            
+            Returns
+            -------
+            array, shape=(2,2)
+                Matrix of complex elements. 
+            """
+            return np.array([[x1 + 1j * x2 for x1, x2 in zip(l1, l2)] for l1, l2 in zip(x[:n * n].reshape((n, n)), x[n * n:].reshape((n, n)))])
+
+        def residue_matrix(r): 
+            """
+            Calculate the residue of a matrix.
+
+            Parameters
+            ----------
+            r : array
+                Matrix used as ansatz for the minimization.
+
+            Returns
+            -------
+            float            
+            """
+            return sum([min(abs(r.dot(b).dot(r.T.conj()) - s * a).sum() for s in (1, -1)) for a, b in zip(S1, S2)])
+
+        def residue(x): 
+            """
+            Calculate the normalized residue.
+
+            Parameters
+            ----------
+            x : list, length=8
+                Length is 8. `x[:4]` contains the real parts, `x[4:]` the 
+                imaginary parts.
+            
+            Returns
+            -------
+            float
+            """
+            return residue_matrix(RR(x)) / len(S1)
+
+        for i in range(11):
+            x0 = np.random.random(2 * n * n)
+            res = minimize(residue, x0)
+            r = res.fun
+#            print("accuracy achieved : ",r)
+            if r < 1e-4:
+                break
+        if r > 1e-3:
+            raise RuntimeError(
+                "the accurcy is only {0}. Is this good?".format(r))
+
+        R1 = RR(res.x)
+#        print ("R=")
+#        np.savetxt(stdout,np.hstack( (abs(R1),np.angle(R1)/np.pi) ),fmt="%8.5f")
+
+        return np.array([R1.dot(b).dot(R1.T.conj()).dot(np.linalg.inv(
+            a)).diagonal().mean().real.round() for a, b in zip(S1, S2)], dtype=int)
+
+    def __gen_refUC():
+        '''used somewhere?'''
+        nmax = 3
+
+    def get_irreps_from_table(self, kpname, K):
         """
-        Separate band structure according to the eigenvalues of a symmetry 
-        operation.
+        Read irreps of the little-group of a maximal k-point. 
         
         Parameters
         ----------
-        isymop : int
-            Index of symmetry used for the separation.
-        degen_thresh : float, default=1e-5
-            Energy threshold used to determine degeneracy of energy-levels.
-        groupKramers : bool, default=True
-            If `True`, states will be coupled by Kramers' pairs.
+        kpname : str
+            Label of the maximal k-point.
+        K : array, shape=(3,)
+            Direct coordinates of the k-point.
 
         Returns
         -------
-        subspaces : dict
-            Each key is an eigenvalue of the symmetry operation and the
-            corresponding value is an instance of `class` `BandStructure` for 
-            the subspace of that eigenvalue.
-        """
-        if isymop == 1:
-            return {1: self}
-        symop = self.spacegroup.symmetries[isymop - 1]
-        #print("Separating by symmetry operation # ", isymop)
-        symop.show()
-        kpseparated = [
-            kp.Separate(symop, degen_thresh=degen_thresh, groupKramers=groupKramers)
-            for kp in self.kpoints
-        ] # each element is a dict with separated bandstructure of a k-point
-        allvalues = np.array(sum((list(kps.keys()) for kps in kpseparated), []))
-        #        print (allvalues)
-        #        for kps in kpseparated :
-        #            allvalues=allvalues | set( kps.keys())
-        #        allvalues=np.array(allavalues)
-        if groupKramers:
-            allvalues = allvalues[np.argsort(np.real(allvalues))].real
-            borders = np.hstack(
-                (
-                    [0],
-                    np.where(abs(allvalues[1:] - allvalues[:-1]) > 0.01)[0] + 1,
-                    [len(allvalues)],
-                )
-            )
-            #            nv=len(allvalues)
-            if len(borders) > 2:
-                allvalues = set(
-                    [allvalues[b1:b2].mean() for b1, b2 in zip(borders, borders[1:])]
-                ) # unrepeated Re parts of all eigenvalues
-                subspaces = {}
-                for v in allvalues:
-                    other = copy.copy(self)
-                    other.kpoints = []
-                    for K in kpseparated:
-                        vk = list(K.keys())
-                        vk0 = vk[np.argmin(np.abs(v - vk))]
-                        if abs(vk0 - v) < 0.05:
-                            other.kpoints.append(K[vk0])
-                    subspaces[v] = other # unnecessary indent ?
-                return subspaces
-            else:
-                return dict({allvalues.mean(): self})
-        else:
-            allvalues = allvalues[np.argsort(np.angle(allvalues))]
-            print("allvalues:", allvalues)
-            borders = np.where(abs(allvalues - np.roll(allvalues, 1)) > 0.01)[0]
-            nv = len(allvalues)
-            if len(borders) > 0:
-                allvalues = set(
-                    [
-                        np.roll(allvalues, -b1)[: (b2 - b1) % nv].mean()
-                        for b1, b2 in zip(borders, np.roll(borders, -1))
-                    ]
-                )
-                print("distinct values:", allvalues)
-                subspaces = {}
-                for v in allvalues:
-                    other = copy.copy(self)
-                    other.kpoints = []
-                    for K in kpseparated:
-                        vk = list(K.keys())
-                        vk0 = vk[np.argmin(np.abs(v - vk))]
-                        #                    print ("v,vk",v,vk)
-                        #                    print ("v,vk",v,vk[np.argmin(np.abs(v-vk))])
-                        if abs(vk0 - v) < 0.05:
-                            other.kpoints.append(K[vk0])
-                        subspaces[v] = other
-                return subspaces
-            else:
-                return dict({allvalues.mean(): self})
+        tab : dict
+            Each key is the label of an irrep, each value another `dict`. Keys 
+            of every secondary `dict` are indices of symmetries (starting from 
+            1 and following order of operations in tables of BCS) and 
+            values are traces of symmetries.
+
+        Raises
+        ------
+        RuntimeError
+            Translational or rotational parts read from tables and found by 
+            `spglib` do not match for a symmetry operation.
+        RuntimeError
+            A symmetry from the tables matches with many symmetries found by 
+            `spglib`.
+        RuntimeError
+            The label of a k-point given in the CLI matches with the label of a 
+            k-point read from tables, but direct coordinates of these 
+            k-vectors do not match.
+        RuntimeError
+            There is not any k-point in the tables whose label matches that 
+            given in parameter `kpname`.
+        """
+        #        self.show()
+        table = IrrepTable(self.number, self.spinor)
+        tab = {}
+        for irr in table.irreps:
+            if irr.kpname == kpname:
+                k1 = np.round(np.linalg.inv(self.refUC.T).dot(irr.k), 5) % 1
+                k2 = np.round(K, 5) % 1
+                if not all(np.isclose(k1, k2)):
+                    raise RuntimeError(
+                        "the kpoint {0} does not correspond to the point {1} ({2} in refUC / {3} in primUC) in the table".format(
+                            K,
+                            kpname,
+                            np.round(
+                                irr.k,
+                                3),
+                            k1))
+#            print (irr.characters)
+                tab[irr.name] = {}
+                for i,(sym1,sym2) in enumerate(zip(self.symmetries,table.symmetries)):
+                    try:
+                        dt = sym2.t - sym1.translation_refUC(self.refUC, self.shiftUC)
+                        tab[irr.name][i + 1] = irr.characters[i + 1] * \
+                            sym1.sign * np.exp(2j * np.pi * dt.dot(irr.k))
+                    except KeyError as err:
+                        pass
+        if len(tab) == 0:
+            raise RuntimeError(
+                "the k-point with name {0} is not found in the spacegroup {1}. found only :\n{2}".format(
+                    kpname, table.number, "\n ".join(
+                        "{0}({1}/{2})".format(
+                            irr.kpname, irr.k, np.linalg.inv(self.refUC).dot(
+                                irr.k) %
+                            1) for irr in table.irreps)))
+#            raise RuntimeError("the k-point with name {0} is not found in the spacegroup {1}. found only {2}".format(kpname,table.number,set([irr.kpname for irr in table.irreps]) ) )
+        return tab
+
+#            irr.characters[i]
+# return( { irr.name: np.array([irr.characters[i]*signs[j] for j,i in
+# enumerate(ind)]) for irr in table.irreps if irr.kpname==kpname})
+
+    def determine_basis_transf(
+            self,
+            refUC_cli,
+            shiftUC_cli,
+            refUC_lib,
+            shiftUC_lib,
+            search_cell,
+            trans_thresh
+            ):
+        """ 
+        Determine basis transformation to conventional cell. Priority
+        is given to the transformation set by the user in CLI.
 
-    def zakphase(self):
-        """
-        Calculate Zak phases along a path for a set of states.
+        Parameters
+        ----------
+        refUC_cli : array
+            3x3 array describing the transformation of vectors defining the 
+            unit cell to the standard setting. Set in CLI.
+        shiftUC_cli : array
+            Translation taking the origin of the unit cell used in the DFT 
+            calculation to that of the standard setting. Set in CLI.
+        refUC_lib : array
+            Obtained via spglib.
+        shiftUC_lib : array
+            Obtained via spglib. It may not be the shift taking the
+            origin to the position adopted in the tables (BCS). For 
+            example, origin choice 1 of ITA is adopted in spglib for 
+            centrosymmetric groups, while origin choice 2 in BCS.
+        search_cell : bool, default=False
+            Whether the transformation to the conventional cell should be computed.
+            It is `True` if kpnames was specified in CLI.
+        trans_thresh : float, default=1e-5
+            Threshold to compare translational parts of symmetries.
 
         Returns
         -------
-        z : array
-            `z[i]` contains the total  (trace) zak phase (divided by 
-            :math:`2\pi`) for the subspace of the first i-bands.
-        array
-            The :math:`i^{th}` element is the gap between :math:`i^{th}` and
-            :math:`(i+1)^{th}` bands in the considered set of bands. 
+        array 
+            Transformation of vectors defining the unit cell to the 
+            standard setting.
         array
-            The :math:`i^{th}` element is the mean energy between :math:`i^{th}` 
-            and :math:`(i+1)^{th}` bands in the considered set of bands. 
-        array
-            Each line contains the local gaps between pairs of bands in a 
-            k-point of the path. The :math:`i^{th}` column is the local gap 
-            between :math:`i^{th}` and :math:`(i+1)^{th}` bands.
-        """
-        overlaps = [
-            x.overlap(y)
-            for x, y in zip(self.kpoints, self.kpoints[1:] + [self.kpoints[0]])
-        ]
-        print("overlaps")
-        for O in overlaps:
-            print(np.abs(O[0, 0]), np.angle(O[0, 0]))
-        print("   sum  ", np.sum(np.angle(O[0, 0]) for O in overlaps) / np.pi)
-        #        overlaps.append(self.kpoints[-1].overlap(self.kpoints[0],g=np.array( (self.kpoints[-1].K-self.kpoints[0].K).round(),dtype=int )  )  )
-        nmax = np.min([o.shape for o in overlaps])
-        # calculate zak phase in incresing dimension of the subspace (1 band,
-        # 2 bands, 3 bands,...)
-        z = np.angle(
-            [[la.det(O[:n, :n]) for n in range(1, nmax + 1)] for O in overlaps]
-        ).sum(axis=0) % (2 * np.pi)
-        #        print (np.array([k.Energy[1:] for k in self.kpoints] ))
-        #        print (np.min([k.Energy[1:] for k in self.kpoints],axis=0) )
-        emin = np.hstack(
-            (np.min([k.Energy[1:nmax] for k in self.kpoints], axis=0), [np.Inf])
-        )
-        emax = np.max([k.Energy[:nmax] for k in self.kpoints], axis=0)
-        locgap = np.hstack(
-            (
-                np.min(
-                    [k.Energy[1:nmax] - k.Energy[0 : nmax - 1] for k in self.kpoints],
-                    axis=0,
-                ),
-                [np.Inf],
-            )
-        )
-        return z, emin - emax, (emin + emax) / 2, locgap
+            Shift taking the origin of the unit cell used in the DFT 
+            calculation to that of the convenctional setting used in 
+            BCS.
+
+        Raises
+        ------
+        RuntimeError
+            Could not find a pait (refUC,shiftUC) matching symmetries 
+            obtained from spglib to those in tables (mod. lattice 
+            translations of the primitive cell).
+
+        """
+        # Give preference to CLI input
+        refUC_cli_bool = refUC_cli is not None
+        shiftUC_cli_bool = shiftUC_cli is not None
+        if refUC_cli_bool and shiftUC_cli_bool:  # Both specified in CLI.
+            refUC = refUC_cli.T  # User sets refUC as if it was acting on column
+            shiftUC = shiftUC_cli
+            print('refUC and shiftUC read from CLI')
+            return refUC, shiftUC
+        elif refUC_cli_bool and not shiftUC_cli_bool:  # shiftUC not given in CLI.
+            refUC = refUC_cli.T  # User sets refUC as if it was acting on column
+            shiftUC = np.zeros(3, dtype=float)
+            print(('refUC was specified in CLI, but shiftUC was not. Taking '
+                   'shiftUC=(0,0,0).'))
+            return refUC, shiftUC
+        elif not refUC_cli_bool and shiftUC_cli_bool:  # refUC not given in CLI.
+            refUC = np.eye(3, dtype=float)
+            shiftUC = shiftUC_cli
+            print(('shitfUC was specified in CLI, but refUC was not. Taking '
+                   '3x3 identity matrix as refUC.'))
+            return refUC, shiftUC
+        elif not search_cell:
+            refUC = np.eye(3, dtype=float)
+            shiftUC = np.zeros(3, dtype=float)
+            print(('Neither refUC nor shiftUC were specified in CLI '
+                   'and searchcell was False. Taking 3x3 identity '
+                   'matrix as refUC and shiftUC=(0,0,0). If you want '
+                   'to calculate the transformation to conventional '
+                   'cell, run IrRep with -searchcell'
+                   ))
+            return refUC, shiftUC
+        else:  # Neither specifiend in CLI.
+            refUC = np.linalg.inv(refUC_lib)  # from DFT to convenctional cell
+            found = False
+
+            # Check if the shift given by spglib works
+            shiftUC = -refUC.dot(shiftUC_lib)
+            try:
+                ind, dt, signs = self.match_symmetries(
+                                    refUC,
+                                    shiftUC,
+                                    trans_thresh=trans_thresh
+                                    )
+                return refUC, shiftUC
+            except RuntimeError:
+                pass
+
+            # Check if the group is centrosymmetric
+            inv = None
+            for sym in self.symmetries:
+                if np.allclose(sym.rotation, -np.eye(3)):
+                    inv = sym
+
+            if inv is None:  # Not centrosymmetric
+                for r_center in self.vecs_centering():
+                    shiftUC = shiftUC_lib + refUC.dot(r_center)
+                    try:
+                        ind, dt, signs = self.match_symmetries(
+                                            refUC,
+                                            shiftUC,
+                                            trans_thresh=trans_thresh
+                                            )
+                        print(('ShiftUC achieved with the centering: {}'
+                                   .format(r_center))
+                              )
+                        return refUC, shiftUC
+                    except RuntimeError:
+                        pass
+                raise RuntimeError(("Could not find any shift that leads to "
+                                    "the expressions for the symmetries found "
+                                    "in the tables."))
+
+            else:  # Centrosymmetric. Origin must sit in an inv. center
+                for r_center in self.vecs_inv_centers():
+                    shiftUC = 0.5 * inv.translation + refUC.dot(0.5 * r_center)
+                    try:
+                        ind, dt, signs = self.match_symmetries(
+                                            refUC,
+                                            shiftUC,
+                                            trans_thresh=trans_thresh
+                                            )
+                        print(('ShiftUC achieved in 2 steps:\n'
+                               '  (1) Place origin of primitive cell on '
+                               'inversion center: {}\n'
+                               '  (2) Move origin of convenctional cell to the '
+                               'inversion-center: {}'
+                               .format(0.5 * inv.translation, r_center)
+                               )
+                              )
+                        return refUC, shiftUC
+                    except RuntimeError:
+                        pass
+                raise RuntimeError(("Could not find any shift that places the "
+                                    "origin on an inversion center which leads "
+                                    "to the expressions for the symmetries "
+                                    "found in the tables. Enter refUC and "
+                                    "shiftUC in command line"))
+
 
-    def wcc(self):
+
+    def match_symmetries(
+            self,
+            refUC=None,
+            shiftUC=None,
+            signs=False,
+            trans_thresh=1e-5
+            ):
         """
-        Calculate Wilson loops.
+        Matches symmetry operations of two lists. Translational parts 
+        are matched mod. lattice translations (important for centered 
+        structures).
 
+        Parameters
+        ----------
+        refUC : array, default=None
+            3x3 array describing the transformation of vectors defining the 
+            unit cell to the standard setting.
+        shiftUC : array, default=None
+            Translation taking the origin of the unit cell used in the DFT 
+            calculation to that of the standard setting.
+        signs : bool, default=False
+            If `True`, match also rotations of spinors corresponding to 
+            each symmetry.
+        trans_thresh : float, default=1e-5
+            Threshold used to compare translational parts of symmetries.
+        
         Returns
         -------
+        list
+            The :math:`i^{th}` element corresponds to the :math:`i^{th}` 
+            symmetry found by `spglib` and it is the position that the 
+            same symmetry has in the tables.
+        list
+            The :math:`i^{th}` element corresponds to the :math:`i^{th}` 
+            symmetry found by `spglib` and it is the phase difference 
+            w.r.t. the same symmetry in the tables, which may arise if 
+            their translational parts differ by a lattice vector.
         array
-            Eigenvalues of the Wilson loop operator, divided by :math:`2\pi`.
+            The :math:`i^{th}` element corresponds to the :math:`i^{th}` 
+            symmetry found by `spglib` and it is the sign needed to make
+            the matrix for spinor rotation identical to that in tables.
+
+        Note
+        ----
+        Arguments symmetries1 and symmetries2 always take values of 
+        attributes self.symmetry and self.symmetries_tables, so they can
+        be removed, but this way keeps the function more generic.
+        """
+
+        if refUC is None:
+            refUC = self.refUC
+        if shiftUC is None:
+            shiftUC = self.shiftUC
+        ind = []
+        dt = []
+        errtxt = ""
+        for j, sym in enumerate(self.symmetries):
+            R = sym.rotation_refUC(refUC)
+            t = sym.translation_refUC(refUC, shiftUC)
+            found = False
+            for i, sym2 in enumerate(self.symmetries_tables):
+                t1 = refUC.dot(sym2.t - t) % 1
+                #t1 = np.dot(sym2.t - t, refUC) % 1
+                t1[1 - t1 < trans_thresh] = 0
+                if np.allclose(R, sym2.R):
+                    if np.allclose(t1, [0, 0, 0], atol=trans_thresh):
+                        ind.append(i)
+                        dt.append(sym2.t - t)
+                        found = True
+                        break
+                        # Tolerance for rotational part comparison
+                        # is much more restrictive than for transl.
+                        # Make them consistent?
+                    else:
+                        raise RuntimeError((
+                            "Error matching translational part for symmetry {}."
+                            " A symmetry with identical rotational part has "
+                            " been fond in tables, but their translational "
+                            "parts do not match:\n"
+                            "R (found, in conv. cell)= \n{} \n"
+                            "t(found) = {} \n"
+                            "t(table) = {} \n"
+                            "t(found, in conv. cell) = {}\n"
+                            "t(table)-t(found) "
+                            "(in conv. cell, mod. lattice translation)= {}"
+                            .format(
+                                j+1, 
+                                R, 
+                                sym.translation, 
+                                sym2.t, 
+                                t,
+                                t1
+                                ))
+                            )
+            if not found:
+                raise RuntimeError(
+                    "Error matching rotational part for symmetry {0}. In the "
+                    .format(j+1) +
+                     "tables there is not any symmetry with identical " + 
+                     "rotational part. \nR(found) = \n{} \nt(found) = {}"
+                     .format(R, t))
 
-        """
-        overlaps = [
-            x.overlap(y)
-            for x, y in zip(self.kpoints, self.kpoints[1:] + [self.kpoints[0]])
-        ]
-        nmax = np.min([o.shape for o in overlaps])
-        wilson = functools.reduce(
-            np.dot,
-            [functools.reduce(np.dot, np.linalg.svd(O)[0:3:2]) for O in overlaps],
-        )
-        return np.sort((np.angle(np.linalg.eig(wilson)) / (2 * np.pi)) % 1)
+        if (len(set(ind)) != len(self.symmetries)):
+            raise RuntimeError(
+                "Error in matching symmetries detected by spglib with the \
+                 symmetries in the tables. Try to modify the refUC and shiftUC \
+                 parameters")
+        if signs:
+            S1 = [sym.spinor_rotation for sym in self.symmetries]
+            S2 = [self.symmetries_tables[i].S for i in ind]
+            signs_array = self.__match_spinor_rotations(S1, S2)
+        else:
+            signs_array = np.ones(len(ind), dtype=int)
+        return ind, dt, signs_array
 
-    def write_bands(self, locs=None):
-        """
-        Generate lines for a band structure plot, with cummulative length of the
-        k-path as values for the x-axis and energy-levels for the y-axis.
+    def vecs_centering(self):
+        """ 
+        Check the space group and generate vectors of centering.
 
         Returns
         -------
-        str
-            Lines to write into a file that will be parsed to plot the band 
-            structure.
+        array
+            Each row is a lattice vector describing the centering.
         """
-        #        print (locs)
-        kpline = self.KPOINTSline()
-        nbmax = max(k.Nband for k in self.kpoints)
-        EN = np.zeros((nbmax, len(kpline)))
-        EN[:, :] = np.Inf
-        for i, k in enumerate(self.kpoints):
-            EN[: k.Nband, i] = k.Energy - self.efermi
-        if locs is not None:
-            loc = np.zeros((nbmax, len(kpline), len(locs)))
-            for i, k in enumerate(self.kpoints):
-                loc[: k.Nband, i, :] = k.getloc(locs).T
-            return "\n\n\n".join(
-                "\n".join(
-                    (
-                        "{0:8.4f}   {1:8.4f}  ".format(k, e)
-                        + "  ".join("{0:8.4f}".format(l) for l in L)
-                    )
-                    for k, e, L in zip(kpline, E, LC)
-                )
-                for E, LC in zip(EN, loc)
-            )
-        else:
-            return "\n\n\n".join(
-                "\n".join(
-                    ("{0:8.4f}   {1:8.4f}  ".format(k, e)) for k, e in zip(kpline, E)
-                )
-                for E in EN
-            )
+        cent = np.array([[0,0,0]])
+        if self.name[0] == 'P':
+            pass  # Just to make it explicit
+        elif self.name[0] == 'C':
+            cent = np.vstack((cent, cent + [1/2,1/2,0]))
+        elif self.name[0] == 'I':
+            cent = np.vstack((cent, cent + [1/2,1/2,1/2]))
+        elif self.name[0] == 'F':
+            cent = np.vstack((cent,
+                              cent + [0,1/2,1/2],
+                              cent + [1/2,0,1/2],
+                              cent + [1/2,1/2,0],
+                              )
+                             )
+        elif self.name[0] == 'A':  # test this
+            cent = np.vstack((cent, cent + [0,1/2,1/2]))
+        else:  # R-centered
+            cent = np.vstack((cent,
+                              cent + [2/3,1/3,1/3],
+                              cent + [1/3,2/3,2/3],
+                              )
+                             )
+        return cent
 
-    def write_trace_all(
-        self,
-        degen_thresh=1e-8,
-        symmetries=None,
-        fname="trace_all.dat",
-    ):
+    def vecs_inv_centers(self):
         """
-        Write in a file the description of symmetry operations, energy-levels 
-        and irreps calculated in all k-points.
-
-        Parameters
-        ----------
-        degen_thresh : float, default=1e-8
-            Threshold energy used to decide whether wave-functions are
-            degenerate in energy.
-        symmetries : list, default=None
-            Index of symmetry operations whose traces will be printed. 
-        fname : str, default=trace_all.dat
-            Name of output file.
-        """
-        f = open(fname, "w")
-        kpline = self.KPOINTSline()
-
-        f.write(
-            (
-                "# {0}  # Number of bands below the Fermi level\n"
-                + "# {1}  # Spin-orbit coupling. No: 0, Yes: 1\n"  #
-            ).format(self.getNbands(), 1 if self.spinor else 0)
-        )
-        # add lines describing symmetry operations
-        f.write(
-            "\n".join(
-                ("#" + l)
-                for l in self.spacegroup.write_trace().split("\n")
-            )
-            + "\n\n"
-        )
-        for KP, KPL in zip(self.kpoints, kpline):
-            f.write(
-                KP.write_trace_all(
-                    degen_thresh, symmetries=symmetries, efermi=self.efermi, kpline=KPL
-                )
-            )
-
-
-    def KPOINTSline(self, kpred=None, breakTHRESH=0.1):
-        """
-        Calculate cumulative length along a path in reciprocal space.
-
-        Parameters
-        ----------
-        kpred : list, default=None
-            Each element contains the direct coordinates of a k-point in the
-            attribute `kpoints`.
-        breakTHRESH : float, default=0.1
-            If the distance between two neighboring k-points in the path is 
-            larger than `breakTHRESH`, it is taken to be 0.
+        Get the positions of all inversion centers in the unit cell.
 
         Returns
         -------
         array
-            Each element is the cumulative distance along the path up to a 
-            k-point. The first element is 0, so that the number of elements
-            matches the number of k-points in the path.
-        """
-        if kpred is None:
-            kpred = [k.K for k in self.kpoints]
-        KPcart = np.array(kpred).dot(self.RecLattice)
-        K = np.zeros(KPcart.shape[0])
-        k = np.linalg.norm(KPcart[1:, :] - KPcart[:-1, :], axis=1)
-        k[k > breakTHRESH] = 0.0
-        K[1:] = np.cumsum(k)
-        return K
+            Each element is a vector pointing to a position center in 
+            the convenctional unit cell.
+
+        Notes
+        -----
+        If the space group is primitive, there are 8 inversion centers, 
+        but there are more if it is a group with a centering.
+
+        """
+        vecs = np.array(
+                        [
+                        [0,0,0],
+                        [1,0,0],
+                        [0,1,0],
+                        [0,0,1],
+                        [1,1,0],
+                        [1,0,1],
+                        [0,1,1],
+                        [1,1,1]
+                        ]
+                        )
+        vecs = np.vstack([vecs + r for r in self.vecs_centering()])
+        return vecs
```

### Comparing `irrep-1.8.3/irrep/cli.py` & `irrep-1.9.0/irrep/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -314,24 +314,14 @@
                "irrep --help"
                ))
         print(("Warning: -kpnames not specified. Only traces of "
                "symmetry operations will be calculated. Remember that "
                "-kpnames must be specified to identify irreps"
                ))
 
-    #if kpnames is None:
-    #    identify_irreps = False
-    #    print(("Warning: kpnames not specified. Only traces of "
-    #           "symmetry operations will be calculated. Remember that "
-    #           "kpnames must be specified to identify irreps"
-    #           )
-    #          )
-    #else:
-    #    identify_irreps = True
-
     # parse input arguments into lists if supplied
     if symmetries:
         symmetries = str2list(symmetries)
     if kpoints:
         kpoints = str2list(kpoints)
     if isymsep:
         isymsep = str2list(isymsep)
@@ -340,15 +330,14 @@
 
     try:
         print(fwfk.split("/")[0].split("-"))
         preline = " ".join(s.split("_")[1] for s in fwfk.split("/")[0].split("-")[:3])
     except Exception as err:
         print(err)
         preline = ""
-    json_data = {}
 
     bandstr = BandStructure(
         fWAV=fwav,
         fWFK=fwfk,
         prefix=prefix,
         fPOS=fpos,
         Ecut=ecut,
@@ -358,51 +347,81 @@
         spinor=spinor,
         code=code,
         EF=ef,
         onlysym=onlysym,
         refUC = refuc,
         shiftUC = shiftuc,
         search_cell = searchcell,
-        _correct_Ecut0=correct_ecut0
+        degen_thresh=degenthresh
     )
 
-    json_data ["spacegroup"] = bandstr.spacegroup.show(symmetries=symmetries)
+    bandstr.spacegroup.show()
 
     if onlysym:
         exit()
 
     with open("irreptable-template", "w") as f:
         f.write(
                 bandstr.spacegroup.str()
                 )
 
+    # Identify irreps. If kpnames wasn't set, all will be labelled as None
+    bandstr.identify_irreps(kpnames)
+
+    # Temporary, until we make it valid for isymsep
+    bandstr.write_characters()
+
+    # Write irreps.dat file
+    bandstr.write_irrepsfile()
+
+    # Write trace.txt file
+    bandstr.write_trace()
+
+    # Temporary, until we make it valid for isymsep
+    json_data = {}
+    json_data ["spacegroup"] = bandstr.spacegroup.json(symmetries=symmetries)
+    json_bandstr = bandstr.json()
+    json_data['characters_and_irreps'] = [{"subspace": json_bandstr}]
+
+    # Separate in terms of symmetry eigenvalues
     subbands = {(): bandstr}
 
     if isymsep is not None:
         json_data["separated by symmetry"]=True
         json_data["separating symmetries"]=isymsep
+        tmp_subbands = {}
         for isym in isymsep:
-            print("Separating by symmetry operation # ", isym)
-            subbands = {
-                tuple(list(s_old) + [s_new]): sub
-                for s_old, bands in subbands.items()
-                for s_new, sub in bands.Separate(
-                    isym, degen_thresh=degenthresh, groupKramers=groupkramers
-                ).items()
-            }
+            print("\n-------- SEPARATING BY SYMMETRY # {} --------".format(isym))
+            for s_old, bs in subbands.items():
+                separated = bs.Separate(isym, degen_thresh=degenthresh, groupKramers=groupkramers)
+                for s_new, bs_separated in separated.items():
+                    tmp_subbands[tuple(list(s_old) + [s_new])] = bs_separated
+            subbands = tmp_subbands
+        json_data["characters_and_irreps"]=[]
+        for k, sub in subbands.items():
+            if isymsep is not None:
+                print(
+                    "\n\n\n\n ################################################ \n\n\n NEXT SUBSPACE:  ",
+                    " , ".join(
+                        "sym # {0} -> eigenvalue {1}".format(s, short(ev)) for s, ev in zip(isymsep, k)
+                    ),
+                )
+                plotfile=None # being implemented, not finished yet...
+                sub.write_characters()
+                json_data["characters_and_irreps"].append({"symmetry_eigenvalues":k , "subspace": sub.json(symmetries)})
     else :
         json_data["separated by symmetry"]=False
         
 
+    dumpfn(json_data,"irrep-output.json",indent=4)
+
     if zak:
         for k in subbands:
             print("symmetry eigenvalue : {0} \n Traces are : ".format(k))
-            subbands[k].write_characters(
-                degen_thresh=0.001, symmetries=symmetries
-            )
+            subbands[k].write_characters()
             print("symmetry eigenvalue : {0} \n Zak phases are : ".format(k))
             zak = subbands[k].zakphase()
             for n, (z, gw, gc, lgw) in enumerate(zip(*zak)):
                 print(
                     "   {n:4d}    {z:8.5f} pi gapwidth = {gap:8.4f} gapcenter = {cent:8.3f} localgap= {lg:8.4f}".format(
                         n=n + 1, z=z / np.pi, gap=gw, cent=gc, lg=lgw
                     )
@@ -417,38 +436,14 @@
             print(
                 "symmetry eigenvalue : {0} \n  WCC are : {1} \n sumWCC={2}".format(
                     k, wcc, np.sum(wcc) % 1
                 )
             )
         exit()
 
-    bandstr.write_trace(
-        degen_thresh=degenthresh,
-        symmetries=symmetries,
-    )
-    json_data["characters_and_irreps"]=[]
-    for k, sub in subbands.items():
-        if isymsep is not None:
-            print(
-                "\n\n\n\n ################################################ \n\n\n next subspace:  ",
-                " , ".join(
-                    "{0}:{1}".format(s, short(ev)) for s, ev in zip(isymsep, k)
-                ),
-            )
-        plotfile=None # being implemented, not finished yet...
-        characters = sub.write_characters(
-            degen_thresh=degenthresh,
-            symmetries=symmetries,
-            kpnames=kpnames,
-            preline=preline,
-            plotFile=plotfile,
-        )
-        json_data["characters_and_irreps"].append( {"symmetry_eigenvalues":k , "subspace": characters  }  )
-#        json_data["characters_and_irreps"].append( [k ,characters  ]  )
-
     if plotbands:
         json_data["characters_and_irreps"] = {}
         print("plotbands = True --> writing bands")
         for k, sub in subbands.items():
             if isymsep is not None:
                 print(
                     "\n\n\n\n ################################################ \n\n\n next subspace:  ",
```

### Comparing `irrep-1.8.3/irrep/gvectors.py` & `irrep-1.9.0/irrep/gvectors.py`

 * *Files identical despite different names*

### Comparing `irrep-1.8.3/irrep/kpoint.py` & `irrep-1.9.0/irrep/kpoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import numpy as np
 import numpy.linalg as la
 import copy
 from .gvectors import calc_gvectors, symm_eigenvalues, NotSymmetryError, symm_matrix, sortIG
 from .readfiles import Hartree_eV
 from .readfiles import record_abinit
-from .utility import compstr, is_round
+from .utility import compstr, is_round, format_matrix
 from scipy.io import FortranFile as FF
 from lazy_property import LazyProperty
 
 class Kpoint:
     """
     Parses files and organizes info about the states and energy-levels of a 
     particular k-point in attributes. Contains methods to calculate and write 
@@ -160,78 +160,71 @@
                     )
                 except NotSymmetryError as err:
                     pass  # print  ( err )
         return symmetries
 
     def __init__(
         self,
-        ik,
-        NBin,
-        IBstart,
-        IBend,
-        Ecut,
-        Ecut0,
-        RecLattice,
+        ik=None,
+        IBstart=None,
+        IBend=None,
+        RecLattice=None,  # this was last mandatory argument
         symmetries_SG=None,
         spinor=None,
         code="vasp",
         kpt=None,
-        npw_=None,
-        fWFK=None,
-        WCF=None,
-        prefix=None,
-        kptxml=None,
-        flag=-1,
-        usepaw=0,
-        eigenval=None,
-        spin_channel=None,
-        IBstartE=0
+        WF=None,  # first arg added for abinit (to be kept at the end)
+        Energy=None,
+        ig=None,
+        upper=None,
+        degen_thresh=1e-8,
+        symmetries=None,
+        refUC=np.eye(3),
+        shiftUC=np.zeros(3),
+        symmetries_tables=None  # calculate_traces needs it
     ):
         self.spinor = spinor
         self.ik0 = ik + 1  # the index in the WAVECAR (count start from 1)
         self.Nband = IBend - IBstart
         #        self.n=np.arange(IBstart,IBend)+1
         self.RecLattice = RecLattice
         self.symmetries_SG = symmetries_SG  # lazy_property needs it
+        self.upper = upper
 
-        if code.lower() == "vasp":
-            self.WF, self.ig = self.__init_vasp(
-                WCF, ik, NBin, IBstart, IBend, Ecut, Ecut0
-            )
-        elif code.lower() == "abinit":
-            self.WF, self.ig = self.__init_abinit(
-                fWFK,
-                ik,
-                NBin,
-                IBstart,
-                IBend,
-                Ecut,
-                Ecut0,
-                kpt=kpt,
-                npw_=npw_,
-                flag=flag,
-                usepaw=usepaw,
-            )
-        elif code.lower() == "espresso":
-            self.WF, self.ig = self.__init_espresso(
-                prefix, ik, IBstart, IBend, Ecut, Ecut0, kptxml=kptxml,
-                spin_channel=spin_channel,IBstartE=IBstartE
-            )
-        elif code.lower() == "wannier":
-            self.WF, self.ig = self.__init_wannier(
-                NBin, IBstart, IBend, Ecut, kpt=kpt, eigenval=eigenval
-            )
-        else:
-            raise RuntimeError("unknown code : {}".format(code))
+        self.K = kpt
+        self.WF = WF
+        self.Energy = Energy
+        self.ig = ig
+        self.upper = upper
 
+        self.k_refUC = np.dot(refUC.T, self.K)
         self.WF /= (
             np.sqrt(np.abs(np.einsum("ij,ij->i", self.WF.conj(), self.WF)))
         ).reshape(self.Nband, 1)
 
-    def copy_sub(self, E, WF):
+        # Calculate traces
+        self.char, self.char_refUC, self.Energy, self.degeneracies, self.borders = self.calculate_traces(refUC, shiftUC, symmetries, symmetries_tables, degen_thresh)
+
+        # Determine number of band inversions based on parity
+        found = False
+        for sym in self.symmetries:
+            if (
+                sum(abs(sym.translation)) < 1e-6
+                and
+                abs(sym.rotation + np.eye(3)).sum() < 1e-6
+            ):
+                found = True
+                break
+        if found:
+            self.num_bandinvs = int(round(sum(1 - self.symmetries[sym].real) / 2))
+        else:
+            self.num_bandinvs = None
+
+
+    def copy_sub(self, E, WF, degen_thresh, inds):
         """
         Create an instance of class `Kpoint` for a restricted set of states.
 
         Parameters
         ----------
         E : array
             Energy-levels of states.
@@ -241,25 +234,37 @@
 
         Returns
         -------
         other : class
             Instance of `Kpoints` corresponding to the group of states passed. 
             They are shorted by energy-levels.
         """
-        #        print ("making a subspace with E={0}\n WF = {1}".format(E,WF.shape))
+
         other = copy.copy(self) # copy of whose class
+
+        # Sort energy levels
         sortE = np.argsort(E)
         other.Energy = E[sortE]
         other.WF = WF[sortE]
         other.Nband = len(E)
-        # other.__calc_sym_eigenvalues()
-        #        print ( self.Energy,other.Energy)
-        #        print ( self.WF.shape, other.WF.shape)
-        #        other.write_characters()
-        #        print ("self overlap:\n",self.overlap(self))
+        inds = inds[sortE]
+
+        # Do not group by degeneracy of energy-levels for printing
+        other.degeneracies = [1] * self.Nband
+        char = []
+        char_refUC = []
+        for i in inds:
+            char.append(other.char[i])
+            char_refUC.append(other.char_refUC[i])
+        other.char = np.array(char)
+        other.char_refUC = np.array(char_refUC)
+        irreps = []
+        for i in inds:
+            irreps.append(other.irreps[i])
+        other.irreps = irreps
         return other
 
     def unfold(self, supercell, kptPBZ, degen_thresh=1e-4):
         """
         Unfolds a kpoint of a supercell onto the point of the primitive cell 
         `kptPBZ`.
 
@@ -401,15 +406,15 @@
                 Sy = 1j * (-Smatrix[0][1] + Smatrix[1][0])
                 Sz = Smatrix[0][0] - Smatrix[1][1]
                 result.append((b1, b2, E, (W, Sx, Sy, Sz)))
             else:
                 result.append((b1, b2, E, (W,)))
         return result
 
-    def Separate(self, symop, degen_thresh=1e-5, groupKramers=True):
+    def Separate(self, symop, degen_thresh, groupKramers=True):
         """
         Separate the band structure in a particular k-point according to the 
         eigenvalues of a symmetry operation.
 
         Parameters
         ----------
         isymop : int
@@ -422,813 +427,374 @@
         Returns
         -------
         subspaces : dict
             Each key is an eigenvalue of the symmetry operation and the
             corresponding value is an instance of `class` `Kpoint` for the 
             states with that eigenvalue.
         """
-        borders = np.hstack(
-            [
-                [0],
-                np.where(self.Energy[1:] - self.Energy[:-1] > degen_thresh)[0] + 1,
-                [self.Nband],
-            ]
-        )
+
+        # Check orthogonality of wave functions
+        # Rm once tests are fixed
+        norms = self.WF.conj().dot(self.WF.T)
+        check = np.max(abs(norms - np.eye(norms.shape[0])))
+        if check > 1e-5:
+            print(
+                "orthogonality (largest of diag. <psi_nk|psi_mk>): {0:7.5} > 1e-5   \n".format(
+                    check
+                )
+            )
+
         S = symm_matrix(
             self.K,
             self.RecLattice,
             self.WF,
             self.ig,
             symop.rotation,
             symop.spinor_rotation,
             symop.translation,
             self.spinor,
         )
-        # check orthogonality
-        S1 = self.WF.conj().dot(self.WF.T)
-        check = np.max(abs(S1 - np.eye(S1.shape[0])))
-        if check > 1e-5:
-            print(
-                "orthogonality (largest of diag. <psi_nk|psi_mk>): {0:7.5} > 1e-5   \n".format(
-                    check
-                )
-            )
-        #        print ("symmetry matrix \n",shortS)
-        eigenvalues = []
-        eigenvectors = []
-        Eloc = []
 
-        def short(A):
-            """
-            Format array to print it.            
-            
-            Parameters
-            ----------
-            A : array
-                Matrix that should be printed.
-                
-            Returns
-            -------
-            str
-                Description of the matrix. Ready to be printed.
-            """
-            return "".join(
-                "   ".join("{0:+5.2f} {1:+5.2f}".format(x.real, x.imag) for x in a)
-                + "\n"
-                for a in A
-            )
 
-        # check that S is block-diagonal
+        # Check that S is block-diagonal
         Sblock = np.copy(S)
-        for b1, b2 in zip(borders, borders[1:]):
+        for b1, b2 in zip(self.borders, self.borders[1:]):
             Sblock[b1:b2, b1:b2] = 0
         check = np.max(abs(Sblock))
         if check > 0.1:
-            print("WARNING: off-block:  \n", check)
-            print(short(Sblock))
+            print(("WARNING: matrix of symmetry has non-zero elements between "
+                   "states of different energy:  \n", check))
+            print("Printing matrix of symmetry at k={}".format(self.K))
+            print(format_matrix(Sblock))
 
-        # calculate eigenvalues and eigenvectors in each block
-        for b1, b2 in zip(borders, borders[1:]):
+        # Calculate eigenvalues and eigenvectors in each block
+        eigenvalues = []
+        eigenvectors = []
+        inds_states = []
+        Eloc = []
+        for istate, num_states in  enumerate(self.degeneracies):
+            b1 = self.borders[istate]
+            b2 = self.borders[istate+1]
+            inds_states += [istate] * num_states  # index for set of states
             W, V = la.eig(S[b1:b2, b1:b2])
-            #            print (b1,b2,"symmetry submatrix \n",short(S[b1:b2,b1:b2]))
             for w, v in zip(W, V.T):
                 eigenvalues.append(w)
-                Eloc.append(self.Energy[b1:b2].mean())
+                Eloc.append(self.Energy[istate])
                 eigenvectors.append(
                     np.hstack((np.zeros(b1), v, np.zeros(self.Nband - b2)))
                 )
         w = np.array(eigenvalues)
         v = np.array(eigenvectors).T # each col an eigenvector
         Eloc = np.array(Eloc)
+        inds_states = np.array(inds_states)
 
-        #        print ("eigenvalues:",w)
-        #        print ("eigenvectors:\n",v)
-        #        print ("Eloc:\n",Eloc)
+        # Check unitarity of the symmetry
         if np.abs((np.abs(w) - 1.0)).max() > 1e-4:
             print("WARNING : some eigenvalues are not unitary :{0} ".format(w))
         if np.abs((np.abs(w) - 1.0)).max() > 3e-1:
             raise RuntimeError(" some eigenvalues are not unitary :{0} ".format(w))
         w /= np.abs(w)
-        nb = len(w)
 
         subspaces = {}
 
         if groupKramers:
-            w1 = np.argsort(np.real(w))
-            w = w[w1]
-            v = v[:, w1]
-            Eloc = Eloc[w1]
+
+            # Sort based on real part of eigenvalues
+            arg = np.argsort(np.real(w))
+            w = w[arg]
+            v = v[:, arg]
+            Eloc = Eloc[arg]
+            inds_states = inds_states[arg]
             borders = np.hstack(
-                ([0], np.where((w[1:] - w[:-1]) > 0.05)[0] + 1, [len(w)])
+                ([0], np.where((w[1:] - w[:-1]) > 0.05)[0] + 1, [self.Nband])
             )
+
+            # Probably this if-else statement can be removed
             if len(borders) > 0:
                 for b1, b2 in zip(borders, borders[1:]):
                     v1 = v[:, b1:b2]
-                    subspaces[w[b1:b2].mean()] = self.copy_sub(
-                        E=Eloc[b1:b2], WF=v1.T.dot(self.WF)
-                    )
+                    print(w[b1:b2].mean())
+                    subspaces[w[b1:b2].mean()] = self.copy_sub(E=Eloc[b1:b2], WF=v1.T.dot(self.WF), degen_thresh=degen_thresh, inds=inds_states[b1:b2])
             else:
                 v1 = v
-                subspaces[w.mean()] = self.copy_sub(E=Eloc, WF=v1.T.dot(self.WF))
-        else:
+                subspaces[w.mean()] = self.copy_sub(E=Eloc, WF=v1.T.dot(self.WF), degen_thresh=degen_thresh, inds_states=inds_states)
+
+        else:  # don't group Kramers pairs
             
-            w1 = np.argsort(np.angle(w))
-            w = w[w1]
-            v = v[:, w1]
-            Eloc = Eloc[w1]
+            # Sort based on the argument of eigenvalues
+            arg = np.argsort(np.angle(w))
+            w = w[arg]
+            v = v[:, arg]
+            Eloc = Eloc[arg]
             borders = np.where(abs(w - np.roll(w, 1)) > 0.1)[0]
+
             if len(borders) > 0:
                 for b1, b2 in zip(borders, np.roll(borders, -1)):
-                    v1 = np.roll(v, -b1, axis=1)[:, : (b2 - b1) % nb]
-                    subspaces[np.roll(w, -b1)[: (b2 - b1) % nb].mean()] = self.copy_sub(
-                        E=np.roll(Eloc, -b1)[: (b2 - b1) % nb], WF=v1.T.dot(self.WF)
+                    v1 = np.roll(v, -b1, axis=1)[:, : (b2 - b1) % self.Nband]
+                    subspaces[np.roll(w, -b1)[: (b2 - b1) % self.Nband].mean()] = self.copy_sub(
+                        E=np.roll(Eloc, -b1)[: (b2 - b1) % self.Nband], degen_thresh=degen_thresh, WF=v1.T.dot(self.WF)
                     )
+
             else:
                 v1 = v
-                subspaces[w.mean()] = self.copy_sub(E=Eloc, WF=v1.T.dot(self.WF))
+                subspaces[w.mean()] = self.copy_sub(E=Eloc, degen_thresh=degen_thresh, WF=v1.T.dot(self.WF))
 
         return subspaces
 
-    def __init_vasp(self, WCF, ik, NBin, IBstart, IBend, Ecut, Ecut0):
-        """
-        Initialization for vasp. Read data and save it in attributes.
-
-        Parameters
-        ----------
-        WCF : class
-            Instance of `class` `WAVECARFILE`.
-        ik : int
-            Index of kpoint, starting count from 0.
-        NBin : int
-            Number of bands considered at every k-point in the DFT calculation.
-        IBstart : int
-            First band to be considered.
-        IBend : int
-            Last band to be considered.
-        Ecut : float
-            Plane-wave cutoff (in eV) to consider in the expansion of wave-functions.
-            Will be set equal to `Ecut0` if input parameter `Ecut` was not set or 
-            the value of this is negative or larger than `Ecut0`.
-        Ecut0 : float
-            Plane-wave cutoff (in eV) used for DFT calulations. Always read from 
-            DFT files. Insignificant if `code`=`wannier90`.
-
-        Returns
-        -------
-        WF : array
-            `WF[i,j]` contains the coefficient corresponding to :math:`j^{th}`
-            plane-wave in the expansion of the wave-function in :math:`i^{th}`
-            band. Only plane-waves if energy smaller than `Ecut` are kept.
-        ig : array
-            Every column corresponds to a plane-wave of energy smaller than 
-            `Ecut`. The number of rows is 6: the first 3 contain direct 
-            coordinates of the plane-wave, the fourth row stores indices needed
-            to short plane-waves based on energy (ascending order). Fitfth 
-            (sixth) row contains the index of the first (last) groups of 
-            plane-waves of identical energy.
-        """
-        r = WCF.record(2 + ik * (NBin + 1))
-        # get the number of planewave coefficients. It should be even for spinor wavefunctions
-        #    print (r)
-        npw = int(r[0])
-        if self.spinor:
-            if npw != int(npw / 2) * 2:
-                raise RuntimeError(
-                    "odd number of coefs {0} for spinor wavefunctions".format(npw)
-                )
-        self.K = r[1:4]
-        eigen = np.array(r[4 : 4 + NBin * 3]).reshape(NBin, 3)[:, 0]
-        self.Energy = eigen[IBstart:IBend]
-        try:
-            self.upper = eigen[IBend]
-        except BaseException:
-            self.upper = np.NaN
-
-        ig = calc_gvectors(
-            self.K, self.RecLattice, Ecut0, npw, Ecut, spinor=self.spinor
-        )
-        selectG = np.hstack((ig[3], ig[3] + int(npw / 2))) if self.spinor else ig[3]
-        WF = np.array(
-            [
-                WCF.record(3 + ik * (NBin + 1) + ib, npw, np.complex64)[selectG]
-                for ib in range(IBstart, IBend)
-            ]
-        )
-        return WF, ig
-
-    def __init_abinit(
-        self,
-        fWFK,
-        ik,
-        NBin,
-        IBstart,
-        IBend,
-        Ecut,
-        Ecut0,
-        kpt,
-        npw_,
-        flag,
-        usepaw,
-    ):
-        """
-        Initialization for Abinit. Read data and store it in attibutes.
-
-        Parameters
-        ----------
-        fWFK : file object
-            File object corresponding to Abinit's WFK. Returned by `FortranFile`.
-        ik : int
-            Index of kpoint, starting count from 0.
-        NBin : int
-            Number of bands considered at every k-point in the DFT calculation.
-        IBstart : int
-            First band to be considered.
-        IBend : int, default=None
-            Last band to be considered.
-        Ecut : float
-            Plane-wave cutoff (in eV) to consider in the expansion of wave-functions.
-            Will be set equal to `Ecut0` if input parameter `Ecut` was not set or 
-            the value of this is negative or larger than `Ecut0`.
-        Ecut0 : float
-            Plane-wave cutoff (in eV) used for DFT calulations. Always read from 
-            DFT files. Insignificant if `code`=`wannier90`.
-        kpt : list or array
-            Direct coordinates of the k-point.
-        npw_ : int
-            Number of plane-waves considered in the expansion of wave-functions. 
-        flag : int
-            Index of the k-point, used when parsing WFK file (Abinit). Info is read 
-            for all k-points, but stored only for k-points whose index is passed 
-            through `flag`.
-        usepaw : int
-            Only used for Abinit. 1 if pseudopotentials are PAW, 0 otherwise. When 
-            `usepaw`=0, normalization of wave-functions is checked.
-
-        Returns
-        -------
-        array
-            Contains the coefficients (same row-column formatting as argument 
-            `CG`) of the expansion of wave-functions corresponding to 
-            plane-waves of energy smaller than `Ecut`. Columns (plane-waves) 
-            are shorted based on their energy, from smaller to larger. 
-            Only plane-waves if energy smaller than `Ecut` are kept.
-        array
-            Every column corresponds to a plane-wave of energy smaller than 
-            `Ecut`. The number of rows is 6: the first 3 contain direct 
-            coordinates of the plane-wave, the third row stores indices needed
-            to short plane-waves based on energy (ascending order). Fitfth 
-            (sixth) row contains the index of the first (last) plane-wave with 
-            the same energy as the plane-wave of the current column.
-        """
-        assert not (kpt is None)
-        self.K = kpt
-        nspinor = 2 if self.spinor else 1
-        print("Reading k-point", ik)
-
-        # We need to skip lines in fWFK until we reach the lines of ik
-        while flag < ik:
-
-            # 1st record: npw, nspinor, nband
-            record = record_abinit(fWFK, "i4")  # [0]
-            npw, nspinor_loc, nband_loc = record
-
-            # 2nd record: reciprocal lattice vectors in the expansion
-            kg = record_abinit(fWFK, "i4").reshape(npw, 3)
-
-            # 3rd record: energies and occupations
-            record = record_abinit(fWFK, "f8")
-            eigen, occ = record[:nband_loc], record[nband_loc:]
-
-            # 4th record: coefficients of expansions in plane waves
-            CG = np.zeros((IBend - IBstart, npw * nspinor), dtype=complex)
-            for iband in range(nband_loc):
-                record = record_abinit(fWFK, "f8")
-                if iband >= IBstart and iband < IBend:
-                    CG[iband - IBstart] = record[0::2] + 1.0j * record[1::2]
-            flag += 1
-
-        # Check consistency of WFK file
-        assert npw == npw_, ("Different number of plane waves in header and "
-                             "k-point's block. Probably a bug in Abinit..."
-                             )
-        assert nband_loc == NBin, ("Different number of bands in header and "
-                                   "k-point's block. Probably a bug in "
-                                   "Abinit..."
-                                   )
-
-        assert (
-            (nspinor_loc == 2 and self.spinor)
-            or (nspinor_loc == 1 and not self.spinor)
-        ), ("Different values of nspinor in header and "
-            "k-point's block. Probably a bug in Abinit..."
-            )
-
-        # Check orthonormality for norm-conserving pseudos
-        if usepaw == 0:
-            largest_value = np.max(np.abs(CG.conj().dot(CG.T)
-                                          - np.eye(IBend - IBstart)))
-            assert largest_value < 1e-10, "Wave functions are not orthonormal"
-
-        # Convert energies to eV and pick upper value
-        self.Energy = eigen[IBstart:IBend] * Hartree_eV
-        try:
-            self.upper = eigen[IBend] * Hartree_eV
-        except BaseException:
-            self.upper = np.NaN
-
-        return sortIG(self.ik0, kg, kpt, CG, self.RecLattice, Ecut0, Ecut, self.spinor)
-
-    def __init_wannier(self, NBin, IBstart, IBend, Ecut, kpt, eigenval):
-        """
-        Initialization for wannier90. Read info and store it in attributes.
-       
-        Parameters
-        ----------
-        NBin : int
-            Number of bands considered at every k-point in the DFT calculation.
-        IBstart : int
-            First band to be considered.
-        IBend : int, default=None
-            Last band to be considered.
-        Ecut : float
-            Plane-wave cutoff (in eV) to consider in the expansion of wave-functions.
-            Will be set equal to `Ecut0` if input parameter `Ecut` was not set or 
-            the value of this is negative or larger than `Ecut0`.
-        kpt : list or array
-            Direct coordinates of the k-point.
-        eigenval : array, default=None
-            Contains all energy-levels in a particular k-point.
-
-        Returns
-        -------
-        WF : array
-            `WF[i,j]` contains the coefficient corresponding to :math:`j^{th}`
-            plane-wave in the expansion of the wave-function in :math:`i^{th}`
-            band. Only plane-waves if energy smaller than `Ecut` are kept.
-        ig : array
-            Every column corresponds to a plane-wave of energy smaller than 
-            `Ecut`. The number of rows is 6: the first 3 contain direct 
-            coordinates of the plane-wave, the fourth row stores indices needed
-            to short plane-waves based on energy (ascending order). Fitfth 
-            (sixth) row contains the index of the first (last) groups of 
-            plane-waves of identical energy.
-        """
-        self.K = np.array(kpt, dtype=float)
-        self.Energy = eigenval[IBstart:IBend]
-        fname = "UNK{:05d}.{}".format(self.ik0, "NC" if self.spinor else "1")
-        fUNK = FF(fname, "r")
-        ngx, ngy, ngz, ik, nbnd = record_abinit(fUNK, "i4,i4,i4,i4,i4")[0]
-        ngtot = ngx * ngy * ngz
-        if ik != self.ik0:
-            raise RuntimeError(
-                "file {} contains point number {}, expected {}".format(
-                    fname, ik, self.ik0
-                )
-            )
-        if nbnd != NBin:
-            raise RuntimeError(
-                "file {} contains {} bands , expected {}".format(fname, nbnd, NBin)
-            )
-        nspinor = 2 if self.spinor else 1
-
-        try:
-            self.upper = eigenval[IBend]
-        except BaseException:
-            self.upper = np.NaN
-
-        ig = calc_gvectors(
-            self.K,
-            self.RecLattice,
-            Ecut,
-            spinor=self.spinor,
-            nplanemax=np.max([ngx, ngy, ngz]) // 2,
-        )
-
-        selectG = tuple(ig[0:3])
-
-        def _readWF_1(skip=False):
-            """
-            Parse coefficients of a wave-function corresponding to one element
-            of the spinor.
-
-            Parameters
-            ----------
-            skip : bool, default=False
-                Read coefficients but do not return them.
-            
-            Returns
-            -------
-            array
-                Coefficients of the plane-wave expansion.
-            """
-            cg_tmp = record_abinit(fUNK, "{}f8".format(ngtot * 2))
-            if skip:
-                return np.array([0], dtype=complex)
-            cg_tmp = (cg_tmp[0::2] + 1.0j * cg_tmp[1::2]).reshape(
-                (ngx, ngy, ngz), order="F"
-            )
-            cg_tmp = np.fft.fftn(cg_tmp)
-            return cg_tmp[selectG]
-
-        def _readWF(skip=False):
-            """
-            Read and return the coefficients of the plane-wave expansion of a 
-            wave-function.
-
-            Parameters
-            ----------
-            skip : bool, default=False
-                Read coefficients but do not return them.
-
-            Returns
-            -------
-            array
-                Coefficients of the plane-wave expansion.
-            """
-            return np.hstack([_readWF_1(skip) for i in range(nspinor)])
-
-        for ib in range(IBstart):
-            _readWF(skip=True)
-        WF = np.array([_readWF(skip=False) for ib in range(IBend - IBstart)])
-        return WF, ig
-
-    def __init_espresso(
-        self, prefix, ik, IBstart, IBend, Ecut, Ecut0, kptxml,
-           spin_channel=None,IBstartE=0
-    ):
-        """
-        Initialization QE. Read info and store it in attributes.
-
-        Parameters
-        ----------
-        prefix : str
-            Prefix used for Quantum Espresso calculations or seedname of 
-            Wannier90 files.
-        ik : int
-            Index of kpoint, starting count from 0.
-        IBstart : int, default=None
-            First band to be considered.
-        IBend : int, default=None
-            Last band to be considered.
-        Ecut : float
-            Plane-wave cutoff (in eV) to consider in the expansion of 
-            wave-functions. Will be set equal to `Ecut0` if input parameter 
-            `Ecut` was not set or the value of this is negative or larger than 
-            `Ecut0`.
-        Ecut0 : float
-            Plane-wave cutoff (in eV) used for DFT calulations. Always read from 
-            DFT files. Insignificant if `code`=`wannier90`.
-        kptxml
-            `Element` object (see `ElementTree XML API`) corresponding to a 
-            k-point.
-        spin_channel : str
-            Selection of the spin-channel. 'up' for spin-up, 'dw' for spin-down.
-        IBstartE : int
-            Only used with Quantum Espresso. Index of first band in particular 
-            spin channel. If `spin_channel`='dw', `IBstartE` is equal to the 
-            number of bands in spin-up channel.
-        
-        Returns
-        -------
-        array
-            Contains the coefficients (same row-column formatting as argument 
-            `CG`) of the expansion of wave-functions corresponding to 
-            plane-waves of energy smaller than `Ecut`. Columns (plane-waves) 
-            are shorted based on their energy, from smaller to larger. 
-            Only plane-waves if energy smaller than `Ecut` are kept.
-        array
-            Every column corresponds to a plane-wave of energy smaller than 
-            `Ecut`. The number of rows is 6: the first 3 contain direct 
-            coordinates of the plane-wave, the third row stores indices needed
-            to short plane-waves based on energy (ascending order). Fitfth 
-            (sixth) row contains the index of the first (last) plane-wave with 
-            the same energy as the plane-wave of the current column.
-        """
-        self.K = np.array(kptxml.find("k_point").text.split(), dtype=float)
-
-        eigen = np.array(kptxml.find("eigenvalues").text.split(), dtype=float)
-
-        self.Energy=eigen[IBstartE+IBstart:IBstartE+IBend]*Hartree_eV
-        try:
-            self.upper=eigen[IBstartE+IBend]*Hartree_eV
-        except:
-            self.upper = np.NaN
-
-
-        npw = int(kptxml.find("npw").text)
-        #        kg= np.random.randint(100,size=(npw,3))-50
-        npwtot = npw * (2 if self.spinor else 1)
-        CG = np.zeros((IBend - IBstart, npwtot), dtype=complex)
-        wfcname="wfc{}{}".format({None:"","dw":"dw","up":"up"}[spin_channel],ik+1)
-        try:
-            fWFC=FF("{}.save/{}.dat".format(prefix,wfcname.lower()),"r")
-        except FileNotFoundError:
-            fWFC=FF("{}.save/{}.dat".format(prefix,wfcname.upper()),"r")
-
-        rec = record_abinit(fWFC, "i4,3f8,i4,i4,f8")[0]
-        ik, xk, ispin, gamma_only, scalef = rec
-        #        xk/=bohr
-        #        xk=xk.dot(np.linalg.inv(RecLattice))
-
-        rec = record_abinit(fWFC, "4i4")
-        #        print ('rec=',rec)
-        ngw, igwx, npol, nbnd = rec
-
-        rec = record_abinit(fWFC, "(3,3)f8")
-        #        print ('rec=',rec)
-        B = np.array(rec)
-        #        print (np.mean(B/RecLattice))
-        self.K = xk.dot(np.linalg.inv(B))
-
-        rec = record_abinit(fWFC, "({},3)i4".format(igwx))
-        #        print ('rec=',rec)
-        kg = np.array(rec)
-        #        print (np.mean(B/RecLattice))
-        #        print ("k-point {0}: {1}/{2}={3}".format(ik, self.K,xk,self.K/xk))
-        #        print ("k-point {0}: {1}".format(ik,self.K ))
-
-        for ib in range(IBend):
-            cg_tmp = record_abinit(fWFC, "{}f8".format(npwtot * 2))
-            if ib >= IBstart:
-                CG[ib - IBstart] = cg_tmp[0::2] + 1.0j * cg_tmp[1::2]
-
-        return sortIG(self.ik0, kg, self.K, CG, B, Ecut0, Ecut, self.spinor)
-
-    def write_characters(
-        self,
-        degen_thresh=1e-8,
-        irreptable=None,
-        symmetries=None,
-        preline="",
-        efermi=0.0,
-        plotFile=None,
-        kpl="",
-        symmetries_tables=None,
-        refUC=np.eye(3),
-        shiftUC=np.zeros(3)
-    ):
-        """
-        Calculate traces and determine and print irreps in a k-point. Write them 
-        in files passed as `plotFile` (for plotting) and `irreps.dat`. Also 
-        calculates and prints the number of band-inversions.
-
-        Parameters
-        ----------
-        degen_thresh : float, default=1e-8
-            Threshold energy used to decide whether wave-functions are
-            degenerate in energy.
-        irreptable : dict, default=None
-            Returned by method `get_irreps_from_table` of class `SpaceGroup`. 
-            Each key is the label of an irrep, each value another `dict`. Keys 
-            of every secondary `dict` are indices of symmetries (starting from 
-            1 and following order of operations in tables of BCS) and 
-            values are traces of symmetries.
-        symmetries : list, default=None
-            Index of symmetry operations whose traces will be printed. 
-        preline : str, default=''
-            Characters to write before labels of irreps in file `irreps.dat`.
-        efermi : float, default=0.0
-            Fermi-energy. Used as origin for energy-levels.
-        plotFile : file object, default=None
-            File in which energy-levels and corresponding irreps will be written 
-            to later place irreps in a band structure plot.
-        kpl : float, default=''
-            Length accumulated until the k-point. Can be used to locate irreps 
-            in the x-axis of a band structure plot.
-        symmetries_tables : list, default=None
-            Each component is an instance of class `SymopTable` corresponding to a 
-            symmetry operation in the "point-group" of the space-group. Values 
-            passed are attributes `symmetries` of class `IrrepTable`.
-        refUC : array, default=np.eye(3)
-            3x3 array describing the transformation of vectors defining the 
-            unit cell to the standard setting.
-        shiftUC : array, default=np.zeros(3)
-            Translation taking the origin of the unit cell used in the DFT 
-            calculation to that of the standard setting.
+    def calculate_traces(self, refUC, shiftUC, symmetries, symmetries_tables, degen_thresh=1e-8):
+        '''
+        Calculate traces of symmetry operations
+        '''
 
-        Returns
-        -------
-        int
-            Number of inversion-odd states.
-        float
-            Last energy-level within the considered range of states.
-        float
-            First energy-level above the range of considered bands. If the last 
-            band in the range of considered bands coincides with the last band 
-            calculated by DFT, it will be set to `numpy.NaN`.
-        json_data : `json` object
-            Object with output structured in `json` format.
-        """
-        json_data = {}
         if symmetries is None:
             sym = {s.ind: s for s in self.symmetries}
         else:
             sym = {s.ind: s for s in self.symmetries if s.ind in symmetries}
-        json_data ["symmetries"] = list(sym.keys())
-    
-        
-        # Generate array char, where each row corresponds to a sym. op
-        # and every column to a wave function
+
+        # Put all traces in an array. Rows (cols) correspond to syms (wavefunc)
         char = np.vstack([self.symmetries[sym[i]] for i in sorted(sym)])
         borders = np.hstack(
             [
                 [0],
                 np.where(self.Energy[1:] - self.Energy[:-1] > degen_thresh)[0] + 1,
                 [self.Nband],
             ]
         )
+        degeneracies = borders[1:] - borders[:-1]
+
+        # Check that number of irreps is int
         Nirrep = np.linalg.norm(char.sum(axis=1)) ** 2 / char.shape[0]
         if abs(Nirrep - round(Nirrep)) > 1e-2:
             print("WARNING - non-integer number of states : {0}".format(Nirrep))
         Nirrep = int(round(Nirrep))
+
+        # Sum traces of degenerate states. Rows (cols) correspond to states (syms)
         char = np.array(
             [char[:, start:end].sum(axis=1) for start, end in zip(borders, borders[1:])]
-        )  # Every column in char corresponds to a sym. op.
-
-        #        print(" char ",char.shape,"\n",char)
-        writeimaginary = np.abs(char.imag).max() > 1e-4
-
-        s1 = " " * 4 if writeimaginary else ""
+            )
 
-        E = np.array(
+        # Take average of energies over degenerate states
+        Energy_mean = np.array(
             [self.Energy[start:end].mean() for start, end in zip(borders, borders[1:])]
         )
-        json_data["energies"] = E
-        json_data["characters"] = char
-
-        dim = np.array([end - start for start, end in zip(borders, borders[1:])])
-        if irreptable is None:
-            irreps = ["None"] * (len(borders) - 1)
-            json_data["irreps"] = None 
-        else:
-            try:
-                # irreps is a list. Each element is a dict corresponding to a 
-                # group of degen. states. Every key is an irrep and its value 
-                # the multiplicity of the irrep in the rep. of degen. states
-                irreps = [
-                    {
-                        ir: np.array(
-                            [irreptable[ir][sym.ind] for sym in self.symmetries]
-                        ).dot(ch.conj())
-                        / len(ch)
-                        for ir in irreptable
-                    }
-                    for ch in char
-                ]
-                json_data["irreps"] = [{ir:(val.real,val.imag) for ir,val in irr.items()} for irr in irreps]
-            except KeyError as ke:
-                print(ke)
-                print("irreptable:", irreptable)
-                print([sym.ind for sym in self.symmetries])
-                raise ke
-            # Generate str describing irrep corresponding to sets of states
-            irreps = [
-                ", ".join(
-                    ir
-                    + "({0:.5}".format(irr[ir].real)
-                    + (
-                        "{0:+.5f}i".format(irr[ir].imag)
-                        if abs(irr[ir].imag) > 1e-4
-                        else ""
-                    )
-                    + ")"
-                    for ir in irr  # Irreps of little-group
-                    if abs(irr[ir]) > 1e-3  # Check multiplicity
-                )
-                for irr in irreps  # Group of degen. states
-            ]
-        #            irreps=[ "None" ]*(len(borders)-1)
 
         # Transfer traces in calculational cell to refUC
         char_refUC = char.copy()
-        k_refUC = np.dot(refUC.T, self.K)
         if (not np.allclose(refUC, np.eye(3, dtype=float)) or
             not np.allclose(shiftUC, np.zeros(3, dtype=float))):
             # Calculational and reference cells are not identical
             for i,ind in enumerate(sym):
                 dt = (symmetries_tables[ind-1].t 
                       - sym[ind].translation_refUC(refUC, shiftUC))
                 char_refUC[:,i] *= (sym[ind].sign 
-                                     * np.exp(-2j*np.pi*dt.dot(k_refUC)))
+                                     * np.exp(-2j*np.pi*dt.dot(self.k_refUC)))
+
+        return char, char_refUC, Energy_mean, degeneracies, borders
+
+
+    def identify_irreps(self, irreptable=None):
+
+        self.onlytraces = irreptable is None
+        if self.onlytraces:
+            irreps = ["None"] * (len(self.degeneracies) - 1)
 
-        json_data["characters_refUC"] = char_refUC
-        if np.allclose(char, char_refUC, rtol=0.0, atol=1e-4):
-            write_refUC = False  # Tr identical in both unit cells
-            json_data["characters_refUC_is_the_same"] = True
         else:
-            write_refUC = True   # Write traces in refUC
-            json_data["characters_refUC_is_the_same"] = False
-            print(("For each irrep, traces of symmetries in the calculation "
-                   "unit cell will be printed first and traces of symmetries "
-                   "in tables will be printed in the line below")
-                 )
-        json_data["dimensions"] = dim
-
-        irreplen = max(len(irr) for irr in irreps)  # len of largest line
-        if irreplen % 2 == 1:
-            irreplen += 1
-        s2 = " " * int(irreplen / 2 - 3)
 
-        # Header of the block
+            # irreps is a list. Each element is a dict corresponding to a 
+            # group of degen. states. Every key is an irrep and its value 
+            # the multiplicity of the irrep in the rep. of degen. states
+            try:
+                irreps = []
+                for ch in self.char:
+                    multiplicities = {}
+                    for ir in irreptable:
+                        multipl = np.dot(np.array([irreptable[ir][sym.ind] for sym in self.symmetries]),
+                                         ch.conj()
+                                         ) / len(ch)
+                        if abs(multipl) > 1e-3:
+                            multiplicities[ir] = multipl
+                    irreps.append(multiplicities)
+            except KeyError as ke:
+                print(ke)
+                print("irreptable:", irreptable)
+                print([sym.ind for sym in self.symmetries])
+                raise ke
+
+        self.irreps = irreps
+
+
+    def write_characters(self):
+
+        # Print header for k-point
         print(("\n\n k-point {0:3d} : {1} (in DFT cell)\n"
                "               {2} (after cell trasformation)\n\n"
                " number of states : {3}\n"
                .format(self.ik0,
                        np.round(self.K, 5),
-                       np.round(k_refUC,5),
-                       self.Nband
-                       )
+                       np.round(self.k_refUC, 5),
+                       self.Nband)
               ))
 
-        print("   Energy  |   degeneracy  |{0} irreps {0}| sym. operations  ".format(s2))
+        # Generate str describing irrep corresponding to sets of states
+        str_irreps = []
+        for irreps in self.irreps:  # set of IRs for a set of degenerate states
+            if self.onlytraces:
+                s = '  None  '
+            else:
+                s = ''
+                for ir in irreps:  # label and multiplicity of one irrep
+                    if s != '':
+                        s += ', '  # separation between labels for irreps
+                    s += ir
+                    s += '({0:.5}'.format(irreps[ir].real)
+                    if abs(irreps[ir].imag) > 1e-4:
+                        s += '{0:+.5f}i'.format(irreps[ir].imag)
+                    s += ')'
+            str_irreps.append(s)
+
+        # Set auxiliary blank strings for formatting
+        writeimaginary = np.abs(self.char.imag).max() > 1e-4
+        if writeimaginary:
+            aux1 = ' ' * 4
+        else:
+            aux1 = ''
+        irreplen = max(len(irr) for irr in str_irreps)
+        #if irreplen % 2 == 1:
+        #    irreplen += 1
+        #aux2 = " " * int(irreplen / 2 - 3)
+        num_spaces = (irreplen-8) / 2
+        aux2 = " " * int(num_spaces)
+        if irreplen % 2 == 0:
+            aux3 = aux2 
+        else:
+            aux3 = aux2 + " "
 
-        # Symmetry operations
-        print(
-            "           |               |{0}        {0}| ".format(s2),
-            " ".join(s1 + "{0:4d}    ".format(i) + s1 for i in sorted(sym)),
-        )
+        print("   Energy  |   degeneracy  | {0} irreps {1} | sym. operations  ".format(aux2, aux3))
+
+        # Print indices of little-group symmetries
+        s = "           |               | {0}        {1} | ".format(aux2, aux3)
+        inds = []
+        for sym in self.symmetries:
+            inds.append(aux1 + "{0:4d}    ".format(sym.ind) + aux1)
+        s += " ".join(inds)
+        print(s)
+        #print(
+        #    "           |               |{0}        {0}| ".format(aux2),
+        #    " ".join(aux1 + "{0:4d}    ".format(i) + aux1 for i in sorted(sym)),
+        #)
+
+        # Print line associated to a set of degenerate states
+        for e, d, ir, ch1, ch2 in zip(self.Energy, self.degeneracies, str_irreps, self.char, self.char_refUC):
+
+            # Traces in DFT unit cell
+            right_str1 = []
+            right_str2 = []
+            for tr1, tr2 in zip(ch1, ch2):
+                s1 = "{0:8.4f}".format(tr1.real)
+                s2 = "{0:8.4f}".format(tr2.real)
+                if writeimaginary:
+                    s1 += "{0:+7.4f}j".format(tr1.imag)
+                    s2 += "{0:+7.4f}j".format(tr2.imag)
+                right_str1.append(s1)
+                right_str2.append(s2)
+            right_str1 = ' '.join(right_str1)
+            right_str2 = ' '.join(right_str2)
 
-        # Energy-levels, irrep's label and traces
-        for e, d, ir, ch, ch2 in zip(E, dim, irreps, char, char_refUC):
-            # Print characters in calculational unit cell
+            # Energy, degeneracy, irrep's label and character in DFT cell
             left_str = (" {0:8.4f}  |    {1:5d}      | {2:{3}s} |"
-                        .format(e - efermi, d, ir, irreplen)
-                       )
-            right_str = " ".join(
-                        "{0:8.4f}".format(c.real)
-                        + ("{0:+7.4f}j".format(c.imag) if writeimaginary else "")
-                        for c in ch
-                    )
-            print(left_str + " " + right_str)
-            # Print characters in reference unit cell
-            if write_refUC:
-                left_str = ("           |               | {0:{1}s} |"
-                            .format(len(ir)*" ", irreplen)
-                           )
-                right_str = " ".join(
-                            "{0:8.4f}".format(c.real)
-                            + ("{0:+7.4f}j".format(c.imag) if writeimaginary else "")
-                            for c in ch2
+                        .format(e, d, ir, irreplen)
                         )
-                print(left_str + " " + right_str)
+            print(left_str + " " + right_str1)
 
-        if plotFile is not None:
-            plotFile.write(
-                (
-                    "\n".join(
-                        ("{2:8.4f}   {0:8.4f}      {1:5d}   ").format(
-                            e - efermi, d, kpl
-                        )
-                        + " ".join(
-                            "{0:8.4f}".format(c.real)
-                            + ("{0:+7.4f}j".format(c.imag) if writeimaginary else "")
-                            for c in ch
+            # Line for character in reference cell
+            left_str = ("           |               | {0:{1}s} |"
+                        .format(len(ir)*" ", irreplen)
                         )
-                        for e, d, ch in zip(E, dim, char)
-                    )
-                )
-                + "\n\n"
-            )
+            print(left_str + " " + right_str2)  # line for character in DFT
 
-        isyminv = None
-        for s in sym:
-            if (
-                sum(abs(sym[s].translation)) < 1e-6
-                and abs(sym[s].rotation + np.eye(3)).sum() < 1e-6
-            ):
-                isyminv = s
-        if isyminv is None:
-            print("no inversion")
-            NBANDINV = 0
+
+    def json(self, symmetries=None):
+
+        json_data = {}
+
+        # Dictionary with symmetry eigenvalues (do we need this?)
+        if symmetries is None:
+            sym = {s.ind: s for s in self.symmetries}
         else:
-            print("inversion is #", isyminv)
-            NBANDINV = int(round(sum(1 - self.symmetries[sym[isyminv]].real) / 2))
-            if self.spinor:
-                print("number of inversions-odd Kramers pairs : ", int(NBANDINV / 2))
-            else:
-                print("number of inversions-odd states : ", NBANDINV)
-            print("Gap with upper bands : ", self.upper - self.Energy[-1])
+            sym = {s.ind: s for s in self.symmetries if s.ind in symmetries}
+        json_data ['symmetries'] = list(sym.keys())
+
+        # Energy levels and degeneracies
+        json_data['energies'] = self.Energy
+        json_data['dimensions'] = self.degeneracies
+
+        # Irreps and multiplicities
+        if self.onlytraces:
+            json_data['irreps'] = None 
+        else:
+            json_data['irreps'] = []
+            for state in self.irreps:
+                d = {}
+                for irrep, multipl in state.items():
+                    d[irrep] = (multipl.real, multipl.imag)
+                json_data['irreps'].append(d)
+
+        # Traces of symmetries
+        json_data['characters'] = self.char
+        json_data['characters_refUC'] = self.char_refUC
+        if np.allclose(self.char, self.char_refUC, rtol=0.0, atol=1e-4):
+            json_data['characters_refUC_is_the_same'] = True
+        else:
+            json_data['characters_refUC_is_the_same'] = False
+        
+        return json_data
+        
+    def write_irrepsfile(self, file):
+
+        for energy, irrep_dict in zip(self.Energy, self.irreps):
+            irrep = ''.join(irrep_dict.keys())
+            s = '{:15.7f}    {:15s}\n'.format(energy, irrep)
+            file.write(s)
+
+
+    def write_plotfile(self, plotfile, kpl, efermi):
+
+        writeimaginary = np.abs(self.character.imag).max() > 1e-4
+        s = []
+        for e, dim, char in zip(self.Energy, self.degeneracies, self.character):
+            s_loc = '{2:8.4f}   {0:8.4f}      {1:5d}   '.format(e-efermi, d, kpl)
+            for tr in char:
+                s_loc += "{0:8.4f}".format(tr.real)
+                if writeimaginary:
+                    s_loc += "{0:+7.4f}j ".format(tr.imag)
+            s.append(s_loc)
+        s = '\n'.join(s)
+        s += '\n\n'
 
-        firrep = open("irreps.dat", "a")
-        for e, ir in zip(E, irreps):
+
+    def write_irrepfile(self, firrep, efermi):
+
+        file = open(firrep, "a")
+        for e, ir in zip(self.Energy, self.irreps):
             for irrep in ir.split(","):
                 try:
                     weight = abs(compstr(irrep.split("(")[1].strip(")")))
                     if weight > 0.3:
-                        firrep.write(
+                        file.write(
                             preline
                             + " {0:10s} ".format(irrep.split("(")[0])
                             + "  {0:10.5f}\n".format(e - efermi)
                         )
                 except IndexError:
                     pass
+        file.close()
 
-        return NBANDINV, self.Energy[-1], self.upper , json_data
 
-    def write_trace(self, degen_thresh=1e-8, symmetries=None, efermi=0.0):
+
+    def write_trace(self):
         """
         Write in `trace.txt` the block corresponding to a single k-point.
 
         Parameters
         ----------
         degen_thresh : float, default=1e-8
             Threshold energy used to decide whether wave-functions are
@@ -1240,48 +806,29 @@
 
         Returns
         -------
         res : str
             Block to write in `trace.txt` with description of traces in a
             single k-point.
         """
-        if symmetries is None:
-            sym = {s.ind: s for s in self.symmetries}
-        else:
-            sym = {s.ind: s for s in self.symmetries if s.ind in symmetries}
 
+        sym = {s.ind: s for s in self.symmetries}
         res = (
             "{0} \n"
             + " {1} \n"  # Number of symmetry operations of the little co-group of the 1st maximal k-vec. In the next line the position of each element of the point group in the list above.
             # For each band introduce a row with the followind data: (1) 1+number of bands below, (2) dimension (degeneracy) of the band,
             # (3) energy and eigenvalues (real part, imaginary part) for each symmetry operation of the little group (listed above).
         ).format(len(sym.keys()), "  ".join(str(x) for x in sym))
 
-        char = np.vstack([self.symmetries[sym[i]] for i in sorted(sym)])
-        borders = np.hstack(
-            [
-                [0],
-                np.where(self.Energy[1:] - self.Energy[:-1] > degen_thresh)[0] + 1,
-                [self.Nband],
-            ]
-        )
-        char = np.array(
-            [char[:, start:end].sum(axis=1) for start, end in zip(borders, borders[1:])]
-        )
-
-        E = np.array(
-            [self.Energy[start:end].mean() for start, end in zip(borders, borders[1:])]
-        )
-        dim = np.array([end - start for start, end in zip(borders, borders[1:])])
-        IB = np.cumsum(np.hstack(([0], dim[:-1]))) + 1
+        IB = np.cumsum(np.hstack(([0], self.degeneracies[:-1]))) + 1
         res += (
             "\n".join(
-                (" {ib:8d}  {d:8d}   {E:8.4f} ").format(E=e - efermi, d=d, ib=ib)
+                (" {ib:8d}  {d:8d}   {E:8.4f} ").format(E=e, d=d, ib=ib)
                 + "  ".join("{0:10.6f}   {1:10.6f} ".format(c.real, c.imag) for c in ch)
-                for e, d, ib, ch in zip(E, dim, IB, char)
+                for e, d, ib, ch in zip(self.Energy, self.degeneracies, IB, self.char)
             )
             + "\n"
         )
 
         return res
 
     def write_trace_all(self, degen_thresh=1e-8, symmetries=None, efermi=0.0, kpline=0):
```

### Comparing `irrep-1.8.3/irrep/utility.py` & `irrep-1.9.0/irrep/utility.py`

 * *Files 9% similar despite different names*

```diff
@@ -210,7 +210,45 @@
     """
     fmt = "{{0:+.{0}f}}".format(nd)
     if abs(x.imag) < 10 ** (-nd):
         return fmt.format(x.real)
     if abs(x.real) < 10 ** (-nd):
         return fmt.format(x.imag) + "j"
     return short(x.real, nd) + short(1j * x.imag)
+
+
+def split(l):
+    """
+    Determine symbol used for assignment and split accordingly.
+
+    Parameters
+    ---------
+    l : str
+        Part of a line read from .win file.
+    """
+    if "=" in l:
+        return l.split("=")
+    elif ":" in l:
+        return l.split(":")
+    else:
+        return l.split()
+
+
+def format_matrix(A):
+    """
+    Format array to print it.
+
+    Parameters
+    ----------
+    A : array
+        Matrix that should be printed.
+
+    Returns
+    -------
+    str
+        Description of the matrix. Ready to be printed.
+    """
+    return "".join(
+        "   ".join("{0:+5.2f} {1:+5.2f}".format(x.real, x.imag) for x in a)
+        + "\n"
+        for a in A
+    )
```

### Comparing `irrep-1.8.3/irrep.egg-info/PKG-INFO` & `irrep-1.9.0/irrep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: irrep
-Version: 1.8.3
+Version: 1.9.0
 Summary: A tool to get symmetry proberties of ab-initio wavefunctions, irreduible representations and more.
 Home-page: https://github.com/stepan-tsirkin/irrep
 Author: Stepan S. Tsirkin
-Author-email: stepan.tsirkin@uzh.ch
+Author-email: stepan.tsirkin@ehu.eus
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IrRep
@@ -149,7 +151,9 @@
    known output.
 7. Make changes to the code as required. The `irrep` command line tool 
    will also be available inside this environment.
 
 You can verify your development environment by opening a Python interpretor 
 (e.g. running `python`) and running `import irrep` and then `print(irrep.__file__)`.
 This should print the path to your local repository containing irrep.
+
+
```

### Comparing `irrep-1.8.3/setup.py` & `irrep-1.9.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 import irrep
 
 setuptools.setup(
     name="irrep",
     author="Stepan S. Tsirkin",
-    author_email="stepan.tsirkin@uzh.ch",
+    author_email="stepan.tsirkin@ehu.eus",
     description="A tool to get symmetry proberties of ab-initio wavefunctions, irreduible representations and more.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "numpy",
         "scipy>=1.0",
         "spglib>=1.14",
```

