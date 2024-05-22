# Comparing `tmp/kssdtree-1.1.1.tar.gz` & `tmp/kssdtree-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kssdtree-1.1.1.tar", last modified: Fri Mar 15 09:42:02 2024, max compression
+gzip compressed data, was "kssdtree-1.1.2.tar", last modified: Wed May 22 06:01:30 2024, max compression
```

## Comparing `kssdtree-1.1.1.tar` & `kssdtree-1.1.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-03-15 09:42:02.285481 kssdtree-1.1.1/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       99 2024-03-15 09:41:31.000000 kssdtree-1.1.1/MANIFEST.in
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      477 2024-03-15 09:42:02.285481 kssdtree-1.1.1/PKG-INFO
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5769 2024-03-15 09:41:32.000000 kssdtree-1.1.1/README.md
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    11874 2024-03-15 09:41:31.000000 kssdtree-1.1.1/align.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    24008 2024-03-15 09:41:31.000000 kssdtree-1.1.1/buildtree.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      791 2024-03-15 09:41:31.000000 kssdtree-1.1.1/bytescale.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    11214 2024-03-15 09:41:31.000000 kssdtree-1.1.1/cluster.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14308 2024-03-15 09:41:31.000000 kssdtree-1.1.1/co2mco.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     8670 2024-03-15 09:41:31.000000 kssdtree-1.1.1/command_composite.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    85597 2024-03-15 09:41:31.000000 kssdtree-1.1.1/command_dist.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1491 2024-03-15 09:41:31.000000 kssdtree-1.1.1/command_dist_wrapper.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    30339 2024-03-15 09:41:31.000000 kssdtree-1.1.1/command_set.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5456 2024-03-15 09:41:31.000000 kssdtree-1.1.1/command_shuffle.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    16270 2024-03-15 09:41:31.000000 kssdtree-1.1.1/distancemat.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    31139 2024-03-15 09:41:31.000000 kssdtree-1.1.1/dnj.c
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-03-15 09:42:02.269480 kssdtree-1.1.1/dnjheaders/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      848 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/bytescale.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2455 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/dnj.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1823 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/filebuff.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2376 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/hclust.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1476 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/matrix.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1809 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/mman.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2894 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/nj.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1349 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/nwck.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1769 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/pherror.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1442 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/phy.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1097 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/qseqs.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      863 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/str.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1630 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/threader.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      787 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/tmp.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      997 2024-03-15 09:41:33.000000 kssdtree-1.1.1/dnjheaders/vector.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7897 2024-03-15 09:41:31.000000 kssdtree-1.1.1/filebuff.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    17969 2024-03-15 09:41:31.000000 kssdtree-1.1.1/global_basic.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    34136 2024-03-15 09:41:31.000000 kssdtree-1.1.1/hclust.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    24287 2024-03-15 09:41:31.000000 kssdtree-1.1.1/iseq2comem.c
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-03-15 09:42:02.273480 kssdtree-1.1.1/kssdheaders/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1915 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/co2mco.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      965 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/command_composite.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3905 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/command_dist.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1455 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/command_dist_wrapper.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      931 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/command_set.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1337 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/command_shuffle.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7850 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/global_basic.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1482 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/iseq2comem.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1809 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/mman.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      791 2024-03-15 09:41:33.000000 kssdtree-1.1.1/kssdheaders/mytime.h
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-03-15 09:42:02.273480 kssdtree-1.1.1/kssdtree.egg-info/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      477 2024-03-15 09:42:02.000000 kssdtree-1.1.1/kssdtree.egg-info/PKG-INFO
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1274 2024-03-15 09:42:02.000000 kssdtree-1.1.1/kssdtree.egg-info/SOURCES.txt
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       32 2024-03-15 09:42:02.000000 kssdtree-1.1.1/kssdtree.egg-info/dependency_links.txt
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)        1 2024-03-15 09:42:02.000000 kssdtree-1.1.1/kssdtree.egg-info/not-zip-safe
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       20 2024-03-15 09:42:02.000000 kssdtree-1.1.1/kssdtree.egg-info/requires.txt
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       31 2024-03-15 09:42:02.000000 kssdtree-1.1.1/kssdtree.egg-info/top_level.txt
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    18966 2024-03-15 09:41:31.000000 kssdtree-1.1.1/kssdtree.py
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    16438 2024-03-15 09:41:31.000000 kssdtree-1.1.1/matrix.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3564 2024-03-15 09:41:31.000000 kssdtree-1.1.1/mman.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1362 2024-03-15 09:41:31.000000 kssdtree-1.1.1/mytime.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    35423 2024-03-15 09:41:31.000000 kssdtree-1.1.1/nj.c
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-03-15 09:42:02.285481 kssdtree-1.1.1/njheaders/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3691 2024-03-15 09:41:34.000000 kssdtree-1.1.1/njheaders/align.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4993 2024-03-15 09:41:34.000000 kssdtree-1.1.1/njheaders/buildtree.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     6506 2024-03-15 09:41:34.000000 kssdtree-1.1.1/njheaders/cluster.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7468 2024-03-15 09:41:34.000000 kssdtree-1.1.1/njheaders/distancemat.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2584 2024-03-15 09:41:34.000000 kssdtree-1.1.1/njheaders/sequence.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14344 2024-03-15 09:41:34.000000 kssdtree-1.1.1/njheaders/tree.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3782 2024-03-15 09:41:34.000000 kssdtree-1.1.1/njheaders/util.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7969 2024-03-15 09:41:31.000000 kssdtree-1.1.1/nwck.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1925 2024-03-15 09:41:31.000000 kssdtree-1.1.1/pherror.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14122 2024-03-15 09:41:32.000000 kssdtree-1.1.1/phy.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5398 2024-03-15 09:41:32.000000 kssdtree-1.1.1/pydnj.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    20098 2024-03-15 09:41:32.000000 kssdtree-1.1.1/pykssd.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1713 2024-03-15 09:41:32.000000 kssdtree-1.1.1/pynj.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1935 2024-03-15 09:41:32.000000 kssdtree-1.1.1/qseqs.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4428 2024-03-15 09:41:32.000000 kssdtree-1.1.1/sequence.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       38 2024-03-15 09:42:02.285481 kssdtree-1.1.1/setup.cfg
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3581 2024-03-15 09:41:32.000000 kssdtree-1.1.1/setup.py
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1313 2024-03-15 09:41:32.000000 kssdtree-1.1.1/str.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2193 2024-03-15 09:41:32.000000 kssdtree-1.1.1/tmp.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    12251 2024-03-15 09:41:32.000000 kssdtree-1.1.1/toolutils.py
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    30399 2024-03-15 09:41:32.000000 kssdtree-1.1.1/tree.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4616 2024-03-15 09:41:32.000000 kssdtree-1.1.1/util.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1267 2024-03-15 09:41:32.000000 kssdtree-1.1.1/vector.c
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.415833 kssdtree-1.1.2/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       99 2024-03-15 09:41:31.000000 kssdtree-1.1.2/MANIFEST.in
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      477 2024-05-22 06:01:30.415833 kssdtree-1.1.2/PKG-INFO
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5769 2024-03-15 09:41:32.000000 kssdtree-1.1.2/README.md
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    11874 2024-03-15 09:41:31.000000 kssdtree-1.1.2/align.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    24008 2024-03-15 09:41:31.000000 kssdtree-1.1.2/buildtree.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      791 2024-03-15 09:41:31.000000 kssdtree-1.1.2/bytescale.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    11214 2024-03-15 09:41:31.000000 kssdtree-1.1.2/cluster.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14308 2024-03-15 09:41:31.000000 kssdtree-1.1.2/co2mco.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     8670 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_composite.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    85597 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_dist.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1491 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_dist_wrapper.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    30339 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_set.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5456 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_shuffle.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    16270 2024-03-15 09:41:31.000000 kssdtree-1.1.2/distancemat.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    31139 2024-03-15 09:41:31.000000 kssdtree-1.1.2/dnj.c
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.411833 kssdtree-1.1.2/dnjheaders/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      848 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/bytescale.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2455 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/dnj.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1823 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/filebuff.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2376 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/hclust.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1476 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/matrix.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1809 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/mman.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2894 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/nj.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1349 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/nwck.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1769 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/pherror.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1442 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/phy.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1097 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/qseqs.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      863 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/str.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1630 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/threader.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      787 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/tmp.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      997 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/vector.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7897 2024-03-15 09:41:31.000000 kssdtree-1.1.2/filebuff.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    17969 2024-03-15 09:41:31.000000 kssdtree-1.1.2/global_basic.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    34136 2024-03-15 09:41:31.000000 kssdtree-1.1.2/hclust.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    24287 2024-03-15 09:41:31.000000 kssdtree-1.1.2/iseq2comem.c
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.411833 kssdtree-1.1.2/kssdheaders/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1915 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/co2mco.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      965 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_composite.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3905 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_dist.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1455 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_dist_wrapper.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      931 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_set.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1337 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_shuffle.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7850 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/global_basic.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1482 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/iseq2comem.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1809 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/mman.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      791 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/mytime.h
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.411833 kssdtree-1.1.2/kssdtree.egg-info/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      477 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/PKG-INFO
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1274 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/SOURCES.txt
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       32 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/dependency_links.txt
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)        1 2024-03-15 09:42:02.000000 kssdtree-1.1.2/kssdtree.egg-info/not-zip-safe
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       20 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/requires.txt
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       31 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/top_level.txt
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    17560 2024-05-22 04:25:44.000000 kssdtree-1.1.2/kssdtree.py
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    16438 2024-03-15 09:41:31.000000 kssdtree-1.1.2/matrix.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3564 2024-03-15 09:41:31.000000 kssdtree-1.1.2/mman.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1362 2024-03-15 09:41:31.000000 kssdtree-1.1.2/mytime.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    35423 2024-03-15 09:41:31.000000 kssdtree-1.1.2/nj.c
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.415833 kssdtree-1.1.2/njheaders/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3691 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/align.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4993 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/buildtree.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     6506 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/cluster.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7468 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/distancemat.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2584 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/sequence.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14344 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/tree.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3782 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/util.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7969 2024-03-15 09:41:31.000000 kssdtree-1.1.2/nwck.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1925 2024-03-15 09:41:31.000000 kssdtree-1.1.2/pherror.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14122 2024-03-15 09:41:32.000000 kssdtree-1.1.2/phy.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5398 2024-03-15 09:41:32.000000 kssdtree-1.1.2/pydnj.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    20098 2024-03-15 09:41:32.000000 kssdtree-1.1.2/pykssd.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1713 2024-03-15 09:41:32.000000 kssdtree-1.1.2/pynj.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1935 2024-03-15 09:41:32.000000 kssdtree-1.1.2/qseqs.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4428 2024-03-15 09:41:32.000000 kssdtree-1.1.2/sequence.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       38 2024-05-22 06:01:30.415833 kssdtree-1.1.2/setup.cfg
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3581 2024-05-22 06:01:27.000000 kssdtree-1.1.2/setup.py
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1313 2024-03-15 09:41:32.000000 kssdtree-1.1.2/str.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2193 2024-03-15 09:41:32.000000 kssdtree-1.1.2/tmp.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    12433 2024-05-22 04:11:36.000000 kssdtree-1.1.2/toolutils.py
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    30399 2024-03-15 09:41:32.000000 kssdtree-1.1.2/tree.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4616 2024-03-15 09:41:32.000000 kssdtree-1.1.2/util.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1267 2024-03-15 09:41:32.000000 kssdtree-1.1.2/vector.c
```

### Comparing `kssdtree-1.1.1/README.md` & `kssdtree-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/align.c` & `kssdtree-1.1.2/align.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/buildtree.c` & `kssdtree-1.1.2/buildtree.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/bytescale.c` & `kssdtree-1.1.2/bytescale.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/cluster.c` & `kssdtree-1.1.2/cluster.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/co2mco.c` & `kssdtree-1.1.2/co2mco.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/command_composite.c` & `kssdtree-1.1.2/command_composite.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/command_dist.c` & `kssdtree-1.1.2/command_dist.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/command_dist_wrapper.c` & `kssdtree-1.1.2/command_dist_wrapper.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/command_set.c` & `kssdtree-1.1.2/command_set.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/command_shuffle.c` & `kssdtree-1.1.2/command_shuffle.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/distancemat.c` & `kssdtree-1.1.2/distancemat.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnj.c` & `kssdtree-1.1.2/dnj.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/bytescale.h` & `kssdtree-1.1.2/dnjheaders/bytescale.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/dnj.h` & `kssdtree-1.1.2/dnjheaders/dnj.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/filebuff.h` & `kssdtree-1.1.2/dnjheaders/filebuff.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/hclust.h` & `kssdtree-1.1.2/dnjheaders/hclust.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/matrix.h` & `kssdtree-1.1.2/dnjheaders/matrix.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/mman.h` & `kssdtree-1.1.2/dnjheaders/mman.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/nj.h` & `kssdtree-1.1.2/dnjheaders/nj.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/nwck.h` & `kssdtree-1.1.2/dnjheaders/nwck.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/pherror.h` & `kssdtree-1.1.2/dnjheaders/pherror.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/phy.h` & `kssdtree-1.1.2/dnjheaders/phy.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/qseqs.h` & `kssdtree-1.1.2/dnjheaders/qseqs.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/str.h` & `kssdtree-1.1.2/dnjheaders/str.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/threader.h` & `kssdtree-1.1.2/dnjheaders/threader.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/tmp.h` & `kssdtree-1.1.2/dnjheaders/tmp.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/dnjheaders/vector.h` & `kssdtree-1.1.2/dnjheaders/vector.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/filebuff.c` & `kssdtree-1.1.2/filebuff.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/global_basic.c` & `kssdtree-1.1.2/global_basic.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/hclust.c` & `kssdtree-1.1.2/hclust.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/iseq2comem.c` & `kssdtree-1.1.2/iseq2comem.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/co2mco.h` & `kssdtree-1.1.2/kssdheaders/co2mco.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/command_composite.h` & `kssdtree-1.1.2/kssdheaders/command_composite.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/command_dist.h` & `kssdtree-1.1.2/kssdheaders/command_dist.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/command_dist_wrapper.h` & `kssdtree-1.1.2/kssdheaders/command_dist_wrapper.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/command_set.h` & `kssdtree-1.1.2/kssdheaders/command_set.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/command_shuffle.h` & `kssdtree-1.1.2/kssdheaders/command_shuffle.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/global_basic.h` & `kssdtree-1.1.2/kssdheaders/global_basic.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/iseq2comem.h` & `kssdtree-1.1.2/kssdheaders/iseq2comem.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/mman.h` & `kssdtree-1.1.2/kssdheaders/mman.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdheaders/mytime.h` & `kssdtree-1.1.2/kssdheaders/mytime.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdtree.egg-info/SOURCES.txt` & `kssdtree-1.1.2/kssdtree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/kssdtree.py` & `kssdtree-1.1.2/kssdtree.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,386 +5,398 @@
 import os
 import platform
 import shutil
 import time
 import requests
 
 
