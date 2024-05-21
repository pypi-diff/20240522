# Comparing `tmp/pdr-1.0.7.tar.gz` & `tmp/pdr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdr-1.0.7.tar", last modified: Tue Apr 23 19:09:26 2024, max compression
+gzip compressed data, was "pdr-1.1.0.tar", last modified: Tue May 21 22:23:23 2024, max compression
```

## Comparing `pdr-1.0.7.tar` & `pdr-1.1.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.443641 pdr-1.0.7/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2276 2023-12-08 19:57:58.000000 pdr-1.0.7/LICENSE.md
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3952 2024-04-23 19:09:26.443641 pdr-1.0.7/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2863 2024-04-23 19:03:14.000000 pdr-1.0.7/README.md
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.415640 pdr-1.0.7/pdr/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1948 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/__init__.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.419640 pdr-1.0.7/pdr/_patches/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       54 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/_patches/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      505 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/_patches/patches.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    34581 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/_patches/six_new.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    34581 2024-03-28 17:21:19.000000 pdr-1.0.7/pdr/_patches/six_old.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4063 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/_scaling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8351 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/bit_handling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    12781 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/browsify.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8608 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/datatypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      261 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/errors.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.439641 pdr-1.0.7/pdr/formats/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1576 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5148 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/cassini.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    30523 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/checkers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1283 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/clementine.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      453 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/dawn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1100 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/diviner.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      542 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/epoxi.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3894 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/galileo.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2792 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/ihw.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1227 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/juno.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2411 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/lro.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      182 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/lroc.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      324 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mariner.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      397 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mer.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4987 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mex.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2566 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mgn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      963 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mgs.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1651 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/mro.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      276 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/msl_apxs.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      273 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/msl_ccam.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1463 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/msl_cmn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      323 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/msl_places.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4910 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/nh.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      557 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/odyssey.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3458 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/phoenix.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      633 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/pvo.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      281 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/rosetta.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      410 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/saturn_rpx.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1373 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/themis.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2152 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/ulysses.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1640 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/vega.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1877 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/viking.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3575 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/formats/voyager.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7162 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/func.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.439641 pdr-1.0.7/pdr/loaders/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.0.7/pdr/loaders/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3779 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/_helpers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     6101 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/datawrap.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4629 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/dispatch.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    11010 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/handlers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7880 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/image.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    31425 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/queries.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     8990 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/table.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4693 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/text.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1902 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/loaders/utility.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4843 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/np_utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.439641 pdr-1.0.7/pdr/parselabel/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.0.7/pdr/parselabel/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    15718 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/parselabel/pds3.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2861 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/parselabel/pds4.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      939 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/parselabel/utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    13514 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/pd_utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    36037 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/pdr.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3682 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/pdrtypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      512 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/pvl_utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.443641 pdr-1.0.7/pdr/tests/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5158 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/objects.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1991 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/tests/test_bit_handling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2478 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_browsify.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      752 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_data.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1526 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_datatypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      509 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_fits_load.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3218 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_func.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      396 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_image.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2785 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/tests/test_loader_helpers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      474 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_metadata.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2112 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_np_utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      601 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_parselabel_pds3.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1731 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_queries.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      548 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_scaling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1038 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/tests/test_table.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4818 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/test_vax.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1544 2023-12-08 19:57:58.000000 pdr-1.0.7/pdr/tests/utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7686 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4481 2024-04-23 19:03:14.000000 pdr-1.0.7/pdr/vax.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-04-23 19:09:26.443641 pdr-1.0.7/pdr.egg-info/
--rw-r--r--   0 sierra    (1000) sierra    (1000)     3952 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1980 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/SOURCES.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/dependency_links.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      200 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/requires.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2024-04-23 19:09:26.000000 pdr-1.0.7/pdr.egg-info/top_level.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2024-04-23 19:09:26.443641 pdr-1.0.7/setup.cfg
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1111 2024-04-23 19:03:14.000000 pdr-1.0.7/setup.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-05-21 22:23:23.115715 pdr-1.1.0/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2276 2023-12-08 19:57:58.000000 pdr-1.1.0/LICENSE.md
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3952 2024-05-21 22:23:23.115715 pdr-1.1.0/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2863 2024-04-23 19:03:14.000000 pdr-1.1.0/README.md
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-05-21 22:23:23.107715 pdr-1.1.0/pdr/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1948 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/__init__.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-05-21 22:23:23.111715 pdr-1.1.0/pdr/_patches/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       54 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/_patches/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      505 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/_patches/patches.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    34581 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/_patches/six_new.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    34581 2024-05-21 20:25:07.000000 pdr-1.1.0/pdr/_patches/six_old.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4176 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/_scaling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     8351 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/bit_handling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    12781 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/browsify.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     8608 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/datatypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      261 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/errors.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-05-21 22:23:23.111715 pdr-1.1.0/pdr/formats/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1576 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5148 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/cassini.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    30523 2024-05-01 22:28:05.000000 pdr-1.1.0/pdr/formats/checkers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1280 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/formats/clementine.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      453 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/dawn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1100 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/diviner.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      542 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/epoxi.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3894 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/galileo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2792 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/ihw.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1227 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/juno.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2411 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/lro.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      182 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/lroc.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      324 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/mariner.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      397 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/mer.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4987 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/mex.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2566 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/mgn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      963 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/mgs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1651 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/mro.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      276 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/msl_apxs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      273 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/msl_ccam.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1463 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/msl_cmn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      323 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/msl_places.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4910 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/nh.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      557 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/odyssey.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3458 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/phoenix.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      633 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/pvo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      281 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/rosetta.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      410 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/saturn_rpx.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1373 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/themis.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2152 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/ulysses.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1640 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/vega.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1877 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/viking.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3575 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/formats/voyager.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7162 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/func.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-05-21 22:23:23.115715 pdr-1.1.0/pdr/loaders/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.1.0/pdr/loaders/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3779 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/loaders/_helpers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     6101 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/loaders/datawrap.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4592 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/loaders/dispatch.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11010 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/loaders/handlers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7880 2024-04-30 23:00:16.000000 pdr-1.1.0/pdr/loaders/image.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    33014 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/loaders/queries.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    10044 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/loaders/table.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4693 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/loaders/text.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1902 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/loaders/utility.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4843 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/np_utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-05-21 22:23:23.115715 pdr-1.1.0/pdr/parselabel/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.1.0/pdr/parselabel/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    15678 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/parselabel/pds3.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2861 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/parselabel/pds4.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      939 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/parselabel/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    14189 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/pd_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    34635 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/pdr.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3682 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/pdrtypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      512 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/pvl_utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-05-21 22:23:23.115715 pdr-1.1.0/pdr/tests/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5158 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/objects.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1969 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/tests/test_bit_handling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2478 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_browsify.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      752 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_data.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1526 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_datatypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      509 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_fits_load.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3218 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_func.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      396 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_image.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2785 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/tests/test_loader_helpers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      474 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_metadata.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2112 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_np_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      539 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/tests/test_parselabel_pds3.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1699 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/tests/test_queries.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      548 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_scaling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1038 2024-04-23 19:03:14.000000 pdr-1.1.0/pdr/tests/test_table.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4818 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/test_vax.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1544 2023-12-08 19:57:58.000000 pdr-1.1.0/pdr/tests/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7748 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4664 2024-05-21 22:13:50.000000 pdr-1.1.0/pdr/vax.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2024-05-21 22:23:23.115715 pdr-1.1.0/pdr.egg-info/
+-rw-r--r--   0 sierra    (1000) sierra    (1000)     3952 2024-05-21 22:23:23.000000 pdr-1.1.0/pdr.egg-info/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1980 2024-05-21 22:23:23.000000 pdr-1.1.0/pdr.egg-info/SOURCES.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2024-05-21 22:23:23.000000 pdr-1.1.0/pdr.egg-info/dependency_links.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      200 2024-05-21 22:23:23.000000 pdr-1.1.0/pdr.egg-info/requires.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2024-05-21 22:23:23.000000 pdr-1.1.0/pdr.egg-info/top_level.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2024-05-21 22:23:23.115715 pdr-1.1.0/setup.cfg
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1111 2024-05-21 22:13:50.000000 pdr-1.1.0/setup.py
```

### Comparing `pdr-1.0.7/LICENSE.md` & `pdr-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/PKG-INFO` & `pdr-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 1.0.7
+Version: 1.1.0
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pdr-1.0.7/README.md` & `pdr-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/__init__.py` & `pdr-1.1.0/pdr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Collection, Optional, TYPE_CHECKING, Union
 
 from pdr.pdr import Data, Metadata
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-__version__ = "1.0.7"
+__version__ = "1.1.0"
 
 pkg_dir = _osp.abspath(_osp.dirname(__file__))
 
 
 def read(
     fp: Union[str, Path],
     debug: bool = False,
```

### Comparing `pdr-1.0.7/pdr/_patches/six_new.py` & `pdr-1.1.0/pdr/_patches/six_new.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/_patches/six_old.py` & `pdr-1.1.0/pdr/_patches/six_old.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/_scaling.py` & `pdr-1.1.0/pdr/_scaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,8 +108,10 @@
     # TODO: is this important?
     #     dtype = pds_to_numpy_type(struct.meta_data.data_type(),
     #     data=array, **scale_kwargs)
     special_constants = struct.meta_data.get("Special_Constants")
     array = apply_scaling_and_value_offset(
         array, special_constants=special_constants, **scale_kwargs
     )
-    return array
+    if hasattr(array, "mask"):
+        return np.ma.masked_array(np.asarray(array.data), array.mask)
+    return np.asarray(array)
```

### Comparing `pdr-1.0.7/pdr/bit_handling.py` & `pdr-1.1.0/pdr/bit_handling.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/browsify.py` & `pdr-1.1.0/pdr/browsify.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/datatypes.py` & `pdr-1.1.0/pdr/datatypes.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/__init__.py` & `pdr-1.1.0/pdr/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/cassini.py` & `pdr-1.1.0/pdr/formats/cassini.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/checkers.py` & `pdr-1.1.0/pdr/formats/checkers.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/clementine.py` & `pdr-1.1.0/pdr/formats/clementine.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 def get_offset(data, pointer):
     """
     HITS
     * clem_GEO
         * bsr_rdr_data
     """
-    start_row = int(re.split(r",|[(|)]", data.metadata[f"^{pointer}"])[2])
-    return True, (start_row - 1) * data.metadata["RECORD_BYTES"]
+    start_row = int(re.split(r",|[(|)]", data.metaget(f"^{pointer}"))[2])
+    return True, (start_row - 1) * data.metaget("RECORD_BYTES")
 
 
 def get_fn(data, object_name):
     """
     HITS
     * clem_GEO
         * bsr_rdr_data
     """
-    target = re.split(r",|[(|)]", data.metadata[f"^{object_name}"])[1]
+    target = re.split(r",|[(|)]", data.metaget(f"^{object_name}"))[1]
     return True, target
 
 
 def get_structure(block, name, filename, data, identifiers):
     """
     HITS:
     * clem_GEO
```

### Comparing `pdr-1.0.7/pdr/formats/diviner.py` & `pdr-1.1.0/pdr/formats/diviner.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/epoxi.py` & `pdr-1.1.0/pdr/formats/epoxi.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/galileo.py` & `pdr-1.1.0/pdr/formats/galileo.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/ihw.py` & `pdr-1.1.0/pdr/formats/ihw.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/juno.py` & `pdr-1.1.0/pdr/formats/juno.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/lro.py` & `pdr-1.1.0/pdr/formats/lro.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/mex.py` & `pdr-1.1.0/pdr/formats/mex.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/mgn.py` & `pdr-1.1.0/pdr/formats/mgn.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/mgs.py` & `pdr-1.1.0/pdr/formats/mgs.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/mro.py` & `pdr-1.1.0/pdr/formats/mro.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/msl_cmn.py` & `pdr-1.1.0/pdr/formats/msl_cmn.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/nh.py` & `pdr-1.1.0/pdr/formats/nh.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/odyssey.py` & `pdr-1.1.0/pdr/formats/odyssey.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/phoenix.py` & `pdr-1.1.0/pdr/formats/phoenix.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/pvo.py` & `pdr-1.1.0/pdr/formats/pvo.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/themis.py` & `pdr-1.1.0/pdr/formats/themis.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/ulysses.py` & `pdr-1.1.0/pdr/formats/ulysses.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/vega.py` & `pdr-1.1.0/pdr/formats/vega.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/viking.py` & `pdr-1.1.0/pdr/formats/viking.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/formats/voyager.py` & `pdr-1.1.0/pdr/formats/voyager.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/func.py` & `pdr-1.1.0/pdr/func.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/loaders/_helpers.py` & `pdr-1.1.0/pdr/loaders/_helpers.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/loaders/datawrap.py` & `pdr-1.1.0/pdr/loaders/datawrap.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/loaders/dispatch.py` & `pdr-1.1.0/pdr/loaders/dispatch.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,31 +73,27 @@
         return ReadText()
     if "DESC" in pointer:  # probably points to a reference file
         return ReadText()
     if "ARRAY" in pointer:
         return ReadArray()
     if "LINE_PREFIX_TABLE" in pointer:
         return TBD()
+    table_words = ["TABLE", "SPREADSHEET", "CONTAINER",
+                   "SERIES", "SPECTRUM", "HISTOGRAM"]
     if (
-        ("TABLE" in pointer)
-        or ("SPREADSHEET" in pointer)
-        or ("CONTAINER" in pointer)
-        or ("TIME_SERIES" in pointer)
-        or ("SERIES" in pointer)
-        or ("SPECTRUM" in pointer)
+        any(val in pointer for val in table_words)
+        and not any(val+"_HEADER" in pointer for val in table_words)
     ):
         return ReadTable()
     if "HEADER" in pointer:
         if looks_like_this_kind_of_file(
             data.file_mapping[pointer], FITS_EXTENSIONS
         ):
             return ReadFits()
         return ReadHeader()
-    if "HISTOGRAM" in pointer:
-        return ReadTable()
     # I have moved this below "table" due to the presence of a number of
     # binary tables named things like "Image Time Table". If there are pictures
     # of tables, we will need to do something more sophisticated.
     if (
         ("IMAGE" in pointer)
         or ("QUB" in pointer)
         or ("XDR_DOCUMENT" in pointer)
```

### Comparing `pdr-1.0.7/pdr/loaders/handlers.py` & `pdr-1.1.0/pdr/loaders/handlers.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/loaders/image.py` & `pdr-1.1.0/pdr/loaders/image.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/loaders/queries.py` & `pdr-1.1.0/pdr/loaders/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pathlib import Path
 from types import MappingProxyType
 from typing import (
     Any, Collection, Mapping, Optional, Sequence, TYPE_CHECKING, Union
 )
 import warnings
 
+from dustgoggles.func import gmap
 from multidict import MultiDict
 
 from pdr.datatypes import sample_types
 from pdr.formats import check_special_block, check_special_offset
 from pdr.func import specialize
 from pdr.loaders._helpers import (
     count_from_bottom_of_file,
@@ -141,17 +142,18 @@
             "Objects that contain both 'conventional' line pre/suffixes and "
             "ISIS-style side/back/bottomplanes are not supported."
         )
     if len(gt0f((props["rowpad"], props["colpad"], props["bandpad"]))) > 1:
         raise NotImplementedError(
             "ISIS-style axplanes along multiple axes are not supported."
         )
-    if (props["linepad"] > 0) and props["band_storage_type"] not in (
-        None,
-        "LINE_INTERLEAVED",
+    if (
+        (props["linepad"] > 0)
+        and props["band_storage_type"] not in (None, "LINE_INTERLEAVED")
+        and props["nbands"] > 1
     ):
         raise NotImplementedError(
             "'Conventional' line pre/suffixes are not supported for non-BIL "
             "multiband images."
         )
 
 
@@ -289,15 +291,17 @@
     """
     target = data.metaget_(name)
     if isinstance(target, Mapping) or target is None:
         target = data.metaget_(pointerize(name))
     return target
 
 
-def data_start_byte(identifiers: DataIdentifiers, block: Mapping, target, fn) -> int:
+def data_start_byte(
+    identifiers: DataIdentifiers, block: Mapping, target, fn
+) -> int:
     """
     Determine the first byte of the data in a file from its pointer.
     """
     if (block is not None) and ("RECORD_BYTES" in block.keys()):
         record_bytes = block["RECORD_BYTES"]
     else:
         record_bytes = identifiers["RECORD_BYTES"]
@@ -471,18 +475,14 @@
     (see `read_table_structure()`. If that specification contains byte-position
     information for columns, further parse them into explicit offsets. If the
     table is binary, also create a numpy dtype object (usually a compound
     dtype). These typically become inputs for np.fromfile (for binary tables)
     or for one of several ASCII parsers.
     """
     fmtdef = read_table_structure(block, name, fn, data, identifiers)
-    if fmtdef['DATA_TYPE'].str.contains('VAX_REAL').any():
-        raise NotImplementedError(
-            "VAX reals are not currently supported in tables."
-        )
     if "BYTES" not in fmtdef.columns:
         if _probably_ascii(block, fmtdef, name):
             # this is either a nonstandard fixed-width table or a DSV table.
             # don't bother trying to calculate explicit byte offsets.
             return fmtdef, None
         fmtdef["BYTES"] = float('nan')
     if fmtdef['BYTES'].isna().any():
@@ -491,15 +491,14 @@
         except (KeyError, TypeError, IndexError):
             raise ValueError("This table's byte sizes are underspecified.")
     for end in ("_PREFIX", "_SUFFIX", ""):
         length = block.get(f"ROW{end}_BYTES")
         if length is not None:
             fmtdef[f"ROW{end}_BYTES"] = length
     from pdr.pd_utils import compute_offsets, insert_sample_types_into_df
-
     if "START_BYTE" in fmtdef.columns:
         fmtdef = compute_offsets(fmtdef)
     if _probably_ascii(block, fmtdef, name):
         # don't attempt to compute numpy dtypes for ASCII tables
         return fmtdef, None
     return insert_sample_types_into_df(fmtdef, identifiers)
 
@@ -523,50 +522,76 @@
     called by `parse_table_structure()` or `parse_array_structure()`, but some
     special cases use it on its own.
     """
     if "HISTOGRAM" in name:
         fields = get_histogram_fields(block)
     else:
         fields, _ = read_format_block(block, name, fn, data, identifiers)
-    # give columns unique names so that none of our table handling explodes
     import pandas as pd
+    from pdr.pd_utils import reindex_df_values
 
     fmtdef = pd.DataFrame.from_records(fields)
     if "NAME" not in fmtdef.columns:
         fmtdef["NAME"] = name
-
-    from pdr.pd_utils import reindex_df_values
+    # give columns unique names so that none of our table handling explodes
     return reindex_df_values(fmtdef)
 
 
 def parse_array_structure(
     name: str,
     block: MultiDict,
     fn: str,
     data: PDRLike,
     identifiers: DataIdentifiers
-) -> tuple[Optional[pd.DataFrame], Optional[str]]:
-    """
-    Modification of `parse_table_structure()` for the special needs of ARRAYs.
-    """
+) -> tuple[Optional[pd.DataFrame], Optional[Union[str, np.dtype]]]:
+    """`parse_table_structure()` modified for the special needs of ARRAYs."""
     if not block.get("INTERCHANGE_FORMAT") == "BINARY":
         return None, None
     has_sub = check_array_for_subobject(block)
     if not has_sub:
         dt = sample_types(block["DATA_TYPE"], block["BYTES"], True)
         return None, dt
     fmtdef = read_table_structure(block, name, fn, data, identifiers)
-    # Sometimes arrays define start_byte, sometimes their elements do
+    # Sometimes ARRAYS give START_BYTE at top level; sometimes only their
+    # elements do. We want to defer responsibility for figuring this out to
+    # compute_offsets(). This satisfies its type expectations.
     if "START_BYTE" in fmtdef.columns:
         fmtdef['START_BYTE'].fillna(1, inplace=True)
 
     from pdr.pd_utils import insert_sample_types_into_df
     return insert_sample_types_into_df(fmtdef, identifiers)
 
 
+def create_placeholder_field(block_info, definition):
+    dummy_column = {
+        'NAME': f'PLACEHOLDER_{definition["NAME"]}',
+        'DATA_TYPE': 'VOID',
+        'START_BYTE': definition['START_BYTE'],
+        'BYTES': 0,
+        'BLOCK_REPETITIONS': definition.get("REPETITIONS", 1),
+        'BLOCK_BYTES': definition.get("BYTES"),
+        'BLOCK_NAME': f'PLACEHOLDER_{block_info["BLOCK_NAME"]}'
+    }
+    if definition.get("AXIS_ITEMS"):
+        dummy_column = dummy_column | {'AXIS_ITEMS': definition['AXIS_ITEMS']}
+    return dummy_column
+
+
+PDS3_STRUCTURED_DATA_PARAMETERS = (
+    "ARRAY",
+    "COLLECTION",
+    "COLUMN",
+    'CONTAINER',
+    "ELEMENT",
+    "FIELD",
+    "PRIMITIVE_ARRAY",
+    "STRUCTURE",
+)
+
+
 def read_format_block(
     block: MultiDict,
     object_name: str,
     fn: str,
     data: PDRLike,
     identifiers: DataIdentifiers,
     within_container: bool = False
@@ -587,71 +612,82 @@
     block_info = {
         f"BLOCK_NAME": block.get("NAME"),
         f"BLOCK_REPETITIONS": block.get("REPETITIONS", 1),
         f"BLOCK_BYTES": block.get("BYTES")
     }
     while "^STRUCTURE" in [obj[0] for obj in format_block]:
         format_block = inject_format_files(format_block, object_name, fn, data)
-    fields, needs_placeholder, add_placeholder = [], False, False
+    fields, needs_placeholder, add_placeholder, reps = [], False, False, None
     for item_type, definition in format_block:
+        if item_type not in PDS3_STRUCTURED_DATA_PARAMETERS:
+            # things formally unrelated to data structure (e.g. physical units)
+            continue
         if item_type == "ARRAY":
             if not check_array_for_subobject(definition):
                 item_type = "PRIMITIVE_ARRAY"
         if item_type in ("COLUMN", "FIELD", "ELEMENT", "PRIMITIVE_ARRAY"):
+            # TODO: this `if "^STRUCTURE"...` block smells incredibly bad. Why
+            #  is it guarded by the COLUMN/FIELD/ELEMENT/PRIMITIVE_ARRAY
+            #  contitional? Why are we scrupulously calling MultiDict.add()
+            #  and then immediately casting `definition` back to `dict`,
+            #  discarding any duplicate keys we took such care to retain? What
+            #  nightmarish class of cases does this catch?
             if "^STRUCTURE" in definition:
-                definition_l = list(definition.items())
-                definition_l = inject_format_files(definition_l, object_name, fn, data)
-                # TODO: this smells bad. why are we scrupulously calling MultiDict.add()
-                #  and then immediately casting definition back to dict (which would 
-                #  discard any of the duplicate keys we so carefully added)?
+                definition_l = inject_format_files(
+                    list(definition.items()), object_name, fn, data
+                )
                 definition = MultiDict()
                 for key, val in definition_l:
                     definition.add(key, val)
             obj = dict(definition) | block_info
-            repeat_count = definition.get("ITEMS")
+            # TODO: also smells very bad. Why is this inside a branch that
+            #  matches many things that are not ARRAYS (but does not match
+            #  every ARRAY)?
             if "BIT_ELEMENT" in obj.keys():
-                raise NotImplementedError("BIT_ELEMENTS in ARRAYS not yet supported")
+                raise NotImplementedError(
+                    "BIT_ELEMENTS in ARRAYS not yet supported"
+                )
+            reps = definition.get("ITEMS")
             obj = add_bit_column_info(obj, definition, identifiers)
-            add_placeholder = False
         elif item_type in ("CONTAINER", "COLLECTION", "ARRAY"):
-            if within_container is True and len(fields) == 0:
+            # This is a somewhat convoluted way to tell the caller to place a
+            # PLACEHOLDER pseudo-field between a running sequence of fields
+            # and the fields this function returns.
+            if within_container is False or len(fields) == 0:
                 needs_placeholder = True
             obj, add_placeholder = read_format_block(
-                definition, object_name, fn, data, identifiers, True
+                definition, object_name, fn, data, identifiers
             )
             if item_type == "ARRAY":
                 add_placeholder = True
             else:
-                repeat_count = definition.get("REPETITIONS")
+                reps = definition.get("REPETITIONS")
         else:
-            continue
+            # this suggests we made a typo
+            raise NotImplementedError(f"No defined behavior for {item_type}.")
+        # Format-level data structures like CONTAINERs should not be exposed
+        # to the parser; we only care about the things they contain. However,
+        # because START_BYTE is always expressed relative to the parent data
+        # structure in PDS3 table format specifications, we still need to
+        # account for cases in which these structures are separated from
+        # preceding elements by pad bytes / whitespace. These PLACEHOLDER
+        # pseudo-fields inform downstream code about spacing while also
+        # signaling that bytes / characters within that interval should be
+        # ignored by the parser.
         if add_placeholder is True:
-            dummy_column = {
-                'NAME': f'PLACEHOLDER_{definition["NAME"]}',
-                'DATA_TYPE': 'VOID',
-                'START_BYTE': definition['START_BYTE'],
-                'BYTES': 0,
-                'BLOCK_REPETITIONS': definition.get("REPETITIONS", 1),
-                'BLOCK_BYTES': definition.get("BYTES"),
-                'BLOCK_NAME': f'PLACEHOLDER_{block_info["BLOCK_NAME"]}'
-            }
-            if definition.get("AXIS_ITEMS"):
-                dummy_column = dummy_column | {'AXIS_ITEMS': definition['AXIS_ITEMS']}
-            fields.append(dummy_column)
-        # containers can have REPETITIONS,
-        # and some "columns" contain a lot of columns (ITEMS)
-        # repeat the definition, renaming duplicates, for these cases
-        if repeat_count is not None:
-            fields = append_repeated_object(obj, fields, repeat_count)
+            fields.append(create_placeholder_field(block_info, definition))
+        # CONTAINERs can have REPETITIONS, and some so-called COLUMNS contain
+        # a lot of "columns" (ITEMS) as the term is generally used. We express
+        # these cases by simply repeating the definition, renaming duplicates.
+        if reps is not None:
+            fields = append_repeated_object(obj, fields, reps)
+        elif isinstance(obj, list):
+            fields.extend(obj)
         else:
-            if type(obj) == list and object_name in ("COLLECTION", "ARRAY"):
-                # list obj should only happen in COLLECTIONs and ARRAYs; extra guard
-                fields.extend(obj)
-            else:
-                fields.append(obj)
+            fields.append(obj)
     # semi-legal top-level containers not wrapped in other objects
     if object_name == "CONTAINER":
         if (repeat_count := block.get("REPETITIONS")) is not None:
             fields = list(chain(*[fields for _ in range(repeat_count)]))
     return fields, needs_placeholder
 
 
@@ -676,17 +712,17 @@
 def inject_format_files(
     block: list[tuple[str, Any]],
     name: str,
     fn: str,
     data: PDRLike
 ) -> list[tuple[str, Any]]:
     """
-    Load format files (recursively, if necessary) referenced by a
-    TABLE/SPREADSHEET/CONTAINER/COLLECTION definition and insert them into
-    that definition.
+    Load format files referenced by a TABLE/SPREADSHEET/CONTAINER/COLLECTION
+    definition (or recursively referenced by a referenced format file), parse
+    them, and insert them into the referencing definition.
     """
     format_fns = {
         ix: kv[1] for ix, kv in enumerate(block) if kv[0] == "^STRUCTURE"
     }
     # make sure to insert the structure blocks in the correct order --
     # and remember that keys are not unique, so we have to use the index
     assembled_structure = []
@@ -717,17 +753,15 @@
             Path(find_repository_root(Path(fn)), label_path)
             for label_path in ("label", "LABEL")
         ]
         label_fns += [Path(path, format_file) for path in repo_paths]
     except (ValueError, IndexError):
         pass
     try:
-        fmtpath = check_cases(label_fns)
-        aggregations, _ = read_pvl(fmtpath)
-        return literalize_pvl(aggregations)
+        return read_pvl(check_cases(label_fns))[0]
     except FileNotFoundError:
         warnings.warn(
             f"Unable to locate external table format file:\n\t {format_file}. "
             f"Try retrieving this file and placing it in the same path as the "
             f"{name} file."
         )
         raise FileNotFoundError
@@ -773,22 +807,25 @@
     ]
     start_bytes = {
         m: data_start_byte(
             identifiers, get_block(data, m), get_target(data, m), fn
         )
         for m in matches
     }
