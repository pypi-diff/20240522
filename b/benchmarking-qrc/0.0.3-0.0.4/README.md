# Comparing `tmp/benchmarking-qrc-0.0.3.tar.gz` & `tmp/benchmarking_qrc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchmarking-qrc-0.0.3.tar", last modified: Tue Aug  2 11:39:30 2022, max compression
+gzip compressed data, was "benchmarking_qrc-0.0.4.tar", last modified: Wed May 22 12:55:40 2024, max compression
```

## Comparing `benchmarking-qrc-0.0.3.tar` & `benchmarking_qrc-0.0.4.tar`

### file list

```diff
@@ -1,201 +1,200 @@
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.480249 benchmarking-qrc-0.0.3/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     1063 2022-08-01 09:58:02.000000 benchmarking-qrc-0.0.3/LICENSE.txt
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)      155 2022-08-01 12:49:08.000000 benchmarking-qrc-0.0.3/MANIFEST.in
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     1575 2022-08-02 11:39:30.480249 benchmarking-qrc-0.0.3/PKG-INFO
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)      942 2022-08-01 12:37:49.000000 benchmarking-qrc-0.0.3/README.md
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.440250 benchmarking-qrc-0.0.3/data/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.440250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.460250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:58:03.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.460250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:58:03.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.440250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.460250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 04:12:22.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.460250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 04:12:22.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.460250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:33:31.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.460250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:33:32.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.460250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:34:53.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:34:54.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:35:01.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:35:02.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:35:07.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:35:08.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:35:12.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:35:13.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:39:30.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:39:30.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:24.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:25.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:29.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:30.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:32.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:34.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.464249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:37.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:38.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:41.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:42.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:47.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:48.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.448250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:52.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:54.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:58.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:50:59.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:08.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:10.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:15.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:16.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:19.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:20.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:24.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:25.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:29.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:30.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:34.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.468249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:35.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:40.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:41.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.452250 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:46.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:52:47.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:53:55.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:53:56.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:00.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:01.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:04.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:05.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:07.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:08.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:11.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:12.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:17.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:18.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:23.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:24.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.456250 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:29.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8128 2022-08-01 03:54:30.000000 benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.472249 benchmarking-qrc-0.0.3/notebooks/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.476249 benchmarking-qrc-0.0.3/notebooks/.ipynb_checkpoints/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)    45846 2022-08-01 03:33:23.000000 benchmarking-qrc-0.0.3/notebooks/.ipynb_checkpoints/Tutorial - Memory capacity-checkpoint.ipynb
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)    66174 2022-08-01 09:35:00.000000 benchmarking-qrc-0.0.3/notebooks/.ipynb_checkpoints/Tutorial - Quantum Reservoir Computing-checkpoint.ipynb
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)    66484 2022-08-02 10:47:30.000000 benchmarking-qrc-0.0.3/notebooks/.ipynb_checkpoints/Tutorial-checkpoint.ipynb
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)    65173 2022-08-02 11:01:08.000000 benchmarking-qrc-0.0.3/notebooks/Tutorial.ipynb
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.476249 benchmarking-qrc-0.0.3/notebooks/images/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     6765 2022-07-30 09:46:20.000000 benchmarking-qrc-0.0.3/notebooks/images/QRC_diagram.png
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)   164367 2022-07-30 10:05:35.000000 benchmarking-qrc-0.0.3/notebooks/images/nn_rc.png
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)   124118 2022-07-30 10:11:51.000000 benchmarking-qrc-0.0.3/notebooks/images/rnn_and_rc.png
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)    28525 2022-07-31 15:30:34.000000 benchmarking-qrc-0.0.3/notebooks/images/table.png
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)       38 2022-08-02 11:39:30.480249 benchmarking-qrc-0.0.3/setup.cfg
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)      947 2022-08-02 11:37:04.000000 benchmarking-qrc-0.0.3/setup.py
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.460250 benchmarking-qrc-0.0.3/src/
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.476249 benchmarking-qrc-0.0.3/src/benchmarking_qrc/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 10:34:36.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc/__init__.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     8963 2022-07-31 18:25:23.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc/hamiltonian.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     9774 2022-08-01 02:47:37.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc/measurements.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     5848 2022-07-31 19:02:16.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc/reservoir.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)    10692 2022-08-02 10:37:52.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc/run_memory_capacity.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)      854 2022-01-14 10:10:12.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc/utils.py
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.476249 benchmarking-qrc-0.0.3/src/benchmarking_qrc.egg-info/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     1575 2022-08-02 11:39:30.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc.egg-info/PKG-INFO
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     7676 2022-08-02 11:39:30.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc.egg-info/SOURCES.txt
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)        1 2022-08-02 11:39:30.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc.egg-info/dependency_links.txt
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)       19 2022-08-02 11:39:30.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc.egg-info/requires.txt
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)       17 2022-08-02 11:39:30.000000 benchmarking-qrc-0.0.3/src/benchmarking_qrc.egg-info/top_level.txt
-drwxrwxr-x   0 gllodra12  (1000) gllodra12  (1000)        0 2022-08-02 11:39:30.480249 benchmarking-qrc-0.0.3/tests/
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)      565 2021-10-06 08:17:39.000000 benchmarking-qrc-0.0.3/tests/conftest.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     7591 2022-07-31 18:25:21.000000 benchmarking-qrc-0.0.3/tests/test_hamiltonian.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)    15332 2022-08-01 02:49:09.000000 benchmarking-qrc-0.0.3/tests/test_measurements.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     4373 2022-08-02 11:22:32.000000 benchmarking-qrc-0.0.3/tests/test_memory_capacity.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     3341 2022-07-31 17:01:34.000000 benchmarking-qrc-0.0.3/tests/test_reservoir.py
--rw-rw-r--   0 gllodra12  (1000) gllodra12  (1000)     6591 2022-05-22 17:10:04.000000 benchmarking-qrc-0.0.3/tests/utils.py
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:40.224894 benchmarking_qrc-0.0.4/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     1063 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/LICENSE.txt
+-rw-r--r--   0 guillemllodra  (1124) users      (100)      155 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/MANIFEST.in
+-rw-r--r--   0 guillemllodra  (1124) users      (100)      974 2024-05-22 12:55:40.216894 benchmarking_qrc-0.0.4/PKG-INFO
+-rw-r--r--   0 guillemllodra  (1124) users      (100)      376 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/README.md
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.792753 benchmarking_qrc-0.0.4/data/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.872758 benchmarking_qrc-0.0.4/data/memory_capacity/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.792753 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.980764 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.020766 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.796753 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.040767 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.080770 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.800753 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.128772 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.204777 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.800753 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.252780 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.292782 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.804754 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.324784 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.360786 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.808754 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.384787 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.408789 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.808754 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.432790 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.456791 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.812754 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.484793 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.516795 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.812754 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.540796 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.560798 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.816754 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.580799 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.604800 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.816754 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.624801 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.648803 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.820755 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.680804 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.704806 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.824755 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.732807 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.784810 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:39.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.824755 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.816812 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.844814 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.828755 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.872816 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.888816 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.828755 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.912818 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.936819 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.836755 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.964821 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:38.980822 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.836755 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.000823 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.016824 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.840756 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.032825 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.048826 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.844756 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.084828 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.116830 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.844756 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.140831 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.164832 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.848756 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.184834 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.200835 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.852756 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.220836 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.248837 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.852756 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.264838 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.296840 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.856757 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.308841 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.332842 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.860757 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.348843 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.364844 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.860757 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.488851 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.540854 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.864757 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.560855 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.576856 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.864757 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.592857 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.604858 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.868757 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.632860 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.648861 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.872758 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.664862 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.676862 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.872758 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.700864 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.724865 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8128 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.812870 benchmarking_qrc-0.0.4/notebooks/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)    31610 2024-05-20 12:54:36.000000 benchmarking_qrc-0.0.4/notebooks/Benchmarking the role of particle statistis in Quantum Reservoir Computing.ipynb
+-rw-r--r--   0 guillemllodra  (1124) users      (100)    54067 2024-05-22 12:25:29.000000 benchmarking_qrc-0.0.4/notebooks/Practice.ipynb
+-rw-r--r--   0 guillemllodra  (1124) users      (100)    89553 2024-05-22 12:25:32.000000 benchmarking_qrc-0.0.4/notebooks/Practice_solutions.ipynb
+-rw-r--r--   0 guillemllodra  (1124) users      (100)    67515 2024-05-21 09:34:45.000000 benchmarking_qrc-0.0.4/notebooks/Tutorial.ipynb
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.896875 benchmarking_qrc-0.0.4/notebooks/images/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     6765 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/notebooks/images/QRC_diagram.png
+-rw-r--r--   0 guillemllodra  (1124) users      (100)   164367 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/notebooks/images/nn_rc.png
+-rw-r--r--   0 guillemllodra  (1124) users      (100)   124118 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/notebooks/images/rnn_and_rc.png
+-rw-r--r--   0 guillemllodra  (1124) users      (100)    28525 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/notebooks/images/table.png
+-rw-r--r--   0 guillemllodra  (1124) users      (100)       38 2024-05-22 12:55:40.224894 benchmarking_qrc-0.0.4/setup.cfg
+-rw-r--r--   0 guillemllodra  (1124) users      (100)      947 2024-05-22 12:32:36.000000 benchmarking_qrc-0.0.4/setup.py
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:37.876758 benchmarking_qrc-0.0.4/src/
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:39.964879 benchmarking_qrc-0.0.4/src/benchmarking_qrc/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)        0 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc/__init__.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     8981 2024-05-20 11:44:09.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc/hamiltonian.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     9774 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc/measurements.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     5848 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc/reservoir.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)    10692 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc/run_memory_capacity.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)      854 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc/utils.py
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:40.204893 benchmarking_qrc-0.0.4/src/benchmarking_qrc.egg-info/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)      974 2024-05-22 12:55:37.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc.egg-info/PKG-INFO
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     7614 2024-05-22 12:55:37.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc.egg-info/SOURCES.txt
+-rw-r--r--   0 guillemllodra  (1124) users      (100)        1 2024-05-22 12:55:37.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc.egg-info/dependency_links.txt
+-rw-r--r--   0 guillemllodra  (1124) users      (100)       19 2024-05-22 12:55:37.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc.egg-info/requires.txt
+-rw-r--r--   0 guillemllodra  (1124) users      (100)       17 2024-05-22 12:55:37.000000 benchmarking_qrc-0.0.4/src/benchmarking_qrc.egg-info/top_level.txt
+drwxr-xr-x   0 guillemllodra  (1124) users      (100)        0 2024-05-22 12:55:40.184892 benchmarking_qrc-0.0.4/tests/
+-rw-r--r--   0 guillemllodra  (1124) users      (100)      565 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/tests/conftest.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     7629 2024-05-20 12:38:04.000000 benchmarking_qrc-0.0.4/tests/test_hamiltonian.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)    15332 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/tests/test_measurements.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     4373 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/tests/test_memory_capacity.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     3341 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/tests/test_reservoir.py
+-rw-r--r--   0 guillemllodra  (1124) users      (100)     6591 2024-05-20 10:18:40.000000 benchmarking_qrc-0.0.4/tests/utils.py
```

### Comparing `benchmarking-qrc-0.0.3/LICENSE.txt` & `benchmarking_qrc-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_2_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_3_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_4_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_5_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_6_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_7_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_fermion_8_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_2_spin_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_1_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_2_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_3_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_4_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_5_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_6_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_7_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_5_boson_8_ij_1000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_1_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_2_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_3_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_4_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy` & `benchmarking_qrc-0.0.4/data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/notebooks/.ipynb_checkpoints/Tutorial - Quantum Reservoir Computing-checkpoint.ipynb` & `benchmarking_qrc-0.0.4/notebooks/Tutorial.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677973368500712%*

 * *Differences: {"'cells'": "{0: {'id': 'fbd2ddcb', 'source': {insert: [(7, '- Evaluate the performance for "*

 * *            "different particles.\\n'), (9, 'This tutorial is based on the paper [_Benchmarking "*

 * *            'the role of particle statistics in Quantum Reservoir '*

 * *            "Computing_](https://onlinelibrary.wiley.com/doi/full/10.1002/qute.202200100).\\n')], "*

 * *            "delete: [10, 9, 7]}}, 1: {'id': 'c578d6ce', 'source': ['# Run in Google Colab\\n', "*

 * *            "'!pip install benchmarking_qrc --quiet']} […]*

```diff
@@ -1,81 +1,113 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "9c00837d",
+            "id": "fbd2ddcb",
             "metadata": {},
             "source": [
                 "# Tutorial - Benchmarking the role of particle statistis in Quantum Reservoir Computing\n",
                 "\n",
                 "The main goal of this notebook is to familiarize you with Quantum Reservoir Computing (QRC). \n",
                 "\n",
                 "In this tutorial you will learn:\n",
                 "- What is QRC?\n",
                 "- How you can train a QRC to perform a machine learning task?\n",
-                "- Evaluate the performance for different particles\n",
+                "- Evaluate the performance for different particles.\n",
                 "\n",
-                "This tutorial is based on the paper [_Benchmarking the role of particle statistics in Quantum Reservoir Computing_](https://ifisc.uib-csic.es/es/).\n",
-                "<font color='red'> Put arxiv link </font>"
+                "This tutorial is based on the paper [_Benchmarking the role of particle statistics in Quantum Reservoir Computing_](https://onlinelibrary.wiley.com/doi/full/10.1002/qute.202200100).\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "fbf2af80",
+            "id": "c578d6ce",
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Run in Google Colab\n",
+                "!pip install benchmarking_qrc --quiet"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "d386c044",
+            "metadata": {},
+            "outputs": [
+                {
+                    "ename": "ModuleNotFoundError",
+                    "evalue": "No module named 'benchmarking_qrc'",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[0;31mModuleNotFoundError\u001b[0m                       Traceback (most recent call last)",
+                        "Cell \u001b[0;32mIn[2], line 7\u001b[0m\n\u001b[1;32m      4\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mpathlib\u001b[39;00m\n\u001b[1;32m      5\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mscipy\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mlinalg\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m lstsq\n\u001b[0;32m----> 7\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mbenchmarking_qrc\u001b[39;00m \u001b[38;5;28;01mas\u001b[39;00m \u001b[38;5;21;01mqrc\u001b[39;00m\n\u001b[1;32m      8\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mbenchmarking_qrc\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m run_memory_capacity \u001b[38;5;28;01mas\u001b[39;00m mc\n",
+                        "\u001b[0;31mModuleNotFoundError\u001b[0m: No module named 'benchmarking_qrc'"
+                    ]
+                }
+            ],
+            "source": [
                 "import matplotlib.pyplot as plt\n",
                 "import matplotlib.patches as mpatches\n",
                 "import numpy as np\n",
                 "import pathlib\n",
                 "from scipy.linalg import lstsq\n",
                 "\n",
                 "import benchmarking_qrc as qrc\n",
-                "from python_scripts import memory_capacity as mc"
+                "from benchmarking_qrc import run_memory_capacity as mc"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "f76ebf7d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "np.random.seed(1)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "af5b5bc6",
+            "id": "4b23c885",
             "metadata": {},
             "source": [
                 "## Introduction - What is QRC?\n",
                 "\n",
                 "\n",
                 "Quantum Reservoir Computing (QRC) is based on a machine learning technique called Reservoir Computing (RC). RC is specially suited to solve temporal tasks (ex: historical power consumtion, annual temperatures, stock market) because it exploits the dynamics of a nonlinear system called reservoir. The intuition behind RC is to map an input into a high-dimensional space (reservoir) that facilittes the separtion of the initial data. After this mapping, the output layer is trained to extract valuable reservoir features and mathc the expected output.\n",
                 "\n",
                 "There are other machine learning techniques like Recurrent Neural Networks, which its dynamics also exploits the fact that the information can remain stored in the network for a finite amount of time. This characteristic is often defined as memory, making RNN and RC suitable to process sequential data. However, RNN feedback loops (see Figure) can be extremely hard to train. In constrat, RC only train the weights in the output layer, which leads to an easy training and fast learning because backpropagation is not need to optimize weights.\n",
                 "\n",
-                "<img src=\"images/rnn_and_rc.png\" width=\"700\" height=\"300\">\n",
+                "<img src=\"./images/rnn_and_rc.png\" alt=\"drawing\"/>\n",
                 "\n",
                 "As shown in the above Figure the architecture of RNN looks rather complex compare to RC with only three layers. To ensure a proper performance the reservoir must satisfy several requirements:  \n",
                 "- **Convergence** or **Echo State Property**: The result obtained in the output layer must be totally independent of the initial conditions of the reservoir.\n",
                 "- **Nonlinearity**: The reservoir must provide a nonlinear transformation with respect to the inputs. In this way, most of the computational cost can be outsourced to the reservoir while the output layer can be taken as a linear funtion, which its easier to train. \n",
                 "- **Fading memory**: The dynamics in the reservoir is able to retain memory of present and past inputs, but it also able to dissipate the information for irrelevant inputs very far in the past.\n",
                 "- **Separability**: Different inputs sequence should produce different outputs.\n",
                 "\n",
-                "All these features (complex dynamics and high-dimensional space) can be enhanced if we move to the field of Quantum Reservoir Computing (QRC). A major advantatge lies in the fact that quantum computers can store exponentially more information in the Hilbert space, where quantum particles reside, than classical computers. In addition, QRC is suitable for Noisy intermediate-scale quantum (NISQ) since it doesn't need perfect dynamics to perform computation. As shown, in the seminal work of Nakajima et. al <font color='red'> ref Nakajima 2017 paper </font>, a QRC of 5-7 qubits exhibits similar performance to an echo state network (classical method) of 100-500 nodes.\n",
+                "All these features (complex dynamics and high-dimensional space) can be enhanced if we move to the field of Quantum Reservoir Computing (QRC). A major advantatge lies in the fact that quantum computers can store exponentially more information in the Hilbert space, where quantum particles reside, than classical computers. In addition, QRC is suitable for Noisy intermediate-scale quantum (NISQ) since it doesn't need perfect dynamics to perform computation. As shown, in the [seminal work](https://arxiv.org/abs/1602.08159) of Nakajima et. al, a QRC of 5-7 qubits exhibits similar performance to an echo state network (classical method) of 100-500 nodes.\n",
                 "\n",
                 "The standard algorithm of RC/QRC can be explained in three steps as shown in the following Figure:\n",
                 "- **Input**: Injecting data into an ancilla particle, which is coupled to the reservoir. In this step, the low-dimensional input data is mapped into a high-dimensional dynamical system. \n",
                 "- **Reservoir**: Let the reservoir evolve for a certain period of time following its natural dynamics. At each iteration, a new input will be injected driving the dynamics. \n",
-                "- **Output**: Extract features from the reservoir. Then, a linear combination of all the features will be optimized to reproduce the desired target.\n",
+                "- **Output**: Extract features from the reservoir using a set of observables. Then, a linear combination of all the features will be optimized to reproduce the desired target.\n",
                 "\n",
                 "In the next section, we will introduce the mathematical formalism describing each step.\n",
                 "\n",
-                "<img src=\"images/QRC_diagram.png\" width=\"600\" height=\"200\">\n",
+                "<img src=\"./images/QRC_diagram.png\" alt=\"drawing\"/>\n",
                 "\n",
-                "Although different types of systems have been proposed as quantum reservoirs, the role of the statistics has not been established yet. In this work, we have assessed the ability of different particles (fermions, bosons and spins) to store information from past inputs. This has allowed us to find two key ingredients to take into account for future QRC projects. Firstly, fermions are better information carriers than spins due to the anticommutation rules. Secondly, under a tailored input injection strategy bosons can exploit the abundance of degrees of freedom in its Hilbert space and improve its ability to store information. For more details, check out the article in this link <font color='red'> Put arxiv link/or github link to the paper. </font>"
+                "Although different types of systems have been proposed as quantum reservoirs, the role of the statistics has not been established yet. In this work, we have assessed the ability of different particles (fermions, bosons and spins) to store information from past inputs. This has allowed us to find two key ingredients to take into account for future QRC projects. Firstly, fermions are better information carriers than spins due to the anticommutation rules. Secondly, under a tailored input injection strategy bosons can exploit the abundance of degrees of freedom in its Hilbert space and improve its ability to store information. For more details, check out the article in this [link](https://onlinelibrary.wiley.com/doi/full/10.1002/qute.202200100)."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "862a407c-0b35-4dfd-b876-42ac48cabbbb",
+            "id": "5413a1e2",
             "metadata": {},
             "source": [
                 "### The task\n",
                 "\n",
                 "In this section, we will briefly introduce the machine learning task that the QRC is going to perform and the metric to quantify the results.\n",
                 "\n",
                 "Our objective is to quantify the how well the quantum system can recover past information. So, we will inject a sequence of random inputs ($u_k$) into the reservoir and the system will be trained to match a target function\n",
@@ -104,40 +136,38 @@
                 "$$ MC = \\frac{Cov^2(y,\\hat{y})}{\\sigma^2(y)\\sigma^2(\\hat{y})} $$\n",
                 "\n",
                 "where $\\sigma(y)$ and $\\sigma(\\hat{y})$ are the standard deviation of the reservoir and target outputs, respectively. The $MC$ may look familiar to some readers because it is simply the Pearson correlation coefficient to the power 2. This implies that the MC is bounded between 0 (there is no correlation between $y$ and $\\hat{y}$) and 1 (the system has been able to fully recover the target function)."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8ced6201",
+            "id": "abc55e3d",
             "metadata": {},
             "source": [
                 "## Hands-on approach - How to train a QRC \n",
                 "\n",
                 "In this section we explain the mathematical formalism to train a Quantum Reservoir with a fermionic reservoir of only two particles to visualize what the code is actually doing. Later on, we will increase the reservoir size up to 4 fermions. The following table summarizes all the equations that we are going to introduce:\n",
                 "\n",
-                "\n",
-                "<img src=\"images/table.png\" width=\"350\" height=\"600\">"
+                "<img src=\"../notebooks/images/rnn_and_rc.png\" alt=\"drawing\"/>\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "fee07344-018c-4ca4-b225-c11548a247ff",
+            "id": "e719d57f",
             "metadata": {},
             "source": [
                 "### Step 0: Setting up the system\n",
-                " \n",
                 "\n",
-                "The first step is to define the reservoir initial conditions, namely define a the initial state of a quantum many-body system. In this case the reservoir is build with 2 fermions in the ground state $\\lvert 0 \\rangle$ using the function `dm_zero_states`. Since fermions are a two-level systems ($\\lvert 0 \\rangle$, $\\lvert 1 \\rangle$) the Hilbert dimensions of fermions is always 2 (`dim_fermion=2`)."
+                "The first step is to define the reservoir initial conditions, namely define a the initial state of a quantum many-body system. In this case the reservoir is build with 2 fermions in the ground state $\\lvert 0 \\rangle$ using the function `initial_state`. Since fermions are a two-level systems ($\\lvert 0 \\rangle$, $\\lvert 1 \\rangle$) the Hilbert dimensions of fermions is always 2 (`dim_fermion=2`)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "036ecdd1",
+            "id": "2f40fb62",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[1., 0., 0., 0.],\n",
                             "       [0., 0., 0., 0.],\n",
@@ -157,28 +187,28 @@
                 "\n",
                 "initial_reservoir = qrc.reservoir.initial_state(n_fermions, dim_fermion)\n",
                 "initial_reservoir"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2dbfa3a5",
+            "id": "ce491793",
             "metadata": {},
             "source": [
                 "To process information particles must interact with each other. The interaction strenght between particles $i$ and $j$ is defined by the parameter $J_{ij}$ and the natural dynamics of the system is ruled by the following quadratic Hamiltonian\n",
                 "\n",
                 "$$ H = \\sum_{i,j=1}^{N}J_{ij}a_{i}^{\\dagger}a_{j} $$\n",
                 "\n",
                 "This Hamiltonian encodes the onsite interation ($J_{ii}$) and the coupling iterations ($J_{ij}$) among all particles.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "23cd72bc",
+            "id": "b31bb5c1",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "matrix([[0.  +0.j, 0.  +0.j, 0.  +0.j, 0.  +0.j],\n",
                             "        [0.  +0.j, 0.72+0.j, 0.  +0.j, 0.  +0.j],\n",
@@ -198,28 +228,28 @@
                 "fermionic_hamiltonian = qrc.hamiltonian.quadratic_op(n_fermions, is_bosonic=False, dimensions=dim_fermion, coefficients=J_ij)\n",
                 "\n",
                 "np.around(fermionic_hamiltonian.todense(), 2)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "369ffb56",
+            "id": "9e5a00ab",
             "metadata": {},
             "source": [
                 "As a last ingredient to simulate the dynamics of the reservoir, we need the evolution operator ($e^{-iH\\Delta t}$) to compute the next state of reservoir ($\\rho(t)$). \n",
                 "\n",
                 "$$ \\rho(t_f) = e^{-iH\\Delta t}\\rho(t_i)e^{iH\\Delta t}$$\n",
                 "\n",
                 "The $\\Delta t$ quantifies how much time we let system evolve. By default, $\\Delta t = 10$ because we want that the injected information in the system is spread through the whole system."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "ca89bda8",
+            "id": "6ee92d43",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 1.  +0.j  ,  0.  +0.j  ,  0.  +0.j  ,  0.  +0.j  ],\n",
                             "       [ 0.  +0.j  ,  0.61-0.8j ,  0.  -0.j  ,  0.  +0.j  ],\n",
@@ -235,15 +265,15 @@
             "source": [
                 "fermionic_evolution = qrc.hamiltonian.get_evolution_op(fermionic_hamiltonian, dt=10)\n",
                 "np.around(fermionic_evolution, 2)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "de6ce1d5",
+            "id": "b99cc711",
             "metadata": {},
             "source": [
                 "### Step 1: Echo state property (wash out)\n",
                 "\n",
                 "To avoid any possible effect of the initial conditions of the reservoir we always start with the wash out step before training the system. This step consists in injecting a set of inputs until the initial conditions become irrelevant. The amount of iterations needed to wash out the initial conditions can be found in Figure 2 of the paper.\n",
                 "\n",
                 "To encode classical data ($u_k$) into a quantum state ($\\lvert \\psi \\rangle$) we can use `get_input_state`.\n",
@@ -252,15 +282,15 @@
                 "\n",
                 "For fermions we need to inject 3000 inputs to erase the initial conditions according to the Figure 2. However, it is possible that for certain values of $J_{ij}$ the numbers of iterations required is lower. Notice that for fermions the excited level is obvioulsy $\\lvert 1 \\rangle$, but for bosons the excited level could be $\\lvert 1 \\rangle$, $\\lvert 2 \\rangle$ ... $\\lvert n \\rangle$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "d8501e79",
+            "id": "b5583242",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0.54984777],\n",
                             "       [0.83526488]])"
@@ -279,26 +309,26 @@
                 "excited_state=1\n",
                 "input_state = qrc.reservoir.get_input_state(wash_out_signals[0], dim_fermion, excited_state)\n",
                 "input_state"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "de60c716",
+            "id": "4c3e58f7",
             "metadata": {},
             "source": [
                 "Then, we can inject this quantum state into the first particle of the reservoir with `insert_input`. This function computes the tensor product between the input state, $\\rho_{1, k}^{(e)}=\\lvert \\psi_k^{(e)} \\rangle \\langle \\psi_k^{(e)} \\lvert$, and all particles of the reservoir except the first one, ${\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\}$\n",
                 "\n",
                 "$$ \\rho(k\\Delta t)= \\rho_{1, k}^{(e)} \\otimes {\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\} $$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "15da2cc7",
+            "id": "75fcece4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[0.30233257, 0.        , 0.45926854, 0.        ],\n",
                             "       [0.        , 0.        , 0.        , 0.        ],\n",
@@ -314,50 +344,50 @@
             "source": [
                 "reservoir_with_input = qrc.reservoir.insert_input(input_state, initial_reservoir)\n",
                 "reservoir_with_input"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ec7127e4",
+            "id": "61f8436e",
             "metadata": {},
             "source": [
                 "To let the information spread through the whole system we let the system evolve following the quantum dynamics of a closed system, as shown in the table above.\n",
                 "\n",
                 "\n",
                 "$$ \\rho\\left(k\\Delta t\\right)=e^{-iH\\Delta t}\\left[\\rho_{1,k}^{(e)}\\otimes {\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\} \\right]e^{iH\\Delta t} $$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "458d8d0c",
+            "id": "031f9222",
             "metadata": {},
             "outputs": [],
             "source": [
                 "reservoir = qrc.reservoir.evolve(reservoir_with_input, fermionic_evolution)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9430a0a2",
+            "id": "459a20b9",
             "metadata": {},
             "source": [
                 "So, at each iteration the reservoir will change following these 3 steps:\n",
                 "- Encoding classical data into a quantum state $\\Longrightarrow \\lvert \\psi_k^{(e)} \\rangle$.\n",
                 "- Injecting the quantum state into the reservoir $\\Longrightarrow \\rho(k)$.\n",
                 "- Evolving the reservoir $\\Longrightarrow  \\rho(k\\Delta t)$.\n",
                 "\n",
                 "To avoid calling the previous three functions at each iteration, we have packed the previous 3 points in a single function call `cptp_map` which will generate a reservoir state for each injected input. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "99d6fc81",
+            "id": "78fb94f3",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 0.191+0.j   , -0.   +0.j   , -0.203-0.337j,  0.   +0.001j],\n",
                             "       [-0.   -0.j   ,  0.   +0.j   ,  0.   +0.001j, -0.   -0.j   ],\n",
@@ -377,15 +407,15 @@
                 "# Take the last reservoir from the previous list\n",
                 "washed_reservoir = reservoirs[-1]\n",
                 "np.around(washed_reservoir, 3)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e3b5f16f",
+            "id": "2dad0293",
             "metadata": {},
             "source": [
                 "### Step 2: Data prepartion\n",
                 "\n",
                 "Once we have a `washed_reservoir` you can start training the reservoir to perform any typical supervise machine learning task. In a real world scenario you will have a dataset with a time-series (ex: temperatures over several years, stock market, etc.).\n",
                 "\n",
                 "In our case, we are interested in benchmarking the ability to store past inputs, so a random sequence of number is good enough for our porpuses. Let's start by setting some parameters, as the `delay`, `train_time` and `test_time`.\n",
@@ -396,38 +426,38 @@
                 "_Remember that we have already set a seed for generating the coefficients $J_{ij}$, so the following results are totally reproducible_.\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "id": "f102d174",
+            "id": "7a4f8670",
             "metadata": {},
             "outputs": [],
             "source": [
                 "delay = 1\n",
                 "train_time, test_time = 10, 10\n",
                 "\n",
                 "# Prepare random data\n",
                 "train_signals = np.random.uniform(low=0, high=1, size=train_time + delay)\n",
                 "test_signals = np.random.uniform(low=0, high=1, size=test_time + delay)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d405454f",
+            "id": "6fab93f3",
             "metadata": {},
             "source": [
                 "Let's also prepare the input with the function `get_inputs`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "id": "eea016e2",
+            "id": "c9e57c50",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "inputs = [0.96 0.56 0.65 0.27 0.95 0.67 0.67 0.01 0.85 0.78 0.74 0.16 0.72 0.1\n",
@@ -441,24 +471,24 @@
                 "test_inputs = mc.get_inputs(test_signals, delay)\n",
                 "inputs = np.concatenate((train_inputs, test_inputs))\n",
                 "print(\"inputs =\", np.around(inputs, 2))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "31b23cbd",
+            "id": "6b3c13ed",
             "metadata": {},
             "source": [
                 "As well, the function `get_targets` generates the target for linear task when $\\hat{y}=u_k$ and for the non-linear task $\\hat{y}=u_k^q$ ($q \\neq 1$)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
-            "id": "cef6d00a",
+            "id": "4f80a288",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "train_targets = [0.98 0.96 0.56 0.65 0.27 0.95 0.67 0.67 0.01 0.85]\n"
@@ -470,72 +500,72 @@
                 "train_targets = mc.get_targets(train_signals, delay, degree=1)\n",
                 "test_targets = mc.get_targets(test_signals, delay, degree=1)\n",
                 "print(\"train_targets =\", np.around(train_targets, 2))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "dbb64d70",
+            "id": "45e6ea52",
             "metadata": {},
             "source": [
                 "### Step 3: Enconding data into a high dimensional space\n",
                 "\n",
                 "The following line it should look familiar:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "id": "c796a754",
+            "id": "5a86aa1e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "reservoirs = list(qrc.reservoir.cptp_map(inputs, washed_reservoir, fermionic_evolution, dim_fermion, excited_state))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "22fd3963",
+            "id": "7459017f",
             "metadata": {},
             "source": [
                 "Exactly, this function is used to generate a sequence of reservoir states (just as in the wash out step). The imporant thing to remember is that each of these reservoir states contain some information from the past inputs. \n",
                 "\n",
                 "Now, we would like to extract some information ($x_j$) from the quantum system by performing some measurements.   \n",
                 "\n",
                 "$$ x_{j}\\left(k\\Delta t\\right)={\\rm Tr}\\left[O_{j}\\rho\\left(u_k\\Delta t\\right)\\right]   \\qquad  (1)$$\n",
                 "\n",
                 "To do that, we need to define a set of observables. For this tutorial we will use observables of the form $a_i^\\dagger a_j$. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
-            "id": "94da0e5b",
+            "id": "500bacc6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "obs = qrc.measurements.observables(\"fermion\", n_fermions, dim_fermion, \"ij\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9585a761",
+            "id": "3e84bea7",
             "metadata": {},
             "source": [
                 "In the following you can notice that `obs` is a list that contain the diagonal a non-diagonal observables:\n",
                 "\n",
                 "- $a_0^\\dagger a_0$\n",
                 "- $a_1^\\dagger a_1$\n",
                 "- $a_0^{\\dagger}a_1 + a_1^{\\dagger}a_0$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
-            "id": "377eb960",
+            "id": "e5d12fd9",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
@@ -549,15 +579,15 @@
                 "# diagonal observable: adag_0 a_0\n",
                 "print(obs[0])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
-            "id": "60823ee2",
+            "id": "d16cf664",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
@@ -571,15 +601,15 @@
                 "# diagonal observable: adag_1 a_1 \n",
                 "print(obs[2])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
-            "id": "382b44cc",
+            "id": "3db8b906",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
@@ -592,15 +622,15 @@
             "source": [
                 "# non-diagonal observable: adag_0 a_1 + adag_1 a_0\n",
                 "print(obs[1])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "87cb27be",
+            "id": "eb22062e",
             "metadata": {},
             "source": [
                 "Typically, conventional neural networks (NN) algorithms use a nonlinear function ($f$) like the ReLU or sigmoid to fit the input data ($x$)\n",
                 "\n",
                 "$$y_{NN}=f(\\rm{wx}+\\rm{b})$$\n",
                 "\n",
                 "where $y$ is the output of the NN and $w$, $b$ is the weights and bias that the network will optimize to fit the target data.  \n",
@@ -627,15 +657,15 @@
                 "\n",
                 "To compute the previous matrix, you can use the `get_features` function."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
-            "id": "5ae1a939",
+            "id": "3551c323",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([[ 0.039,  0.001,  0.001,  1.   ],\n",
                             "       [ 0.443,  0.   ,  0.001,  1.   ],\n",
@@ -669,30 +699,30 @@
                 "\n",
                 "# Approximate dataset values up to 3 decimals\n",
                 "np.around(dataset, 3)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "59de76b3",
+            "id": "3d1d4dfb",
             "metadata": {},
             "source": [
                 "### Step 4: Optimizing weights\n",
                 "\n",
                 "The optimal weights are computing minimizing the 2-norm error between the target values $\\hat{y}$ and the actual predictions $y=XW$ \n",
                 "\n",
                 "$$ arg\\min_{W} |\\hat{y}-XW|.$$\n",
                 "\n",
                 "In the well-known package `scipy` there is a specific function to optimize linear regression problems called `lstsq`. But before we split the dataset into train and test to later evaluate the results and check if the parameters used overfit the data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
-            "id": "f245c39f",
+            "id": "31d14d7b",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "optimal weights=[ 2.3400000e-01  2.1895000e+01 -4.8755787e+04  2.8595000e+01]\n"
@@ -707,15 +737,15 @@
                 "opt_weights, _, _, _ = lstsq(train_X, train_targets)\n",
                 "\n",
                 "print(f\"optimal weights={np.around(opt_weights, 3)}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "67506a75",
+            "id": "fa770239",
             "metadata": {},
             "source": [
                 "### Step 5: Evaluating the memory capacity\n",
                 "\n",
                 "The memory capacity ($MC$) is a metric that quantifies the linear correlation between two vectors. If both vectors are identical $MC=1$, if there is no linear correlation $MC=0$.\n",
                 "\n",
                 "$$MC=\\frac{Cov^2(\\hat{y}, y)}{\\sigma^2(\\hat{y})\\sigma^2(y)} $$\n",
@@ -723,15 +753,15 @@
                 "The algorithm predictions with the best weights are:\n",
                 "$$ y_{train}^{\\, p}=X_{train}w_{opt}$$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
-            "id": "e8237b60",
+            "id": "67278344",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "train predictions= [0.701 0.798 0.656 0.601 0.479 0.605 0.733 0.809 0.641 0.543]\n"
@@ -741,25 +771,25 @@
             "source": [
                 "train_predictions = np.matmul(train_X, opt_weights)\n",
                 "print(\"train predictions=\", np.around(train_predictions, 3))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cfdc9f1e",
+            "id": "96951c6c",
             "metadata": {},
             "source": [
                 "We can also compute the predictions on the test dataset `test_X`. \n",
                 "$$ y_{pred}^{test} = X_{test}w_{opt}$$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
-            "id": "cf2145b4",
+            "id": "786a226a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "test predictions= [0.436 0.531 0.508 0.688 0.649 0.713 0.442 0.362 0.409 0.404]\n"
@@ -769,24 +799,24 @@
             "source": [
                 "test_predictions = np.matmul(test_X, opt_weights)\n",
                 "print(\"test predictions=\", np.around(test_predictions, 3))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0336dd05",
+            "id": "117aea8f",
             "metadata": {},
             "source": [
                 "Finally, we can measure the memory capacity."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 21,
-            "id": "c21fbd72",
+            "id": "3c119e41",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Train MC=0.113\n"
@@ -797,15 +827,15 @@
                 "train_mc = mc.memory_capacity(train_predictions, train_targets)\n",
                 "print(f\"Train MC={np.around(train_mc, 3)}\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
-            "id": "34539b20",
+            "id": "bf15318e",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Test MC=0.015\n"
@@ -815,42 +845,42 @@
             "source": [
                 "test_mc = mc.memory_capacity(test_predictions, test_targets)\n",
                 "print(f\"Test MC={np.around(test_mc, 3)}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1cb12215",
+            "id": "b4a98128",
             "metadata": {},
             "source": [
                 "Cleary, this results by no means great. The memory capacity is quite low and the algorithm is overfitting the data. To get good results the hyperparameters that must be optimized are:\n",
                 "\n",
                 "- Number of particles \n",
                 "- Training data\n",
                 "- $\\Delta t$.\n",
                 "\n",
                 "The Hamiltonian coefficients $J_{ij}$ also play an important role on how the informtion is spread through the system and it will be the next topic we are going to explore.\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "03eed7be",
+            "id": "7ea41962",
             "metadata": {},
             "source": [
                 "### Summary\n",
                 "\n",
                 "In this tutorial, you have learnt how to train a QRC to perform a supervise task. \n",
                 "\n",
                 "If you want to play around (try different reservoir sizes, particles, train times, etc) we have introudce all the steps shown above in a function called `main`. So, there is no need to re-run previous cells, just set the parameters you are curios about and find out if the performance is improved or not."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
-            "id": "7851d951",
+            "id": "46b9ed06",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Parameters for fermions \n",
                 "\n",
                 "# Reservoir parameters\n",
                 "n_particles = 4 # 2, 3, .., n\n",
@@ -867,15 +897,15 @@
                 "train_time = 1200\n",
                 "test_time = 300\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
-            "id": "6c39d168",
+            "id": "ddf4e10a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Reservoir with 4 fermions:\n",
@@ -902,24 +932,24 @@
                 "print(f\"Reservoir with {n_particles} {operator}s:\")\n",
                 "print(f\"\\tTrain MC={np.around(train_mc, 3)}\")\n",
                 "print(f\"\\tTest  MC={np.around(test_mc, 3)}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3661bae0",
+            "id": "2f25cb6a",
             "metadata": {},
             "source": [
                 "To see the perfomance of spins write `operator=\"spin\"`.  _Remember that as shown in the Figure 2 of the paper the wash time for spins is lower than for fermions_."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 25,
-            "id": "02c9dfed",
+            "id": "0ec9a0fd",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Reservoir with 4 spins:\n",
@@ -950,23 +980,23 @@
                 "print(f\"Reservoir with {n_particles} {operator}s:\")\n",
                 "print(f\"\\tTrain MC={np.around(train_mc, 3)}\")\n",
                 "print(f\"\\tTest  MC={np.around(test_mc, 3)}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a5074c22",
+            "id": "c03290c8",
             "metadata": {},
             "source": [
                 "In particular, for this configuration of parameters spins perform better than fermions. But as shown in our paper fermions will in general have better perfomance than spins. In the last section, of the tutorial we reproduce the Figure 3, in which its shown that fermions outperform spins."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a035b4ba",
+            "id": "48754aee",
             "metadata": {},
             "source": [
                 "## Extra: Bosonic reservoir\n",
                 "\n",
                 "The main goal of the tutorial was to explain how QRC work. So, in the previous section we explained the basic componets of this machine learning framework using fermions. In this section, there isn't any new concept related to QRC, we will only explain a few key parameters to build a bosonic reservoir.\n",
                 "\n",
                 "For bosons, there are two new hyperparameters that we can modify: \n",
@@ -981,15 +1011,15 @@
                 "\n",
                 "_If for instance you use `excited_state=2` and `dimensions=3` the particles in the reservoir will be a poor approximation to the actual bosons_."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 32,
-            "id": "ffb4da5b",
+            "id": "39c956f5",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Reservoir with 4 bosons:\n",
@@ -1023,28 +1053,28 @@
                 "print(f\"Reservoir with {n_particles} {operator}s:\")\n",
                 "print(f\"\\tTrain MC={np.around(train_mc, 3)}\")\n",
                 "print(f\"\\tTest  MC={np.around(test_mc, 3)}\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bf8afab2",
+            "id": "d3411f0a",
             "metadata": {},
             "source": [
                 "## Extra: Reproducing Fig. 3\n",
                 "\n",
                 "\n",
                 "Previous results are not statistical relevant since the performance is based one only one realization of $J_{ij}$.  However, it can be a bit time-consuming to run these code from `seed=1`to `seed=1000` to reproduce exactly the same results as in Figure 3. For this reason, we have shared this information in the `data` folder. Now, we will simple upload and plot the results of Figure 3.\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 26,
-            "id": "53d36d37",
+            "id": "d66a4651",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def get_path(foldername, test_data):\n",
                 "    \"\"\"Generates the path to train or test data location\"\"\"\n",
                 "    REPO = pathlib.Path().cwd().parent\n",
                 "    data = \"test\" if test_data else \"train\"\n",
@@ -1072,16 +1102,16 @@
                 "    plt.grid()\n",
                 "    background = mpatches.Patch(color=color, alpha=0.6)\n",
                 "    return tick, background"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
-            "id": "43a822c1",
+            "execution_count": 27,
+            "id": "55f06ad9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Parameters (change the foldername to upload spin or boson data)\n",
                 "delays = [1, 2, 3, 4, 5, 6, 7, 8]\n",
                 "foldername = \"4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)\"\n",
                 "test_data = True\n",
@@ -1097,21 +1127,21 @@
                 "    quantiles_1[idx] = q1\n",
                 "    quantiles_2[idx] = q2\n",
                 "    quantiles_3[idx] = q3"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
-            "id": "a6d51c67",
+            "execution_count": 28,
+            "id": "211af89e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -1124,39 +1154,31 @@
                 "    delays,\n",
                 "    quantiles_2, \n",
                 "    fmt=\"o--\",\n",
                 "    color=\"#1a9641\",\n",
                 "    error_bars=np.array([quantiles_1, quantiles_3])\n",
                 ")"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "141dbce4-829e-485f-8767-825506eb4b8d",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "q_reservoir",
+            "display_name": "openfermion",
             "language": "python",
-            "name": "q_reservoir"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.12.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `benchmarking-qrc-0.0.3/notebooks/.ipynb_checkpoints/Tutorial-checkpoint.ipynb` & `benchmarking_qrc-0.0.4/notebooks/Practice.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7853078451452827%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Hands-on session on Quantum reservoir computing\\n'), "*

 * *            '(2, \'During this lecture we are going to use the library "benchmarking_qrc" to learn '*

 * *            "about quantum reservoir computing. But, we will also use numpy and matplotlib.\\n'), "*

 * *            "(4, 'The goal of this session is to complete 2 exercises.\\n'), (5, '1. Plot the echo "*

 * *            "state property.\\n'), (6, '2. Evaluate the model performance to recall past "*

 * *            "input […]*

```diff
@@ -1,1173 +1,883 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "9c00837d",
             "metadata": {},
             "source": [
-                "# Tutorial - Benchmarking the role of particle statistis in Quantum Reservoir Computing\n",
+                "# Hands-on session on Quantum reservoir computing\n",
                 "\n",
-                "The main goal of this notebook is to familiarize you with Quantum Reservoir Computing (QRC). \n",
+                "During this lecture we are going to use the library \"benchmarking_qrc\" to learn about quantum reservoir computing. But, we will also use numpy and matplotlib.\n",
                 "\n",
-                "In this tutorial you will learn:\n",
-                "- What is QRC?\n",
-                "- How you can train a QRC to perform a machine learning task?\n",
-                "- Evaluate the performance for different particles\n",
-                "\n",
-                "This tutorial is based on the paper [_Benchmarking the role of particle statistics in Quantum Reservoir Computing_](https://ifisc.uib-csic.es/es/).\n",
-                "<font color='red'> Put arxiv link </font>"
+                "The goal of this session is to complete 2 exercises.\n",
+                "1. Plot the echo state property.\n",
+                "2. Evaluate the model performance to recall past inputs."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "id": "13f44615",
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Run in Google Colab\n",
-                "!pip install git+https://github.com/quantumlib/OpenFermion-FQE"
+                "# Only for local use\n",
+                "import os\n",
+                "import sys\n",
+                "\n",
+                "repo_path = os.path.dirname(os.getcwd())\n",
+                "package_path = repo_path + \"/src\"\n",
+                "sys.path.append(package_path)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
-            "id": "fbf2af80",
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from collections import deque\n",
+                "\n",
                 "import matplotlib.pyplot as plt\n",
-                "import matplotlib.patches as mpatches\n",
                 "import numpy as np\n",
-                "import pathlib\n",
                 "from scipy.linalg import lstsq\n",
                 "\n",
                 "import benchmarking_qrc as qrc\n",
-                "from benchmarking_qrc import run_memory_capacity as mc"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "af5b5bc6",
-            "metadata": {},
-            "source": [
-                "## Introduction - What is QRC?\n",
-                "\n",
-                "\n",
-                "Quantum Reservoir Computing (QRC) is based on a machine learning technique called Reservoir Computing (RC). RC is specially suited to solve temporal tasks (ex: historical power consumtion, annual temperatures, stock market) because it exploits the dynamics of a nonlinear system called reservoir. The intuition behind RC is to map an input into a high-dimensional space (reservoir) that facilittes the separtion of the initial data. After this mapping, the output layer is trained to extract valuable reservoir features and mathc the expected output.\n",
-                "\n",
-                "There are other machine learning techniques like Recurrent Neural Networks, which its dynamics also exploits the fact that the information can remain stored in the network for a finite amount of time. This characteristic is often defined as memory, making RNN and RC suitable to process sequential data. However, RNN feedback loops (see Figure) can be extremely hard to train. In constrat, RC only train the weights in the output layer, which leads to an easy training and fast learning because backpropagation is not need to optimize weights.\n",
-                "\n",
-                "<img src=\"images/rnn_and_rc.png\" width=\"700\" height=\"300\">\n",
-                "\n",
-                "As shown in the above Figure the architecture of RNN looks rather complex compare to RC with only three layers. To ensure a proper performance the reservoir must satisfy several requirements:  \n",
-                "- **Convergence** or **Echo State Property**: The result obtained in the output layer must be totally independent of the initial conditions of the reservoir.\n",
-                "- **Nonlinearity**: The reservoir must provide a nonlinear transformation with respect to the inputs. In this way, most of the computational cost can be outsourced to the reservoir while the output layer can be taken as a linear funtion, which its easier to train. \n",
-                "- **Fading memory**: The dynamics in the reservoir is able to retain memory of present and past inputs, but it also able to dissipate the information for irrelevant inputs very far in the past.\n",
-                "- **Separability**: Different inputs sequence should produce different outputs.\n",
+                "from benchmarking_qrc import run_memory_capacity as mc\n",
                 "\n",
-                "All these features (complex dynamics and high-dimensional space) can be enhanced if we move to the field of Quantum Reservoir Computing (QRC). A major advantatge lies in the fact that quantum computers can store exponentially more information in the Hilbert space, where quantum particles reside, than classical computers. In addition, QRC is suitable for Noisy intermediate-scale quantum (NISQ) since it doesn't need perfect dynamics to perform computation. As shown, in the seminal work of Nakajima et. al <font color='red'> ref Nakajima 2017 paper </font>, a QRC of 5-7 qubits exhibits similar performance to an echo state network (classical method) of 100-500 nodes.\n",
-                "\n",
-                "The standard algorithm of RC/QRC can be explained in three steps as shown in the following Figure:\n",
-                "- **Input**: Injecting data into an ancilla particle, which is coupled to the reservoir. In this step, the low-dimensional input data is mapped into a high-dimensional dynamical system. \n",
-                "- **Reservoir**: Let the reservoir evolve for a certain period of time following its natural dynamics. At each iteration, a new input will be injected driving the dynamics. \n",
-                "- **Output**: Extract features from the reservoir. Then, a linear combination of all the features will be optimized to reproduce the desired target. <font color='red'> Cambiar la f de Readout por observables </font>\n",
-                "\n",
-                "In the next section, we will introduce the mathematical formalism describing each step.\n",
-                "\n",
-                "<img src=\"images/QRC_diagram.png\" width=\"600\" height=\"200\">\n",
-                "\n",
-                "Although different types of systems have been proposed as quantum reservoirs, the role of the statistics has not been established yet. In this work, we have assessed the ability of different particles (fermions, bosons and spins) to store information from past inputs. This has allowed us to find two key ingredients to take into account for future QRC projects. Firstly, fermions are better information carriers than spins due to the anticommutation rules. Secondly, under a tailored input injection strategy bosons can exploit the abundance of degrees of freedom in its Hilbert space and improve its ability to store information. For more details, check out the article in this link <font color='red'> Put arxiv link/or github link to the paper. </font>"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "862a407c-0b35-4dfd-b876-42ac48cabbbb",
-            "metadata": {},
-            "source": [
-                "### The task\n",
-                "\n",
-                "In this section, we will briefly introduce the machine learning task that the QRC is going to perform and the metric to quantify the results.\n",
-                "\n",
-                "Our objective is to quantify the how well the quantum system can recover past information. So, we will inject a sequence of random inputs ($u_k$) into the reservoir and the system will be trained to match a target function\n",
-                "\n",
-                "$$ \\hat{y}_k = u_{k-\\tau}$$\n",
-                "\n",
-                "where $\\tau$ is the delay between the input and target.\n",
-                "\n",
-                "<div class=\"alert alert-block alert-info\">\n",
-                "    <b>Example:</b>    \n",
+                "def check_solution(solution, exp_solution):\n",
                 "    \n",
-                "Given an input sequence:\n",
-                "$$ u = (0.2, 0.3, 0.4, 0.5) $$\n",
-                "\n",
-                "The target function after a delay, $\\tau=1$ is:\n",
-                "\n",
-                "$$ \\hat{y} = (0.1, 0.2, 0.3, 0.4) $$\n",
-                "\n",
-                "But the reservoir after the training procedure may output a different result:\n",
-                "\n",
-                "$$ y = (0.11, 0.19, 0.3, 0.398) $$\n",
-                "</div>\n",
-                "\n",
-                "Let us introduce the metric to meause the system memory. The memory capacity is a standard measure of memory in recurrent neural network and is defined as:\n",
-                "\n",
-                "$$ MC = \\frac{Cov^2(y,\\hat{y})}{\\sigma^2(y)\\sigma^2(\\hat{y})} $$\n",
-                "\n",
-                "where $\\sigma(y)$ and $\\sigma(\\hat{y})$ are the standard deviation of the reservoir and target outputs, respectively. The $MC$ may look familiar to some readers because it is simply the Pearson correlation coefficient to the power 2. This implies that the MC is bounded between 0 (there is no correlation between $y$ and $\\hat{y}$) and 1 (the system has been able to fully recover the target function)."
+                "    if solution.shape == exp_solution.shape:\n",
+                "        if np.all(solution == exp_solution):\n",
+                "            print(\"Correct!\")\n",
+                "        else:\n",
+                "            print(\"Try again!\")\n",
+                "    else:\n",
+                "        print(\"Try again!\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8ced6201",
             "metadata": {},
             "source": [
-                "## Hands-on approach - How to train a QRC \n",
+                "### Exercise 0 - Define density matrix and hamiltonian\n",
                 "\n",
-                "In this section we explain the mathematical formalism to train a Quantum Reservoir with a fermionic reservoir of only two particles to visualize what the code is actually doing. Later on, we will increase the reservoir size up to 4 fermions. The following table summarizes all the equations that we are going to introduce:\n",
+                "In this first exercise, we will learn to define a quantum state in the density matrix formalism and construct our first hamiltonian.\n",
                 "\n",
-                "\n",
-                "<img src=\"images/table.png\" width=\"350\" height=\"600\">"
+                "To define the initial state you can use `qrc.reservoir.initial_state(num_sites, dim_site)` or `numpy`."
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "fee07344-018c-4ca4-b225-c11548a247ff",
+            "cell_type": "code",
+            "execution_count": 3,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Step 0: Setting up the system\n",
-                " \n",
+                "def initial_reservoir(num_sites, dim_site):\n",
+                "    \"\"\"Density matrix with all states at |0>\n",
                 "\n",
-                "The first step is to define the reservoir initial conditions, namely define a the initial state of a quantum many-body system. In this case the reservoir is build with 2 fermions in the ground state $\\lvert 0 \\rangle$ using the function `dm_zero_states`. Since fermions are a two-level systems ($\\lvert 0 \\rangle$, $\\lvert 1 \\rangle$) the Hilbert dimensions of fermions is always 2 (`dim_fermion=2`)."
+                "    Args:\n",
+                "        num_sites (int): Number of sites in the system\n",
+                "        dim_site (int): Hilbert dimension of each site.\n",
+                "    \"\"\"\n",
+                "    # Put your code here: Prepare the state |00><00|\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
-            "id": "036ecdd1",
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "array([[1., 0., 0., 0.],\n",
-                            "       [0., 0., 0., 0.],\n",
-                            "       [0., 0., 0., 0.],\n",
-                            "       [0., 0., 0., 0.]])"
-                        ]
-                    },
-                    "execution_count": 2,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Correct!\n"
+                    ]
                 }
             ],
             "source": [
-                "# initial parameters\n",
-                "n_fermions = 2\n",
-                "dim_fermion = 2\n",
+                "num_sites, dim_site = 2, 2\n",
+                "solution = initial_reservoir(num_sites, dim_site)\n",
+                "exp_solution = np.array([[1, 0, 0, 0], [0]*4, [0]*4, [0]*4])\n",
                 "\n",
-                "initial_reservoir = qrc.reservoir.initial_state(n_fermions, dim_fermion)\n",
-                "initial_reservoir"
+                "check_solution(solution, exp_solution)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2dbfa3a5",
             "metadata": {},
             "source": [
-                "To process information particles must interact with each other. The interaction strenght between particles $i$ and $j$ is defined by the parameter $J_{ij}$ and the natural dynamics of the system is ruled by the following quadratic Hamiltonian\n",
-                "\n",
+                "Now, we will define the dynamics of the system following this quadratic hamiltonian \n",
                 "$$ H = \\sum_{i,j=1}^{N}J_{ij}a_{i}^{\\dagger}a_{j} $$\n",
+                "and the evolution operator associated to it: $e^{-iH\\Delta t}$.\n",
                 "\n",
-                "This Hamiltonian encodes the onsite interation ($J_{ii}$) and the coupling iterations ($J_{ij}$) among all particles.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "id": "23cd72bc",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "matrix([[0.  +0.j, 0.  +0.j, 0.  +0.j, 0.  +0.j],\n",
-                            "        [0.  +0.j, 0.72+0.j, 0.  +0.j, 0.  +0.j],\n",
-                            "        [0.  +0.j, 0.  +0.j, 0.42+0.j, 0.  +0.j],\n",
-                            "        [0.  +0.j, 0.  +0.j, 0.  +0.j, 1.14+0.j]])"
-                        ]
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "# Generates random values between [0, 1)\n",
-                "J_ij = qrc.hamiltonian.get_coefficients(n_fermions, coef_range=[0, 1], seed=1) \n",
+                "You can define the $J_{ij}$ coefficients with: \n",
+                "- `qrc.hamiltonian.get_coefficients(num_sites, coef_range=[0, 1], seed=1)`.  \n",
                 "\n",
-                "fermionic_hamiltonian = qrc.hamiltonian.quadratic_op(n_fermions, is_bosonic=False, dimensions=dim_fermion, coefficients=J_ij)\n",
+                "Define a quadratic hamiltonian with:  \n",
+                "- `qrc.hamiltonian.quadratic_op(num_sites, is_bosonic=..., dimensions=..., coefficients=...)`\n",
                 "\n",
-                "np.around(fermionic_hamiltonian.todense(), 2)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "369ffb56",
-            "metadata": {},
-            "source": [
-                "As a last ingredient to simulate the dynamics of the reservoir, we need the evolution operator ($e^{-iH\\Delta t}$) to compute the next state of reservoir ($\\rho(t)$). \n",
-                "\n",
-                "$$ \\rho(t_f) = e^{-iH\\Delta t}\\rho(t_i)e^{iH\\Delta t}$$\n",
-                "\n",
-                "The $\\Delta t$ quantifies how much time we let system evolve. By default, $\\Delta t = 10$ because we want that the injected information in the system is spread through the whole system."
+                "and build the evolution operator with:\n",
+                "-  `qrc.hamiltonian.get_evolution_op(hamiltonian, dt=...)`\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "ca89bda8",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "array([[ 1.  +0.j  ,  0.  +0.j  ,  0.  +0.j  ,  0.  +0.j  ],\n",
-                            "       [ 0.  +0.j  ,  0.61-0.8j ,  0.  -0.j  ,  0.  +0.j  ],\n",
-                            "       [ 0.  +0.j  ,  0.  -0.j  , -0.52+0.86j,  0.  +0.j  ],\n",
-                            "       [ 0.  +0.j  ,  0.  +0.j  ,  0.  +0.j  ,  0.37+0.93j]])"
-                        ]
-                    },
-                    "execution_count": 4,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "fermionic_evolution = qrc.hamiltonian.get_evolution_op(fermionic_hamiltonian, dt=10)\n",
-                "np.around(fermionic_evolution, 2)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "de6ce1d5",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Step 1: Echo state property (wash out)\n",
-                "\n",
-                "To avoid any possible effect of the initial conditions of the reservoir we always start with the wash out step before training the system. This step consists in injecting a set of inputs until the initial conditions become irrelevant. The amount of iterations needed to wash out the initial conditions can be found in Figure 2 of the paper.\n",
+                "def my_hamiltonian(num_sites, dim_site):\n",
+                "    \"\"\"Define previous quadratic hamiltonian\n",
                 "\n",
-                "To encode classical data ($u_k$) into a quantum state ($\\lvert \\psi \\rangle$) we can use `get_input_state`.\n",
+                "    Args:\n",
+                "        num_sites (int): Number of sites in the system.\n",
+                "        dim_site (int): Hilbert dimension of each site.\n",
+                "    \"\"\"\n",
+                "    # Put your code here: Define J_ij coefficients\n",
+                "    \n",
+                "    # Put your code here: Define quadratic hamiltonian\n",
                 "\n",
-                "$$ \\lvert \\psi_k^{(e=1)} \\rangle = \\sqrt{u_k}\\lvert 0 \\rangle + \\sqrt{1-u_k}\\lvert 1 \\rangle$$\n",
                 "\n",
-                "For fermions we need to inject 3000 inputs to erase the initial conditions according to the Figure 2. However, it is possible that for certain values of $J_{ij}$ the numbers of iterations required is lower. Notice that for fermions the excited level is obvioulsy $\\lvert 1 \\rangle$, but for bosons the excited level could be $\\lvert 1 \\rangle$, $\\lvert 2 \\rangle$ ... $\\lvert n \\rangle$."
+                "def evolution_op(hamiltonian, delta_t):\n",
+                "    \"\"\"Define the evolution operator related to the previous hamiltonian\n",
+                "    and let it evolves for 10 units.\n",
+                "\n",
+                "    Args:\n",
+                "        hamiltonian (np.array): Matrix describing system dynamics.\n",
+                "        delta_t (float): Time we let the system evolve.\n",
+                "    \"\"\"\n",
+                "    # Put your code here: Define evolution operator\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "d8501e79",
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "array([[0.54984777],\n",
-                            "       [0.83526488]])"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Checking solution hamiltonian...\n",
+                        "Correct!\n",
+                        "Checking evolution operator...\n",
+                        "Correct!\n"
+                    ]
                 }
             ],
             "source": [
-                "wash_time = 3000\n",
-                "wash_out_signals = np.random.uniform(low=0, high=1, size=wash_time)\n",
+                "solution_hamiltonian = my_hamiltonian(2, 2)\n",
+                "solution_evolution = evolution_op(my_hamiltonian(2, 2), 10)\n",
                 "\n",
-                "# Generating the first input state\n",
-                "excited_state=1\n",
-                "input_state = qrc.reservoir.get_input_state(wash_out_signals[0], dim_fermion, excited_state)\n",
-                "input_state"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "de60c716",
-            "metadata": {},
-            "source": [
-                "Then, we can inject this quantum state into the first particle of the reservoir with `insert_input`. This function computes the tensor product between the input state, $\\rho_{1, k}^{(e)}=\\lvert \\psi_k^{(e)} \\rangle \\langle \\psi_k^{(e)} \\lvert$, and all particles of the reservoir except the first one, ${\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\}$\n",
                 "\n",
-                "$$ \\rho(k\\Delta t)= \\rho_{1, k}^{(e)} \\otimes {\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\} $$"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "id": "15da2cc7",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "array([[0.30233257, 0.        , 0.45926854, 0.        ],\n",
-                            "       [0.        , 0.        , 0.        , 0.        ],\n",
-                            "       [0.45926854, 0.        , 0.69766743, 0.        ],\n",
-                            "       [0.        , 0.        , 0.        , 0.        ]])"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "reservoir_with_input = qrc.reservoir.insert_input(input_state, initial_reservoir)\n",
-                "reservoir_with_input"
+                "exp_sol_hamiltonian = np.array([\n",
+                "    [0.+0.j]*4, \n",
+                "    [0.+0.j, 0.72+0.j, 0.+0.j  , 0.+0.j  ], \n",
+                "    [0.+0.j, 0.+0.j  , 0.42+0.j, 0.+0.j  ], \n",
+                "    [0.+0.j, 0.+0.j  , 0.+0.j  , 1.14+0.j]\n",
+                "])\n",
+                "exp_sol_evolution = np.array([\n",
+                "   [ 1.+0.j, 0.  +0.j ,  0.  +0.j  ,  0.  +0.j  ], \n",
+                "   [ 0.+0.j, 0.61-0.8j,  0.  -0.j  ,  0.  +0.j  ],\n",
+                "   [ 0.+0.j, 0.  -0.j , -0.52+0.86j,  0.  +0.j  ],\n",
+                "   [ 0.+0.j, 0.  +0.j ,  0.  +0.j  ,  0.37+0.93j]\n",
+                "])\n",
+                "\n",
+                "print(\"Checking solution hamiltonian...\")\n",
+                "check_solution(np.around(solution_hamiltonian.todense(), 2), exp_sol_hamiltonian)\n",
+                "print(\"Checking evolution operator...\")\n",
+                "check_solution(np.around(solution_evolution, 2), exp_sol_evolution)\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ec7127e4",
             "metadata": {},
             "source": [
-                "To let the information spread through the whole system we let the system evolve following the quantum dynamics of a closed system, as shown in the table above.\n",
+                "### Exercise 1 - Echo State Property\n",
                 "\n",
+                "To avoid any possible effect of the initial conditions of the reservoir we always start with the wash out step before training the system. This step consists in injecting a set of inputs until the initial conditions become irrelevant.\n",
                 "\n",
-                "$$ \\rho\\left(k\\Delta t\\right)=e^{-iH\\Delta t}\\left[\\rho_{1,k}^{(e)}\\otimes {\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\} \\right]e^{iH\\Delta t} $$"
+                "So, in this section, you are going to compute how many iterations (wash-out steps) does your system need to wash out the initial conditions.\n",
+                "\n",
+                "Each iteration have these 3 steps:\n",
+                "- Encoding classical data into a quantum state $\\Longrightarrow \\lvert \\psi_k^{(e)} \\rangle$.\n",
+                "    - qrc.reservoir.get_input_state(signal, dim, exc_state)\n",
+                "    - $ \\lvert \\psi_k^{(e=1)} \\rangle = \\sqrt{s_k}\\lvert 0 \\rangle + \\sqrt{1-s_k}\\lvert 1 \\rangle$\n",
+                "- Injecting the quantum state into the reservoir $\\Longrightarrow \\rho(k)$.\n",
+                "    - qrc.reservoir.insert_input(input_state, initial_reservoir)\n",
+                "    - $ \\rho(k\\Delta t)= \\rho_{1, k}^{(e)} \\otimes {\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\} $\n",
+                "- Evolving the reservoir $\\Longrightarrow  \\rho(k\\Delta t)$.\n",
+                "    - qrc.reservoir.evolve(reservoir, evo_op)\n",
+                "    - $ \\rho\\left(k\\Delta t\\right)=e^{-iH\\Delta t}\\left[\\rho_{1,k}^{(e)}\\otimes {\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\} \\right]e^{iH\\Delta t} $\n",
+                "\n",
+                "So, let's start building these 3 functions:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "458d8d0c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "reservoir = qrc.reservoir.evolve(reservoir_with_input, fermionic_evolution)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "9430a0a2",
-            "metadata": {},
-            "source": [
-                "So, at each iteration the reservoir will change following these 3 steps:\n",
-                "- Encoding classical data into a quantum state $\\Longrightarrow \\lvert \\psi_k^{(e)} \\rangle$.\n",
-                "- Injecting the quantum state into the reservoir $\\Longrightarrow \\rho(k)$.\n",
-                "- Evolving the reservoir $\\Longrightarrow  \\rho(k\\Delta t)$.\n",
+                "# Use signal=0.25 to test your solution\n",
+                "def get_input_state(signal, dim_site, exc_state=1):\n",
+                "    \"\"\"Encode classical data into a superposition state\n",
+                "\n",
+                "        |\u03c8> = \u221as|0> + \u221a1-s|1>\n",
+                "\n",
+                "    Args:\n",
+                "        signal (float): Classical data.\n",
+                "        dim_site (int): Hilbert dimension of each site.\n",
+                "        exc_state (int): Highest superposition state\n",
+                "    \"\"\"\n",
+                "    # Put your code here: \n",
+                "\n",
+                "\n",
+                "def inject_state(input_state, reservoir):\n",
+                "    \"\"\"Introduce the input state into the reservoir\n",
+                "\n",
+                "    Args:\n",
+                "        input_state (np.array): Classical data in a superposition state.\n",
+                "        reservoir (np.array): Current state of the quantum system\n",
+                "\n",
+                "    \"\"\"\n",
+                "    # Put your code here:\n",
+                "\n",
+                "\n",
+                "def evolve_reservoir(reservoir, evo_op):\n",
+                "    \"\"\"Evolve the quantum system following the evolution operator.\n",
                 "\n",
-                "To avoid calling the previous three functions at each iteration, we have packed the previous 3 points in a single function call `cptp_map` which will generate a reservoir state for each injected input. "
+                "    Args:\n",
+                "        reservoir (np.array): Current state of the quantum system\n",
+                "        evo_op (np.array): Evolution operator\n",
+                "    \"\"\"\n",
+                "    # Put your code here:\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "99d6fc81",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "array([[ 0.191+0.j   , -0.   +0.j   , -0.203-0.337j,  0.   +0.001j],\n",
-                            "       [-0.   -0.j   ,  0.   +0.j   ,  0.   +0.001j, -0.   -0.j   ],\n",
-                            "       [-0.203+0.337j,  0.   -0.001j,  0.808+0.j   , -0.002-0.001j],\n",
-                            "       [ 0.   -0.001j, -0.   +0.j   , -0.002+0.001j,  0.   +0.j   ]])"
-                        ]
-                    },
-                    "execution_count": 8,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Checking solution input state...\n",
+                        "Correct!\n",
+                        "Checking evolution inject state...\n",
+                        "Correct!\n",
+                        "Checking evolution evolve reservoir...\n",
+                        "Correct!\n"
+                    ]
                 }
             ],
             "source": [
-                "# Generates a list with the state of the reservoir after each iteration\n",
-                "reservoirs = list(qrc.reservoir.cptp_map(wash_out_signals, initial_reservoir, fermionic_evolution, dim_fermion, excited_state))\n",
+                "# Use signal = 0.25\n",
+                "sol_input_state = get_input_state(0.25, dim_site=2)\n",
+                "\n",
+                "# Inject the previous input and the initial reservoir\n",
+                "sol_inject_state = inject_state(sol_input_state, initial_reservoir(2, 2))\n",
+                "\n",
+                "# Evolve the reservoir with the classical data\n",
+                "sol_evolve_reservoir = evolve_reservoir(sol_inject_state, evolution_op(my_hamiltonian(2, 2), 10))\n",
+                "\n",
+                "\n",
+                "exp_input_state = np.array([[np.sqrt(0.25)], [np.sqrt(1-0.25)]])\n",
+                "exp_inject_state = np.array([\n",
+                "   [ 0.25     , 0.  ,  0.433    ,  0.], \n",
+                "   [ 0.       , 0.  ,  0.       ,  0.],\n",
+                "   [ 0.433    , 0.  ,  0.75     ,  0.],\n",
+                "   [ 0.       , 0.  ,  0.       ,  0.]\n",
+                "])\n",
+                "exp_evolve_reservoir = np.array([\n",
+                "   [ 0.25 +0.j  , 0.  +0.j ,  -0.22-0.37j,  0.  +0.j], \n",
+                "   [ 0.   +0.j  , 0.  -0.j,   0.  -0.j   ,   0.  +0.j],\n",
+                "   [ -0.22+0.37j, 0.  -0.j ,  0.75+0.j   ,   0.  +0.j],\n",
+                "   [ 0.   +0.j  , 0.  +0.j ,  0.  +0.j   ,   0.  +0.j]\n",
+                "])\n",
+                "\n",
+                "print(\"Checking solution input state...\")\n",
+                "check_solution(sol_input_state, exp_input_state)\n",
+                "print(\"Checking evolution inject state...\")\n",
+                "check_solution(np.around(sol_inject_state, 3), exp_inject_state)\n",
+                "print(\"Checking evolution evolve reservoir...\")\n",
+                "check_solution(np.around(sol_evolve_reservoir, 2), exp_evolve_reservoir)\n",
                 "\n",
-                "# Take the last reservoir from the previous list\n",
-                "washed_reservoir = reservoirs[-1]\n",
-                "np.around(washed_reservoir, 3)"
+                "    "
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e3b5f16f",
             "metadata": {},
             "source": [
-                "### Step 2: Data prepartion\n",
+                "These 3 steps can be summarized with the following map:\n",
                 "\n",
-                "Once we have a `washed_reservoir` you can start training the reservoir to perform any typical supervise machine learning task. In a real world scenario you will have a dataset with a time-series (ex: temperatures over several years, stock market, etc.).\n",
+                "$$ \\rho\\left(k\\Delta t\\right)=e^{-iH\\Delta t}\\left[\\rho_{1,k}^{(e)}\\otimes {\\rm Tr}_{1}\\left\\{ \\rho\\left(\\left(k-1\\right)\\Delta t\\right)\\right\\} \\right]e^{iH\\Delta t} $$\n",
                 "\n",
-                "In our case, we are interested in benchmarking the ability to store past inputs, so a random sequence of number is good enough for our porpuses. Let's start by setting some parameters, as the `delay`, `train_time` and `test_time`.\n",
-                "- `delay`: Number of iterations between the input and target data. As the delay increase, it will become harder to remember the input.\n",
-                "- `train_time` and `test_time`: Number of iterations to train/test the reservoir.\n",
-                "\n",
-                "Then, instead of uploading a dataset we will simply generate random numbers. \n",
-                "_Remember that we have already set a seed for generating the coefficients $J_{ij}$, so the following results are totally reproducible_.\n",
-                "\n"
+                "Now, it will be great if you could buid a new function with the previous functions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "id": "f102d174",
             "metadata": {},
             "outputs": [],
             "source": [
-                "delay = 1\n",
-                "train_time, test_time = 10, 10\n",
-                "\n",
-                "# Prepare random data\n",
-                "train_signals = np.random.uniform(low=0, high=1, size=train_time + delay)\n",
-                "test_signals = np.random.uniform(low=0, high=1, size=test_time + delay)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "d405454f",
-            "metadata": {},
-            "source": [
-                "Let's also prepare the input with the function `get_inputs`."
+                "def cptp_map(signals, ini_reservoir, evo_op, dim_site=2, exc_state=1):\n",
+                "    \"\"\"Generates a new reservoir state after completing the 3-step iteration.\n",
+                "            1. Encode classical data into a quantum state.\n",
+                "            2. Injecting the quantum state into the reservoir.\n",
+                "            3. Evolving the reservoir.\n",
+                "\n",
+                "    Args:\n",
+                "        signals (np.array): List of numbers that it is going to be injected into the reservoir.\n",
+                "        ini_reservoir (np.array): Initial state of the reservoir\n",
+                "        evo_op (np.array): Evolution operator.\n",
+                "    \"\"\"\n",
+                "    new_reservoir = ini_reservoir\n",
+                "    for signal in signals:\n",
+                "        # Put your code here:\n",
+                "        #input_state = ...\n",
+                "        #new_reservoir = ...\n",
+                "        #new_reservoir = ...\n",
+                "        yield new_reservoir"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "id": "eea016e2",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "inputs = [0.96 0.56 0.65 0.27 0.95 0.67 0.67 0.01 0.85 0.78 0.74 0.16 0.72 0.1\n",
-                        " 0.71 0.   0.78 0.49 0.2  0.73]\n"
-                    ]
-                }
-            ],
-            "source": [
-                "# Generating inputs to train and test the reservoir.\n",
-                "train_inputs = mc.get_inputs(train_signals, delay)\n",
-                "test_inputs = mc.get_inputs(test_signals, delay)\n",
-                "inputs = np.concatenate((train_inputs, test_inputs))\n",
-                "print(\"inputs =\", np.around(inputs, 2))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "31b23cbd",
-            "metadata": {},
-            "source": [
-                "As well, the function `get_targets` generates the target for linear task when $\\hat{y}=u_k$ and for the non-linear task $\\hat{y}=u_k^q$ ($q \\neq 1$)."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 11,
-            "id": "cef6d00a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "train_targets = [0.98 0.96 0.56 0.65 0.27 0.95 0.67 0.67 0.01 0.85]\n"
+                        "Checking solution cptp map...\n",
+                        "Correct!\n"
                     ]
                 }
             ],
             "source": [
-                "# Generating targets\n",
-                "train_targets = mc.get_targets(train_signals, delay, degree=1)\n",
-                "test_targets = mc.get_targets(test_signals, delay, degree=1)\n",
-                "print(\"train_targets =\", np.around(train_targets, 2))"
+                "# Check solution:\n",
+                "sol_cptp_map = list(cptp_map([0.25], initial_reservoir(2, 2), evolution_op(my_hamiltonian(2, 2), 10)))\n",
+                "\n",
+                "exp_sol_cptp = np.array([\n",
+                "   [ 0.25 +0.j  , 0.  +0.j ,  -0.22-0.37j,  0.  +0.j], \n",
+                "   [ 0.   +0.j  , 0.  -0.j,   0.  -0.j   ,   0.  +0.j],\n",
+                "   [ -0.22+0.37j, 0.  -0.j ,  0.75+0.j   ,   0.  +0.j],\n",
+                "   [ 0.   +0.j  , 0.  +0.j ,  0.  +0.j   ,   0.  +0.j]\n",
+                "])\n",
+                "\n",
+                "print(\"Checking solution cptp map...\")\n",
+                "check_solution(np.around(sol_cptp_map[0], 2), exp_sol_cptp)\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "dbb64d70",
             "metadata": {},
             "source": [
-                "### Step 3: Enconding data into a high dimensional space\n",
-                "\n",
-                "The following line it should look familiar:"
+                "Finally, let's find how many iterations do you need to erase the initial conditions of the reservoir."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "id": "c796a754",
             "metadata": {},
             "outputs": [],
             "source": [
-                "reservoirs = list(qrc.reservoir.cptp_map(inputs, washed_reservoir, fermionic_evolution, dim_fermion, excited_state))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "22fd3963",
-            "metadata": {},
-            "source": [
-                "Exactly, this function is used to generate a sequence of reservoir states (just as in the wash out step). The imporant thing to remember is that each of these reservoir states contain some information from the past inputs. \n",
+                "# Auxiliar functions: Don't forget to run this cell\n",
+                "def tensor_product(matrices: list):\n",
+                "    if len(matrices) == 2:\n",
+                "        return np.kron(matrices[0], matrices[1])\n",
+                "    return np.kron(matrices[0], tensor_product(matrices[1:]))\n",
                 "\n",
-                "Now, we would like to extract some information ($x_j$) from the quantum system by performing some measurements.   \n",
                 "\n",
-                "$$ x_{j}\\left(k\\Delta t\\right)={\\rm Tr}\\left[O_{j}\\rho\\left(u_k\\Delta t\\right)\\right]   \\qquad  (1)$$\n",
+                "def excited_reservoir(num_sites: int, dim_site: int, exc_sites=list()):\n",
+                "    \"\"\"By default the reservoir has all sites at |0>, except the sites in \n",
+                "    exc_sites found at |1>\n",
+                "    \"\"\"\n",
+                "    state = np.zeros((dim_site, 1))\n",
+                "    state[0, 0] = 1\n",
+                "    ground_state = state\n",
                 "\n",
-                "To do that, we need to define a set of observables. For this tutorial we will use observables of the form $a_i^\\dagger a_j$. "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 13,
-            "id": "94da0e5b",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "obs = qrc.measurements.observables(\"fermion\", n_fermions, dim_fermion, \"ij\")"
+                "    state = np.zeros((dim_site, 1))\n",
+                "    state[1, 0] = 1\n",
+                "    excited_state = state\n",
+                "\n",
+                "    ground_dm = np.outer(ground_state, ground_state)\n",
+                "    excited_dm = np.outer(excited_state, excited_state)\n",
+                "\n",
+                "    sites_dm = [ground_dm] * num_sites\n",
+                "\n",
+                "    for site_i in exc_sites:\n",
+                "        sites_dm[site_i - 1] = excited_dm\n",
+                "\n",
+                "    return tensor_product(sites_dm)\n",
+                "\n",
+                "\n",
+                "def convergence(rho_a_generator, rho_b_generator):\n",
+                "    distance = list()\n",
+                "    for rho_a, rho_b in zip(rho_a_generator, rho_b_generator):\n",
+                "        rho = rho_a - rho_b\n",
+                "        distance.append(np.linalg.norm(rho, \"fro\"))\n",
+                "    return np.array(distance)\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9585a761",
             "metadata": {},
             "source": [
-                "In the following you can notice that `obs` is a list that contain the diagonal a non-diagonal observables:\n",
+                "In the following function we will have two reservoirs with different initials conditions:\n",
                 "\n",
-                "- $a_0^\\dagger a_0$\n",
-                "- $a_1^\\dagger a_1$\n",
-                "- $a_0^{\\dagger}a_1 + a_1^{\\dagger}a_0$"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 14,
-            "id": "377eb960",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "[[0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
-                        " [0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
-                        " [0.+0.j 0.+0.j 1.+0.j 0.+0.j]\n",
-                        " [0.+0.j 0.+0.j 0.+0.j 1.+0.j]]\n"
-                    ]
-                }
-            ],
-            "source": [
-                "# diagonal observable: adag_0 a_0\n",
-                "print(obs[0])"
+                "$$\\rho_a = \\lvert 0010\\rangle \\langle 0010 \\lvert $$\n",
+                "$$\\rho_b = \\lvert 0001\\rangle \\langle 0001 \\lvert $$\n",
+                "\n",
+                "Then, we will evolve both reservoirs injecting the same classical data. After each iteration we will measure the Frobenius distance between the reservoir. \n",
+                "\n",
+                "How many iterations are necessary to erase the initial conditions? \n",
+                "- You can answer either numerically or visually with the plot"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
-            "id": "60823ee2",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "[[0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
-                        " [0.+0.j 1.+0.j 0.+0.j 0.+0.j]\n",
-                        " [0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
-                        " [0.+0.j 0.+0.j 0.+0.j 1.+0.j]]\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "# diagonal observable: adag_1 a_1 \n",
-                "print(obs[2])"
+                "def echo_state_property(signals, num_sites, dim_site, exc_sites_a, exc_sites_b, dt):\n",
+                "    \"\"\"Compute the number of iterations needed to erase the initial conditions.\n",
+                "\n",
+                "    Args:\n",
+                "        signals (np.array): List of numbers that it is going to be injected into the reservoir.\n",
+                "        num_sites (int): Number of sites in the system.\n",
+                "        dim_site (int): Hilbert dimension of each site.\n",
+                "        exc_sites_a (list): Sites excited from |0> to |1> for system A\n",
+                "        exc_sites_b (list): Sites excited from |0> to |1> for system B\n",
+                "        dt (float): Time we let the system evolve\n",
+                "    \"\"\"\n",
+                "    # Create two initial reservoir: |0010><0010| and |0001><0001|\n",
+                "    rho_a = excited_reservoir(num_sites, dim_site, exc_sites_a)\n",
+                "    rho_b = excited_reservoir(num_sites, dim_site, exc_sites_b)\n",
+                "    \n",
+                "    # Put your code here: Compute evolution operator    \n",
+                "    # hamiltonian = ... \n",
+                "    # evo_op = ...\n",
+                "    \n",
+                "    # Put your code here: Evolve the reservoir state\n",
+                "    # rho_a_generator = ...\n",
+                "    # rho_b_generator = ...\n",
+                "    \n",
+                "    # Measure the Frobenius distance \n",
+                "    return convergence(rho_a_generator, rho_b_generator)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
-            "id": "382b44cc",
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[[0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
-                        " [0.+0.j 0.+0.j 1.+0.j 0.+0.j]\n",
-                        " [0.+0.j 1.+0.j 0.+0.j 0.+0.j]\n",
-                        " [0.+0.j 0.+0.j 0.+0.j 0.+0.j]]\n"
+                        "Checking solution echo state property...\n",
+                        "Correct!\n",
+                        "\n",
+                        "Now, you can plot it and try different parameters\n"
                     ]
                 }
             ],
             "source": [
-                "# non-diagonal observable: adag_0 a_1 + adag_1 a_0\n",
-                "print(obs[1])"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "87cb27be",
-            "metadata": {},
-            "source": [
-                "Typically, conventional neural networks (NN) algorithms use a nonlinear function ($f$) like the ReLU or sigmoid to fit the input data ($x$)\n",
-                "\n",
-                "$$y_{NN}=f(\\rm{wx}+\\rm{b})$$\n",
-                "\n",
-                "where $y$ is the output of the NN and $w$, $b$ is the weights and bias that the network will optimize to fit the target data.  \n",
-                "\n",
-                "With the reservoir computing (RC) framework such a nonlinear function is already introduce in the dynamics of the reservoir. Hence, optimizing the weights becomes an easy task, since they can be found using a linear regression algorithm. \n",
+                "num_iterations = 1000\n",
+                "rng_signals = np.random.default_rng(seed=1)\n",
+                "signals = rng_signals.uniform(low=0, high=1, size=num_iterations)\n",
                 "\n",
-                "$$ y_{RC}=\\rm{wx}+\\rm{b}$$\n",
+                "num_sites = 4\n",
+                "exc_sites_a, exc_sites_b  = [3], [4]\n",
+                "dt = 10\n",
                 "\n",
-                "In our case, we have a output ($y_k$) for each input value ($u_k$). So our linear equation is of the form  \n",
-                "\n",
-                "$$ y_k = \\sum_{j=1}^M \\rm{x_{kj}w_j}$$\n",
-                "\n",
-                "This can be written in a vectorize notation as:\n",
-                "\n",
-                "$$ y = XW$$\n",
-                "\n",
-                "where $y=[y_1, y_2, ... y_k, ... y_L]$ are the predictions of the algorithm, $W=[w_1, w_2, ... w_j, ... w_M, b]$ are the weights and bias to be optimized and $X$ is matrix with shape (L, M+1).\n",
-                "\n",
-                "$$X=\\begin{bmatrix} {\\rm Tr}\\left[O_{1}\\rho\\left(u_1\\Delta t\\right)\\right]  & {\\rm Tr}\\left[O_{2}\\rho\\left(u_1\\Delta t\\right)\\right] & .. & {\\rm Tr}\\left[O_{M}\\rho\\left(u_1\\Delta t\\right)\\right] & 1 \\\\\n",
-                "{\\rm Tr}\\left[O_{1}\\rho\\left(u_2\\Delta t\\right)\\right]  & .. & .. & {\\rm Tr}\\left[O_{M}\\rho\\left(u_2\\Delta t\\right)\\right] & 1\\\\ \n",
-                ".. & .. & .. & .. & ..\\\\\n",
-                "{\\rm Tr}\\left[O_{1}\\rho\\left(u_L\\Delta t\\right)\\right]  & .. & .. & {\\rm Tr}\\left[O_{M}\\rho\\left(u_L\\Delta t\\right)\\right] & 1\n",
-                "\\end{bmatrix}$$\n",
-                "\n",
-                "To compute the previous matrix, you can use the `get_features` function."
+                "frobenius_norm = echo_state_property(signals, num_sites, 2, exc_sites_a, exc_sites_b, dt)\n",
+                "exp_solution = np.array([1.41, 1.32, 1.15, 0.97, 0.82, 0.74, 0.69, 0.65, 0.58, 0.53])\n",
+                "print(\"Checking solution echo state property...\")\n",
+                "check_solution(np.around(frobenius_norm[:10], 2), exp_solution)\n",
+                "print()\n",
+                "print(\"Now, you can plot it and try different parameters\")\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
-            "id": "5ae1a939",
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([[ 0.039,  0.001,  0.001,  1.   ],\n",
-                            "       [ 0.443,  0.   ,  0.001,  1.   ],\n",
-                            "       [ 0.354, -0.002,  0.001,  1.   ],\n",
-                            "       [ 0.728, -0.004,  0.001,  1.   ],\n",
-                            "       [ 0.048, -0.001,  0.001,  1.   ],\n",
-                            "       [ 0.33 ,  0.001,  0.001,  1.   ],\n",
-                            "       [ 0.333,  0.002,  0.001,  1.   ],\n",
-                            "       [ 0.989, -0.001,  0.001,  1.   ],\n",
-                            "       [ 0.147,  0.   ,  0.001,  1.   ],\n",
-                            "       [ 0.222, -0.002,  0.001,  1.   ],\n",
-                            "       [ 0.259, -0.003,  0.001,  1.   ],\n",
-                            "       [ 0.843, -0.002,  0.001,  1.   ],\n",
-                            "       [ 0.281,  0.001,  0.001,  1.   ],\n",
-                            "       [ 0.903,  0.   ,  0.001,  1.   ],\n",
-                            "       [ 0.293,  0.002,  0.001,  1.   ],\n",
-                            "       [ 0.997, -0.001,  0.001,  1.   ],\n",
-                            "       [ 0.224, -0.002,  0.001,  1.   ],\n",
-                            "       [ 0.508, -0.004,  0.001,  1.   ],\n",
-                            "       [ 0.796, -0.002,  0.001,  1.   ],\n",
-                            "       [ 0.271,  0.001,  0.001,  1.   ]])"
+                            "Text(0, 0.5, 'Frobenius norm')"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
+                },
+                {
+                    "data": {
+                        "image/png": "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",
+                        "text/plain": [
+                            "<Figure size 600x300 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "dataset, _ = qrc.measurements.get_features(reservoirs, obs)\n",
+                "num_iterations = 1000\n",
+                "rng_signals = np.random.default_rng(seed=1)\n",
+                "signals = rng_signals.uniform(low=0, high=1, size=num_iterations)\n",
                 "\n",
-                "# Approximate dataset values up to 3 decimals\n",
-                "np.around(dataset, 3)"
+                "# You can modify the following parameters and see if the frobenius norm between system A and B changes.\n",
+                "num_sites = 4\n",
+                "exc_sites_a = [3]\n",
+                "exc_sites_b = [4]\n",
+                "dt = 10\n",
+                "\n",
+                "frobenius_norm = echo_state_property(signals, num_sites, 2, exc_sites_a, exc_sites_b, dt)\n",
+                "plt.figure(figsize=(6, 3))\n",
+                "plt.plot(frobenius_norm)\n",
+                "plt.xlabel(\"Number of iterations\")\n",
+                "plt.grid()\n",
+                "plt.ylabel(\"Frobenius norm\")\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "59de76b3",
             "metadata": {},
             "source": [
-                "### Step 4: Optimizing weights\n",
+                "### Exercise 2 - Evaluate model\n",
                 "\n",
-                "The optimal weights are computing minimizing the 2-norm error between the target values $\\hat{y}$ and the actual predictions $y=XW$ \n",
+                "You will train a quantum system to recall past inputs and evaluate the performance with the memory capacity.\n",
                 "\n",
-                "$$ arg\\min_{W} |\\hat{y}-XW|.$$\n",
+                "Our objective is to quantify how well the quantum system can recover past information. So, we will inject a sequence of random inputs ($s_k$) into the reservoir and the system will be trained to match a target function\n",
                 "\n",
-                "In the well-known package `scipy` there is a specific function to optimize linear regression problems called `lstsq`. But before we split the dataset into train and test to later evaluate the results and check if the parameters used overfit the data."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 18,
-            "id": "f245c39f",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "optimal weights=[ 2.3400000e-01  2.1895000e+01 -4.8755787e+04  2.8595000e+01]\n"
-                    ]
-                }
-            ],
-            "source": [
-                "train_X = dataset[:train_time, :]\n",
-                "test_X = dataset[train_time:, :]\n",
+                "$$ \\hat{y}_k = s_{k-\\tau}$$\n",
                 "\n",
-                "# Getting optimal weights\n",
-                "opt_weights, _, _, _ = lstsq(train_X, train_targets)\n",
+                "where $\\tau$ is the delay between the input and target.\n",
                 "\n",
-                "print(f\"optimal weights={np.around(opt_weights, 3)}\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "67506a75",
-            "metadata": {},
-            "source": [
-                "### Step 5: Evaluating the memory capacity\n",
+                "<div class=\"alert alert-block alert-info\">\n",
+                "    <b>Example:</b>    \n",
+                "    \n",
+                "Given an input sequence:\n",
+                "$$ s = (0.2, 0.3, 0.4, 0.5) $$\n",
                 "\n",
-                "The memory capacity ($MC$) is a metric that quantifies the linear correlation between two vectors. If both vectors are identical $MC=1$, if there is no linear correlation $MC=0$.\n",
+                "The target function after a delay, $\\tau=1$ is:\n",
                 "\n",
-                "$$MC=\\frac{Cov^2(\\hat{y}, y)}{\\sigma^2(\\hat{y})\\sigma^2(y)} $$\n",
+                "$$ \\hat{y} = (0.1, 0.2, 0.3, 0.4) $$\n",
+                "\n",
+                "But the reservoir after the training procedure may output a different result:\n",
+                "\n",
+                "$$ y = (0.11, 0.19, 0.3, 0.398) $$\n",
+                "</div>\n",
                 "\n",
-                "The algorithm predictions with the best weights are:\n",
-                "$$ y_{train}^{\\, p}=X_{train}w_{opt}$$"
+                "Let us introduce the metric to measure the system memory. The memory capacity is a standard measure of memory in recurrent neural network, defined as:\n",
+                "\n",
+                "$$ MC = \\frac{Cov^2(y,\\hat{y})}{\\sigma^2(y)\\sigma^2(\\hat{y})} $$\n",
+                "\n",
+                "where $\\sigma(y)$ and $\\sigma(\\hat{y})$ are the standard deviation of the reservoir and target outputs, respectively."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
-            "id": "e8237b60",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "train predictions= [0.701 0.798 0.656 0.601 0.479 0.605 0.733 0.809 0.641 0.543]\n"
-                    ]
-                }
-            ],
-            "source": [
-                "train_predictions = np.matmul(train_X, opt_weights)\n",
-                "print(\"train predictions=\", np.around(train_predictions, 3))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "cfdc9f1e",
+            "execution_count": 23,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "We can also compute the predictions on the test dataset `test_X`. \n",
-                "$$ y_{pred}^{test} = X_{test}w_{opt}$$"
+                "# Auxiliar functions: Don't forget to run this cell\n",
+                "\n",
+                "def get_targets(prev_signal, current_signal, delay):\n",
+                "    if delay == 0:\n",
+                "        target_signal = current_signal\n",
+                "    elif delay > 0:\n",
+                "        target_signal = np.concatenate((prev_signal[-delay:], current_signal[:-delay]))\n",
+                "    \n",
+                "    return target_signal"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
-            "id": "cf2145b4",
+            "execution_count": 22,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "test predictions= [0.436 0.531 0.508 0.688 0.649 0.713 0.442 0.362 0.409 0.404]\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "test_predictions = np.matmul(test_X, opt_weights)\n",
-                "print(\"test predictions=\", np.around(test_predictions, 3))"
+                "# Prepare input data\n",
+                "delay = 1\n",
+                "wash_time, train_time, test_time = 10, 10, 10\n",
+                "\n",
+                "rng_signals = np.random.default_rng(seed=1)\n",
+                "wash_inputs = rng_signals.uniform(low=0, high=1, size=wash_time)\n",
+                "train_inputs = rng_signals.integers(low=0, high=1, size=train_time, endpoint=True)\n",
+                "test_inputs = rng_signals.integers(low=0, high=1, size=test_time, endpoint=True)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0336dd05",
             "metadata": {},
             "source": [
-                "Finally, we can measure the memory capacity."
+                "Now, your objective is to prepare the dataset. For that we will follow these steps:\n",
+                "1. A wash-out reservoir.\n",
+                "2. Generate a set of reservoir that contain the classical.\n",
+                "3. Extract information by measuring a set of observables.  \n",
+                "    3.1 Build a set of observables. You can use `qrc.measurements.observables(particle_type, num_sites, dim_site, observable_set)`\n",
+                "    - In the case we are using particle_type=\"fermion\"\n",
+                "    - Observable set is $a^\\dagger_i a_j +h.c.$, so observable_set=\"ij\".\n",
+                "4. Collect all of this information in a dataset.\n",
+                "    - If you have all reservoirs and all observables you can generate the dataset with `dataset, _ = qrc.measurements.get_features(reservoirs, all_obs)`\n",
+                "\n",
+                "The dataset is of the form: \n",
+                "$$X=\\begin{bmatrix} {\\rm Tr}\\left[O_{1}\\rho\\left(u_1\\Delta t\\right)\\right]  & {\\rm Tr}\\left[O_{2}\\rho\\left(u_1\\Delta t\\right)\\right] & .. & {\\rm Tr}\\left[O_{M}\\rho\\left(u_1\\Delta t\\right)\\right] & 1 \\\\\n",
+                "{\\rm Tr}\\left[O_{1}\\rho\\left(u_2\\Delta t\\right)\\right]  & .. & .. & {\\rm Tr}\\left[O_{M}\\rho\\left(u_2\\Delta t\\right)\\right] & 1\\\\ \n",
+                ".. & .. & .. & .. & ..\\\\\n",
+                "{\\rm Tr}\\left[O_{1}\\rho\\left(u_L\\Delta t\\right)\\right]  & .. & .. & {\\rm Tr}\\left[O_{M}\\rho\\left(u_L\\Delta t\\right)\\right] & 1\n",
+                "\\end{bmatrix}$$\n",
+                "\n",
+                "and has shape $(L, M+1)$ where L are the number of inputs (or iterations) and M are the number of measurements."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
-            "id": "c21fbd72",
+            "execution_count": 30,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Train MC=0.113\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "train_mc = mc.memory_capacity(train_predictions, train_targets)\n",
-                "print(f\"Train MC={np.around(train_mc, 3)}\")"
+                "def build_dataset(num_sites, dim_site, dt, signals):\n",
+                "    wash_inputs, train_inputs, test_inputs = signals\n",
+                "    ini_reservoir = initial_reservoir(num_sites, dim_site)\n",
+                "    \n",
+                "    hamiltonian = my_hamiltonian(num_sites, dim_site)\n",
+                "    evo_op = evolution_op(hamiltonian, dt)\n",
+                "    \n",
+                "    # Put your code here: Wash-out reservoir\n",
+                "    # ... (you may need more than one-line of code)\n",
+                "    \n",
+                "    inputs = np.concatenate((train_inputs, test_inputs))\n",
+                "    # Put your code here: Generate a set of reservoir that contain the inputs.\n",
+                "    # ...\n",
+                "    \n",
+                "    # Put your code here: Build a set of observables\n",
+                "    # ...\n",
+                "    \n",
+                "    # Put your code here: Build dataset\n",
+                "    # ...\n",
+                "    \n",
+                "    train_data = dataset[:len(train_inputs), :]\n",
+                "    test_data = dataset[len(train_inputs):, :]\n",
+                "    \n",
+                "    return train_data, test_data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
-            "id": "34539b20",
+            "execution_count": 31,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Test MC=0.015\n"
+                        "Correct!\n"
                     ]
                 }
             ],
             "source": [
-                "test_mc = mc.memory_capacity(test_predictions, test_targets)\n",
-                "print(f\"Test MC={np.around(test_mc, 3)}\")"
+                "# Defualt parameters: You can change them, once you pass the test.\n",
+                "num_sites = 4\n",
+                "dim_site = 2\n",
+                "dt = 10\n",
+                "\n",
+                "signals = (wash_inputs, train_inputs, test_inputs)\n",
+                "train_data, test_data = build_dataset(num_sites, dim_site, dt, signals)\n",
+                "exp_train_data = np.array([\n",
+                "    [0.17, 0.34, 0.12, 0.24, 0.23, 0.04, 0.09, 0.17, 0.41, 0.32, 1.  ],\n",
+                "    [0.1 , 0.25, 0.05, 0.11, 0.21, 0.01, 0.03, 0.16, 0.35, 0.24, 1.  ]]\n",
+                ")\n",
+                "check_solution(np.around(train_data[:2, :], 2), exp_train_data)\n",
+                "\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1cb12215",
             "metadata": {},
             "source": [
-                "Cleary, this results by no means great. The memory capacity is quite low and the algorithm is overfitting the data. To get good results the hyperparameters that must be optimized are:\n",
+                "Finally, to evaluate the performance of the model we need to train the system with the train_data ($X_train$) and train targets ($y_train$). Then, we can find the optimal weights\n",
                 "\n",
-                "- Number of particles \n",
-                "- Training data\n",
-                "- $\\Delta t$.\n",
+                "$$arg\\min_{W}|\\hat{y}-XW|$$\n",
                 "\n",
-                "The Hamiltonian coefficients $J_{ij}$ also play an important role on how the informtion is spread through the system and it will be the next topic we are going to explore.\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "03eed7be",
-            "metadata": {},
-            "source": [
-                "### Summary\n",
+                "and evaluate the performance\n",
                 "\n",
-                "In this tutorial, you have learnt how to train a QRC to perform a supervise task. \n",
+                "$$MC=\\frac{Cov^2(\\hat{y}, y)}{\\sigma^2(\\hat{y})\\sigma^2(y)}.$$\n",
                 "\n",
-                "If you want to play around (try different reservoir sizes, particles, train times, etc) we have introudce all the steps shown above in a function called `main`. So, there is no need to re-run previous cells, just set the parameters you are curios about and find out if the performance is improved or not."
+                "You can also use the optimal weights to make predictions on unseen data.\n",
+                "$$ y_{prediction}=X_{test}w_{opt}.$$\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
-            "id": "7851d951",
+            "execution_count": 32,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Parameters for fermions \n",
-                "\n",
-                "# Reservoir parameters\n",
-                "n_particles = 4 # 2, 3, .., n\n",
-                "dimensions = 2\n",
-                "J_ij = qrc.hamiltonian.get_coefficients(n_particles, coef_range=[0, 1], seed=1) # try different seeds\n",
-                "operator = \"fermion\"\n",
-                "excited_state = 1\n",
-                "dt= 10\n",
-                "\n",
-                "# Performance parameters\n",
-                "delay = 1 # 1, 2, .., n\n",
-                "obs_form = \"ij\"\n",
-                "wash_time = 3000\n",
-                "train_time = 1200\n",
-                "test_time = 300\n"
+                "# Auxiliar function: Don't forget to run this cell\n",
+                "def memory_capacity(predictions, targets):\n",
+                "    return (np.corrcoef(predictions, targets)[0, 1]) ** 2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
-            "id": "6c39d168",
+            "execution_count": 34,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Reservoir with 4 fermions:\n",
-                        "\tTrain MC=0.809\n",
-                        "\tTest  MC=0.808\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "_, _, train_mc, test_mc = mc.main(\n",
-                "    n_particles,\n",
-                "    dimensions,\n",
-                "    J_ij,\n",
-                "    operator,\n",
-                "    delay,\n",
-                "    obs_form,\n",
-                "    wash_time,\n",
-                "    train_time,\n",
-                "    test_time,\n",
-                "    excited_state,\n",
-                "    dt\n",
-                ")\n",
+                "def evaluate_performance(num_sites, dim_site, delay, dt, wash_time, train_time, test_time, seed=1):\n",
+                "    # Prepare input data\n",
+                "    rng_signals = np.random.default_rng(seed=seed)\n",
+                "    wash_inputs = rng_signals.uniform(low=0, high=1, size=wash_time)\n",
+                "    train_inputs = rng_signals.integers(low=0, high=1, size=train_time, endpoint=True)\n",
+                "    test_inputs = rng_signals.integers(low=0, high=1, size=test_time, endpoint=True)\n",
+                "\n",
+                "    # Targets to measure the ability to recall past inputs\n",
+                "    train_targets = get_targets(wash_inputs, train_inputs, delay)\n",
+                "    test_targets = get_targets(train_inputs, test_inputs, delay)\n",
+                "    \n",
+                "    # Generate dataset\n",
+                "    signals = (wash_inputs, train_inputs, test_inputs)\n",
+                "    # Put your code here: Build dataset\n",
+                "    #train_data, test_data = ... \n",
+                "    \n",
+                "    # Put your code here: Get optimal weights: Use lstsq from scipy (once you pass the test you can use sklearn and other optimizers)\n",
+                "    # ...\n",
+                "        \n",
+                "    # Put your code here: Get predictions\n",
+                "    #train_predictions = ...\n",
+                "    #test_predictions = ...\n",
                 "\n",
-                "print(f\"Reservoir with {n_particles} {operator}s:\")\n",
-                "print(f\"\\tTrain MC={np.around(train_mc, 3)}\")\n",
-                "print(f\"\\tTest  MC={np.around(test_mc, 3)}\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "3661bae0",
-            "metadata": {},
-            "source": [
-                "To see the perfomance of spins write `operator=\"spin\"`.  _Remember that as shown in the Figure 2 of the paper the wash time for spins is lower than for fermions_."
+                "    \n",
+                "    # Put your code here: Evaluate model memory capacity\n",
+                "    #train_mc = ...\n",
+                "    #test_mc = ...\n",
+                "    \n",
+                "    return train_mc, test_mc\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
-            "id": "02c9dfed",
+            "execution_count": 49,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Reservoir with 4 spins:\n",
-                        "\tTrain MC=0.832\n",
-                        "\tTest  MC=0.852\n"
+                        "Correct!\n"
                     ]
                 }
             ],
             "source": [
-                "# Spin parameters\n",
-                "operator = \"spin\"\n",
-                "wash_time = 1000\n",
-                "\n",
-                "_, _, train_mc, test_mc = mc.main(\n",
-                "    n_particles,\n",
-                "    dimensions,\n",
-                "    J_ij,\n",
-                "    operator,\n",
-                "    delay,\n",
-                "    obs_form,\n",
-                "    wash_time,\n",
-                "    train_time,\n",
-                "    test_time,\n",
-                "    excited_state,\n",
-                "    dt\n",
-                ")\n",
+                "# Parameters\n",
+                "num_sites = 5\n",
+                "dt = 10\n",
+                "wash_time, train_time, test_time = 10, 10, 10\n",
+                "delay = 1\n",
                 "\n",
-                "print(f\"Reservoir with {n_particles} {operator}s:\")\n",
-                "print(f\"\\tTrain MC={np.around(train_mc, 3)}\")\n",
-                "print(f\"\\tTest  MC={np.around(test_mc, 3)}\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "a5074c22",
-            "metadata": {},
-            "source": [
-                "In particular, for this configuration of parameters spins perform better than fermions. But as shown in our paper fermions will in general have better perfomance than spins. In the last section, of the tutorial we reproduce the Figure 3, in which its shown that fermions outperform spins."
+                "train_mc, test_mc = evaluate_performance(num_sites, 2, delay, dt, wash_time, train_time, test_time, seed=2)\n",
+                "exp_test_mc = 0.97094\n",
+                "if np.around(test_mc, 5) == exp_test_mc:\n",
+                "    print(\"Correct!\")\n",
+                "else:\n",
+                "    print(\"Try again\")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "a035b4ba",
+            "cell_type": "code",
+            "execution_count": 5,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Extra: Bosonic reservoir\n",
-                "\n",
-                "The main goal of the tutorial was to explain how QRC work. So, in the previous section we explained the basic componets of this machine learning framework using fermions. In this section, there isn't any new concept related to QRC, we will only explain a few key parameters to build a bosonic reservoir.\n",
-                "\n",
-                "For bosons, there are two new hyperparameters that we can modify: \n",
-                "- `dimensions`: For fermions/spins the Hilbert space only have 2 dimensions, but for bosons there are infinite dimensions.\n",
-                "- `excited_state`: For bosons we are no restricted to inject information only onto $\\lvert 0 \\rangle$ or $\\lvert 1 \\rangle$. \n",
-                "\n",
-                "As discussed in the paper to exploit the huge Hilbert space of bosons the input injection must excite high energy levels to get an optimal performance. Using `excited_state=2`the input injection would be of the form:\n",
-                "\n",
-                "$$ \\lvert \\psi_k^{(e=2)} \\rangle = \\sqrt{u_k}\\lvert 0 \\rangle + \\sqrt{1-u_k}\\lvert 2 \\rangle$$\n",
-                "\n",
-                "As a drawback (at least for the simulation point of view, not experimentally), as the `excited_state` increases, so it does the number of `dimensions`. As it is shown in Figure 1 for an `excited_state=2` (`excited_state=1`) bosons must have at least `dimensions=6` (`dimensions=5`), in other words 6 (5) energy levels. \n",
-                "\n",
-                "_If for instance you use `excited_state=2` and `dimensions=3` the particles in the reservoir will be a poor approximation to the actual bosons_."
+                "# Parameters\n",
+                "num_sites = 5\n",
+                "dt = 10\n",
+                "\n",
+                "# Put your code here: Which wash_time, train_time and test_time seems reasonable to you\n",
+                "#wash_time, train_time, test_time = ... , ... , ...\n",
+                "\n",
+                "# Put your code here: Make a plot with Performance vs delay\n",
+                "# train_mcs, test_mcs = list(), list()\n",
+                "# ...\n",
+                "# ...\n",
+                "# ...\n",
+                "# ...\n",
+                "# ...\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
-            "id": "ffb4da5b",
+            "execution_count": 6,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Reservoir with 4 bosons:\n",
-                        "\tTrain MC=0.608\n",
-                        "\tTest  MC=0.631\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "# Boson parameters\n",
-                "# This cell can take a few minutes to show the results. And even more if `dimensions=6` and `excited_state=2\n",
-                "operator = \"boson\"\n",
-                "dimensions = 5\n",
-                "excited_state = 1\n",
-                "\n",
-                "\n",
-                "_, _, train_mc, test_mc = mc.main(\n",
-                "    n_particles,\n",
-                "    dimensions,\n",
-                "    J_ij,\n",
-                "    operator,\n",
-                "    delay,\n",
-                "    obs_form,\n",
-                "    wash_time,\n",
-                "    train_time,\n",
-                "    test_time,\n",
-                "    excited_state,\n",
-                "    dt\n",
-                ")\n",
+                "# Plot results \n",
                 "\n",
-                "print(f\"Reservoir with {n_particles} {operator}s:\")\n",
-                "print(f\"\\tTrain MC={np.around(train_mc, 3)}\")\n",
-                "print(f\"\\tTest  MC={np.around(test_mc, 3)}\")"
+                "#plt.figure(figsize=(5, 4))\n",
+                "#plt.plot(delays, train_mcs, \"--o\", label=\"train\")\n",
+                "#plt.plot(delays, test_mcs, \"--o\", label=\"test\")\n",
+                "#plt.grid()\n",
+                "#plt.xlabel(\"Delays\")\n",
+                "#plt.ylabel(\"Performance\")\n",
+                "#plt.legend()\n"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bf8afab2",
             "metadata": {},
             "source": [
-                "## Extra: Reproducing Fig. 3\n",
+                "### Exercise 3 - Define your own model\n",
                 "\n",
+                "Build your own reservoir and evaluate performance.\n",
                 "\n",
-                "Previous results are not statistical relevant since the performance is based one only one realization of $J_{ij}$.  However, it can be a bit time-consuming to run these code from `seed=1`to `seed=1000` to reproduce exactly the same results as in Figure 3. For this reason, we have shared this information in the `data` folder. Now, we will simple upload and plot the results of Figure 3.\n",
-                "\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 26,
-            "id": "53d36d37",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "def get_path(foldername, test_data):\n",
-                "    \"\"\"Generates the path to train or test data location\"\"\"\n",
-                "    REPO = pathlib.Path().cwd().parent\n",
-                "    data = \"test\" if test_data else \"train\"\n",
-                "     \n",
-                "    return REPO / \"data\" / \"memory_capacity\" / foldername / data\n",
-                "\n",
-                "def upload_data(foldername, test_data=True):\n",
-                "    \"\"\"Upload the memory capacity for differents seeds between 1 and 1000\"\"\"\n",
-                "    data_path = get_path(foldername, test_data)\n",
-                "    return np.load(str(data_path / \"range_1_1000.npy\"))\n",
-                "\n",
-                "def rename_folder(foldername, delay):\n",
-                "    \"\"\"It changes the delay value from the foldername configuration\"\"\"\n",
-                "    split_str = foldername.split(\"_\")\n",
-                "    split_str[3]=str(delay)\n",
-                "    return \"_\".join(split_str)\n",
-                "\n",
-                "def plot(x, y, fmt, color, error_bars=None):\n",
-                "    if not isinstance(error_bars, type(None)):\n",
-                "        error = np.abs(error_bars-y)\n",
-                "    \n",
-                "    tick, _, _ = plt.errorbar(x, y, yerr=error, fmt=fmt, color=\"black\", ecolor=\"black\",\n",
-                "                 elinewidth=1, markersize=9, markerfacecolor=\"black\", markeredgecolor=\"black\")\n",
-                "    plt.fill_between(x, error_bars[0], error_bars[1], alpha=0.6, color=color)\n",
-                "    plt.grid()\n",
-                "    background = mpatches.Patch(color=color, alpha=0.6)\n",
-                "    return tick, background"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 46,
-            "id": "43a822c1",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Parameters (change the foldername to upload spin or boson data)\n",
-                "delays = [1, 2, 3, 4, 5, 6, 7, 8]\n",
-                "foldername = \"4_2_fermion_1_ij_3000_1200_300_1_10.0_1_0.0_uniform_(0.0, 1.0)\"\n",
-                "test_data = True\n",
-                "\n",
-                "quantiles_1, quantiles_2, quantiles_3 = np.zeros(len(delays)), np.zeros(len(delays)), np.zeros(len(delays))\n",
-                "for idx, delay in enumerate(delays):\n",
-                "    # Compute the quantile for memory capacities with different delays\n",
-                "    foldername = rename_folder(foldername, delay)\n",
-                "    test_mc = upload_data(foldername, test_data)\n",
-                "    q1, q2, q3 = np.quantile(test_mc, [0.25, 0.5, 0.75])\n",
-                "    \n",
-                "    # Store data into the quantiles arrays\n",
-                "    quantiles_1[idx] = q1\n",
-                "    quantiles_2[idx] = q2\n",
-                "    quantiles_3[idx] = q3"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 47,
-            "id": "a6d51c67",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAXQAAAD4CAYAAAD8Zh1EAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8qNh9FAAAACXBIWXMAAAsTAAALEwEAmpwYAABFHElEQVR4nO3dd3hUZdrH8e9zprf0TqgBQg8lQKihSBMUXQWsuBZQV0XFvvvad1fXRVFXdC3r2lAUFQsiIiWh995Cb+mQAOltnvePhCxiCCEkmTnh+VwX10VmzmR+M4R7Tu7znPsIKSWKoiiK/mmeDqAoiqLUDVXQFUVRGglV0BVFURoJVdAVRVEaCVXQFUVRGgmjp544KChItmjRolaPzcvLw+Fw1G2geqSnvHrKCvrKq6esoK+8esoKl5Z3w4YNx6WUwVXeKaX0yJ8ePXrI2lqyZEmtH+sJesqrp6xS6iuvnrJKqa+8esoq5aXlBdbL89RV1XJRFEVpJFRBVxRFaSQuWNCFEB8KITKEENvPc78QQrwphNgnhNgqhOhe9zEVRVGUC6nJHvpHwMhq7h8FtKn4Mxl459JjKYqiKBfrggVdSrkUyKpmk7HAJxX9+tWAnxAivK4CKoqiKDUjZA2GcwkhWgBzpZSdqrhvLvCylHJ5xdeLgCeklOur2HYy5XvxhIaG9pg1a1atQufm5uJ0Omv1WE/QU149ZQV95dVTVtBXXj1lhUvLO3jw4A1Sytgq7zzf8pez/wAtgO3nuW8u0P+srxcBsRf6nmrZonfSU1Yp9ZVXT1ml1FdePWWV0ruXLSYDTc/6OrLiNkVRFKUB1UVB/wGYWLHaJQ44JaVMrYPv+zvZ2dm8//77PPDgFP743J+Yv2MpR06nUlJWWh9PpyiKoisXPPVfCPEFMAgIEkIcA54FTABSyn8D84ArgX1APnB7XYeUUvLMM88wbdo0DAYDeXl57EraxWcvvU/7a3vR9ZYBNPONoENgFK39mhLpE0aYPRCDZqjrKIqiKF7rggVdSnnjBe6XwH11lqgKzzzzDK+99hqFhYWVt5UVle+V7/5+HU6TDefEeH45tIL50o1AoAmNln5N6BAQRSu/pkS6Qgm2+6MJdS6VoiiNk8eGc9VUdnY206ZN+00xP1tpYQnrvkqk54TBhLmCKm8vc5eRmnuc/dnHAIkEzAYTUb5NaR/Uila+kTR1heFv9UEI0TAvRlEUpR55fUH/+uuvMRiqb51omkZS4hZixsRV3mbQDPhYnPhY/rc0qNRdyuGcFHae2I8mBBKwGa209W9G+8AomvtGEOkKxdfsVEVeURTd8fqCnpaWRn5+frXblBQVk5eVc8HvZdSM+Fpc+FpclbcVl5WQlH2YzZlJaGi4ceNjdtI2oDkdAqNo5gon0hWK02y/5NeiKIpSn7y+oIeFhWG328nLyzvvNgJBbuapWn1/s8GE2WDCHx+g/ABscVkJ2zP3sT51OwbNQJnbTaDNj7YBLegQ2IqmrjCaOEOwmay1ek5FUZT64PUF/frrr2fKlCnVbiOROPzLWyslhcUcWr+HVr3bYTBd/MsTQmAxmrEYzYBv+feXksKyYjak72BV8mY0oSFxE2IPpH1AK6IDWxLpCiXCGYzFYL7o51QURakLXl/Q/f39efTRR3nttdeqbL0YrSZirx9In4nDANi/aic/Pv8pNh877YZ0o+OIWMLaNb2knrgQApvRgs1oqbxNSklBaSErUjaRcHQdmqYhpZsmzlDaBbairX9zmrrCCHdWfWERRVGUuub1BR3ghRdeAPjNOnSj1YR0S2LHxdP/jpGVBbvNgM5c9/Jd7PhlPVt/WsOm71bg3zSYm/51P3a/upv1IITAbrJhN9kqb3NLN6eL81hyZC2LDq9CCA2kJG/mfixt/OkaEq3aNIqi1BtdFHQhBC+++CJTp07l66+/ZvLkycTdPYJuV8Rhddl+s63BaKBVXHtaxbWnKLeApMStHNt6AJtv+fX71n2ViNVppW18DBZH3RZXTWg4zfbfHEAtk24+/eJlbDe1wqgZ6RfZlfjIWFr7N1Nr4hVFqVO6KOhn+Pv7M2nSJCZPnky7UT2wWm3Vbm9x2ugyujddRvcGytskuxdtIi3pKAtf/5bW/TvRcUQsLXq0RTPWz1mlhoqiHeEKodRdyvJjm1h6dD3+Vl9GtOhH7/DOBNn96+W5FUW5vOiqoF8qIQS3/PtBUncdYceC9exevJndizfT68bBxN895sy0yHpbg27UjIQ6AgHILylg1u55fLFrHu0DWzG8RV86B7fFalQHVRVFqZ3LqqBDebGO6NCciA7NGXLfWA6s3kVg81AAjm05wMI3vqXjiFjaD+2OK9i33nKc6b+7peTQ6RTe2PgZZs3IgMgeDIjsQZTfpR3IVRTl8nPZFfSzGUxG2gzoXPm1lBKTzULiv+eS+O5PNO/Rho7De9BucNdaLYGsCU0I/K0++ONDSVkpS46sY9GRNQTb/Bneoi+9w7sQYKu/DxZFURqPy7qgn6tZt9bc8vYUso9lsmPBBnYu2MCSGT/QbnBXAE6mnsAnxB/NUD8HM00GI2HOIKSU5JcWMnPXT8zc9ROdglpzRfM+dA5uo9a5K4pyXqqgV8E/Mpj+d4yk3x+Hcyo9G4PJiHS7+erhf1NWWkaHYd3pODyWoJZh1X6fwpx8khK3ArBl7mqi47tgdV14hIAQAofJhsNkwy3d7Ms+yo7j+7AYzAxsGkv/Jt1p6dtEtWQURfkNVdCrITQNv/Dyg5hSwsC7R7NzwQbWfZnI2i+WENo2kv53jKRVXPvfPE5KyfIP57PuywQ0rXxvfslb37PozTn0nDDoN+vmL0QTWmXLpbishIWHVrHg4EpCHYGMaNmPnmGd8Lf61OGrVhRFr1RBryHNoNFucFfaDe5KXnYOuxdtYseCDbjLygA4lZpF6q7DRPXrxOrPFrJ+diJlxaWUVTy+pLAYgPWzEwEYcOeoi85gNpgIcwYjpSSvpIBPtv/Apzt+JCa4LUObx9ExqDVmg6lOXq+iKPqjCnotOPxd9Lh+ID2uH1i51HHX4k0se38eJruF0sJipFtW+djSwhLWfZlAz/GDfndSVE0JISpPYHJLN7uyDrIlcw8Wg5nBzXrRP7IbzVzhqiWjKJcZVdAv0Zmi2euGwYS3a8qy/8wndefhah9T1fz22tKERqDND4CismJ+Obicnw8sI8IZwoiWfYkN64Svpe5GHiiK4r1UQa8jmkGjeY+2JO84fMGCXtP57RfLYjBXtmRySvL47/bv+Gj793QPac+Q5r3pEBiFyaD+yRWlsVL/u+uYI8CFyWqu7JlXxWgx4whwnff+SyWEwGV24DI7KJNuth3fy4aMndiNVoY2703fiG5EukJVS0ZRGhlV0OtYdHwXFr05p9ptSguLcZeU4i5z19ua9jMMQqucFVNUWsxP+5fy475EmvqEMbxFX2LDOuIyO+o1g6IoDUON+6tjVpednhMGYbRWvdrEYDLiCHCx7D/zKc6v+sLX9cViLG/JhDuDyS48zX+2fct9v/6NNzfMZHvmXkrdZRf+JoqieC21h14P+t8xEqByHXpJYTEmqxm3203PCYPod/sITiafwOqyI91uFkz/hs4jexHRsXmD5BNCVF5Au8xdxqaMXaxN24bTZGeEuytZhacIsKpxA4qiN6qg1wMhBAPuHEXP8fEkJW5lwbTZDL5/LNHxMZVLFQOall/J6GRKFvuW72Drj6tpM7AzA++6koBmIQ2W1aAZCLYHAFBYWsRHH37ED3It46JHMLR5bzVqQFF0RLVc6pHVZa9cmhgz5vcX4wDwjwxi0syn6Hf7CA6t28OHf/wnC179mqK8hm3HAFiNFn74cg4+Fief75zL4wmvsTljd+Vae0VRvJsu99An3HwjBSWFlLnLCLT56X61htluoe9tw4m5ug+rP13I4Y17MVrKe/BSygZ/fRaDmQhXKKeLcnllzYd0Dm7DrR2vItJV/ewaRVE8S5cF/Z67JtOye1u+2DmPrcf34DDZ8bO4dF/YHf4uhk65lrKSUgxGA8UFRcz805t0vrI3Xcf2xWhu2H8uH4sTl9nBnuzDPLn0dUa26MfYNkPUqhhF8VK6bbk094ngid538pe4uwmy+ZGcm0Fucb6nY9WJM7PXC3PycQS4WDLjez6c+A92LNiAdLsbNIsQgmB7ACH2QH45tJKHF/+DJYfXqBUxiuKFdFvQobzYdAyK4m8DpvBg95sxCI3knAwKS4s8Ha1O+IT4M/7Vexg3bTIWl415f/+cjydNp+B0w39wGTUD4c5gbCYbH2z7lj8vfZ2dJ/ar/rqieBFdtlzOpQmN3hFd6BbansSj6/lq93yyCk4RbA9oFKe6t4iNpnn3NuxesoVD65IqD67mnjiNM7BhR+fajBaauEI5WXiav658j14Rnbix3ZWV10pVFMVz9F/tzmI2mBjWog99m3Tl5wPL+HF/AlJKgu0BGDSDp+NdEqFptB/ajfZDuwGQk3GSD259mai+HRhw55X4RwY1aB4/qw8+Fheb0naxMW0XV7cexOhWA7GZrA2aQ1GU/9F1y+V8HCYb10cPZ/rgJxjYNJb0vBNk5GXhbkTtAYvTSs8bBnFg1S4+vO0f/Pr6N/Uy8Ks6mhCEOoMItPnx/b7FTE34J6uSt+CWDdvnVxSlXKMs6GcE2Hy5q8t1vBz/EJ2CWpOam0FWwalG0fc12630v30kd818ii5j4tjyw2o+uPVlj/TXTQYj4c4QNKHxr40zeW7F2+w/ebTBcyjK5a5RtVzOJ9IVxiM9b2NP9iFm7vyJ/SePVi7J0ztnoA/DHr6OHtcP5PDGvdh8yq9ZemDNLpp3b1O5YqYhOEw27EYrKbmZPLP8LQZE9mB8uxFqjICiNJDLoqBD+YqY6ICWPN/vPjak7+SznXNJzkknwOrbKPq+AU2DK8cJnDiczjdPfIBvRCAD7hxFu8ExCK1hfhkTQhBg88UtXaxM2cSalK1cFz2MYS36qDECilLPGnXLpSpCCGLDOvLP+Ee4q8t1FLtLSMnJoLisxNPR6kxAsxCuf2USZpuFuS9+xqf3vMGh9XsaNIMmNMIcwfhYnczaPY/HEl5lY/quRtHuUhRvddkV9DNMBiODm/Xi9cFPMC56OKcKc0jLy6SsEZwwI4SgZa923Pb+w1z555soOJXHd09/RGFOw/fXLQYzEc5QStylvLruI15a8z7HctIaPIeiXA4um5bL+dhMVsa2GcLAprH8uD+BhYdWIYRGsN0fTej7805oGh2H9yB6UAwZe5PLx/VKyYqPfqHTiJ74Rfxv7XhhTj5JiVsB2DJ3NdHxXbC67HWWxWV24DTZ2Zd9lCcTX2d4y75c22ZooziOoSjeokYFXQgxEngDMAAfSClfPuf+ZsDHgF/FNk9KKefVbdT65W/1YWLHqxnWvA+zk35hTeo2rEYLAVZf3c+IMZqNlbPWs45ksG5WAmtmLqbr2L7E3TKUjd8ur5zdDrDkre9Z9OYcek4YRP87RtbZ6xdCEGT3p8xdxsJDq1h6dD03tr+S+KY9Mer8PAFF8QYXLOhCCAMwAxgGHAPWCSF+kFLuPGuz/wO+klK+I4ToAMwDWtRD3noX7gxmSo9b2Jd9hJm7fmJP1iGcZge+Fqeno9WJwOahTJr5FCs+XsCmOSvY/P1KkBJ3mZszzaYz10NdPzsRgAF3jqrTDAbNQJgzmMLSIj7cNoefDy7n9k7X0iGwle4/PBXFk2rSU+gF7JNSHpBSFgOzgLHnbCOBM+eg+wIpdRfRM1r7N+OZPvfweK87cJpsJOekk19S4OlYdcIZ5MuIR8Zx01v3I91u3GVVnwhUWljCui8TKMypn9dtrRgjcLooj7+vfo/p6z8lPe9EvTyXolwOatJyaQKcfZbIMaD3Ods8BywQQjwAOIArqvpGQojJwGSA0NBQEhISLjJuudzc3Fo/tjauEj3JteSTVXCKsjw3Rs2AdpF7kjE5TeopXe1l7dyN2WSmqOj8w8yMwkD+L4fpPWJovWaRQGlqGT+nzMfX4sLX4qrRe9zQPwuXQk9ZQV959ZQV6i9vXR0UvRH4SEr5qhCiD/CpEKKTlL89B1xK+R7wHkBsbKwcNGhQrZ4sISGB2j72UhSWFrPw8Cq+3bOQEncpwXZ/jFrN3sItruR6TnfxducfrbaYAxQVF7E7/ygBDZS/xF1KZl4WTs3OrR2vok9ETLUHpz31s1AbesoK+sqrp6xQf3lr0nJJBpqe9XVkxW1nuxP4CkBKuQqwAg07LaoBWI1mxkTF8/qQJxjZsj/H87NJyzuu29kljgAXJmv1J/uYLGYcAa4GSgQmzUiEKwSjZmDGpi94ZvkM9mUfabDnVxQ9q0lBXwe0EUK0FEKYgRuAH87Z5ggwFEAI0Z7ygp5Zl0G9iY/Fyc0dRjNt8GP0CY8hNTeT4/nZujtpJjq+C+4LXDCjtLiE6PiYBkr0P3aTjSbOUNLyjvPsihn8e9OXZBWcavAciqInFyzoUspS4H7gF2AX5atZdgghXhBCXF2x2SPAJCHEFuAL4I9Sb9WtFkLsAdzbbQJ/GzCFNv7NSM7N4GThad0UdqvLTs8JgzBaTVXebzAZ6Hp1X6wum0de05kxAuHOYFalbmHqklf4cX8CRWXFDZ5FUfSgRg3gijXl88657Zmz/r4T6Fe30fSjhW8Tnux9FztO7OfTHT9yLCcNX4sLp7nuTsypL/3vGAlQuQ69pLAYk9WM2+2uXIcupWTuC58R1q4psePjG3xpoSY0Qh1BFJeV8OWu+Sw4uJLbOo2lR2iHBs2hKN7usj9TtK4IIegU1JqXBj7I2tRtzNz5E8k56QTa/DwdrVpCCAbcOYqe4+NJStzKgmmzGXz/WKLjYyqvjFRaVEJZWRkJ7/xIys7DjHpiAmZ7ww80MxtMRLhCyCnOY/r6T+gQGEUvd6sGz6Eo3krf57Z7IU1oxEXEMG3wo9zWcSz5JQWMnXCt1x84tbrsxIyJAyBmTFxlMQcwWkyMff424u8Zw95l2/j0njc4cTjdU1FxmR1EOEPYf/Iob733Nt/sWdiohqspSm2pgl5PLAYzw1v25fUhT3LzbbeSkpNBYal+e79CCHrdMJjxr95D4el8vnnqP7hLPTfI7MwYgR++nMOcPQv587I31GoY5bKnCno9c5rtBNv8uafreE4Vndb9So1m3Voz8b2HGf2Xm9CMhvIzTT1Y2AEiXCGcKsrluRUz+GLXPF1/cCrKpVAFvYEMbBrLX/tPwcfsIDU30+tbMNVxhfjRpGMLAFZ9upCvHnm3wa9nei5/qw8hjiB+OrCUJxJfY/eJgx7NoyieoAp6A2rqE8ZfBzxAXHgXUnIyKGoEe5K+4YGk7j7CJ5NfI3m7Z4uoUTMQ4QyhsKyYF1b9mw+3zWk083cUpSZUQW9gdpONP3W7gUkx15NdeIrswtOejnRJOg7vwc1vT8FoNjHrwbfZ+O0yj6/D97U4CXcEseTIWh5LeJWtmXs8nklRGoIq6B4ghGBws1680P9+HEZrRQtGvwUnJCqCW999mJa927Fkxg9kHcnwdCQMmoFwZzBuJC+v/oB3t3zF6aJcT8dSlHqlCroHtfBtwt8GPkjPsE4k56Tr+gxIq8vGtX+9nZtmPEBg81AACk43/CXvzuUyO4hwhbAyZTOPJbzKutTtam9dabRUQfcwh8nGA91v4vZO15BVcIqThZ49uHgphKYR3q4ZAHuXb+f9G//G3uXbPZzqfxesNhqMTF//CW9u/IysQn2vNlKUqqiC7gWEEAxv2Zfn+92H1WgmLS9T93uRIa0j8I8M5rv/+y9L35933otoNCSHyUaEK5SN6bt4LOFVVhzbqPv3WVHOpgq6F2nlF8nfBzxIt5D2JOek6/rsR9+wAG588z66XBXHmpmL+Prx98g/6fketiYEoY4g7CYrMzbP4pW1/yUzP8vTsRSlTqiC7mWcZjsP9riFWztexfH8bE7p+ECe0WJixCPjGPn4eI5tPciBNbs9HamSzWiliTOUXSf283jiayw+vEbX5wYoCqjhXF5JExqjWg2gjX9zpm/4lLTcTEIdQbq9gHLnK3vTrFsbfMMDAMg+dhy/JoEefz1CCEIcgRSWFvPB1m9YnryJSV2uI9wZ7NFcilJbag/di7X2b8ZLAx6kc3BbknPSKdFzC+asYv7xXa8y/x9fUlLkHa/HajTTxBXKwVPHeHLpdOYdWEap27PjDBSlNlRB93I+FieP9LyNmzqMJjM/W/drqX3DA4idEM/2+ev4/L43OZlywtORgPK99WB7AP5WXz7b+SPPrZjB0dNpno6lKBdFFXQd0ITGmKh4nu57N5rQSM87rtvVGZpBo//tI/nDS3dyKi2bTyZP58DqXZ6OVclsMNHEGUpq3gn+suwNvtu7WNcHp5XLiyroOhId0JK/D3yQDoFRJOemU+Iu9XSkWovq04GJ7z2MT6g/B9d6z8FSKN9bD7T5Emjz5+ukX3h62b84cPKYp2MpygWpgq4zfhYXj/b8IxOiR5KRd4Kc4jxPR6o1v4hAbp7xAIPuvQqA44fSvOLs0jNMBiMRrlCyik7zzPK3mLXrZzWaV/FqqqDrkEEzMLbNEP7SZzJSStLzTui2BWOymjGYjLjL3Hz39Ed8Onk66Xu8a2+4fDRvIHP3J/DU0ukkZanRvIp3UgVdxzoERvHSwIeIDmhBcm46pTpuwWgGjSufuhF3WRkz7/sX235e6+lIv2HUDES4QskvLeSFlf/m4+3fq9G8itdRBV3n/K0+PN7rDq5rO5z0vBPkFntPy+JiRXRozsT3p9Kkcwvm/+NLfpk2m9Ji7/qQ8rW4CHME8evhVTye+BrbMvd4OpKiVFIFvREwagaua3sFT8VNotRdRoaOWzB2PyfjXplM75uGcDLlOJrmfSdTGSoupFEm3by0+j+8u3m2ro9lKI2HKuiNSKeg1rw88CGi/JqSkpuh25NjNKOBgZNHc/0rk9GMBvKycji8wfv2hMtH8wazInkjjyW8yvq0Hbr9IFUaB1XQG5kAmy9PxU3imtZDSMvL1HULxmA0ALD8v/P56tH3WP3ZQqS7fN5KYU4+W+auBmDL3NUU5njmdWpCI8wZjEEz8Nr6j/nXxs85WaTfEciKvqlZLo2QUTMwrt0I2ga0YMamz8nIO0GwPcDjs1Nqa/CfrqakoIhlH/xM8o5DBDYLZeOc5Wha+f7Ikre+Z9Gbc+g5YRD97xjpkdfpMNmwGa1sSN/BtuN7uL3TtfSJiNHte67ok9pDb8RiQqL5+4CHaOEbQUpuOmU6bcGYbRZG/+Vmhk65lgOrd7HuywTKikspKSxfE15SWExZcSnrZyey/MP5Hst5ZjSv1WDhrU1fMG3dfzmen+2xPMrlRxX0Ri7I7s9f4u5mTNQgUnMzydPpUjshBB2Gda9sw1SltLCEdV8mUJjj2ddoM1lp4gxh+/H9PJb4KkuOrFWjeZUGoQr6ZcBkMHJj+yt5rNftFJUWkZmXpcuDd0mJW9EM5y/oAJqmkZS4pYESnZ8QglBHIC6zg/e3fM1Lqz/Q9XkCij6ogn4Z6Rbanr8PfIgmrhBScjN014LJy8qpbLOcT0lRMXlZ3nNQ0mq00MQVyr7sI7z1/jssPrxGlx+mij6ogn6ZCbEH8EzfexnVsj+puZnklxR6OlKNOQJcmKzmarcxWcw4AlwNlKhmhBAEOwL4fta3fLDtG15b/4mur0SleC9V0C9DZoOJWzpexdTYieSXFOjmwF10fBfc7up70WUlpUTHxzRQoovXxBnKlszdPLl0OjuO7/d0HKWRUQX9MhYb3om/D3yQcEcQKTkZlHn5gTury07PCYMwWk1V3i8MGp2u7IXVZWvgZDUnhCDMUX6Ju7+tfo8vds1T89aVOqMK+mUuzBHEM/3u5YoWfUjJyfB0nAvqf8dIYsfFYzAbK9svJqsZg9lI75uGMHzq9UgpWfbBPK+b2ng2l9lBuCOIn/Yv5bkVb5Oc6/3vveL91IlFChaDmds6Xk27gBYU3LCfrIJTBNh8PR2rSkIIBtw5ip7j40lK3MqCabMZfP9YouNjKvfM80/msmPBBtZ9mcgVD/2BLqN7ezh11QyagQhXCOl5J/jL0jf4Y6driG8aq05GUmpN7aErQHmhjIuI4b5J9+I02bz+MndWl52YMXEAxIyJ+02bxe7nZOJ7DxMZ04pf/vkVP/9jltdckLoqgXY/fCwu3tsymzc2fKb768YqnqMKuvIbJs3I8/3vp6VvJCm5Gbo9Icbu5+T6f0yiz8RhbP95Hd88/r53f0AZzTRxhbIxfSdPLp3OzhPqgKly8VRBV37H1+Lkqbi76NekGyk5Gbo9IUYzaPS/o/yC1LET4r2+lSGEIMwZjAT+tuo9vtz9MyVl+nzvFc+oUUEXQowUQiQJIfYJIZ48zzbjhRA7hRA7hBCf121MpaFZDGbu6Tqe8e1GkpZ7nILSIk9HqrWoPh1o3bcjABu+WcbS9+fhLvPe3zxcZgehjiB+2JfAcytmkJKb6elIik5csKALIQzADGAU0AG4UQjR4Zxt2gBPAf2klB2Bh+o+qtLQNKFxTZshTOlxM6cKTzeK3m7W0QzWzFzE7MfeIy/be84oPZex4iIaqXkn+PPS10k8ss6rW0aKd6jJHnovYJ+U8oCUshiYBYw9Z5tJwAwpZTaAlFKtwWpE4iJieKbvvUikbk5COp9hD13HyCcmkLL9IJ9Mmk7KjsOejnReQgiC7H74WJy8u2U2b26cqa6MpFRLXOhTXwhxPTBSSnlXxde3Ar2llPeftc13wB6gH2AAnpNS/m6OqRBiMjAZIDQ0tMesWbNqFTo3Nxen01mrx3qCnvJWl7XUXUZ6/nFKykoxGox4Q0f6lqtu4LMfL/7n6ND+g7z58nSyT2Tz2vtv4B8YUA/pfqu2WQEkUOouRRMGQuwBWA3Vj0CoC43l59YbXUrewYMHb5BSxlZ1X12tQzcCbYBBQCSwVAjRWUp58uyNpJTvAe8BxMbGykGDBtXqyRISEqjtYz1BT3kvlDWvpIAZG79gS+YWwpwhGITnj6tvcSVf/IO6mpnw/gMc3rCXIy0KOEIy7jI3mqF+X0+tsp7ldFEuOQV5XNN6CNe0GYrJUH+nkjSmn1tvU195a/LTmww0PevryIrbznYM+EFKWSKlPEj53nqbuomoeBOHycbUnrcxrEU/UnIydH3autVlJ3pQ+dyXQ+uT+HjSa5w4nO7hVNXzsTgJdQTx3b7FvLDq36TlHfd0JMWL1KSgrwPaCCFaCiHMwA3AD+ds8x3le+cIIYKAtsCBuoupeBOjZuC2jldze6dryMzP0u1FM86mGQzkZ+Xw6T1vkJTg+Xnq1TlzwDQ5J52nlr7O8mMb1QFTBahBQZdSlgL3A78Au4CvpJQ7hBAvCCGurtjsF+CEEGInsAR4TEp5or5CK54nhGB4y7481vN28ksKyC487elIl6RZt9ZMfO9hgluF8cNzn7B4xveUlXrvvPjyA6b+uMwO3t40i7c3zdL1BcGVulGjhqGUcp6Usq2UMkpK+beK256RUv5Q8XcppZwqpewgpewspazdkR9Fd7qGtuP5fvdhNZjJyDuh6z1FV4gfN7z+J7r/oT8bZi8laclmT0e6IKvRQoQrhDWpW3lq6eskZR30dCTFgzx/REvRvWY+4Tzf/z6a+oRXjAvQb1E3mIwMnXItN7zxJ9pf0R2AolzvbilpQiPMGUyJu5QXV/6br5N+pVRnV6NS6oYq6EqdCLD68pe4ycRFdCE5J133BaVpTBRCCE6mnOD9m/7Omi8We/1vHz4WJyGOQObsXciLK/9Nep7qel5uVEFX6ozVaOa+bjfyhzZDScvNpLC0+ut/6oHdz0Gz7m1Y+u5PfPf0R16/t27UjEQ4Qziak8pTS19nRfImr/8gUuqOKuhKndKExrh2I/hTtxvILjyp+zMbzXYrVz17K4PvG8uBVTv55O7Xydif4ulY1So/YBqAw2xnxqYveGfzl41iJZJyYaqgK/Wif2R3/q/P3ZS5SzmRf9LTcS6JEILYcQOZMP1eSgqL2fTtck9HqhGb0UKEM4RVKVt4aunr7M323jEHSt1QBV2pN9EBLXmh/wP4WV1ef8GMmojs0orb3p/KkAeuAeB0ejalxd493lYTGuHOYIrKSnh+xTt8t3ex7o9vKOenCrpSr8IcQTzX709EB7TU9QUzznAEuDBZzZSVlvH14+/zxZS3OJWW5elYF+RrcRLiCGB20i/8ddW7ZOR7f2bl4qmCrtQ7l9nBYz1vZ3CzXqTkZFCi43EBZxiMBgbcNYqso5l8Mnk6B9fu9nSkCzpzwPTwqRSeTJzOqpQtuv+tSfktVdCVBmEyGLmz8x+4ucNo0vNPkF9S6OlIl6zNgM5MfPchXMG+fP3EB6z46Bek27t/AxFCEOwIwGGy8a8NM3l3y1fkqwOmjYYq6EqDEUIwOiqeR2L/SG5xHicLvfcCEzXlHxnMzTOm0GFYdw6u2U1ZqXcX9DNsJisRrhBWJG/iqaVvsC/7iKcjKXVAFXSlwfUI68Cz/f6EUTOQ2Qh6uSarmSufupHxr96N0WykMCeftKSjlfcX5uSzZe5qALbMXU1hjnfMXCk/YBpCYVkRz618m+/VAVPdq79hyopSjZa+Tfhr/weYtu4jjuSkEu4I9vqLOFdHCIHZbgUg8d2f2PHLOgbffw25mSdZ91Uimla+77Tkre9Z9OYcek4YRP87RnrFa/a1uLAbbXyZNJ8tmXu4t+t4gu31f8EPpe6pPXTFYwJsvjzd5266h7QnOSedskaydzhw0pU07dqahdO/Yc3nSygrLqWksPys2ZLCYsqKS1k/O5HlH/7uol4eYzIYaeIM5cDJozy59HXWpmzzdCSlFlRBVzzKZrLyYI9buCoqntTcTIrK9D8uwObrYPRfbkIYtPMeJC0tLGHdlwkU5njPAUkhBCGOQGxGK69v+JQZ779DVsEpT8dSLoIq6IrHGTQDN7S/kskx4zhRcLJRzPXeu3w7RlP1HU1N00hK9L6LadgrDph+/flXTF3yCt/vW9wo5vJcDlRBV7yCEIJBzXryVO9JFJUV637PMC8rp7LNcj4lRcXkZXnnSh+t4lqxflYfZu9ewCNLXmFNylbdnxjW2KmCrniVjkFRvND/fpxmu67HBZw5o7Q6JosZR4CrgRLVjtlgIsIVggTe2DiT51e8w/6TRy/4OMUzVEFXvE4TZwjP97uP1n7NdDsuIDq+C+4LnGRUUlSMf0RgAyW6NE6znSbOEI7lpvPM8rf496YvOVFw0tOxlHOogq54JV+Lk8d738GAyB7l4wLc3j0E61xWl52eEwZhtJqqvN9gMmCymFn05ndef3bpGUIIAm1+hDuDWZmypby/vlf1172JWoeueC2LwczdMeMIdwTxZdJ8Am3+2IwWT8eqsf53jARg3ZcJaJpGSWExJqsZt9tNzwmD6Dk+nrysHISmUZxfyMF1e2g7sLNXrE2vTvkl74IoLithdtICFhxaya0dr6JXeOfK3rviGaqgK15NCMHYNkMIcwQxY9Msik0l+Fqcno5VI0IIBtw5ip7j40lK3MqCabMZfP9YouNjsLpsQPmePMDmH1aR+O+5tOgZzRUP/QH/JkGejF4jZ/rrucX5vLlxJq39mjGx49W09m/m6WiXLfVxquhC74guPNvvXgRwXGfjAqwuOzFj4gCIGRNXWczPFjsunqFTriFlxyE+uv2frPrkV6+ftX5GeX89lJTcTJ5dMUP11z1IFXRFN6L8mvJi//sJtgeQmpup2xUwVdEMGt3/MIA7P3mCqL4dWf7hfBa98a2nY9WYEIIAmy/hzmBWVfTXv9u7mILSIk9Hu6yolouiK8H2AJ7tey9vbfqCzeneP4P8YjmDfLn6uYkcWLOrsu2Se+I0QhM4/L17iSOU99dDnUGUlJXwdUV/faLqrzcYVdAV3bGbbEyNvY0vds0jb8I+ThXl6qavXlOterev/PuiN+dwZONeBt49hi5X9kJo3l8YTRX99bySAtVfb0De/5OhKFUwagZu6TCGe++6G6fJRnJOOoWN9Nf7/neMJLhVBAumzebzKTPIPJDq6Ug15jDZftNff3vTLI7nZ3s6VqOlCrqiW0IIrEYLLw98mNs7XUteSQGpuRmNZmrjGYHNQ5nw+r2MevIGso9m8smk10hK3OrpWDV2dn99Teo2Hkn4p+qv1xPVclF0z2QwckWLOHqGd+K7vYv49dAqzAYTgTY/r1/TXVNCCDqN7ElUnw6s/ORXmnWNAqAorxCLw+rhdDWjCY1QRyAlZSV8k7SABYdWcGuHq+kdofrrdUW9i0qj4Wtxclunsbw08CGi/JqSnJtOTnGep2PVKZuvg6EPXIPN14G7zM2XD7/Dd09/xOkM/bQxTAYT4a4QhND416bPeXbFDHUJvDqiCrrS6DT1CePPcZN4tOftmDUjKTnpjWLO+u9ISfTgGA6u3c2HE19h3VeJuEv1024q76+HkJp7nGdXzGDGpi9Uf/0SqYKuNEpCCLqHtueVQY9wY/vRnC7MJS03kzIdDvo6H81ooPeNQ7jjo8dp2jWKhLd/4JO7X+dUmn5OvDq7v742dTuPJPyTOXsWUVBS6OlouqQKutKoWQxmRkcN5NUhj9E/sjvpuZmcKDjZqE5K8g0P4A8v3cnYF/+I3d+JM9AHQFev8Ux/PcDqyzd7fmVqwj9ZlbxFl5M2PUkVdOWyEGD1ZXLMOF7o/wCRzlCSc9PJK/Gey79dKiEEbQd0Zvy0uzGYjBTnF/Lp3a+z89cNuirsZ9avaxX99WeWv8Xe7MOejqUbqqArl5VWfpE82+9epnS/GSklKTnplJSVeDpWnSs4lY9m0Pjpb5/z1SPvknU009ORLsqZ/npa3gmeXfE2b238XPXXa0AVdOWyowmNuIgYXh38GNe1Hc6JwlOk5x1vVL/e+4YHcNNbDzDs4etITzrKR3f8kxX//UVXB03P9NcjnMGsS9vB1IR/8s2ehaq/Xg21Dl25bNmMFq5tO5T+kd2YtetnVqduxW6y4WdxNYr165pBo+vYvrTu34mEd34keftBhEF/+3Bnr1+fs3chCw+t5JaOV9EnIkatXz+HejeUy16wPYAHetzMM33vIcjmS0puRqPaC3QG+jDm/27mDy/dhRCC0xnZ/PyPWeSeOO3paBfFZDAR4QzBoBl4e9Ms1V+vgiroilIhOqAlf+0/hXu6jqeorJiU3AxKdXbpu+oYzeW/kKfuPMKuhRv5cOI/2PT9Stxlv201Febks2XuagC2zF1NYU5+g2etjt1kI8IZQlr+CZ6r6K+XNrJxD7VVo5aLEGIk8AZgAD6QUr58nu2uA74Gekop19dZSkVpIAbNwIDIHnQP7cCP+xL46cBSDEIj2B7QKNowANGDYgiOiuDX6d+wcPo37Ji/jmFTryOkdROWfzi/8pJ5AEve+p5Fb86h54RB9L9jpNe8B0IIAqy+uC0u1qXtYOGnX5MZXsSoVgPws3j/mOH6csGCLoQwADOAYcAxYJ0Q4gcp5c5ztnMBDwJr6iOoojQkh8nGDe1HMbBpLDN3zmVTxi5cZmejGdMb0DSY8a/eza6FG1ny9g9smrMCR6AP62cnUlZcypn93ZLC8jNs189OBGDAnaM8lLhqZ/rrn8yag88t0Sw4uJLRUfGMaNkXl9nh6XgNriYtl17APinlASllMTALGFvFdi8C/wAaT/NRuexFOIN5tOcf+XPvSY1uTK8Qgg7DenDnJ08Qd+sVrPsygdLCqpdwlhaWsO7LBApzvHftfpgzGD+ri+/2LeKhRS/zw74l5Deicw1qoiYFvQlw9Kyvj1XcVkkI0R1oKqX8qQ6zKYpXEELQKbhNox3Ta3XZObxhb2Wb5Xw0TSMpcUsDpaqdMwdOnRYHXyX9woOLX2b+geUUljbCWT5VuORli0IIDXgN+GMNtp0MTAYIDQ0lISGhVs+Zm5tb68d6gp7y6ikrNHxeI3CTZRAni3I4fToXTQgMmoGadpZjcppceCMPOJD6v/bK+ZQWleBK9d7XUFUud7Ekddthvtp+FH+rD06zHVHjf636U18/tzUp6MlA07O+jqy47QwX0AlIqDhgEgb8IIS4+twDo1LK94D3AGJjY+WgQYNqFTohIYHaPtYT9JRXT1nBs3mPnk7jkx0/sOPEPnwtrhr1bLe4ki+4jSfkhIPJaq62qBstJnLCvfc1VJeroKSQrMLT+AknN7QfRVx4DCaD507Dqa+f25q0XNYBbYQQLYUQZuAG4Iczd0opT0kpg6SULaSULYDVwO+KuaI0Nr8b05ur3zG90fFdcLurP1O2rLSMfSt2kL7XOwt6dWwmK01cISAE726ezaMJ/2R1ypZG0zY744IFXUpZCtwP/ALsAr6SUu4QQrwghLi6vgMqijf7zZjedvod02t12ek5YRBGq6nK+41WE817tCF56wE+mfQac/7yIWm7j1a5rTdzmGxEuEIocZfxr42f83jia2xI29loxj7U6HcOKeU8YN45tz1znm0HXXosRdGXM2N6+zSJYXbSApYdXY/FaCHA6us1a7cvpP8dIwEq16GXFBZjsppxu93Ejoun/x0jKcotZOOc5WyYncin97xOj+sGMOSBazwbvBacZjtOs53TRbm8tv5jmrrCuLH9lXQJbqubf6+qqFkuilKHAqy+3B0zjmHN+/Dx9u/Ze/Iw/lZfHCabp6NdkBCCAXeOouf4eJISt7Jg2mwG3z+W6PgYrK7y/FaXjb4Th9HjugFs+m4Fgc1DgfJrm2YeSCWyc0tPvoSL5mNx4jI7yC46zStrP6SVbyQ3tL+SDoGtdFnY1an/ilIPfjum101KToanI9WY1WUnZkwcADFj4iqL+dksDitxNw+lTf9OAGz5cRVfPPAWX059h6Ob9zdo3kslhMDX4qocJ/D31e/x11XvsifrkK5myYPaQ1eUenNmTG9MSDvmH1hO7g17SMvNJMjuj1FrXP/1uo7ti9A01n6xhFkPvU1kTCv6ThxG8x5tPR2txoQQ+Ft98LO4OHQ6hedXvkOX4LaMix5BK79IT8erkcb1U6UoXujMmF6fyZASks/Cw6twS0mQzd+jS+fqktlmoef4eLqO7cvWuatZ+8Vi1nyxRFcF/QwhBIE2P6SUJGUd4unl/6JHWEfGtR1OU58wT8erVuP4aVIUHTAIA7d2vIrRUQNZcHAl8w8up0yWEWjzx2yoenWJ3pgsJnpcN4CYMXEUnMoD4HR6Nj/97XN63zSElr3b6aY3LYQgyO6PW7rZmrGHjWk7iYvowh/aDiPCGezpeFVSBV1RGliA1Zcb2o9iVKsB/HpoJT8dWEZJWQmBdj8sBrOn49UJo8WEK8QPKC/op9Oz+ebJDwiLbkqf24YR1aeDbgq7JjRCHAG4pZt1qdtZnbqVgZE9GNt6CKGOQE/H+w11UFRRPMTX4uT66OG8OfRJxkUPJ684n5ScjEY3dySySyvumvkUIx8fT0FOPnP+/CGf3fsGZTq6HB5UTHZ0BhFqD2RF8mYeS5jGR9u+I6vglKejVVJ76IriYS6zg7FthjCsRR8WH1nL9/uWkFVwEn+bLzajxdPx6oTBaKDzlb3pODyWnYs2cTLlOAajAYCjm/cT2aUl4gLDwbyFQTMQ6gik1F3G4iNrWHx0DSNa9Gd01ECPz2JXBV1RvITdZGNMVDxDm/VmWfJGvt2zkOyCk/hZfbGbrJ6OVyc0o4FOI2Irv07fe4xZD71NYItQ+tx6BdGDuqLp5LqnRs1AmDOYUncp8w8u59dDKxnTaiAjWvX32Cx2fbxzinIZsZmsDG/Rl9eHPMkdna+tWMeeTl4jnO0d3CqCMU/fAsDcF2fy3z++wo4FG3DrqB1j1IyEO4Pxt/rw/f4EHlz0Mt/vW+yRWeyqoCuKl7IazQxpHsf0IU8wOWYcGoKUnAxyivM8Ha3OaAaN9kO7cfuHj3L1cxPRTEYWvvEtxQX6u4iIyWAi3BmMy+JgdtICpix6iZ8PLKOgAS+IolouiuLlzAYTA5vG0ieiK+vStvNV0i+k5KTjNDvwaSSXxBOaRvSgGNoO7EzW0UysLjtSSr57+iOi4trTcUQsBpM+ypXFYCbCGUJhaTEzd/7Ed3sXc330cAY27VHvq5jUHrqi6ITJYKRvk65MG/QoU7rfgtNsJzknnVNFObo7Rf18hKZVzofJP5lL7vFT/DJtNh/c8jKbv19JaXHpb7YvzMlny9zVAGyZu5rCnPwGz3w+VqOZCFcIZqOJj7d/x8OLXyHx6DpKykov/OBa0sdHnqIolYyagV4RnYkN78jmjCS+2j2fozlp2E02/Cwu3azvvhCHv4tb3nmQQ2uTWPHxAn6d/g2rPl3IuGmTCWweyvIP51dOhgRY8tb3LHpzDj0nDKL/HSO95n2wGa3YXFbySwp4b8vXfLNnIVkf76yXC1yogq4oOqUJje6h7ekaEs22zL3MTlrAwVPHsBmt+Ft9vKagXQohBC17t6NFr2gOb9jL1p9W498kqLKYlxWXcubw6ZmrLa2fnQjAgDtHeSh11ewmG3aTjbS848z89DM+++TTOn8OVdAVRec0oRETEk2X4LbsPHGA2Um/sDf7MFadzWOvjhCCFrFtaRHblsKc/MpiXpXSwhLWfZlAz/GDqpwU6WmmehzMpnroitJICCHoGBTFs33v5ek+99DKN5LU3Ewy87MbTY8dIClxa2Wb5Xw0TSMpcUsDJfIeag9dURoZIQTtAlvy57hJ7D95lG/3LmRrxh5MmpFAux+a0Pd+XF5WTrUXswYoKSrmdFpWAyXyHqqgK0ojJYSgtX8zHu91BwdPJTNn7yI2pu3AoBkJtvvrtrA7AlyYrOZqi7qmaayblUBeVg5dRscR3qFZo2g9XYgq6IpyGWjp24SpsRM5ejqN7/YtYk3KNgxCI8juj0EzeDreRYmO78KiN+dUu43QBNGDYti9eDPb5q0lqEUY3a7tR9exfRsopWfo8yNaUZRaaeoTxgPdb+Yfg6bSp0lXMvKzSM89TplbP6faW112ek4YhNFa9Qx5o9VEzxsGM/ovN3PvN88y/NFxmGxmUnYertwmecchpNvdUJEbjNpDV5TLUBNnCPd0Hc81bYbw04GlJB5ZB0CQPQCjDvbY+98xEqByHXpJYTEmqxm3203suPjK+y0OKzFj4ogZE1d5UlL63mN8ft+/8I0IpMuVveg0sifOIF+PvZa6pAq6olzGwhxB3Nn5D1wdNYifDy5n4eHVICWBdn9PR6uWEIIBd46i5/h4khK3smDabAbfP5bo+JjzLlU0msvLXUCzUEb/381snbuaZR/8zPIP59Mqrj1Dp1yLb1hAQ76MOqcKuqIoBNsDmNjxasa0imf+weUsOLSSqydcS35JoVeP7rW67MSMiWPBtNnEjImr0WNMFhMdruhOhyu6k30sk23z1rJn6VZsPuUjb5O3H8Tu78K/SVB9Rq8XqqArilIpwObLTR1Gc2XUQBINiSxkKym5GRiFgUCbn+4OoF6If2QwAyePZsCkKytXwSx8/Vsy9qXQrHtruozuTZv+nTFa9HHNV1XQFUX5HT+LC1+LkzfinyQp6xBLjqxlTepW3G43DrMdl9nRqJYBnv1a/vDSXWz/eS3b5q1l7oszsfrY6X/nKLrpYIWMKuiKopyXJjTaB7aifWArbu14FevTdjD/4HKSczLQhCDQ5ofJoI+915pyBfvSZ+Iw4m4ZyuGN+9j20xpsFX35vOwc9q/YQbsh3TDbve/ygKqgK4pSIy6zg8HNejGoaU+O5KSy9OgGEo+uo7C0GJvJ2qgmPUL5KN8z82PO2LtsO7++9jWLZ/xA+yFd6Ty6N+HtveekJVXQFUW5KEIImvtEcGvHCMa3G8HWjD0sOLSCXScOIgT4WRvPxa3PFXNVHMGtwtj60xp2LdrE1p/WEBwVzi1vP+gVfXZV0BVFqTWLwUzP8E70DO9Eet4JVqVsYcGhFaTmnsaoGQiw+jaqA6lCCJp0akmTTi0Zcv817F68iROHMyqL+dpZSwhtG0mzrlGIKgaIFebkk/TrRgDef/99rr/+evz9626JqCroiqLUiVBHINe0GcJVUfHsOnGARUfWsCFtB24kPmYnDpPNa1oTdcHisBJzVZ/Kr4vzi1j7+WIKTufjFxFI59G9y09aCvRBSlk5w11o5e/Bww8/zJQpU3j00Ud54YUX6uS9UQVdUZQ6ZdAMdApuQ6fgNpwqymVd6jbmH1xOal4mBjQC7H71OhPcU8x2C3fPfoa9S7eyde4alr0/j+X/mc+Yp28m80Aq62cn/maGe15e+cW+X3vtNQBefPHFS87Q+N5VRVG8hq/FyRUt+jC0eRwHTh1j6dENLD22npKyUuwmG74WZ6PaazdZTHQY1oMOw3qQdTSTbfPWENwyjHkvfXHeC3Lk5+czbdo0HnnkEfz8/C7p+dVwLkVR6p0Qgii/ptze+RreHvY093W7kXBHEKm5maTmZlBYWv18cz0KaBpM/N1jOLb90AUvyGEwGJg9e/YlP6faQ1cUpUHZjBb6NImhT5MYUnIzWXlsIwsOryar8CRmg4kAq69uZ7VXpSYX5MjPzyctLe2Sn0sVdEVRPCbCGcz17UYwts1Qdp7Yz6+HV7ElIwkpJb5WFw6T910T9GLV5IIcdrudsLCwS34uVdAVRfE4k8FITEg0MSHRZBWeYm3KNuYfWk5KTgYGrXyOjB7G+lalJhfkKCsrY9y4cZf8XKqgK4riVQKsvoxs1Z/hLfuyL/sICUfXsTJ5M6WyFIfJgY/O5sicuSDH+tmJlBaW/O5+u93O1KlTL/mAKKiCriiKl9KERtuAFrQNaMEtHcawIW0n8w8t5/DpVDQ0/G0+WAxmT8eskbMvyCE0QWlhCQ6Hg7KyMqZOncoLL7xQJ89To4IuhBgJvAEYgA+klC+fc/9U4C6gFMgE7pBSHv7dN1IURakFu8nGgKY96B/ZneTcdJYd28iiw2s4UXoSqw7GDJx9QY6Nv65mxZs/MX36dMaNG1cne+ZnXPBQshDCAMwARgEdgBuFEB3O2WwTECul7AJ8DbxSZwkVRVEqCCGIdIVxY/sreXvY//Fw7ERa+zfj6gnXkpKbwcnC07il914r1OqyEz2qOwCTJk2q02IONdtD7wXsk1IeABBCzALGAjvPbCClXHLW9quBW+oypKIoyrnMBhM9wjrQI6wDi+5ugRblYvmxTezJPoSUEovRjJ/F1ahmyVyIkFJWv4EQ1wMjpZR3VXx9K9BbSnn/ebZ/C0iTUv61ivsmA5MBQkNDe8yaNatWoXNzc3E6nbV6rCfoKa+esoK+8uopK+gr79lZ3dJNQWkRuSX5FJQWImX5nr1RGPCGY6ml7jL+OPZmlixZcuGNqzB48OANUsrYqu6r04OiQohbgFggvqr7pZTvAe8BxMbGykGDBtXqeRISEqjtYz1BT3n1lBX0lVdPWUFfec+XtaC0iN0nDrA6ZSvr0rZT4i5FIPC3+mAxeuaA6omCkwD18t7WpKAnA03P+jqy4rbfEEJcAfwFiJdSFtVNPEVRlNqzGS10C21Pt9D23FV2HXtPHmZ92g5WJm8mq/AUAL4WFzajRVdLIc+nJgV9HdBGCNGS8kJ+A3DT2RsIIboB71Lemsmo85SKoiiXyGQw0iEwig6BUdzSYQwHTyWzKX03y45tIC3vOCBxmh04TXbdFvcLFnQpZakQ4n7gF8qXLX4opdwhhHgBWC+l/AH4J+AEZle8EUeklFfXY25FUZRa04RGlF9Tovyacl3bK0jJzWBzRhLLkzdw9HQ6AA6zDZfZoau5MjXqoUsp5wHzzrntmbP+fkUd51IURWkQQgiauEJp4gpldNRAjudns/X4HpYf28Te7MOAxGKw4Gtxev2KGXWmqKIoylmC7P4MadabIc16c6ool50n9rP82Ea2H9+LW7oxakb8rD5eeZEO70ukKIriJXwtTvpExNAnIoaCkkJ2ZR1kdcpm1qftpMRdgiYM+FldXjOCQBV0RVGUGrCZrHQPbU/30PaUlJWyJ/sw69K2l6+YKShfMeNncWH14IoZVdAVRVEukslgpGNQFB2DopjY8SoOnDzGpvRdLEveSFrecaSU+Fga/sLYqqAriqJcAk1otPZvRmv/ZlwfPZzk3HQ2ZySx7NhGknPTQZ5ZMeNEq+firgq6oihKHTkzPCzSFcaYqHgy87PYmrmHZcc2sv/kUUBSWFZ/109VBV1RFKWeBNsDGNo8jqHN4zhZlMOOzH2sSN6E4eYb6+X5VEFXFEVpAH4WF/0iu9EvshsJBa3q5Tn0cwqUoiiKUi1V0BVFURoJVdAVRVEaCVXQFUVRGglV0BVFURoJVdAVRVEaCVXQFUVRGglV0BVFURoJIaX0zBMLkQkcruXDg4DjdRinvukpr56ygr7y6ikr6CuvnrLCpeVtLqUMruoOjxX0SyGEWC+ljPV0jprSU149ZQV95dVTVtBXXj1lhfrLq1ouiqIojYQq6IqiKI2EXgv6e54OcJH0lFdPWUFfefWUFfSVV09ZoZ7y6rKHriiKovyeXvfQFUVRlHOogq4oitJI6KqgCyE+FEJkCCG2ezrLhQghmgohlgghdgohdgghHvR0puoIIaxCiLVCiC0VeZ/3dKYLEUIYhBCbhBBzPZ3lQoQQh4QQ24QQm4UQ6z2dpzpCCD8hxNdCiN1CiF1CiD6eznQ+Qojoivf0zJ/TQoiHPJ3rfIQQD1f8/9ouhPhCCGGt0++vpx66EGIgkAt8IqXs5Ok81RFChAPhUsqNQggXsAG4Rkq508PRqiTKL03ukFLmCiFMwHLgQSnlag9HOy8hxFQgFvCRUo7xdJ7qCCEOAbFSSq8/+UUI8TGwTEr5gRDCDNillCc9HOuChBAGIBnoLaWs7UmL9UYI0YTy/1cdpJQFQoivgHlSyo/q6jl0tYcupVwKZHk6R01IKVOllBsr/p4D7AKaeDbV+clyuRVfmir+eO2nvRAiEhgNfODpLI2JEMIXGAj8B0BKWayHYl5hKLDfG4v5WYyATQhhBOxASl1+c10VdL0SQrQAugFrPBylWhUtjM1ABvCrlNKb874OPA64PZyjpiSwQAixQQgx2dNhqtESyAT+W9HO+kAI4fB0qBq6AfjC0yHOR0qZDEwDjgCpwCkp5YK6fA5V0OuZEMIJfAM8JKU87ek81ZFSlkkpuwKRQC8hhFe2tYQQY4AMKeUGT2e5CP2llN2BUcB9Fe1Db2QEugPvSCm7AXnAk56NdGEVraGrgdmeznI+Qgh/YCzlH5oRgEMIcUtdPocq6PWoohf9DTBTSvmtp/PUVMWv2EuAkR6Ocj79gKsr+tKzgCFCiM88G6l6FXtnSCkzgDlAL88mOq9jwLGzfjv7mvIC7+1GARullOmeDlKNK4CDUspMKWUJ8C3Qty6fQBX0elJxkPE/wC4p5WueznMhQohgIYRfxd9twDBgt0dDnYeU8ikpZaSUsgXlv2YvllLW6Z5OXRJCOCoOjFPRvhgOeOVKLSllGnBUCBFdcdNQwCsP5J/jRry43VLhCBAnhLBX1IehlB9bqzO6KuhCiC+AVUC0EOKYEOJOT2eqRj/gVsr3Hs8sqbrS06GqEQ4sEUJsBdZR3kP3+uWAOhEKLBdCbAHWAj9JKed7OFN1HgBmVvwsdAX+7tk41av4kBxG+R6v16r4redrYCOwjfL6W6cjAHS1bFFRFEU5P13toSuKoijnpwq6oihKI6EKuqIoSiOhCrqiKEojoQq6oihKI6EKuqIoSiOhCrqiKEoj8f/ioBZMft190AAAAABJRU5ErkJggg==",
-                        "text/plain": [
-                            "<Figure size 432x288 with 1 Axes>"
-                        ]
-                    },
-                    "metadata": {
-                        "needs_background": "light"
-                    },
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "# Plot data\n",
-                "tick, background = plot(\n",
-                "    delays,\n",
-                "    quantiles_2, \n",
-                "    fmt=\"o--\",\n",
-                "    color=\"#1a9641\",\n",
-                "    error_bars=np.array([quantiles_1, quantiles_3])\n",
-                ")"
+                "Examples:\n",
+                " - Ising model\n",
+                " - Bose-Hubbard\n",
+                " - Previous hamiltonian with qubits.\n",
+                "\n",
+                "Have fun and explore!\n",
+                "\n",
+                "_Recall: If you feel stuck, you can check: hamiltonian.py_"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "141dbce4-829e-485f-8767-825506eb4b8d",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "q_reservoir",
+            "display_name": "openfermion",
             "language": "python",
-            "name": "q_reservoir"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.12.3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `benchmarking-qrc-0.0.3/notebooks/images/QRC_diagram.png` & `benchmarking_qrc-0.0.4/notebooks/images/QRC_diagram.png`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/notebooks/images/nn_rc.png` & `benchmarking_qrc-0.0.4/notebooks/images/nn_rc.png`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/notebooks/images/rnn_and_rc.png` & `benchmarking_qrc-0.0.4/notebooks/images/rnn_and_rc.png`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/notebooks/images/table.png` & `benchmarking_qrc-0.0.4/notebooks/images/table.png`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/setup.py` & `benchmarking_qrc-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="benchmarking-qrc",
-    version="0.0.3",
+    version="0.0.4",
     description="""Benchmarking QRC measures the ability to store information of 
     different quantum particles""",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     url="https://github.com/gllodra12/Benchmarking_QRC",
     author="Guillem Llodrà",
     author_email="gllodra1225@gmail.com",
```

### Comparing `benchmarking-qrc-0.0.3/src/benchmarking_qrc/hamiltonian.py` & `benchmarking_qrc-0.0.4/src/benchmarking_qrc/hamiltonian.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from itertools import combinations
 
 import numpy as np
 from openfermion.linalg.sparse_tools import boson_operator_sparse, get_sparse_operator
 from openfermion.ops.operators import BosonOperator, FermionOperator, QubitOperator
-from scipy.linalg import expm
+from scipy.sparse.linalg import eigsh, expm
 
 from benchmarking_qrc.utils import is_unitary
 
 
 def quadratic_op(n_particles, is_bosonic, dimensions, coefficients, raising_error=True):
     """Hamiltonian of the form:
 
@@ -93,15 +93,15 @@
 def ham_to_matrix(hamiltonian, particle, dimensions, raising_error):
     """Transform a symbolic representation of a hamiltonian into a matrix.
 
     Args:
         hamiltonian (BosonOperator or FermionOperator): Hamiltonian in symbolic form using openfermion operators.
         particle (BosonOperator or FermionOperator): Particle is a boson or a fermion
         dimensions (int, optional): Number of particles on the same site (dim_boson=n, dim_fermion=2).
-        raising_error (bool, optional): Checks if the hamiltonian is hermitian.
+        raising_error (bool, optional): Check if the hamiltonian is hermitian.
 
     Returns:
         sparse.csc: hamiltonian in matrix form
     """
     if particle == FermionOperator:
         hamiltonian = get_sparse_operator(hamiltonian)
     elif particle == BosonOperator:
@@ -113,15 +113,15 @@
         if not is_hermitian(hamiltonian.todense()):
             raise ValueError("The hamiltonian is not hermitian")
 
     return hamiltonian
 
 
 def get_coefficients(n_particles, coef_range=None, coef_onsites=None, coef_couplings=None, seed=None):
-    """Generates a array with the onsite coefficients J_ii and the coupling coefficients J_ij.
+    """Generates an array with the onsite coefficients J_ii and the coupling coefficients J_ij.
     This seed will also generate the sequence of signal values that will be injected into the reservoir.
 
     Args:
         n_particles (int): Number of particles in the system
         coef_range (list):  Randomly generate all coefficients with a min and max value that is inside the list.
         coef_onsite (list): Alternative to coef_range.
         coef_couplings(list): Alternative to coef_range. List with the coupling values J_ij
@@ -132,15 +132,15 @@
     """
     np.random.seed(seed)
 
     # Randomly generate the values of J_ij
     if coef_range:
         if len(coef_range) != 2:
             raise ValueError(
-                "Amp range must contain only 2 values. First value must be the lowest and the second value the highest to be generated."
+                "Amp range must contain only 2 values. The first value must be the lowest and the second value the highest to be generated."
             )
         if coef_onsites or coef_couplings:
             raise NameError(
                 "Coefficients error. Random and custom coefficients detected, decide which one you want to use"
             )
 
         coefficients = np.random.uniform(
```

### Comparing `benchmarking-qrc-0.0.3/src/benchmarking_qrc/measurements.py` & `benchmarking_qrc-0.0.4/src/benchmarking_qrc/measurements.py`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/src/benchmarking_qrc/reservoir.py` & `benchmarking_qrc-0.0.4/src/benchmarking_qrc/reservoir.py`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/src/benchmarking_qrc/run_memory_capacity.py` & `benchmarking_qrc-0.0.4/src/benchmarking_qrc/run_memory_capacity.py`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/src/benchmarking_qrc/utils.py` & `benchmarking_qrc-0.0.4/src/benchmarking_qrc/utils.py`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/src/benchmarking_qrc.egg-info/SOURCES.txt` & `benchmarking_qrc-0.0.4/src/benchmarking_qrc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,18 @@
 data/memory_capacity/4_6_boson_5_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
 data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
 data/memory_capacity/4_6_boson_6_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
 data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
 data/memory_capacity/4_6_boson_7_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
 data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/test/range_1_1000.npy
 data/memory_capacity/4_6_boson_8_ij_1000_1200_300_2_10.0_1_0.0_uniform_(0.0, 1.0)/train/range_1_1000.npy
+notebooks/Benchmarking the role of particle statistis in Quantum Reservoir Computing.ipynb
+notebooks/Practice.ipynb
+notebooks/Practice_solutions.ipynb
 notebooks/Tutorial.ipynb
-notebooks/.ipynb_checkpoints/Tutorial - Memory capacity-checkpoint.ipynb
-notebooks/.ipynb_checkpoints/Tutorial - Quantum Reservoir Computing-checkpoint.ipynb
-notebooks/.ipynb_checkpoints/Tutorial-checkpoint.ipynb
 notebooks/images/QRC_diagram.png
 notebooks/images/nn_rc.png
 notebooks/images/rnn_and_rc.png
 notebooks/images/table.png
 src/benchmarking_qrc/__init__.py
 src/benchmarking_qrc/hamiltonian.py
 src/benchmarking_qrc/measurements.py
```

### Comparing `benchmarking-qrc-0.0.3/tests/conftest.py` & `benchmarking_qrc-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/tests/test_hamiltonian.py` & `benchmarking_qrc-0.0.4/tests/test_hamiltonian.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     [
         (
             4,
             [0, 1, 2],
             None,
             None,
             3,
-            "Amp range must contain only 2 values. First value must be the lowest and the second value the highest to be generated.",
+            "Amp range must contain only 2 values. The first value must be the lowest and the second value the highest to be generated.",
         ),
         (
             3,
             None,
             [0.8, 0.7, 0.6, 1],
             [0.2, 0.3, 0.4],
             None,
@@ -183,8 +183,10 @@
         (3, None, [1, 1, 1], [2, 2], None, "The length of len(coef_coupling)=2. The expected length is 3"),
     ],
 )
 def test_get_coefficients_errors(n_particles, coef_range, coef_onsites, coef_couplings, seed, exp_msg):
     with pytest.raises(ValueError) as excinfo:
         get_coefficients(n_particles, coef_range, coef_onsites, coef_couplings, seed)
     (msg,) = excinfo.value.args
+    print(msg)
+    print(exp_msg)
     assert msg == exp_msg
```

### Comparing `benchmarking-qrc-0.0.3/tests/test_measurements.py` & `benchmarking_qrc-0.0.4/tests/test_measurements.py`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/tests/test_memory_capacity.py` & `benchmarking_qrc-0.0.4/tests/test_memory_capacity.py`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/tests/test_reservoir.py` & `benchmarking_qrc-0.0.4/tests/test_reservoir.py`

 * *Files identical despite different names*

### Comparing `benchmarking-qrc-0.0.3/tests/utils.py` & `benchmarking_qrc-0.0.4/tests/utils.py`

 * *Files identical despite different names*