-def shuffle(k=8, s=5, l=2, o='default'):
-    print('shuffling...')
+def shuffle(k=None, s=None, l=None, o=None):
     kssd.write_dim_shuffle_file(k, s, l, o)
-    print('shuffle finished!')
 
 
-def sketch(shuffle=None, genomes=None, output=None, set_opt=None):
-    """
-    sketch: sketching genomes into sketch and generating sketch files.
-    :param shuffle: Kssdtree provide 'L3K9.shuf' and 'L3K10.shuf' files as input for genome sketching or decomposition. The default is 'L3K10.shuf'.
-    :param genomes: The folder path for genome files. It supports the input of genome files in fasta/fastq formats.
-    :param output: The output folder path for sketch result files of genome files.
-    :param set_opt: Whether to do the set operation, default is False, if you want to do the set operation, you can set set_opt=True.
-    :return: null
-    """
-    if set_opt is None:
-        set_opt = False
-    if shuffle is not None and genomes is not None and output is not None:
-        current_directory = os.getcwd()
-        shuf_file_path = os.path.join(current_directory, shuffle)
-        if not os.path.exists(shuf_file_path):
-            if shuffle == 'L3K9.shuf':
-                print('downloading...', shuffle)
+def sketch(shuf_file=None, genomes_file=None, output=None, set_opt=None):
+    if shuf_file is not None and genomes_file is not None and output is not None:
+        if not os.path.exists(genomes_file):
+            print('No such file or directory: ', genomes_file)
+            return False
+        if set_opt is None:
+            set_opt = False
+        if not toolutils.allowed_file(genomes_file):
+            for filename in os.listdir(genomes_file):
+                if not toolutils.allowed_file(filename):
+                    print('Genome format error for file:', filename)
+                    return False
+        if not os.path.exists(shuf_file):
+            if shuf_file in ['L3K9.shuf']:
+                print('Downloading...', shuf_file)
                 import http.client
                 http.client.HTTPConnection._http_vsn = 10
                 http.client.HTTPConnection._http_vsn_str = 'HTTP/1.0'