-    ordered = sorted(matches, key=lambda m: start_bytes[m])
-    ordered = tuple(map(str.lower, ordered))
+    ordered = gmap(str.lower, sorted(matches, key=lambda m: start_bytes[m]))
     if other_stubs is not None:
-        noheader = tuple(filter(lambda n: (not n.endswith('header') or n.upper() in other_stubs), ordered))
+        noheader = filter(
+            lambda n: (not n.endswith('header') or n.upper() in other_stubs),
+            ordered
+        )
         num_other_stubs = len(other_stubs)
     else:
-        noheader = tuple(filter(lambda n: not n.endswith('header'), ordered))
+        noheader = filter(lambda n: not n.endswith('header'), ordered)
         num_other_stubs = 0
+    noheader = tuple(noheader)
     # this condition typically implies a "stub" primary hdu whose header but
     # not body is mentioned in the PDS label
     has_stub_primary = (
         (len(noheader) != (len(matches) + num_other_stubs) / 2)
         and (list(start_bytes.keys())[0].lower() not in noheader)
     )
     if not name.endswith('header') or name in noheader:
```

### Comparing `pdr-1.0.7/pdr/loaders/table.py` & `pdr-1.1.0/pdr/loaders/table.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 from pdr import bit_handling
 from pdr.datatypes import sample_types
 from pdr.loaders._helpers import check_explicit_delimiter
 from pdr.loaders.queries import get_array_num_items
 from pdr.np_utils import np_from_buffered_io, enforce_order_and_object
 from pdr.pd_utils import (
-    booleanize_booleans, compute_offsets, convert_ebcdic, convert_ibm_reals
+    booleanize_booleans, compute_offsets, convert_ebcdic, convert_ibm_reals,
+    convert_vax_reals
 )
 from pdr.utils import decompress, head_file
 
 if TYPE_CHECKING:
     from pdr.pdrtypes import DataIdentifiers
 
 
