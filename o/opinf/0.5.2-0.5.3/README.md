# Comparing `tmp/opinf-0.5.2.tar.gz` & `tmp/opinf-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opinf-0.5.2.tar", last modified: Mon Apr 29 19:25:13 2024, max compression
+gzip compressed data, was "opinf-0.5.3.tar", last modified: Wed May 22 19:40:13 2024, max compression
```

## Comparing `opinf-0.5.2.tar` & `opinf-0.5.3.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.548803 opinf-0.5.2/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1079 2023-10-10 16:21:43.000000 opinf-0.5.2/LICENSE
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5032 2024-04-29 19:25:13.548303 opinf-0.5.2/PKG-INFO
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1800 2023-10-10 16:21:43.000000 opinf-0.5.2/README.md
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1937 2024-04-29 19:15:32.000000 opinf-0.5.2/pyproject.toml
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       38 2024-04-29 19:25:13.548852 opinf-0.5.2/setup.cfg
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      161 2023-10-10 16:21:43.000000 opinf-0.5.2/setup.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.506054 opinf-0.5.2/src/
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.510612 opinf-0.5.2/src/opinf/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      394 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/__init__.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.515875 opinf-0.5.2/src/opinf/basis/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      148 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     9891 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    10006 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/_linear.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    20882 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/_multi.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42659 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/_pod.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.517420 opinf-0.5.2/src/opinf/ddt/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/ddt/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7766 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/ddt/_finite_difference.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      565 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/errors.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.519588 opinf-0.5.2/src/opinf/lift/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      134 2024-02-05 19:42:33.000000 opinf-0.5.2/src/opinf/lift/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5092 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/lift/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5660 2024-01-24 16:53:26.000000 opinf-0.5.2/src/opinf/lift/_polynomial.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.524587 opinf-0.5.2/src/opinf/lstsq/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     2764 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/lstsq/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7622 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/lstsq/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18912 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/lstsq/_tikhonov.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      936 2023-12-01 18:52:21.000000 opinf-0.5.2/src/opinf/lstsq/_total.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.525257 opinf-0.5.2/src/opinf/models/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      142 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/__init__.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.527552 opinf-0.5.2/src/opinf/models/mono/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      183 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/mono/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    12644 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/mono/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42164 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/mono/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    55664 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/mono/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.530203 opinf-0.5.2/src/opinf/models/multi/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      185 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/multi/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      106 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/multi/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      105 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/multi/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/multi/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.533974 opinf-0.5.2/src/opinf/operators/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/operators/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    22275 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/operators/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    35032 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/operators/_interpolate.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    51458 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/operators/_nonparametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.537141 opinf-0.5.2/src/opinf/post/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      111 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/post/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7938 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/post/_errors.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.540806 opinf-0.5.2/src/opinf/pre/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      155 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/pre/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    11547 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/pre/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18031 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/pre/_multi.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    27382 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/pre/_shiftscale.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.542135 opinf-0.5.2/src/opinf/roms/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      168 2024-01-12 21:51:13.000000 opinf-0.5.2/src/opinf/roms/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3734 2024-01-13 00:03:24.000000 opinf-0.5.2/src/opinf/roms/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       52 2024-01-12 21:52:14.000000 opinf-0.5.2/src/opinf/roms/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.546136 opinf-0.5.2/src/opinf/utils/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4070 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_hdf5.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      784 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_mpl_config.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      355 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_repr.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3856 2023-12-01 18:52:21.000000 opinf-0.5.2/src/opinf/utils/_reprojection.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1015 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_requires.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3089 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_timer.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.546964 opinf-0.5.2/src/opinf.egg-info/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5032 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/PKG-INFO
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1522 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/SOURCES.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        1 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/dependency_links.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      350 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/requires.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        6 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/top_level.txt
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.046631 opinf-0.5.3/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1079 2024-05-01 20:01:45.000000 opinf-0.5.3/LICENSE
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4709 2024-05-22 19:40:13.045617 opinf-0.5.3/PKG-INFO
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1924 2024-05-22 19:31:31.000000 opinf-0.5.3/README.md
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1703 2024-05-22 19:31:31.000000 opinf-0.5.3/pyproject.toml
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       38 2024-05-22 19:40:13.046689 opinf-0.5.3/setup.cfg
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      161 2024-05-01 20:01:45.000000 opinf-0.5.3/setup.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:12.994347 opinf-0.5.3/src/
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.001176 opinf-0.5.3/src/opinf/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      394 2024-05-22 15:36:52.000000 opinf-0.5.3/src/opinf/__init__.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.011859 opinf-0.5.3/src/opinf/basis/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      148 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/basis/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     9891 2024-05-15 19:23:26.000000 opinf-0.5.3/src/opinf/basis/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    10006 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/basis/_linear.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    20882 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/basis/_multi.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42659 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/basis/_pod.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.013566 opinf-0.5.3/src/opinf/ddt/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      128 2024-05-22 15:36:52.000000 opinf-0.5.3/src/opinf/ddt/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     9495 2024-05-22 15:36:52.000000 opinf-0.5.3/src/opinf/ddt/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    44500 2024-05-22 15:27:01.000000 opinf-0.5.3/src/opinf/ddt/_finite_difference.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      565 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/errors.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.016794 opinf-0.5.3/src/opinf/lift/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      134 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/lift/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5162 2024-05-22 18:42:48.000000 opinf-0.5.3/src/opinf/lift/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5660 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/lift/_polynomial.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.021406 opinf-0.5.3/src/opinf/lstsq/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     2764 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/lstsq/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7598 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/lstsq/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18892 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/lstsq/_tikhonov.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      937 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/lstsq/_total.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.022259 opinf-0.5.3/src/opinf/models/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      142 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/__init__.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.025003 opinf-0.5.3/src/opinf/models/mono/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      183 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/mono/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    12644 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/mono/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42167 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/models/mono/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    55668 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/models/mono/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.028412 opinf-0.5.3/src/opinf/models/multi/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      185 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/multi/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      106 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/multi/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      105 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/multi/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/models/multi/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.031191 opinf-0.5.3/src/opinf/operators/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/operators/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    22275 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/operators/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    35038 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/operators/_interpolate.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    51458 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/operators/_nonparametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.032804 opinf-0.5.3/src/opinf/post/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      111 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/post/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7938 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/post/_errors.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.036975 opinf-0.5.3/src/opinf/pre/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      155 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/pre/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    11550 2024-05-22 17:53:23.000000 opinf-0.5.3/src/opinf/pre/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18031 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/pre/_multi.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    27382 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/pre/_shiftscale.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.038210 opinf-0.5.3/src/opinf/roms/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      168 2024-01-12 21:51:13.000000 opinf-0.5.3/src/opinf/roms/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3611 2024-05-01 16:12:45.000000 opinf-0.5.3/src/opinf/roms/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       52 2024-01-12 21:52:14.000000 opinf-0.5.3/src/opinf/roms/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.043860 opinf-0.5.3/src/opinf/utils/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4070 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_hdf5.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      784 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_mpl_config.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      355 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_repr.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3881 2024-05-22 19:31:31.000000 opinf-0.5.3/src/opinf/utils/_reprojection.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1015 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_requires.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3089 2024-05-01 20:01:45.000000 opinf-0.5.3/src/opinf/utils/_timer.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-05-22 19:40:13.044637 opinf-0.5.3/src/opinf.egg-info/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4709 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/PKG-INFO
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1545 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/SOURCES.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        1 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/dependency_links.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      156 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/requires.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        6 2024-05-22 19:40:12.000000 opinf-0.5.3/src/opinf.egg-info/top_level.txt
```

### Comparing `opinf-0.5.2/LICENSE` & `opinf-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/PKG-INFO` & `opinf-0.5.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: opinf
-Version: 0.5.2
+Version: 0.5.3
 Summary: Operator Inference for data-driven model reduction of dynamical systems.
 Author-email: Willcox Research Group <kwillcox@oden.utexas.edu>