-                url = 'http://18.205.53.149:8000/kssdtree/shuffle/' + shuffle
-                headers = {
-                    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.45 Safari/537.36'
-                }
-                r = requests.get(url, headers=headers, stream=True)
-                with open(os.getcwd() + "\\" + shuffle, mode="wb") as f:
-                    f.write(r.content)
-                print('download finished!', shuffle)
-            else:
-                file_name = shuffle.split('.')[0]
+                url = 'http://www.metakssdcoabundance.link/kssdtree/shuffle/' + shuf_file
+                start_time = time.time()
+                response = requests.get(url, stream=True)
+                with open(shuf_file, 'wb') as file:
+                    for chunk in response.iter_content(chunk_size=1024):
+                        if chunk:
+                            file.write(chunk)
+                end_time = time.time()
+                if end_time - start_time > 120:
+                    print(
+                        "Network timeout, please manually download from github (https://github.com/yhlink/kssdtree/tree/master/shuffle_file)")
+                    return False
+                print('Download finished: ', shuf_file)
+            elif shuf_file in ['L2K8.shuf', 'L3K10.shuf', 'L2K9.shuf', 'L3K11.shuf']:
+                print('Shuffling...', shuf_file)
+                file_name = shuf_file.split('.')[0]
                 k = int(file_name[3:])