@@ -119,14 +120,15 @@
     with decompress(fn) as f:
         table = np_from_buffered_io(
             f, dtype=dt, offset=start_byte, count=count
         )
     table = enforce_order_and_object(table)
     table = pd.DataFrame(table)
     table = convert_ibm_reals(table, fmtdef)
+    table = convert_vax_reals(table, fmtdef)
     table.columns = fmtdef.NAME.tolist()
     table = convert_ebcdic(table, fmtdef)
     table = booleanize_booleans(table, fmtdef)
     table = bit_handling.expand_bit_strings(table, fmtdef)
     return table
 
 
@@ -151,14 +153,37 @@
         raise IndexError("Mismatched column length.")
     for c, d in zip(table.columns, table.dtypes):
         if d.name == "object":
             table[c] = table[c].str.strip(PAD_CHARACTERS)
     return table
 
 
+def read_strictly_fixed(string_buffer, specs, padchars=PAD_CHARACTERS):
+    from collections import defaultdict
+    from more_itertools import windowed
+    startwidth = specs[0][1] - specs[0][0]
+    midwidths = {i0 + 1: b - a for i0, (a, b) in enumerate(specs[1:-1])}
+    lastwidth = specs[-1][1] - specs[-1][0]
+    skips = {
+        i1: (c - b) for i1, ((_a, b), (c, _d)) in enumerate(windowed(specs, 2))
+    }
+    cols = defaultdict(list)
+    while True:
+        firstfield = string_buffer.read(startwidth)
+        if firstfield == '':
+            break
+        cols[0].append(firstfield.strip(padchars))
+        string_buffer.read(skips[0])
+        for i0, width in midwidths.items():
+            cols[i0].append(string_buffer.read(width).strip(padchars))
+            string_buffer.read(skips[i0])
+        cols[len(specs)].append(string_buffer.read(lastwidth).strip(padchars))
+    return pd.DataFrame(cols)
+
+
 def _read_fwf_with_colspecs(
     fmtdef: pd.DataFrame, string_buffer: StringIO
 ) -> pd.DataFrame:
     """
     Attempt to read an ASCII table as a fixed-width file using column
     boundaries specified by or inferred from its format definition.
     """