-Maintainer-email: "Shane A. McQuarrie" <shanemcq@utexas.edu>
+Maintainer-email: "Shane A. McQuarrie" <smcquar@sandia.gov>
 License: MIT License
         
         Copyright (c) 2023 Willcox Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -25,15 +25,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://willcox-research-group.github.io/rom-operator-inference-Python3/source/index.html
 Project-URL: documentation, https://willcox-research-group.github.io/rom-operator-inference-Python3/source/index.html
 Project-URL: repository, https://github.com/Willcox-Research-Group/rom-operator-inference-Python3.git
-Keywords: operator inference,model reduction,scientific machine learning
+Keywords: operator inference,model reduction,data-driven model reduction,scientific machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 4 - Beta
@@ -41,34 +41,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py>=3.9.0
 Requires-Dist: numpy>=1.23.2
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: matplotlib>=3.7
 Requires-Dist: scikit-learn>=1.3.0
-Provides-Extra: tests
-Requires-Dist: pytest>=6.0.2; extra == "tests"
-Requires-Dist: pytest-cov>=2.12.1; extra == "tests"
-Requires-Dist: black>=23.10.0; extra == "tests"
-Requires-Dist: flake8>=3.9.0; extra == "tests"
-Requires-Dist: pre-commit>=3.5.0; extra == "tests"
-Provides-Extra: docs
-Requires-Dist: bibtexparser>=2.0.0b7; extra == "docs"
-Requires-Dist: chardet>=5.0; extra == "docs"
-Requires-Dist: docutils==0.17.1; extra == "docs"
-Requires-Dist: jupyter-book<0.15.0,>=0.14.0; extra == "docs"
-Requires-Dist: jupyterlab>=4.0.9; extra == "docs"
-Requires-Dist: numpydoc>=1.2; extra == "docs"
-Requires-Dist: pandas>=2.0.3; extra == "docs"
-Requires-Dist: sphinx-design>=0.1.0; extra == "docs"
-Requires-Dist: sphinxcontrib-mermaid>=0.7.1; extra == "docs"
+Provides-Extra: dev
+Requires-Dist: tox>=4; extra == "dev"
+Requires-Dist: pre-commit>=3.7.1; extra == "dev"
+Requires-Dist: flake8==7.0.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
+Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: notebook; extra == "dev"
 
 [![License](https://img.shields.io/github/license/Willcox-Research-Group/rom-operator-inference-python3)](./LICENSE)
 [![Top language](https://img.shields.io/github/languages/top/Willcox-Research-Group/rom-operator-inference-python3)](https://www.python.org)
 ![Code size](https://img.shields.io/github/languages/code-size/Willcox-Research-Group/rom-operator-inference-python3)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![Issues](https://img.shields.io/github/issues/Willcox-Research-Group/rom-operator-inference-python3)](https://github.com/Willcox-Research-Group/rom-operator-inference-python3/issues)
 [![Latest commit](https://img.shields.io/github/last-commit/Willcox-Research-Group/rom-operator-inference-python3)](https://github.com/Willcox-Research-Group/rom-operator-inference-python3/commits/main)
 [![PyPI](https://img.shields.io/pypi/wheel/opinf)](https://pypi.org/project/opinf/)
 [![Documentation](https://img.shields.io/badge/Documentation-important)](https://Willcox-Research-Group.github.io/rom-operator-inference-Python3/)
 
 # Operator Inference in Python
```

### Comparing `opinf-0.5.2/README.md` & `opinf-0.5.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![License](https://img.shields.io/github/license/Willcox-Research-Group/rom-operator-inference-python3)](./LICENSE)
 [![Top language](https://img.shields.io/github/languages/top/Willcox-Research-Group/rom-operator-inference-python3)](https://www.python.org)
 ![Code size](https://img.shields.io/github/languages/code-size/Willcox-Research-Group/rom-operator-inference-python3)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![Issues](https://img.shields.io/github/issues/Willcox-Research-Group/rom-operator-inference-python3)](https://github.com/Willcox-Research-Group/rom-operator-inference-python3/issues)
 [![Latest commit](https://img.shields.io/github/last-commit/Willcox-Research-Group/rom-operator-inference-python3)](https://github.com/Willcox-Research-Group/rom-operator-inference-python3/commits/main)
 [![PyPI](https://img.shields.io/pypi/wheel/opinf)](https://pypi.org/project/opinf/)
 [![Documentation](https://img.shields.io/badge/Documentation-important)](https://Willcox-Research-Group.github.io/rom-operator-inference-Python3/)
 
 # Operator Inference in Python
```

### Comparing `opinf-0.5.2/pyproject.toml` & `opinf-0.5.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opinf"
 description = "Operator Inference for data-driven model reduction of dynamical systems."
 dynamic = ["version"]
 authors = [
     { name = "Willcox Research Group", email = "kwillcox@oden.utexas.edu" },
 ]
-maintainers = [{ name = "Shane A. McQuarrie", email = "shanemcq@utexas.edu" }]
+maintainers = [{ name = "Shane A. McQuarrie", email = "smcquar@sandia.gov" }]
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 keywords = [
     "operator inference",
     "model reduction",
+    "data-driven model reduction",
     "scientific machine learning",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Natural Language :: English",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -32,31 +33,21 @@
     "numpy>=1.23.2",
     "scipy>=1.10.1",
     "matplotlib>=3.7",
     "scikit-learn>=1.3.0",
 ]
 
 [project.optional-dependencies]
-tests = [
-    "pytest>=6.0.2",
-    "pytest-cov>=2.12.1",
-    "black>=23.10.0",
-    "flake8>=3.9.0",
-    "pre-commit>=3.5.0",
-]
-docs = [
-    "bibtexparser>=2.0.0b7",
-    "chardet>=5.0",
-    "docutils==0.17.1",
-    "jupyter-book>=0.14.0,<0.15.0",
-    "jupyterlab>=4.0.9",
-    "numpydoc>=1.2",
-    "pandas>=2.0.3",
-    "sphinx-design>=0.1.0",
-    "sphinxcontrib-mermaid>=0.7.1",
+dev = [
+    "tox>=4",
+    "pre-commit>=3.7.1",
+    "flake8==7.0.0",
+    "black==24.4.2",
+    "jupyterlab",
+    "notebook",
 ]
 
 [project.urls]
 homepage = "https://willcox-research-group.github.io/rom-operator-inference-Python3/source/index.html"
 documentation = "https://willcox-research-group.github.io/rom-operator-inference-Python3/source/index.html"
 repository = "https://github.com/Willcox-Research-Group/rom-operator-inference-Python3.git"
```

### Comparing `opinf-0.5.2/src/opinf/basis/_base.py` & `opinf-0.5.3/src/opinf/basis/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/basis/_linear.py` & `opinf-0.5.3/src/opinf/basis/_linear.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/basis/_multi.py` & `opinf-0.5.3/src/opinf/basis/_multi.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/basis/_pod.py` & `opinf-0.5.3/src/opinf/basis/_pod.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/errors.py` & `opinf-0.5.3/src/opinf/errors.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/lift/_base.py` & `opinf-0.5.3/src/opinf/lift/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,21 +102,23 @@
             Tolerance for the finite difference check of :meth:`lift_ddts`.
             Only used if :meth:`lift_ddts` is implemented.
         """
         # Verify lift() and unlift() are inverses.
         lifted_states = self.lift(states)
         if (k1 := lifted_states.shape[1]) != states.shape[1]:
             raise errors.VerificationError(
-                f"{k1} = lift(states).shape[1] != {states.shape[1] = }"
+                f"{k1} = lift(states).shape[1] "
+                f"!= states.shape[1] = {states.shape[1]}"
             )
 
         unlifted_states = self.unlift(lifted_states)
         if (shape := unlifted_states.shape) != states.shape:
             raise errors.VerificationError(
-                f"{shape} = unlift(lift(states)).shape != {states.shape = }"
+                f"{shape} = unlift(lift(states)).shape "
+                f"!= states.shape = {states.shape}"
             )
         if not np.allclose(unlifted_states, states):
             raise errors.VerificationError("unlift(lift(states)) != states")
         print("lift() and unlift() are consistent")
 
         # Finite difference checks for lift_ddts().
         if self.lift_ddts(states, states) is NotImplemented:
@@ -134,10 +136,10 @@
         lddts_est = ddt.ddt(lifted_states, t)
         if (
             diff := la.norm(lifted_ddts - lddts_est) / la.norm(lddts_est)
         ) > tol:
             raise errors.VerificationError(
                 "lift_ddts() failed finite difference check,\n\t"
                 "|| lift_ddts(states, d/dt[states]) - d/dt[lift(states)] || "
-                f" / || d/dt[lift(states)] || = {diff} > {tol = }"
+                f" / || d/dt[lift(states)] || = {diff} > tol = {tol}"
             )
         print("lift() and lift_ddts() are consistent")
```

### Comparing `opinf-0.5.2/src/opinf/lift/_polynomial.py` & `opinf-0.5.3/src/opinf/lift/_polynomial.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/lstsq/__init__.py` & `opinf-0.5.3/src/opinf/lstsq/__init__.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/lstsq/_base.py` & `opinf-0.5.3/src/opinf/lstsq/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,15 @@
     if affines is None:
         affines = {}
 
     qs = [
         (
             len(affines[op])
             if (op in affines and op in modelform)
-            else 1
-            if op in modelform
-            else 0
+            else 1 if op in modelform else 0
         )
         for op in "cAHGB"
     ]
     rs = [1, r, r * (r + 1) // 2, r * (r + 1) * (r + 2) // 6, m]
 
     return sum(qq * rr for qq, rr in zip(qs, rs))
```

### Comparing `opinf-0.5.2/src/opinf/lstsq/_tikhonov.py` & `opinf-0.5.3/src/opinf/lstsq/_tikhonov.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     The solution is calculated using the singular value decomposition of A:
     If A = U Σ V^T, then X = V Σinv(λ) U^T B, where
     Σinv(λ)[i, i] = Σ[i, i] / (Σ[i, i]^2 + λ^2).
     """
 
     _LSTSQ_LABEL = r"min_{X} ||AX - B||_F^2 + ||λX||_F^2"
 
-    def __init__(self, regularizer=0):
+    def __init__(self, regularizer=0.0):
         """Store the regularizer and initialize attributes.
 
         Parameters
         ----------
         regularizer : float ≥ 0
             Scalar L2 regularization hyperparameter.
         """
@@ -177,17 +177,15 @@
 
         Returns
         -------
         resids : (r,) ndarray or float (r = 1)
             Residuals ||Ax_i - b_i||_2^2 + ||λx_i||_2^2, i = 1, ..., r.
         """
         self._check_is_trained()
-        return self.misfit(X) + (self.regularizer**2) * np.sum(
-            X**2, axis=0
-        )
+        return self.misfit(X) + (self.regularizer**2) * np.sum(X**2, axis=0)
 
 
 class L2SolverDecoupled(L2Solver):
     """Solve r independent l2-norm ordinary least-squares problems, each with
     the same data matrix A but different L2 regularizations λ_i > 0 for the
     columns of X and B:
```

### Comparing `opinf-0.5.2/src/opinf/lstsq/_total.py` & `opinf-0.5.3/src/opinf/lstsq/_total.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     regularization, i.e.,
 
         argmin_{X, G, H} ||[G H]||_F such that (A+G)X = B+H
 
     The solution is calculated using standard computations
     (see Wikipedia for example).
     """
+
     _LSTSQ_LABEL = r"argmin_{X, G, H} ||[G H]||_F | (A+G)X = B+H"
 
     def predict(self):
         """Solve the total least-squares problem."""
         # A augmented with B
         Vh = la.svd(np.hstack((self.A, self.B)), full_matrices=False)[2]
         n = self.A.shape[1]
```

### Comparing `opinf-0.5.2/src/opinf/models/mono/_base.py` & `opinf-0.5.3/src/opinf/models/mono/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/models/mono/_nonparametric.py` & `opinf-0.5.3/src/opinf/models/mono/_nonparametric.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,14 +500,15 @@
     ``operators`` argument.
 
     Parameters
     ----------
     operators : list of :mod:`opinf.operators` objects
         Operators comprising the terms of the model.
     """
+
     _LHS_ARGNAME = "forcing"
     _LHS_LABEL = "z"
     _STATE_LABEL = "q"
     _INPUT_LABEL = None
     # TODO: disallow input terms?
 
     def fit(self, states, forcing=None, *, solver=None, regularizer=None):
@@ -622,14 +623,15 @@
     ``operators`` attribute.
 
     Parameters
     ----------
     operators : list of :mod:`opinf.operators` objects
         Operators comprising the terms of the model.
     """
+
     _LHS_ARGNAME = "nextstates"
     _LHS_LABEL = r"q_{j+1}"
     _STATE_LABEL = r"q_{j}"
     _INPUT_LABEL = r"u_{j}"
 
     @staticmethod
     def stack_trajectories(statelist, inputlist=None):
@@ -868,14 +870,15 @@
     ``operators`` argument.
 
     Parameters
     ----------
     operators : list of :mod:`opinf.operators` objects
         Operators comprising the terms of the model.
     """
+
     _LHS_ARGNAME = "ddts"
     _LHS_LABEL = "dq / dt"
     _STATE_LABEL = "q(t)"
     _INPUT_LABEL = "u(t)"
 
     def fit(self, states, ddts, inputs=None, solver=None, *, regularizer=None):
         r"""Learn the model operators from data.
```

### Comparing `opinf-0.5.2/src/opinf/models/mono/_parametric.py` & `opinf-0.5.3/src/opinf/models/mono/_parametric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1007,14 +1007,15 @@
     ``operators`` attribute.
 
     Parameters
     ----------
     operators : list of :mod:`opinf.operators` objects
         Operators comprising the terms of the model.
     """
+
     pass
 
 
 class ParametricContinuousModel(_ParametricContinuousMixin, _ParametricModel):
     r"""Parametric system of ordinary differential equations
     :math:`\ddt\qhat(t; \bfmu) = \fhat(\qhat(t; \bfmu), \u(t); \bfmu)`.
 
@@ -1028,14 +1029,15 @@
     ``operators`` argument.
 
     Parameters
     ----------
     operators : list of :mod:`opinf.operators` objects
         Operators comprising the terms of the model.
     """
+
     pass
 
 
 # Special case: fully interpolation-based models ==============================
 class _InterpolatedModel(_ParametricModel):
     """Base class for parametric monolithic models where all operators MUST be
     interpolation-based parametric operators. In this special case, the
@@ -1403,14 +1405,15 @@
             >>> interpolator_evaluation = interpolator(new_data_point)
 
         This can be, e.g., a class from ``scipy.interpolate``.
         If ``None`` (default), use ``scipy.interpolate.CubicSpline``
         for one-dimensional parameters and
         ``scipy.interpolate.LinearNDInterpolator`` otherwise.
     """
+
     pass
 
 
 class InterpolatedContinuousModel(
     _ParametricContinuousMixin, _InterpolatedModel
 ):
     r"""Parametric system of ordinary differential equations
@@ -1438,8 +1441,9 @@
             >>> interpolator_evaluation = interpolator(new_data_point)
 
         This can be, e.g., a class from ``scipy.interpolate``.
         If ``None`` (default), use ``scipy.interpolate.CubicSpline``
         for one-dimensional parameters and
         ``scipy.interpolate.LinearNDInterpolator`` otherwise.
     """
+
     pass
```

### Comparing `opinf-0.5.2/src/opinf/operators/_base.py` & `opinf-0.5.3/src/opinf/operators/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/operators/_interpolate.py` & `opinf-0.5.3/src/opinf/operators/_interpolate.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,14 +620,15 @@
         ``scipy.interpolate.LinearNDInterpolator`` otherwise.
         If not provided in the constructor, use :meth:`set_interpolator` later.
     fromblock : bool
         If ``True``, interpret ``entries`` as a horizontal concatenation
         of arrays; if ``False`` (default), interpret ``entries`` as a list
         of arrays.
     """
+
     _OperatorClass = ConstantOperator
 
 
 class InterpolatedLinearOperator(_InterpolatedOperator):
     r"""Parametric linear operator
     :math:`\Ophat_{\ell}(\qhat,\u;\bfmu) = \Ahat(\bfmu)\qhat`
     where :math:`\Ahat(\bfmu) \in \RR^{r \times r}` and
@@ -667,14 +668,15 @@
         ``scipy.interpolate.LinearNDInterpolator`` otherwise.
         If not provided in the constructor, use :meth:`set_interpolator` later.
     fromblock : bool
         If ``True``, interpret ``entries`` as a horizontal concatenation
         of arrays; if ``False`` (default), interpret ``entries`` as a list
         of arrays.
     """
+
     _OperatorClass = LinearOperator
 
 
 class InterpolatedQuadraticOperator(_InterpolatedOperator):
     r"""Parametric quadratic operator
     :math:`\Ophat_{\ell}(\qhat,\u;\bfmu) = \Hhat(\bfmu)[\qhat\otimes\qhat]`
     where :math:`\Ahat(\bfmu) \in \RR^{r \times r^2}` and
@@ -714,14 +716,15 @@
         ``scipy.interpolate.LinearNDInterpolator`` otherwise.
         If not provided in the constructor, use :meth:`set_interpolator` later.
     fromblock : bool
         If ``True``, interpret ``entries`` as a horizontal concatenation
         of arrays; if ``False`` (default), interpret ``entries`` as a list
         of arrays.
     """
+
     _OperatorClass = QuadraticOperator
 
 
 class InterpolatedCubicOperator(_InterpolatedOperator):
     r"""Parametric cubic operator
     :math:`\Ophat_{\ell}(\qhat,\u;\bfmu)
     = \Ghat(\bfmu)[\qhat\otimes\qhat\otimes\qhat]`
@@ -762,14 +765,15 @@
         ``scipy.interpolate.LinearNDInterpolator`` otherwise.
         If not provided in the constructor, use :meth:`set_interpolator` later.
     fromblock : bool
         If ``True``, interpret ``entries`` as a horizontal concatenation
         of arrays; if ``False`` (default), interpret ``entries`` as a list
         of arrays.
     """
+
     _OperatorClass = CubicOperator
 
 
 class InterpolatedInputOperator(_InterpolatedOperator, _InputMixin):
     r"""Parametric input operator
     :math:`\Ophat_{\ell}(\qhat,\u;\bfmu) = \Bhat(\bfmu)\u`
     where :math:`\Bhat(\bfmu) \in \RR^{r \times m}` and
@@ -810,14 +814,15 @@
         ``scipy.interpolate.LinearNDInterpolator`` otherwise.
         If not provided in the constructor, use :meth:`set_interpolator` later.
     fromblock : bool
         If ``True``, interpret ``entries`` as a horizontal concatenation
         of arrays; if ``False`` (default), interpret ``entries`` as a list
         of arrays.
     """
+
     _OperatorClass = InputOperator
 
     @property
     def input_dimension(self):
         r"""Dimension of the input :math:`\u` that the operator acts on."""
         return None if self.entries is None else self.shape[1]
 
@@ -862,14 +867,15 @@
         ``scipy.interpolate.LinearNDInterpolator`` otherwise.
         If not provided in the constructor, use :meth:`set_interpolator` later.
     fromblock : bool
         If ``True``, interpret ``entries`` as a horizontal concatenation
         of arrays; if ``False`` (default), interpret ``entries`` as a list
         of arrays.
     """
+
     _OperatorClass = StateInputOperator
 
     @property
     def input_dimension(self):
         r"""Dimension of the input :math:`\u` that the operator acts on."""
         if self.entries is None:
             return None
```

### Comparing `opinf-0.5.2/src/opinf/operators/_nonparametric.py` & `opinf-0.5.3/src/opinf/operators/_nonparametric.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/post/_errors.py` & `opinf-0.5.3/src/opinf/post/_errors.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/pre/_base.py` & `opinf-0.5.3/src/opinf/pre/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
         ddts_est = ddt.ddt(states_transformed, t)
         if (
             diff := la.norm(ddts_transformed - ddts_est) / la.norm(ddts_est)
         ) > tol:
             raise errors.VerificationError(
                 "transform_ddts() failed finite difference check,\n\t"
                 "|| transform_ddts(d/dt[states]) - d/dt[transform(states)] || "
-                f" / || d/dt[transform(states)] || = {diff} > {tol = }"
+                f" / || d/dt[transform(states)] || = {diff} > {tol} = tol"
             )
         ddts_transformed = self.transform_ddts(ddts, inplace=True)
         if ddts_transformed is not ddts:
             raise errors.VerificationError(
                 "transform_ddts(ddts, inplace=True) is not ddts"
             )
         print("transform() and transform_ddts() are consistent")
```

### Comparing `opinf-0.5.2/src/opinf/pre/_multi.py` & `opinf-0.5.3/src/opinf/pre/_multi.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/pre/_shiftscale.py` & `opinf-0.5.3/src/opinf/pre/_shiftscale.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/roms/_nonparametric.py` & `opinf-0.5.3/src/opinf/roms/_nonparametric.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,50 +18,43 @@
 
 
 class ROM:
     """Nonparametric reduced-order model class.
 
     Parameters
     ----------
-    lifting_func : callable
-        Function for lifting the native variables to the learning variables.
-        Must obey the following syntax.
-
-        .. code-block:: python
-           >>> states_lifted = lifting_func(states)
-           >>>
-    unlifting_func : callable
+    lifter
     transformer
     basis
-    ddt_func : callable
+    ddt_estimator
         Function for estimating time derivatives of the training states.
         Must obey the following syntax.
 
         .. code-block:: python
            >>> states, ddts, inputs = ddt_func(states, inputs)
 
-    model :
-    solver :
+    model
+    solver (or make this part of the model?
     """
 
     def __init__(
         self,
         *,
         lifter=None,
         transformer=None,
         basis=None,
-        ddt_func=None,
+        ddt_estimator=None,
         model=None,
         solver=None,
     ):
         """Store each argument as an attribute."""
         self.__lifter = lifter
         self.__transformer = transformer
         self.__basis = basis
-        self.__ddter = ddt_func
+        self.__ddter = ddt_estimator
         self.__model = model
         self.__solver = solver
 
     # Properties --------------------------------------------------------------
     @property
     def lifter(self):
         return self.__lifter
@@ -71,22 +64,26 @@
         return self.__transformer
 
     @property
     def basis(self):
         return self.__basis
 
     @property
-    def ddt_func(self):
-        return self.__ddt_func
+    def ddt_estimator(self):
+        return self.__ddter
 
     @property
     def model(self):
         return self.__model
 
     @property
+    def iscontinuous(self):
+        return isinstance(self.model, models.ContinuousModel)
+
+    @property
     def solver(self):
         return self.__solver
 
     # Printing ----------------------------------------------------------------
     def __str__(self):
         """String representation."""
         lines = ["Nonparametric reduced-order model"]
```

### Comparing `opinf-0.5.2/src/opinf/utils/_hdf5.py` & `opinf-0.5.3/src/opinf/utils/_hdf5.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/utils/_mpl_config.py` & `opinf-0.5.3/src/opinf/utils/_mpl_config.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/utils/_reprojection.py` & `opinf-0.5.3/src/opinf/utils/_reprojection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pre/_reprojection.py
 """Re-projection of trajectories for recovering intrusive models with
 Operator Inference.
 """
 
 __all__ = [
-            "reproject_discrete",
-            "reproject_continuous",
-          ]
+    "reproject_discrete",
+    "reproject_continuous",
+]
 
 import numpy as np
 
 
 # Reprojection schemes ========================================================
 def reproject_discrete(f, basis, init, niters, inputs=None):
     """Sample re-projected trajectories of the discrete dynamical system
@@ -44,22 +44,24 @@
 
     # Create the solution array and fill in the initial condition.
     states_ = np.empty((r, niters))
     states_[:, 0] = basis.T @ init
 
     # Run the re-projection iteration.
     if inputs is None:
-        for j in range(niters-1):
-            states_[:, j+1] = basis.T @ f(basis @ states_[:, j])
+        for j in range(niters - 1):
+            states_[:, j + 1] = basis.T @ f(basis @ states_[:, j])
     elif inputs.ndim == 1:
-        for j in range(niters-1):
-            states_[:, j+1] = basis.T @ f(basis @ states_[:, j], inputs[j])
+        for j in range(niters - 1):
+            states_[:, j + 1] = basis.T @ f(basis @ states_[:, j], inputs[j])
     else:
-        for j in range(niters-1):
-            states_[:, j+1] = basis.T @ f(basis @ states_[:, j], inputs[:, j])
+        for j in range(niters - 1):
+            states_[:, j + 1] = basis.T @ f(
+                basis @ states_[:, j], inputs[:, j]
+            )
 
     return states_
 
 
 def reproject_continuous(f, basis, states, inputs=None):
     """Sample re-projected trajectories of the continuous system of ODEs
 
@@ -83,16 +85,18 @@
     states_reprojected : (r, k) ndarray
         Re-projected state trajectories in the projected low-dimensional space.
     ddts_reprojected : (r, k) ndarray
         Re-projected velocities in the projected low-dimensional space.
     """
     # Validate and extract dimensions.
     if states.shape[0] != basis.shape[0]:
-        raise ValueError("states and basis not aligned, first dimension "
-                         f"{states.shape[0]} != {basis.shape[0]}")
+        raise ValueError(
+            "states and basis not aligned, first dimension "
+            f"{states.shape[0]} != {basis.shape[0]}"
+        )
     n, r = basis.shape
     k = states.shape[1]
 
     # Create the solution arrays.
     states_ = basis.T @ states
     ddts_ = np.empty((r, k))
```

### Comparing `opinf-0.5.2/src/opinf/utils/_requires.py` & `opinf-0.5.3/src/opinf/utils/_requires.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf/utils/_timer.py` & `opinf-0.5.3/src/opinf/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.2/src/opinf.egg-info/PKG-INFO` & `opinf-0.5.3/src/opinf.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: opinf
-Version: 0.5.2
+Version: 0.5.3
 Summary: Operator Inference for data-driven model reduction of dynamical systems.
 Author-email: Willcox Research Group <kwillcox@oden.utexas.edu>
-Maintainer-email: "Shane A. McQuarrie" <shanemcq@utexas.edu>
+Maintainer-email: "Shane A. McQuarrie" <smcquar@sandia.gov>
 License: MIT License
         
         Copyright (c) 2023 Willcox Research Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -25,15 +25,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://willcox-research-group.github.io/rom-operator-inference-Python3/source/index.html
 Project-URL: documentation, https://willcox-research-group.github.io/rom-operator-inference-Python3/source/index.html
 Project-URL: repository, https://github.com/Willcox-Research-Group/rom-operator-inference-Python3.git
-Keywords: operator inference,model reduction,scientific machine learning
+Keywords: operator inference,model reduction,data-driven model reduction,scientific machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 4 - Beta
@@ -41,34 +41,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py>=3.9.0
 Requires-Dist: numpy>=1.23.2
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: matplotlib>=3.7
 Requires-Dist: scikit-learn>=1.3.0
-Provides-Extra: tests
-Requires-Dist: pytest>=6.0.2; extra == "tests"
-Requires-Dist: pytest-cov>=2.12.1; extra == "tests"
-Requires-Dist: black>=23.10.0; extra == "tests"
-Requires-Dist: flake8>=3.9.0; extra == "tests"
-Requires-Dist: pre-commit>=3.5.0; extra == "tests"
-Provides-Extra: docs
-Requires-Dist: bibtexparser>=2.0.0b7; extra == "docs"
-Requires-Dist: chardet>=5.0; extra == "docs"
-Requires-Dist: docutils==0.17.1; extra == "docs"
-Requires-Dist: jupyter-book<0.15.0,>=0.14.0; extra == "docs"
-Requires-Dist: jupyterlab>=4.0.9; extra == "docs"
-Requires-Dist: numpydoc>=1.2; extra == "docs"
-Requires-Dist: pandas>=2.0.3; extra == "docs"
-Requires-Dist: sphinx-design>=0.1.0; extra == "docs"
-Requires-Dist: sphinxcontrib-mermaid>=0.7.1; extra == "docs"
+Provides-Extra: dev
+Requires-Dist: tox>=4; extra == "dev"
+Requires-Dist: pre-commit>=3.7.1; extra == "dev"
+Requires-Dist: flake8==7.0.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
+Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: notebook; extra == "dev"
 
 [![License](https://img.shields.io/github/license/Willcox-Research-Group/rom-operator-inference-python3)](./LICENSE)
 [![Top language](https://img.shields.io/github/languages/top/Willcox-Research-Group/rom-operator-inference-python3)](https://www.python.org)
 ![Code size](https://img.shields.io/github/languages/code-size/Willcox-Research-Group/rom-operator-inference-python3)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![Issues](https://img.shields.io/github/issues/Willcox-Research-Group/rom-operator-inference-python3)](https://github.com/Willcox-Research-Group/rom-operator-inference-python3/issues)
 [![Latest commit](https://img.shields.io/github/last-commit/Willcox-Research-Group/rom-operator-inference-python3)](https://github.com/Willcox-Research-Group/rom-operator-inference-python3/commits/main)
 [![PyPI](https://img.shields.io/pypi/wheel/opinf)](https://pypi.org/project/opinf/)
 [![Documentation](https://img.shields.io/badge/Documentation-important)](https://Willcox-Research-Group.github.io/rom-operator-inference-Python3/)
 
 # Operator Inference in Python
```

### Comparing `opinf-0.5.2/src/opinf.egg-info/SOURCES.txt` & `opinf-0.5.3/src/opinf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/opinf.egg-info/top_level.txt
 src/opinf/basis/__init__.py
 src/opinf/basis/_base.py
 src/opinf/basis/_linear.py
 src/opinf/basis/_multi.py
 src/opinf/basis/_pod.py
 src/opinf/ddt/__init__.py
+src/opinf/ddt/_base.py
 src/opinf/ddt/_finite_difference.py
 src/opinf/lift/__init__.py
 src/opinf/lift/_base.py
 src/opinf/lift/_polynomial.py
 src/opinf/lstsq/__init__.py
 src/opinf/lstsq/_base.py
 src/opinf/lstsq/_tikhonov.py
```