-                if k == 10:
+                if k == 11 or k == 10:
                     s = 6
                 else:
                     s = 5
                 l = int(file_name[1])
-                shuffle(k=k, s=s, l=l, o=file_name)
-        print('sketching...')
+                shuffle(k, s, l, file_name)
+                print('Shuffle finished: ', shuf_file)
+            else:
+                print('No such file or directory: ', shuf_file)
+                return False
+        print('Sketching...')
         start = time.time()
         if set_opt:
-            kssd.dist_dispatch(shuffle, genomes, output, 1, 0, 0)
+            kssd.dist_dispatch(shuf_file, genomes_file, output, 1, 0, 0)
         else:
-            kssd.dist_dispatch(shuffle, genomes, output, 0, 0, 0)
+            kssd.dist_dispatch(shuf_file, genomes_file, output, 0, 0, 0)
         end = time.time()
-        print('sketch spend time：%.2fs' % (end - start))
-        print('sketch finished!')
+        print('Sketch spend time：%.2fs' % (end - start))
+        print('Sketch finished!')
+        return True
     else:
-        print('args error!!!')
+        print('Args error!!!')
+        return False
 
 
 def dist(ref_sketch=None, qry_sketch=None, output=None, flag=None):
-    """
-    computing pairwise distances between reference and query genomes, and then generating a distance matrix in phylip format.
-    :param ref_sketch: The folder path for sketch result files of reference genome files.
-    :param qry_sketch: The folder path for sketch result files of query genome files.
-    :param output: The output filename of distance matrix in phylip format.
-    :param flag: 0 or 1. 0,1 is used to generate the distance matrix required by NJ (0 for diagonal elements) and DNJ (no diagonal elements) respectively.
-    :return: null
-    """
-    if flag is None:
-        flag = 0
     if ref_sketch is not None and qry_sketch is not None and output is not None:
-        print('disting...')
+        if not os.path.exists(ref_sketch):
+            print('No such file or directory: ', ref_sketch)
+            return False
+        if not os.path.exists(qry_sketch):
+            print('No such file or directory: ', qry_sketch)
+            return False
+        if flag is None:
+            flag = 0
+        print('Disting...')
         start = time.time()
-        kssd.dist_dispatch(ref_sketch, output, qry_sketch, 2, 0, flag)
-        end = time.time()
-        print('dist spend time：%.2fs' % (end - start))
-        print('dist finished!')
+        if '/' in output:
+            output_dir = os.path.dirname(output)
+            output_name = output.split('/')[-1]
+            if not os.path.exists(output_dir):
+                os.makedirs(output_dir)
+                print("Created directory:", output_dir)
+        else:
+            output_name = output
+        if output_name.endswith(".phy") or output_name.endswith(".phylip"):
+            kssd.dist_dispatch(ref_sketch, output, qry_sketch, 2, 0, flag)
+            end = time.time()
+            print('Dist spend time：%.2fs' % (end - start))
+            print('Dist finished!')
+            return True
+        else:
+            print('Output type error, only supports .phylip (.phy) format:', output_name)
+            return False
     else:
-        print('args error!!!')
+        print('Args error!!!')
+        return False
 
 
-def retrieve(ref_sketch=None, qry_sketch=None, output=None, N=None):
-    """
-    retrieving N closest sketches from reference or GTDB (R214) sketches and combining query sketch files.
-    :param ref_sketch: The folder path for sketch result files of reference genome files.
-    :param qry_sketch: The folder path for sketch result files of query genome files.
-    :param output: The output folder path for retrieve sketch result files of genome files.
-    :param N: Max number of nearest reference genomes.
-    :return: null
-    """
+def retrieve(ref_sketch=None, qry_sketch=None, output=None, N=None, method=None):
     if ref_sketch is not None and qry_sketch is not None and output is not None:
+        if method is None:
+            method = 'nj'
+        if method not in ['nj', 'dnj']:
+            print('Only support nj and dnj methods!!!')
+            return
+        if not os.path.exists(qry_sketch):
+            print('No such file or directory: ', qry_sketch)
+            return False
         if ref_sketch == 'gtdbr214_sketch':
-            print('retrieving...')
+            print('Retrieving...')
             start = time.time()
-            temp_related_sketch = 'related_sketch'
-            reference = 'static/gtdbr214_sketch'
-            kssd.dist_dispatch(reference, output, qry_sketch, 2, N, 3)
-            kssd.print_gnames(reference, 'gtdb.txt')
-            file_path1 = os.path.join(os.getcwd(), 'distout', 'distance.out')
-            toolutils.deal_gtdb_txt(file_path1)
-            kssd.grouping_genomes('new_gtdb.txt', reference, temp_related_sketch)
-            kssd.dist_dispatch(output, qry_sketch, temp_related_sketch, 3, 0, 0)
+            if not os.path.exists(output):
+                os.makedirs(output)
+                print("Created directory:", output)
+            newick, accession_taxonomy = toolutils.upload_request(qry_sketch=qry_sketch, method=method, N=N)
+            with open(os.path.join(output, 'output.newick'), 'w') as f:
+                f.write(newick)
+            with open(os.path.join(output, 'output_accession_taxonomy.txt'), 'w') as f:
+                for key, value in accession_taxonomy.items():
+                    f.write("%s %s\n" % (key, value))
             end = time.time()
-            print('retrieve spend time：%.2fs' % (end - start))
-            print('retrieve finished!')
+            print('Retrieve spend time：%.2fs' % (end - start))
+            print('Retrieve finished!')
+            return True
         else:
-            print('retrieving...')
-            start = time.time()
-            timeStamp = int(time.mktime(time.localtime(time.time())))
-            temp_related_sketch = 'related_sketch_' + str(timeStamp)
-            kssd.dist_dispatch(ref_sketch, output, qry_sketch, 2, N, 3)
-            kssd.print_gnames(ref_sketch, 'gtdb.txt')
-            file_path1 = os.path.join(os.getcwd(), 'distout', 'distance.out')
-            toolutils.deal_gtdb_txt(file_path1)
-            kssd.grouping_genomes('new_gtdb.txt', ref_sketch, temp_related_sketch)
-            kssd.dist_dispatch(output, qry_sketch, temp_related_sketch, 3, 0, 0)
-            end = time.time()
-            file_path1 = 'new.txt'
-            file_path2 = 'gtdb.txt'
-            file_path3 = 'new_gtdb.txt'
-            file_path4 = 'related_genomes_values.txt'
-            file_path5 = 'modified_file.txt'
-            file_path6 = 'new_accession_taxonomy.txt'
-            if os.path.exists(file_path1):
-                os.remove(file_path1)
-            if os.path.exists(file_path2):
-                os.remove(file_path2)
-            if os.path.exists(file_path3):
-                os.remove(file_path3)
-            if os.path.exists(file_path4):
-                os.remove(file_path4)
-            if os.path.exists(file_path5):
-                os.remove(file_path5)
-            if os.path.exists(file_path6):
-                os.remove(file_path6)
-            print('retrieve spend time：%.2fs' % (end - start))
-            print('retrieve finished!')
+            print("ref_sketch must be set to 'gtdbr214_sketc'")
+            return False
     else:
-        print('args error!!!')
+        print('Args error!!!')
+        return False
 
 
 def build(phylip=None, output=None, method=None):
-    """
-    constructing tree with NJ or DNJ and generating tree in newick format.
-    :param phylip: The distance matrix in phylip format.
-    :param output: 'nj'(NJ) or 'dnj'(DNJ) method for constructing tree. The default is 'nj'.
-    :param method: The output filename of tree in newick format.
-    :return: null
-    """
-    if method is None:
-        method = 'nj'
-    if method not in ['nj', 'dnj']:
-        print('method only support nj and dnj!!!')
-        return
     if phylip is not None:
-        print('building...')
-        start = time.time()
-        if output is None:
-            output = 'kssdtree.newick'
-        if method == 'nj':
-            state = nj.build(phylip, output)
+        if not os.path.exists(phylip):
+            print('No such file or directory: ', phylip)
+            return False
+        if method is None:
+            method = 'nj'
+        if method not in ['nj', 'dnj']:
+            print('Only support nj and dnj methods!!!')
+            return False
+        print('Building...')
+        if '/' in output:
+            output_dir = os.path.dirname(output)
+            output_name = output.split('/')[-1]
+            if not os.path.exists(output_dir):
+                os.makedirs(output_dir)
+                print("Created directory:", output_dir)
         else:
-            if platform.system() == 'Linux':
-                state = dnj.build(phylip, output, method)
-            else:
+            output_name = output
+        if output_name.endswith(".nwk") or output_name.endswith(".newick"):
+            start = time.time()
+            if method == 'nj':
                 state = nj.build(phylip, output)
-        if state == 1:
-            nwk_path = os.path.join(os.getcwd(), output)
-            with open(nwk_path, 'r') as f:
-                lines = f.readlines()
-                newick = ''.join(lines)
-                newick = newick.replace('\n', '')
-            with open(nwk_path, 'w') as f:
-                f.write(newick)
-            end = time.time()
-            print('build spend time：%.2fs' % (end - start))
-            print('build finished!')
+            else:
+                if platform.system() == 'Linux':
+                    state = dnj.build(phylip, output, method)
+                else:
+                    state = nj.build(phylip, output)
+            if state == 1:
+                with open(output, 'r') as f:
+                    lines = f.readlines()
+                    newick = ''.join(lines)
+                    newick = newick.replace('\n', '')
+                with open(output, 'w') as f:
+                    f.write(newick)
+                end = time.time()
+                print('Build spend time：%.2fs' % (end - start))
+                print('Build finished!')
+                return True
     else:
-        print('args error!!!')
+        print('Args error!!!')
+        return False
 
 
 def visualize(newick=None, taxonomy=None, mode=None):
-    """
-    visualizing tree with ETE3 toolkit.
-    :param newick: The tree in newick format.
-    :param taxonomy:  The taxonomy information in txt format, which records the name (accession) of genome and its taxonomy. The default is None.
-    :param mode: 'r'(rectangle) or 'c'(circle) mode for visualizing tree. The default is 'r'.
-    :return: null
-    """
-    if mode is None:
-        mode = 'r'
     if newick is not None:
+        if not os.path.exists(newick):
+            print('No such file or directory: ', newick)
+            return False
+        if mode is None:
+            mode = 'r'
         toolutils.view_tree(newick, taxonomy, mode=mode)
     else:
-        print('args error!!!')
+        print('Args error!!!')
+        return False
 
 
 def union(ref_sketch=None, output=None):
-    """
-    :param sketch:
-    :param output:
-    :return:
-    """
     if ref_sketch is not None and output is not None:
-        kssd.sketch_union(sketch, output)
+        if not os.path.exists(ref_sketch):
+            print('No such file or directory: ', ref_sketch)
+            return False
+        kssd.sketch_union(ref_sketch, output)
+        return True
     else:
-        print('args error!!!')
+        return False
 
 
-def subtract(ref_sketch=None, genomes_sketch=None, output=None, flag=0):
-    """
-    subtracting the ref_sketch from genomes_sketch and creating the remainder sketch files.
-    :param ref_sketch: The folder path for reference sketch result files.
-    :param genomes_sketch: The folder path for sketch result files of genome files.
-    :param output: The output folder path for remainder sketch result files.
-    :param flag: 0.
-    :return: null
-    """
+def subtract(ref_sketch=None, genomes_sketch=None, output=None, flag=None):
     if ref_sketch is not None and genomes_sketch is not None and output is not None:
+        if not os.path.exists(ref_sketch):
+            print('No such file or directory: ', ref_sketch)
+            return False
+        if not os.path.exists(genomes_sketch):
+            print('No such file or directory: ', genomes_sketch)
+            return False
         if flag == 1:
-            print('subtracting...')
+            print('Subtracting...')
             start = time.time()
             kssd.sketch_operate(ref_sketch, output, genomes_sketch)
             end = time.time()