@@ -178,14 +203,15 @@
             col_length = int(record["ITEM_BYTES"])
         colspecs.append(
             (record["SB_OFFSET"], record["SB_OFFSET"] + col_length)
         )
     # NOTE: the 'delimiter' argument to read_fwf() does _not_ specify
     # an actual delimiter. It defines characters the read_fwf parser
     # will treat as 'padding' and strip from each table element.
+    # return read_strictly_fixed(string_buffer, colspecs, PAD_CHARACTERS)
     table = pd.read_fwf(
         string_buffer,
         header=None,
         colspecs=colspecs,
         delimiter=PAD_CHARACTERS
     )
     return table
```

### Comparing `pdr-1.0.7/pdr/loaders/text.py` & `pdr-1.1.0/pdr/loaders/text.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/loaders/utility.py` & `pdr-1.1.0/pdr/loaders/utility.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/np_utils.py` & `pdr-1.1.0/pdr/np_utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/parselabel/pds3.py` & `pdr-1.1.0/pdr/parselabel/pds3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Parsing utilities for PDS3 labels."""
-from ast import literal_eval
 import re
+import warnings
+from ast import literal_eval
 from numbers import Number
 from operator import eq
 from pathlib import Path
-from typing import Iterable, Mapping, Optional, Type, Union, Collection, Any, \
-    Hashable, Callable
-import warnings
+from typing import (
+    Iterable, Optional, Type, Union, Collection, Any, Callable
+)
 
 from cytoolz import groupby, identity
 from dustgoggles.func import constant
 from dustgoggles.structures import dig_for_keys
 from more_itertools import split_before
 from multidict import MultiDict
 
 from pdr.parselabel.utils import trim_label, DEFAULT_PVL_LIMIT
 from pdr.utils import decompress
 
-
 PVL_BLOCK_INITIALS = ("OBJECT", "GROUP", "BEGIN_OBJECT", "BEGIN_GROUP")
 PVL_BLOCK_TERMINAL = re.compile(r"END(_OBJECT|$)")
 PVL_QUANTITY_VALUE = re.compile(r"((\d|\.|-)+([eE]-?\d+)?)|NULL|UNK|N/A")
 PVL_QUANTITY_UNITS = re.compile(r"<(.*)>")
 
 
 def extract_pvl_block_terminal(line: str) -> Optional[str]:
@@ -137,15 +137,15 @@
         None, map(lambda line: line.strip(), uncommented_label.split("\n"))
     )
     statements = chunk_statements(trimmed_lines)
     mapping, params = BlockParser().parse_statements(statements)
     if deduplicate_pointers:
         pointers = get_pds3_pointers(mapping)
         mapping, params = index_duplicate_pointers(pointers, mapping, params)
-    return mapping, params
+    return literalize_pvl(mapping), params
 
 
 def read_pvl(
     filename: Union[str, Path],
     deduplicate_pointers: bool = True,
     max_size: int = DEFAULT_PVL_LIMIT
 ) -> tuple[MultiDict, list[str]]:
@@ -157,17 +157,15 @@
 
 
 def parse_pvl_quantity_object(obj: str) -> dict[str, Union[str, Number]]:
     """
     Parse a PVL quantity string into a dict like {'value': 2, 'units': 'km'}.
     """
     return {
-        "value": literalize_pvl(
-            re.search(PVL_QUANTITY_VALUE, obj).group()
-        ),
+        "value": literalize_pvl(re.search(PVL_QUANTITY_VALUE, obj).group()),
         "units": literalize_pvl(re.search(PVL_QUANTITY_UNITS, obj).group(1)),
     }
 
 
 def parse_pvl_quantity_statement(statement: str) -> Any:
     """
     parse pvl statements including quantities. returns quantities as mappings.
@@ -190,15 +188,15 @@
     if len(output) == 1:
         return output[0]
     return tuple(output)
 
 
 def multidict_dig_and_edit(
     input_multidict: MultiDict,
-    target: Any,
+    target: Any = None,
     input_object: Any = None,
     predicate: Callable[[Any, Any], bool] = eq,
     setter_function: Callable = None,
     key_editor: bool = False,
     keep_values: bool = True,
     mtypes: tuple[type, ...] = (MultiDict,)
 ) -> MultiDict:
@@ -317,25 +315,26 @@
         except (SyntaxError, ValueError):
             pass
         except IndexError:
             a = 1
     return obj
 
 
-def literalize_pvl_block(block: MultiDict) -> MultiDict:
+def literalize_pvl_block(block: MultiDict[str, Any]) -> MultiDict[str, Any]:
     """
     Parse the values of an entire (possibly-nested) MultiDict whose values are
     PVL strings into Python objects.
     """
     literalized = multidict_dig_and_edit(
         block,
         None,
         predicate=lambda x, y: True,
         setter_function=lambda _, obj: literalize_pvl(obj),
     )
+    # noinspection PyTypeChecker
     return literalized
 
 
 def get_pds3_pointers(
     label: Optional[MultiDict] = None,
 ) -> tuple[str]:
     """
@@ -393,23 +392,21 @@
                 indexed_depointer = f"{depointer}_{ix}"
                 mapping = multidict_dig_and_edit(
                     input_multidict=mapping,
                     target=pointer,
                     input_object=list(range(len(group))),
                     setter_function=set_key_index,
                     key_editor=True,
-                    keep_values=True,
                 )
                 mapping = multidict_dig_and_edit(
                     input_multidict=mapping,
                     target=depointer,
                     input_object=list(range(len(group))),
                     setter_function=set_key_index,
                     key_editor=True,
-                    keep_values=True,
                 )
                 params.append(indexed_pointer)
                 params.append(indexed_depointer)
                 params.remove(pointer)
                 params.remove(depointer)
     return mapping, params
```

### Comparing `pdr-1.0.7/pdr/parselabel/pds4.py` & `pdr-1.1.0/pdr/parselabel/pds4.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/parselabel/utils.py` & `pdr-1.1.0/pdr/parselabel/utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/pd_utils.py` & `pdr-1.1.0/pdr/pd_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pandas.errors import SettingWithCopyWarning
 
 from pdr.datatypes import sample_types
 from pdr.formats import check_special_sample_type
 from pdr.np_utils import (
     enforce_order_and_object, ibm32_to_np_f32, ibm64_to_np_f64
 )
+from pdr import vax
 
 if TYPE_CHECKING:
     from pdr.pdrtypes import DataIdentifiers
 
 
 def numeric_columns(df: pd.DataFrame) -> list[Hashable]:
     """Return names of all 'numeric' columns in a DataFrame."""
@@ -339,7 +340,24 @@
                 converted = converted.astype(np.float32)
         reals[field['NAME']] = converted
         # IBM longs just get more precise, not wider-ranged, so we don't need
         # to check for longlong or anything like that
     for k, v in reals.items():
         df[k] = v
     return df
+
+
+def convert_vax_reals(data: pd.DataFrame, properties: pd.DataFrame) -> pd.DataFrame:
+    """If any columns in a DataFrame are in 32-bit VAX real format,
+    convert them to 32-bit float."""
+    if not properties['DATA_TYPE'].str.contains('VAX').any():
+        return data
+    reals = {}
+    for _, field in properties.iterrows():
+        if not re.match(r'VAX.*REAL', field['DATA_TYPE']):
+            continue
+        func = vax.from_vax32  # TODO: if field['BYTES'] == 4 else vax.from_vax64
+        converted = func(data[field['NAME']].values)
+        reals[field['NAME']] = converted
+    for k, v in reals.items():
+        data[k] = v
+    return data
```

### Comparing `pdr-1.0.7/pdr/pdr.py` & `pdr-1.1.0/pdr/pdr.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Callable,
     Collection,
     Literal,
     Mapping,
     Optional,
     Sequence,
     TYPE_CHECKING,
-    Union,
+    Union
 )
 import warnings
 
 import Levenshtein as lev
 from cytoolz import countby, identity
 from dustgoggles.dynamic import Dynamic
 from dustgoggles.func import gmap
@@ -26,15 +26,14 @@
 from multidict import MultiDict
 
 from pdr.errors import AlreadyLoadedError, DuplicateKeyWarning
 from pdr.formats import check_special_fn, special_image_constants
 from pdr.parselabel.pds3 import (
     depointerize,
     get_pds3_pointers,
-    literalize_pvl,
     pointerize,
     read_pvl,
 )
 from pdr.parselabel.pds4 import reformat_pds4_tools_label
 from pdr.parselabel.utils import DEFAULT_PVL_LIMIT
 from pdr.pdrtypes import DataIdentifiers
 from pdr.utils import (
@@ -65,49 +64,26 @@
         **kwargs
     ):
         """"""
         mapping, params = mapping_params
         super().__init__(mapping, **kwargs)
         self.fieldcounts = countby(identity, params)
         self.standard = standard
-        if self.standard == "PDS3":
-            self.formatter = literalize_pvl
-        elif self.standard in ("PDS4", "FITS"):
-            # we're trusting that pds4_tools and/or our astropy wrapper
-            # stringified everything correctly.
-            # also note that this has no
-            # default capacity to describe PDS4 units -- you have to
-            # explicitly check the 'attrib' attribute of the XML node,
-            # which is not preserved by Label.to_dict().
-            # TODO: replace pds4_tools' Label.to_dict() with our own
-            #  literalizer function.
-            self.formatter = identity
-        else:
-            raise NotImplementedError(
-                "Syntaxes other than PDS3-style PVL, preprocessed PDS4 XML,"
-                "and preprocessed FITS headers are not yet implemented."
-            )
-        # note that 'directly' caching these methods can result in recursive
-        # reference chains behind the lru_cache API that can prevent the
-        # Metadata object from being garbage-collected, which is why they are
-        # hidden behind these wrappers. there may be a cleaner way to do this.
+        self.refresh_cache()
+
+    # note that 'directly' caching these methods can result in recursive
+    # reference chains behind the lru_cache API that can prevent the
+    # Metadata object from being garbage-collected, which is why they are
+    # hidden behind these wrappers. there may be a cleaner way to do this.
+    def refresh_cache(self):
         self._metaget_interior = _metaget_factory(self)
         self._metablock_interior = _metablock_factory(self)
 
-    def __getitem__(self, key):
-        """"""
-        value = super().__getitem__(key)
-        return self.formatter(value)
-
     def metaget(
-        self,
-        text: str,
-        default: Any = None,
-        evaluate: bool = True,
-        warn: bool = True
+        self, text: str, default: Any = None, warn: bool = True
     ) -> Any:
         """
         get the first value from this object whose key exactly matches `text`,
         even if it is nested inside a mapping. optionally evaluate it using
         `self.formatter`. raise a warning if there are multiple keys matching
         this.
 