-            print('subtract spend time：%.2fs' % (end - start))
-            print('subtract finished!')
+            print('Subtract spend time：%.2fs' % (end - start))
+            print('Subtract finished!')
+            return True
         else:
             timeStamp = int(time.mktime(time.localtime(time.time())))
-            temp_union_sketch = 'ref_union_sketch_' + str(timeStamp)
-            print('subtracting...')
+            print('Subtracting...')
             start = time.time()
-            union(ref_sketch=ref_sketch, output=temp_union_sketch)
+            temp_txt = 'ref.txt'
+            kssd.print_gnames(ref_sketch, temp_txt)
+            nums = 0
+            with open(temp_txt, 'r') as file:
+                for line in file:
+                    nums += 1
+            if nums == 1:
+                temp_union_sketch = ref_sketch
+            else:
+                temp_union_sketch = 'ref_union_sketch_' + str(timeStamp)
+            r = union(ref_sketch=ref_sketch, output=temp_union_sketch)
+            if not r:
+                print('Union error!!!')
+                return False
             kssd.sketch_operate(temp_union_sketch, output, genomes_sketch)
             end = time.time()
             current_directory = os.getcwd()
             temp_dir = os.path.join(current_directory, temp_union_sketch)
             if platform.system() == 'Linux':
                 if os.path.exists(temp_dir):
                     shutil.rmtree(temp_dir)
+                if os.path.exists(temp_txt):
+                    os.remove(temp_txt)
             else:
                 pass
-            print('subtract spend time：%.2fs' % (end - start))
-            print('subtract finished!')
+            print('Subtract spend time：%.2fs' % (end - start))
+            print('Subtract finished!')
+            return True
     else:
-        print('args error!!!')
+        print('Args error!!!')
+        return False
 
 
-def quick(shuffle=None, genomes=None, output=None, reference=None, taxonomy=None, method='nj', mode='r', N=0):
-    """
-    simplifying pipeline and eliminating the necessity of organizing many intermediate files.
-    :param shuffle: Kssdtree provide frequently-used 'L3K9.shuf' and 'L3K10.shuf' files as input for genome sketching or decomposition. The default is 'L3K10.shuf'. If you want to perform phylogenetic placement, you must use 'L3K9.shuf' file.
-    :param genomes: The folder path for genome files. It supports the input of genome files in fasta/fastq formats.
-    :param output: The output filename of tree in newick format.
-    :param reference: The default is None, will perform the routine workflow. If you want to perform the reference subtraction workflow, you can set reference to the reference genome file or folder path. If you want to perform the phylogenetic placement, you must set reference to ‘gtdbr214’.
-    :param taxonomy: The filename of taxonomy information in txt format, which records the name (accession) of genome and its taxonomy. The default is None.
-    :param method: 'nj'(NJ) or 'dnj'(DNJ) method for constructing tree. The default is 'nj'.
-    :param mode: 'r'(rectangle) or 'c'(circle) mode for visualizing tree. The default is 'r'.
-    :param N: Max number of nearest reference genomes. The default is 0 for computing pairwise distances between genomes on routine and reference subtraction workflows. If you want to perform the phylogenetic placement, you can set N > 0.
-    :return: null
-    """
+def quick(shuf_file=None, genomes_file=None, output=None, reference=None, taxonomy=None, method='nj', mode='r', N=0):
     if reference is None and taxonomy is None:
-        if shuffle is not None and genomes is not None and output is not None:
-            for filename in os.listdir(genomes):
-                if not toolutils.allowed_file(filename):
-                    print('Genome format error for file:', filename)
-                    return 0
+        if shuf_file is not None and genomes_file is not None and output is not None:
             timeStamp = int(time.mktime(time.localtime(time.time())))
-            temp_sketch = genomes + '_sketch_' + str(timeStamp)
+            temp_sketch = genomes_file + '_sketch_' + str(timeStamp)
             temp_phy = 'temp.phy'
-            print('step1...')
-            sketch(shuffle=shuffle, genomes=genomes, output=temp_sketch, set_opt=False)
-            print('step2...')
+            print('Step1...')
+            s1 = sketch(shuf_file=shuf_file, genomes_file=genomes_file, output=temp_sketch, set_opt=False)
+            if not s1:
+                return False
+            print('Step2...')
             if method == 'nj':
-                dist(ref_sketch=temp_sketch, qry_sketch=temp_sketch, output=temp_phy, flag=0)
-            else:
-                dist(ref_sketch=temp_sketch, qry_sketch=temp_sketch, output=temp_phy, flag=1)
-            print('step3...')
-            build(phylip=temp_phy, output=output, method=method)
-            if platform.system() == 'Linux':
-                pass
+                s2 = dist(ref_sketch=temp_sketch, qry_sketch=temp_sketch, output=temp_phy, flag=0)
             else:
-                print('step4...')
-                print('tree visualization finished!')
-                visualize(newick=output, taxonomy=taxonomy, mode=mode)
-            current_directory = os.getcwd()
-            temp_dir1 = os.path.join(current_directory, temp_sketch)
-            temp_dir2 = os.path.join(current_directory, 'distout')
+                s2 = dist(ref_sketch=temp_sketch, qry_sketch=temp_sketch, output=temp_phy, flag=1)
+            if not s2:
+                return False
+            print('Step3...')
+            s3 = build(phylip=temp_phy, output=output, method=method)
+            if not s3:
+                return False
             if platform.system() == 'Linux':
+                current_directory = os.getcwd()
+                temp_dir1 = os.path.join(current_directory, temp_sketch)
+                temp_dir2 = os.path.join(current_directory, 'distout')
                 if os.path.exists(temp_dir1):
                     shutil.rmtree(temp_dir1)
                 if os.path.exists(temp_dir2):
                     shutil.rmtree(temp_dir2)
+                if os.path.exists(temp_phy):
+                    os.remove(temp_phy)
+                return True
             else:
-                pass
+                print('Step4...')
+                print('Tree visualization finished!')
+                visualize(newick=output, taxonomy=taxonomy, mode=mode)
         else:
-            print('args error!!!')
-    elif reference == 'gtdbr214' and taxonomy is None:
-        if shuffle is not None and genomes is not None and output is not None and toolutils.is_positive_integer(N):
-            if shuffle != 'L3K9.shuf':
-                print("shuffle must be set to 'L3K9.shuf'")
-                return 0
-            for filename in os.listdir(genomes):
-                if not toolutils.allowed_file(filename):
-                    print('Genome format error for file:', filename)
-                    return 0
+            print('Args error!!!')
+            return False
+
+    elif reference == 'gtdbr214_sketch' and taxonomy is None:
+        if shuf_file is not None and genomes_file is not None and output is not None:
+            if not toolutils.is_positive_integer(N):
+                print("N must >0 !!!")
+                return False
+            if shuf_file != 'L3K9.shuf':
+                print("shuffle file must be set to 'L3K9.shuf'")
+                return False
             timeStamp = int(time.mktime(time.localtime(time.time())))
-            temp_sketch = genomes + '_sketch_' + str(timeStamp)
-            sketch(shuffle=shuffle, genomes=genomes, output=temp_sketch, set_opt=True)
-            newick, accession_taxonomy = toolutils.upload_request(dir_name=temp_sketch, method=method, N=N)
-            with open(output, 'w') as f:
-                f.write(newick)
-            with open('accession_taxonomy.txt', 'w') as f:
-                for key, value in accession_taxonomy.items():
-                    f.write("%s %s\n" % (key, value))
+            qry_sketch = genomes_file + '_sketch_' + str(timeStamp)
+            s1 = sketch(shuf_file=shuf_file, genomes_file=genomes_file, output=qry_sketch, set_opt=True)
+            if not s1:
+                return False
+            s2 = retrieve(ref_sketch=reference, qry_sketch=qry_sketch, output=output, N=N, method=method)
+            if not s2:
+                return False
             if platform.system() == 'Linux':
-                pass
+                return True
             else:
-                print('tree visualization finished!')
-                visualize(newick=output, taxonomy='accession_taxonomy.txt', mode=None)
+                print('Tree visualization finished!')
+                visualize(newick=os.path.join(output, 'output.newick'),
+                          taxonomy=os.path.join(output, 'output_accession_taxonomy.txt'), mode=None)
         else:
-            print('args error or N<=0!!!')
+            print('Args error!!!')
+            return False
     else:
-        if shuffle is not None and genomes is not None and output is not None and method in ['nj', 'dnj']:
-            if shuffle is not None and genomes is not None and output is not None and method in ['nj', 'dnj']:
+        if shuf_file is not None and genomes_file is not None and output is not None and method in ['nj', 'dnj']:
+            if shuf_file is not None and genomes_file is not None and output is not None and method in ['nj', 'dnj']:
                 timeStamp = int(time.mktime(time.localtime(time.time())))
                 temp_reference_sketch = 'ref_sketch_' + str(timeStamp)
-                temp_genomes_sketch = genomes + '_sketch_' + str(timeStamp)
+                temp_genomes_sketch = genomes_file + '_sketch_' + str(timeStamp)
                 if not toolutils.allowed_file(reference):
                     cur_path = os.getcwd()
                     ref_path = os.path.join(cur_path, reference)
                     num = toolutils.get_file_num(ref_path)
                     if num == 1:
                         temp_union_sketch = temp_reference_sketch
                     else:
                         temp_union_sketch = 'ref_union_sketch_' + str(timeStamp)
                 else:
                     temp_union_sketch = temp_reference_sketch
-                temp_subtract_sketch = genomes + '_subtract_sketch_' + str(timeStamp)
+                temp_subtract_sketch = genomes_file + '_subtract_sketch_' + str(timeStamp)
                 temp_phy = 'temp.phy'
-                print('step1...')
-                sketch(shuffle=shuffle, genomes=reference, output=temp_reference_sketch, set_opt=True)
-                sketch(shuffle=shuffle, genomes=genomes, output=temp_genomes_sketch, set_opt=True)
-                print('step2...')
-                union(ref_sketch=temp_reference_sketch, output=temp_union_sketch)
-                subtract(ref_sketch=temp_union_sketch, genomes_sketch=temp_genomes_sketch,
-                         output=temp_subtract_sketch, flag=1)
-                print('step3...')
+                print('Step1...')
+                s1 = sketch(shuf_file=shuf_file, genomes_file=reference, output=temp_reference_sketch, set_opt=True)
+                if not s1:
+                    return False
+                s2 = sketch(shuf_file=shuf_file, genomes_file=genomes_file, output=temp_genomes_sketch, set_opt=True)
+                if not s2:
+                    return False
+                print('Step2...')
+                s3 = union(ref_sketch=temp_reference_sketch, output=temp_union_sketch)
+                if not s3:
+                    return False
+                s4 = subtract(ref_sketch=temp_union_sketch, genomes_sketch=temp_genomes_sketch,
+                              output=temp_subtract_sketch, flag=1)
+                if not s4:
+                    return False
+                print('Step3...')
                 if method == 'nj':
-                    dist(ref_sketch=temp_subtract_sketch, qry_sketch=temp_subtract_sketch, output=temp_phy,
-                         flag=0)
+                    s5 = dist(ref_sketch=temp_subtract_sketch, qry_sketch=temp_subtract_sketch, output=temp_phy,
+                              flag=0)
                 else:
-                    dist(ref_sketch=temp_subtract_sketch, qry_sketch=temp_subtract_sketch, output=temp_phy,
-                         flag=1)
-                print('step4...')
-                build(phylip=temp_phy, output=output, method=method)
-                if platform.system() == 'Linux':
-                    pass
-                else:
-                    print('step5...')
-                    print('tree visualization finished!')
-                    visualize(newick=output, taxonomy=taxonomy, mode=mode)
-                current_directory = os.getcwd()
-                temp_dir1 = os.path.join(current_directory, temp_reference_sketch)
-                temp_dir2 = os.path.join(current_directory, temp_genomes_sketch)
-                temp_dir3 = os.path.join(current_directory, temp_union_sketch)
-                temp_dir4 = os.path.join(current_directory, temp_subtract_sketch)
-                temp_dir5 = os.path.join(current_directory, 'distout')
+                    s5 = dist(ref_sketch=temp_subtract_sketch, qry_sketch=temp_subtract_sketch, output=temp_phy,
+                              flag=1)
+                if not s5:
+                    return False
+                print('Step4...')
+                s6 = build(phylip=temp_phy, output=output, method=method)
+                if not s6:
+                    return False
                 if platform.system() == 'Linux':