@@ -122,37 +98,32 @@
             return default
         if (count > 1) and (warn is True):
             warnings.warn(
                 f"More than one value for {text} exists in the metadata. "
                 f"Returning only the first.",
                 DuplicateKeyWarning,
             )
-        return self._metaget_interior(text, default, evaluate)
+        return self._metaget_interior(text, default)
 
-    def metaget_(
-        self, text: str, default: Any = None, evaluate: bool = True
-    ) -> Any:
+    def metaget_(self, text: str, default: Any = None) -> Any:
         """quiet-by-default version of metaget"""
-        return self.metaget(text, default, evaluate, False)
+        return self.metaget(text, default, False)
 
-    def metaget_fuzzy(self, text: str, evaluate: bool = True) -> Any:
+    def metaget_fuzzy(self, text: str) -> Any:
         """Like `metaget()`, but fuzzy-matches key names."""
         levratio = {
             key: lev.ratio(key, text) for key in set(self.fieldcounts.keys())
         }
         if levratio == {}:
             return None
         peak = max(levratio.values())
-        for k, v in levratio.items():
-            if v == peak:
-                return self.metaget(k, None, evaluate)
-
-    def metablock(
-        self, text: str, evaluate: bool = True, warn: bool = True
-    ) -> Optional[Mapping]:
+        for k, v in filter(lambda kv: kv[1] == peak, levratio.items()):
+            return self.metaget(k)
+
+    def metablock(self, text: str, warn: bool = True) -> Optional[Mapping]:
         """
         get the first value from this object whose key exactly
         matches `text`, even if it is nested inside a mapping, if the value
         itself is a mapping (e.g., nested PVL block, XML 'area', etc.)
         evaluate it using self.formatter. raise a warning if there are
         multiple keys matching this.
         if there is no key matching 'text', will evaluate and return the
@@ -169,30 +140,31 @@
             return None
         if (count > 1) and (warn is True):
             warnings.warn(
                 f"More than one block named {text} exists in the metadata. "
                 f"Returning only the first.",
                 DuplicateKeyWarning,
             )
-        return self._metablock_interior(text, evaluate)
+        return self._metablock_interior(text)
 
-    def metablock_(
-        self, text: str, evaluate: bool = True
-    ) -> Optional[Mapping]:
+    def metablock_(self, text: str) -> Optional[Mapping]:
         """quiet-by-default version of metablock"""
-        return self.metablock(text, evaluate, False)
+        return self.metablock(text, False)
 
     def __str__(self):
         """"""
         return f"Metadata({prettify_multidict(self)})"
 
     def __repr__(self):
         """"""
         return f"Metadata({prettify_multidict(self)})"
 
+    _metaget_interior: Callable[[str, Any], Any]
+    _metablock_interior: Callable[[str], Mapping]
+
 
 class DebugExceptionPreempted(Exception):
     """
     Stub Exception subclass for selectively ignoring Exceptions from load
     failures when not in debug mode.
     """
     pass
@@ -272,16 +244,15 @@
             self.standard = "PDS3"
         try:
             self.metadata = self.read_metadata(pvl_limit=pvl_limit)
         except (UnicodeError, FileNotFoundError) as ex:
             raise ValueError(
                 f"Can't load this product's metadata: {ex}, {type(ex)}"
             )
-        self._metaget_interior = _metaget_factory(self.metadata)
-        self._metablock_interior = _metablock_factory(self.metadata)
+        self.load_metadata_changes()
         if self.standard == "PDS4":
             return
         if primary_format is not None:
             self._init_primary_format()
             return
         self.pointers = get_pds3_pointers(self.metadata)
         # if self.pointers is None, we've probably got a weird edge case where
@@ -295,14 +266,21 @@
             for field in get_annotations(DataIdentifiers)
         }
         # it never does us any favors to have tuples or sets in here
         for k, v in self.identifiers.items():
             if isinstance(v, (tuple, set)):
                 self.identifiers[k] = str(v)
 
+    # noinspection PyProtectedMember
+    def load_metadata_changes(self):
+        if "_metaget_interior" in dir(self):
+            self.metadata.refresh_cache()
+        self._metaget_interior = self.metadata._metaget_interior
+        self._metablock_interior = self.metadata._metablock_interior
+
     def _init_pds4(self):
         """use pds4_tools to open pds4 files, but in our interface idiom."""
         # pds4_tools currently uses an outdated version of six.py that is
         # incompatible with Python 3.12. Replace it if necessary at runtime.
         from pdr._patches import patch_pds4_tools_six
 
         patch_pds4_tools_six()
@@ -338,15 +316,17 @@
         # TODO: make this not add objects again if called multiple times
         for pointer in self.pointers:
             object_name = depointerize(pointer)
             if is_trivial(object_name):
                 continue
             self.index.append(object_name)
 
-    def _object_to_filename(self, object_name: str) -> Union[str, list[str]]:
+    def _object_to_filename(
+        self, object_name: str
+    ) -> Union[str, list[str], Optional[tuple[Path, ...]]]:
         """
         Construct one or more on-disk search paths for the file that contains
         a named data object. Does not actually check if files exist at those
         paths (typically performed by calls to `utils.check_cases()).
         """
         is_special, special_target = check_special_fn(
             self, object_name, self.identifiers
@@ -545,15 +525,17 @@
         """
         structure = self._pds4_structures[object_name]
         from pds4_tools.reader.label_objects import Label
 
         if isinstance(structure, Label):
             setattr(self, "label", structure)
         elif structure.is_array():
-            setattr(self, object_name, structure.data)
+            import numpy as np
+
+            setattr(self, object_name, np.asarray(structure.data))
         elif structure.is_table():
             from pdr.pd_utils import structured_array_to_df
 
             df = structured_array_to_df(structure.data)
             df.columns = df.columns.str.replace(r"GROUP_?\d+", "", regex=True)
             df.columns = df.columns.str.strip(", ")
             setattr(self, object_name, df)
@@ -685,58 +667,48 @@
             return consts
         from pdr._scaling import find_special_constants
         return find_special_constants(
             self.metadata, self[object_name], object_name
         )
 
     def metaget(
-        self,
-        text: str,
-        default: Any = None,
-        evaluate: bool = True,
-        warn: bool = True
+        self, text: str, default: Any = None, warn: bool = True
     ) -> Any:
         """
         get the first value from this object's metadata whose key exactly
         matches `text`, even if it is nested inside a mapping. evaluate it
         using `self.metadata.formatter`.
 
         Warning:
             this function's return values are memoized for performance.
             updating elements of self.metadata that have already been accessed
             with this function will not update future calls to this function.
         """
-        return self.metadata.metaget(text, default, evaluate, warn)
+        return self.metadata.metaget(text, default, warn)
 
-    def metaget_(
-        self, text: str, default: Any = None, evaluate: bool = True
-    ) -> Any:
+    def metaget_(self, text: str, default: Any = None) -> Any:
         """quiet-by-default version of metaget"""
-        return self.metadata.metaget(text, default, evaluate, False)
+        return self.metadata.metaget(text, default, False)
 
-    def metablock(
-        self, text: str, evaluate: bool = True, warn: bool = True
-    ) -> Optional[Mapping]:
+    def metablock(self, text: str, warn: bool = True) -> Optional[Mapping]:
         """
         get the first value from this object's metadata whose key exactly
         matches `text`, even if it is nested inside a mapping, if the value
         itself is a mapping (e.g., nested PVL block, XML 'area', etc.)
         evaluate it using self.metadata.formatter. if there is no key matching
         'text', will evaluate and return the metadata as a whole.
         WARNING: this function's return values are memoized for performance.
         updating elements of self.metadata that have already been accessed
         with this function will not update future calls to this function.
         """
-        return self.metadata.metablock(text, evaluate, warn)
+        return self.metadata.metablock(text, warn)
 
-    def metablock_(
-        self, text: str, evaluate: bool = True
-    ) -> Optional[Mapping]:
+    def metablock_(self, text: str) -> Optional[Mapping]:
         """quiet-by-default version of metablock"""
-        return self.metadata.metablock(text, evaluate, False)
+        return self.metadata.metablock(text, False)
 
     def get_absolute_paths(self, filename: Union[str, Path]) -> list[str]:
         """
         Construct `Path`s for a filename in all our search paths. (These are
         places we can look for that file).
         """
         return gmap(
@@ -885,44 +857,34 @@
         return len(self.index)
 
     def __iter__(self):
         """"""
         for key in self.keys():
             yield self[key]
 
+    _metaget_interior: Callable[[str, Any], Any]
+    _metablock_interior: Callable[[str], Mapping]
 
-def _metaget_factory(
-    metadata: Metadata, cached: bool = True
-) -> Callable[[str, bool, bool], Any]:
-    """
-    Factory function for an internal component of `metaget()`. Reduces the risk
-    that the metadata access cache will create reference cycles.
-    """
-    def metaget_interior(text, default, evaluate):
+
+def _metaget_factory(metadata: Metadata) -> Callable[[str, Any], Any]:
+
+    def metaget_interior(text, default):
         """"""
         value = dig_for_value(metadata, text, mtypes=(dict, MultiDict))
-        if value is not None:
-            return metadata.formatter(value) if evaluate is True else value
-        return default
-
-    if cached is True:
-        return cache(metaget_interior)
-    return metaget_interior
+        return default if value is None else value
+
+    return cache(metaget_interior)
 
 
-def _metablock_factory(
-    metadata: Metadata, cached: bool = True
-) -> Callable[[str, bool], Mapping]:
+def _metablock_factory(metadata: Metadata) -> Callable[[str], Mapping]:
     """
     Factory function for an internal component of `metablock()`. Reduces the
     risk that the metadata access cache will create reference cycles.
     """
-    def metablock_interior(text, evaluate):
+    def metablock_interior(text):
         """"""
         value = dig_for_value(metadata, text, mtypes=(dict, MultiDict))
         if not isinstance(value, Mapping):
-            value = metadata
-        return metadata.formatter(value) if evaluate is True else value
+            return metadata
+        return value
 
-    if cached is True:
-        return cache(metablock_interior)
-    return metablock_interior
+    return cache(metablock_interior)
```

### Comparing `pdr-1.0.7/pdr/pdrtypes.py` & `pdr-1.1.0/pdr/pdrtypes.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/pvl_utils.py` & `pdr-1.1.0/pdr/pvl_utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/objects.py` & `pdr-1.1.0/pdr/tests/objects.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_bit_handling.py` & `pdr-1.1.0/pdr/tests/test_bit_handling.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 END_OBJECT              = COLUMN
 """
 
 NULL_IDENTIFIERS = {field: "" for field in get_annotations(DataIdentifiers)}
 
 
 def test_bit_handling():
-    block = literalize_pvl_block(parse_pvl(BIT_STUB)[0])
+    block = parse_pvl(BIT_STUB)[0]
     fmtdef = read_table_structure(block, 'TABLE', None, None, NULL_IDENTIFIERS)
     bits = random.choices((0, 1), k=16)
     table = pd.DataFrame(
         {'BITS1': [int("".join(map(str, bits)), 2).to_bytes(2, 'big')]}
     )
     table = expand_bit_strings(table, fmtdef)
     strings = table.loc[0, 'BITS1']
```

### Comparing `pdr-1.0.7/pdr/tests/test_browsify.py` & `pdr-1.1.0/pdr/tests/test_browsify.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_data.py` & `pdr-1.1.0/pdr/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_datatypes.py` & `pdr-1.1.0/pdr/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_func.py` & `pdr-1.1.0/pdr/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_loader_helpers.py` & `pdr-1.1.0/pdr/tests/test_loader_helpers.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_np_utils.py` & `pdr-1.1.0/pdr/tests/test_np_utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_queries.py` & `pdr-1.1.0/pdr/tests/test_queries.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     block = literalize_pvl(parse_pvl(BLOCK_TEXT)[0]["IMAGE"])
     base = base_sample_info(block)
     assert base == {"BYTES_PER_PIXEL": 4, "SAMPLE_TYPE": "IEEE_REAL"}
     assert im_sample_type(base) == ">"
 
 
 def test_generic_properties():
-    block = literalize_pvl(parse_pvl(BLOCK_TEXT)[0]["IMAGE"])
+    block = parse_pvl(BLOCK_TEXT)[0]["IMAGE"]
     props = generic_image_properties(block, ">f")
     assert props == {
         "BYTES_PER_PIXEL": 4,
         "is_vax_real": False,
         "sample_type": ">f",
         "nrows": 650,
         "ncols": 350,
@@ -32,15 +32,15 @@
         "bandpad": 0,
         "linepad": 0,
     }
 
 
 def test_qube_props():
     params, _ = parse_pvl(QUBE_BLOCK_TEXT)
-    qube_block = literalize_pvl(params["SPECTRAL_QUBE"])
+    qube_block = params["SPECTRAL_QUBE"]
     band_storage_type = get_qube_band_storage_type(qube_block)
     props = generic_qube_properties(qube_block, band_storage_type)
     assert props == {
         "BYTES_PER_PIXEL": 4,
         "sample_type": ">f",
         "axnames": ("SAMPLE", "LINE", "BAND"),
         "ncols": 100,
```

### Comparing `pdr-1.0.7/pdr/tests/test_scaling.py` & `pdr-1.1.0/pdr/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_table.py` & `pdr-1.1.0/pdr/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/test_vax.py` & `pdr-1.1.0/pdr/tests/test_vax.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/tests/utils.py` & `pdr-1.1.0/pdr/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/pdr/utils.py` & `pdr-1.1.0/pdr/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import bz2
 from io import BytesIO
 from itertools import chain
 from numbers import Number
 from pathlib import Path
 import struct
 import textwrap
+from types import MappingProxyType as MPt
 from typing import (
     Collection,
     IO,
     Mapping,
+    MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Union,
 )
 import warnings
 from zipfile import ZipFile
```

### Comparing `pdr-1.0.7/pdr/vax.py` & `pdr-1.1.0/pdr/vax.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,7 +125,12 @@
     data = to_vax32_bytes(array)
     output = np.frombuffer(data, dtype='<f4')
 
     if scalar:
         return output[0]
     else:
         return output.reshape(array.shape)
+
+
+# TODO: VAX_REAL_CONVERTERS = {4: vax32_to_np_float32, 8: vax64_to_np_float64}
+#  def vax_real_to_np(bytestream, bytewidth):
+#     return VAX_REAL_CONVERTERS[bytewidth](bytestream)
```

### Comparing `pdr-1.0.7/pdr.egg-info/PKG-INFO` & `pdr-1.1.0/pdr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 1.0.7
+Version: 1.1.0
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pdr-1.0.7/pdr.egg-info/SOURCES.txt` & `pdr-1.1.0/pdr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdr-1.0.7/setup.py` & `pdr-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdr",
-    version="1.0.7",
+    version="1.1.0",
     author="Chase Million",
     author_email="chase@millionconcepts.com",
     description="Planetary Data Reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MillionConcepts/pdr",
     packages=setuptools.find_packages(),
```