+                    current_directory = os.getcwd()
+                    temp_dir1 = os.path.join(current_directory, temp_reference_sketch)
+                    temp_dir2 = os.path.join(current_directory, temp_genomes_sketch)
+                    temp_dir3 = os.path.join(current_directory, temp_union_sketch)
+                    temp_dir4 = os.path.join(current_directory, temp_subtract_sketch)
+                    temp_dir5 = os.path.join(current_directory, 'distout')
                     if os.path.exists(temp_dir1):
                         shutil.rmtree(temp_dir1)
                     if os.path.exists(temp_dir2):
                         shutil.rmtree(temp_dir2)
                     if os.path.exists(temp_dir3):
                         shutil.rmtree(temp_dir3)
                     if os.path.exists(temp_dir4):
                         shutil.rmtree(temp_dir4)
                     if os.path.exists(temp_dir5):
                         shutil.rmtree(temp_dir5)
+                    if os.path.exists(temp_phy):
+                        os.remove(temp_phy)
+                    return True
                 else:
-                    pass
+                    print('Step5...')
+                    print('Tree visualization finished!')
+                    visualize(newick=output, taxonomy=taxonomy, mode=mode)
             else:
-                print('args error!!!')
+                print('Args error!!!')
+                return False
```

### Comparing `kssdtree-1.1.1/matrix.c` & `kssdtree-1.1.2/matrix.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/mman.c` & `kssdtree-1.1.2/mman.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/mytime.c` & `kssdtree-1.1.2/mytime.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/nj.c` & `kssdtree-1.1.2/nj.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/njheaders/align.h` & `kssdtree-1.1.2/njheaders/align.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/njheaders/buildtree.h` & `kssdtree-1.1.2/njheaders/buildtree.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/njheaders/cluster.h` & `kssdtree-1.1.2/njheaders/cluster.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/njheaders/distancemat.h` & `kssdtree-1.1.2/njheaders/distancemat.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/njheaders/sequence.h` & `kssdtree-1.1.2/njheaders/sequence.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/njheaders/tree.h` & `kssdtree-1.1.2/njheaders/tree.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/njheaders/util.h` & `kssdtree-1.1.2/njheaders/util.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/nwck.c` & `kssdtree-1.1.2/nwck.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/pherror.c` & `kssdtree-1.1.2/pherror.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/phy.c` & `kssdtree-1.1.2/phy.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/pydnj.c` & `kssdtree-1.1.2/pydnj.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/pykssd.c` & `kssdtree-1.1.2/pykssd.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/pynj.c` & `kssdtree-1.1.2/pynj.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/qseqs.c` & `kssdtree-1.1.2/qseqs.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/sequence.c` & `kssdtree-1.1.2/sequence.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/setup.py` & `kssdtree-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     'pyqt5',
     'ete3',
     'requests'
 ]
 
 setup(
     name='kssdtree',
-    version='1.1.1',
+    version='1.1.2',
     author='Hang Yang',
     author_email='yhlink1207@gmail.com',
     description="Kssdtree is a versatile Python package for phylogenetic analysis. It also provides one-stop tree construction and visualization. It can handle DNA sequences of both fasta or fastq format, whether gzipped or not. ",
     url='https://github.com/yhlink/kssdtree',
     download_url='https://pypi.org/project/kssdtree',
     ext_modules=[
         Extension(MOD1, sources=sources1, include_dirs=include_dirs1, libraries=['z'],
```

### Comparing `kssdtree-1.1.1/str.c` & `kssdtree-1.1.2/str.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/tmp.c` & `kssdtree-1.1.2/tmp.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/toolutils.py` & `kssdtree-1.1.2/toolutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,28 @@
             get_file_num(sub_dir)
         else:
             ax = os.path.basename(sub_dir)
             res.append(ax)
     return len(res)
 
 
-def upload_request(dir_name, method, N):
-    zip_file = dir_name + '.zip'
+def decompress_zip(zip_path, dir_path):
+    f = zipfile.ZipFile(zip_path, 'r')
+    for file in f.namelist():
+        f.extract(file, dir_path)
+    f.close()
+
+
+def upload_request(qry_sketch, method, N):
+    zip_file = qry_sketch + '.zip'
     zip = zipfile.ZipFile(zip_file, 'w', zipfile.ZIP_DEFLATED)
-    for item in os.listdir(dir_name):
-        zip.write(dir_name + os.sep + item)
+    for item in os.listdir(qry_sketch):
+        zip.write(qry_sketch + os.sep + item)
     zip.close()
-    url = "http://18.205.53.149:8000/kssdtree/upload"
+    url = "http://www.metakssdcoabundance.link/kssdtree/upload"
     header = {
         "kssdtree": 'upload'
     }
     data = {
         'method': method,
         "N": N
     }
@@ -215,15 +222,14 @@
                 nst["vt_line_type"] = 0
                 nst["hz_line_type"] = 0
                 node.img_style = nst
                 node.set_style(nst)
         # t.render("bubble_map.png", w=600, dpi=300, tree_style=ts)
         t.show(tree_style=ts)
 
-
 def deal_gtdb_txt(temp_dist_output):
     data = pd.read_csv(temp_dist_output, delimiter='\t', header=None, skiprows=1)
     column_2 = data.iloc[:, 1]
     with open('new.txt', 'w') as file:
         for item in column_2:
             file.write(str(item) + '\n')
     with open('new.txt', 'r') as file:
```

### Comparing `kssdtree-1.1.1/tree.c` & `kssdtree-1.1.2/tree.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/util.c` & `kssdtree-1.1.2/util.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.1/vector.c` & `kssdtree-1.1.2/vector.c`

 * *Files identical despite different names*

